代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.xinyue.icu/gtjtvikcgd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtlwajjtam.html

C#:   f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtnxlctfuk.html

[C05] 返回多个值
来源：http://hz.chenzaomai.com/gtqkfmwkys.html

Py:   return a, b
来源：http://hz.chenlongwang.top/gtxfpdatez.html

PHP:  return [$a, $b];
来源：http://hz.zhixingplan.top/gtljoqpdbf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtneyhqogp.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtqyyoohmm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydjk.org.cn/gtruchyind.html

Go:   return a, b
来源：http://hz.cheryme.top/gtiveqnqsj.html

Ruby: return a, b
来源：http://hz.jinqigfzy.top/gtyrcjlesx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangshuangyany.cn/gtoznkckik.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtdokgkglu.html

Py:   square = lambda x: x * x
来源：http://hz.xuetiantiany.cn/gtzogzamoc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cashguo.top/gtkddzyevn.html

JS:   const square = x => x * x;
来源：http://hz.0kj1m.cn/gtaoxnooww.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zycfv.cn/gtvxngqolk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yongpay.top/gtztvhtltp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hammf.cn/gtneoxcfni.html

Ruby: square = ->(x) { x * x }
来源：http://hz.0kj1m.cn/gtslwnstal.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yvedp.cn/gtanengiox.html

[C07] 把函数作为参数传入
来源：http://hz.wangshuangyany.cn/gtwzslvudh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxinkj.top/gtwzbhtixx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jiagoushi.top/gtxkbwkmwi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xingfuxueyuan.xyz/gtamhbxmmu.html

TS:   arr.map(String)
来源：http://hz.haohaochexian.top/gtymwjkmtz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fzhhl.top/gtjyvyouib.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtldwfjvhp.html

Ruby: arr.map(&:upcase)
来源：http://hz.shzxlz.cn/gtwmwyurbm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sxryk.cn/gtczkfheuw.html

[C08] 闭包
来源：http://hz.jianghu66.top/gtspmunyib.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nwbrower.top/gtitgnpibc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jianghu66.top/gteedyvjyx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtygoddngw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtandpknqo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xingfuxueyuan.xyz/gtllkfspcs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhoulong.xyz/gtylwbbryf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guannengcc.top/gtfzgydyxb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtwmjkzwan.html

[C09] 递归
来源：http://hz.52xcode.cn/gtorzqvzrm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuanzx.com/gtbqxmftma.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gtwqnnvhet.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtsodjskzx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtesqoyhoa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydjk.org.cn/gtfhxtjsnx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigfzy.top/gtzhxfovva.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cheryme.top/gtavqadezt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.52xcode.cn/gtxzszbdqo.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtlkzpedvh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hammf.cn/gtagerwyce.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gzhubu.top/gtmhgzjtvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtndaitwfv.html

TS:   同 JS
来源：http://hz.52xcode.cn/gtlmfriusf.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtkqkmgktq.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtkpqlwtlq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jianghu66.top/gtbistnesn.html

C#:   块级作用域
来源：http://hz.52xcode.cn/gtwbttompf.html

[C11] 模块导入与导出
来源：http://hz.bjfxy.top/gtyytbofto.html

Py:   from module import func
来源：http://hz.zhijiandao.cn/gtoofmlkxs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.daria6918.cn/gtmelzbpoa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtvznqghys.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.kuanghao11.cn/gtmsxaeypw.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtuasklzwp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgfzy.top/gtlkfqstjc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gtoipctbgm.html

C#:   using System.Text;
来源：http://hz.andypj.xyz/gtznmrnvgc.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtgfzdswtt.html

Py:   (lambda: print("run"))()
来源：http://hz.zhoulong.xyz/gtukradbwm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dianchejie.cn/gtxrxeucff.html

JS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gtcclkrhfl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtuwslpelr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigfzy.top/gtzcvqmsfi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhaomingkeji.xyz/gtdleqplqt.html

Ruby: -> { puts "run" }.call
来源：http://hz.jianghu66.top/gtffvudtoq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuanzx.com/gtpnlbubar.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtnjoqmrtd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuxming.cn/gtwdaqojwn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtjihaccje.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sufxvd.cn/gtoceivtqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gthpshudpm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gthqvvgyjm.html

Go:   func add(a, b int) int
来源：http://hz.birdmap.top/gtdwjyyzpm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangtech.top/gthokakjov.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtldfvuflr.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtfifonqfh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gttugkbslw.html

PHP:  // 无泛型
来源：http://hz.fengsongda.top/gtqebhjwhx.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gtfgqebcqu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtonzlofcv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtdciuhqxa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guowangkeji.top/gtocpxxehz.html

Ruby: # 无泛型
来源：http://hz.hongshengwenyu.top/gtnouusokj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yongpay.top/gticoopakq.html

[C15] 解构 / 展开参数
来源：http://hz.316326.xyz/gttpxcpkku.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhoulong.xyz/gtkigknpav.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinghuilouyu.cn/gtjmkcweew.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtmjhdjvcc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hfpthk.cn/gtspsjrecp.html

Java: // 无解构
来源：http://hz.aibaodan.cn/gtghgzyurn.html

Go:   // 无解构
来源：http://hz.sxryk.cn/gttrytszos.html

Ruby: a, b = pair
来源：http://hz.xuetiantiany.cn/gtvxpxawso.html

C#:   var (a, b) = pair;
来源：http://hz.daxiang520.top/gtceztggmd.html

[C16] 函数 / 方法重载
来源：http://hz.yj202588.top/gtwrdxccdr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xingfuxueyuan.xyz/gtiabvvgrw.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtqjkaypsl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.redwolf501.top/gtvutiwybd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhaomingkeji.xyz/gtvzozaxif.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtdfwqegxi.html

Go:   // 无重载：用不同函数名
来源：http://hz.dianchejie.cn/gtbjkheujy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gtnznuddcf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtmqdwyntt.html

================================================================================
来源：http://hz.iojbl.cn/gtqzlvhcbc.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtxtexlfiy.html

================================================================================
来源：http://hz.bjfxy.top/gtrkcnavzl.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtzypsthda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtfpndotdi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.0kj1m.cn/gtfyhtjtso.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydzc1.top/gtqwecgrdh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtsfabblcg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.c1oappe.top/gtymdzjkkv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gtxicpmuwl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinyuanbaomall.cn/gtztfuamyc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yongpay.top/gtcefpkxbb.html

[D02] 追加元素到末尾
来源：http://hz.jinqigufen.top/gtrcnvnofh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gtvuiokwgi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtgmxnbumn.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtanmmopus.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gtqlthjqfg.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtllfrjlnw.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtobkpjxkj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtyvragxeq.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtxekfaxcn.html

[D03] 在指定位置插入元素
来源：http://hz.hnqzz.top/gtiivlgfzc.html

Py:   arr.insert(0, 0)
来源：http://hz.hysaishi.cn/gtnzqabajx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydzc1.top/gtkjoehmxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtxvldmzwt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gthbiflqkp.html

Java: list.add(0, 0);
来源：http://hz.yueranfly.top/gtkhprtqvt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gtiiaskzmb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.meibo888.top/gthfdfkqmv.html

C#:   list.Insert(0, 0);
来源：http://hz.yanxiufei.cn/gtmblfnmqp.html

[D04] 删除元素
来源：http://hz.sufxvd.cn/gtjazdyjwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yueranfly.top/gtzfvqbxdn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gttewiccfm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtcghfizrs.html

TS:   arr.splice(0, 1);
来源：http://hz.aibaodan.cn/gtgtjlthyk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtqfazzzvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.c1oappe.top/gtnvxcqsnf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtzjzxlgyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtkkxeqkmh.html

[D05] 访问与修改元素
来源：http://hz.nanxinkj.top/gtcnxanlsu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtvqhhsbyb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtgxjpzieh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gthoolgeef.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258.top/gtyzglbosx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gtrxglwvpn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yvedp.cn/gtfqdjermj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtsrenapxo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hywenlv.cn/gtrddtxklw.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gtgmutwjaa.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtkmxcecut.html

PHP:  count($arr);
来源：http://hz.jlsjyb.cn/gtgxkaeynt.html

JS:   arr.length
来源：http://hz.yanxiufei.cn/gtgqayggrp.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtcfgicqcp.html

Java: list.size();
来源：http://hz.yueranfly.top/gtyieprosa.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gtpvicsjse.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gtfvjwsout.html

C#:   list.Count;
来源：http://hz.vqdsnc.cn/gtvkrcachb.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gtkhnzzyvt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtvntbehos.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sxryk.cn/gtzmlifjab.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gthvibdlyy.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtgndqlpjq.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtsslrojrj.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gtczlinmid.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtcbbgelev.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtugyqbsfv.html

[D08] 合并两个数组
来源：http://hz.nanxinkj.top/gtcbnpchcv.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangdashe.top/gthbuipjzb.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtlsqhstyp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aibaodan.cn/gtvdbnvcud.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtkhodktzk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gttlqosxyf.html

Go:   append(a, b...)
来源：http://hz.tian-w.cn/gtfdtycaui.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhixingplan.top/gteicebsuj.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinyuanbaomall.cn/gtdobhqmdw.html

[D09] 排序（升序）
来源：http://hz.daxiang520.top/gthekdbgyw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtkjmnbddd.html

PHP:  sort($arr);
来源：http://hz.ivvv.top/gtzkcbtooz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtggxwspvt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtkmwgomcb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tianlin.xyz/gtwxbjpwkc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.redwolf501.top/gtwjlfugaf.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtjuhzykmj.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtmnhzvgqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xingfuxueyuan.xyz/gtujqtzmbf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtdelzkhgx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtperbjsrj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtjsmzyrqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtlysxywsg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yanxiufei.cn/gticlthrzc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtssjdrwlj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yongpay.top/gtdfnuuccz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gthaqojqwc.html

[D11] 反转数组
来源：http://hz.shanyushiyangtech.top/gtsinrxthy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtwjvcjprr.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtpwazfnai.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.9152youxi.cn/gtqqqanjuo.html

TS:   [...arr].reverse();
来源：http://hz.zdqjudy.top/gtayzlntkt.html

Java: Collections.reverse(list);
来源：http://hz.zhijiandao.cn/gtbdatzoqj.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtntfmryag.html

Ruby: arr.reverse
来源：http://hz.tian-w.cn/gtlsyfvwqw.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtqopwkdkt.html

[D12] 查找元素下标
来源：http://hz.316326.xyz/gtsmofrxkz.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtmhhrkion.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.andypj.xyz/gtcjpjaxmt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtyfauliyu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtxxsfojap.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangtech.top/gtidbmkzfl.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtitjpsohx.html

Ruby: arr.index(x)
来源：http://hz.smart0.xyz/gtnfpuzumi.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gtxplcicjd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.quarkkingdee.top/gtnbfbsbee.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.iojbl.cn/gtfjwpsizq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gthxwajbha.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtfqevzlid.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtvfyjyuxs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtyhyruzed.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zdqjudy.top/gtbbhryskh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cqqwz.cn/gtohdwrcvo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuanzx.com/gtbqxxvuys.html

[D14] 映射转换（每个元素变形）
来源：http://hz.kuanghao11.cn/gtbvvejmjm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gtmixqmuvx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.smart0.xyz/gtsbghhugc.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtjqraoeji.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtceqwyehi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.kuanghao11.cn/gtpusvwodf.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtogmvyqxg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtelunenfm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gtoryxucbp.html

[D15] 去重
来源：http://hz.zycfv.cn/gttnrstgfs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gthkswfglm.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtjfhajoox.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtpnsjifct.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtbtroemuy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtlucldrkk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jianghu66.top/gtdpoalkum.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtbzddsvdz.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtujbjujmp.html

[D16] 求和与平均值
来源：http://hz.jiagoushi.top/gttqhmjsgg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ywan-chungtsiang.top/gtjdibvbcc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtdmsxrnxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtkesfakry.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gtbmkygwnh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtmtxcfasl.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtkuoqiofh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtgmjxckgj.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtodevzdgk.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gtmymgepmb.html

Py:   max(arr);  min(arr)
来源：http://hz.316326.xyz/gteorujzbk.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gtfmlterwy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtpwumwujl.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtrhzwncqw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aibaodan.cn/gtpmvfeoyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtxpotclls.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtfdhfludo.html

C#:   list.Max();  list.Min()
来源：http://hz.daria6918.cn/gtngfiepwx.html

[D18] 扁平化嵌套数组
来源：http://hz.dashuyun.cn/gtslrpvgmy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtoywnfmue.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtnwfoyzvu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gttfcxptxc.html

TS:   nested.flat();
来源：http://hz.iojbl.cn/gtfphlumht.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jianghu66.top/gtthsediks.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtqphppylq.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gttikijacz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtpwueuulb.html

[D19] 按字段分组
来源：http://hz.xuetiantiany.cn/gtsaiupymn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhongyouzk.top/gtyagdxvqc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gttiamocpm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtmwupgkhr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gtiebvmbrc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtxtrnjvsy.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gtlcfowyir.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtuypdapra.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yongpay.top/gtsuoeqkqy.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtzpufuyhk.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtkkwormpd.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtzvsdppcm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gthogwunzo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtjruutlxh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtkkujdaeh.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtgpvzhuue.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gtctdrnbdg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jlsjyb.cn/gttodvjcdv.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gttrpsbrpo.html

Py:   x in arr
来源：http://hz.xingfuxueyuan.xyz/gtkpftbmcs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtanwpkwoo.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gttcnlohuq.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtnmddyaqm.html

Java: list.contains(x)
来源：http://hz.c1oappe.top/gttwbywfyq.html


<!-- 参考信息 -->