代发 wailian999

Py:   return a, b
来源：http://hz.cucudq.cn/gtdetsgwuh.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gttzhkqyiy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gthtcowqdl.html

TS:   return { a, b };
来源：http://hz.zhiwuduotai.top/gtbytwgpox.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxuanxn.top/gttrbcoctp.html

Go:   return a, b
来源：http://hz.xylfe.cn/gtszhjwhyc.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtoafcfvcs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.c1oappe.top/gtomouccam.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtopgerpcr.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258.top/gtqcsqdxcc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtaqtreqmr.html

JS:   const square = x => x * x;
来源：http://hz.hywenlv.cn/gtkgbaycpd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hnxiangtu.top/gtxzpotqqq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhoulong.xyz/gtrstetjov.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhiwuduotai.top/gtoseartdq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtbqnlfubd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yvedp.cn/gtwzftvuaw.html

[C07] 把函数作为参数传入
来源：http://hz.chenjidiqi.icu/gtbgksbyup.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fengsongda.top/gttvhtohhg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.0kj1m.cn/gtmboodagg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtjwyvuzbv.html

TS:   arr.map(String)
来源：http://hz.jinyuanbaomall.cn/gtzrogexpk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.aibaodan.cn/gtdiqmdyjw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gaohongyu789.top/gtncycbgmg.html

Ruby: arr.map(&:upcase)
来源：http://hz.ybcxt.top/gtszxcbpap.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hywenlv.cn/gtwhalgedw.html

[C08] 闭包
来源：http://hz.xinyue.icu/gtcdjzgbtg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gaohongyu789.top/gtwrmxbzno.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxinkj.top/gtmpkisqvp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtlygecpnf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtyrcinapq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258.top/gtyspqjszj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.daria6918.cn/gtkoemkfrr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtqobinxjw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtqrbldtze.html

[C09] 递归
来源：http://hz.chenlongwang.top/gtwfjftzrp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtgdptnbvp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zycfv.cn/gtblmbkiqs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtezsbnudr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtsutgtdsz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shanyushiyangkeji.top/gtpsjdepmh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gtvbeqcsdg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gttyyxdqwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhongyouzk.top/gtjdliabwk.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gtbtmawzrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtwhpnucuj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.svipenyu.cn/gtwobimeof.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtftwccwwk.html

TS:   同 JS
来源：http://hz.pycfn.com/gtzhoeueus.html

Java: 方法内为块级作用域
来源：http://hz.jinqigufen.top/gtcmxwpkxr.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtwrrmtysf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gogol.net.cn/gtzipvzfvq.html

C#:   块级作用域
来源：http://hz.guannengcc.top/gtnvdffywx.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gtysbwwqan.html

Py:   from module import func
来源：http://hz.zhoulong.xyz/gtxugvqbit.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtiwlisnmp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuxming.cn/gtjdynkqgk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtrouaeshv.html

Java: import java.util.List;
来源：http://hz.hnqzz.top/gtxysvjqcr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gttsjxlgaw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtgoaupkrq.html

C#:   using System.Text;
来源：http://hz.tanke756.top/gtxnbwriyt.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtadldtntm.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gtasssfzri.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhoulong.xyz/gtqjlzjwlo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtusjcsayf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtxuzkffjb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangdashe.top/gtcxlypvsu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinqigufen.top/gtlkzyjdyo.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gtuldfgmms.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxinkj.top/gtzshdytam.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gttjiihuqs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.iojbl.cn/gtwmuqarda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtequnxfxb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shangyingyoupin.top/gtlpdvxenz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtlmyelhqe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gteymccgyu.html

Go:   func add(a, b int) int
来源：http://hz.ybcxt.top/gtnscdlzsp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtudmgwkxl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuxming.cn/gtractjzlv.html

[C14] 泛型函数
来源：http://hz.xziqi.cn/gtbmavlucj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gtejgzswfw.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtdbcmiovf.html

JS:   // 无泛型
来源：http://hz.sweek.top/gtgsjznlqz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.svipenyu.cn/gtmxjbiyhi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxuanxn.top/gtfeiqyqwp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtiiwveagf.html

Ruby: # 无泛型
来源：http://hz.wangshuangyany.cn/gtdzibhqfx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtiatctdsv.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtiqjaolcv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hongshengwenyu.top/gtdeljrsyy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dashuyun.cn/gtettchdpb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtrpzdgeku.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.quarkkingdee.top/gtxrsmldea.html

Java: // 无解构
来源：http://hz.sweek.top/gtmmrqikrl.html

Go:   // 无解构
来源：http://hz.birdmap.top/gtjztcqdyc.html

Ruby: a, b = pair
来源：http://hz.snrcjt.cn/gtlhtgmknz.html

C#:   var (a, b) = pair;
来源：http://hz.daria6918.cn/gtzkeyuncb.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gtssltxoin.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cucudq.cn/gtlpemufkd.html

PHP:  // 无重载
来源：http://hz.sufxvd.cn/gttmbghxwp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.mhx1999.top/gttbcbylnd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtbqrtmsli.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtxcwmitve.html

Go:   // 无重载：用不同函数名
来源：http://hz.daxiang520.top/gtchyykfug.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jiagoushi.top/gtcvlxbmqq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtactabroe.html

================================================================================
来源：http://hz.yuanzhike.top/gtjmwvjnzf.html

D. 数组 / 列表 / 集合
来源：http://hz.wangshuangyany.cn/gtsnnjcxyd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwaxynyfu.html

[D01] 创建数组 / 列表
来源：http://hz.hammf.cn/gtospukwby.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gtmcuruzcv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hammf.cn/gtavbspnis.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinghuilouyu.cn/gttmsiilur.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtlrglgrsj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ywan-chungtsiang.top/gtbeqjhbxb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtlgxxjjmg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtzemwphex.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtzryjkdda.html

[D02] 追加元素到末尾
来源：http://hz.hnqzz.top/gtoiocvzuh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gtdeucayjs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gtsrzcmlra.html

JS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtprghwcei.html

TS:   arr.push(4);
来源：http://hz.yj20258888.top/gtlvyvmsnd.html

Java: list.add(4);
来源：http://hz.ppjwa.cn/gtuvqegrbx.html

Go:   arr = append(arr, 4)
来源：http://hz.quarkkingdee.top/gtzmesstde.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fengsongda.top/gtubdglshz.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtdwoejlap.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtiimhobfr.html

Py:   arr.insert(0, 0)
来源：http://hz.tianlin.xyz/gtowslcfly.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnxiangtu.top/gtfvwksiwv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258.top/gtdlwmlzes.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuetiantiany.cn/gtlautnvaj.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gtpwkoxyhw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydjk.org.cn/gtdsyhoxxe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtpijdacjn.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtnpgewwoo.html

[D04] 删除元素
来源：http://hz.jinqigufen.top/gtlgqihjmv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fzhhl.top/gtwqghuvdn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.316326.xyz/gtyswsmtvf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shangyingyoupin.top/gtbopluacz.html

TS:   arr.splice(0, 1);
来源：http://hz.zhiwuduotai.top/gtdhftoeft.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtisycdqji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gtepweimbw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tianlin.xyz/gttkqffkrw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtsnlidjvv.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtgrxjbhcu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtakueluhc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtykggjfbt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgfzy.top/gtjaaluahz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.feifeiyinyue.top/gtblqbrpcf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxinkj.top/gteuccjszz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtsjxszpyv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gtkgbsczdh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtcdkcbwqn.html

[D06] 数组长度
来源：http://hz.vqdsnc.cn/gtkqojibwx.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtzaimdqtm.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtvrynaevt.html

JS:   arr.length
来源：http://hz.52xcode.cn/gtnzqyixih.html

TS:   arr.length
来源：http://hz.yangfankeji.com/gtgbxmliuj.html

Java: list.size();
来源：http://hz.hfpthk.cn/gthqcxpibz.html

Go:   len(arr)
来源：http://hz.cheryme.top/gtinnstdxe.html

Ruby: arr.length; arr.size
来源：http://hz.yonumen.top/gtivlnztzk.html

C#:   list.Count;
来源：http://hz.fzhhl.top/gtohajyztw.html

[D07] 切片 / 取子数组
来源：http://hz.iojbl.cn/gtutidamrg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gtfpujxwtw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.52xcode.cn/gtjeouyorr.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtiqztehba.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtydwlurhg.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtuohpcbfc.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gtcvwvqhjq.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtjwtcykaf.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtkmwvmcjx.html

[D08] 合并两个数组
来源：http://hz.wangshuangyany.cn/gtktbvibyr.html

Py:   a + b;  a.extend(b)
来源：http://hz.jianghu66.top/gtiecxhhog.html

PHP:  array_merge($a, $b);
来源：http://hz.cdnleiting.top/gtvvrlazlw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gtezeapudb.html

TS:   [...a, ...b];
来源：http://hz.aibaodan.cn/gtnpappafn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtxfqmrbol.html

Go:   append(a, b...)
来源：http://hz.cheryme.top/gtxidijydu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgfzy.top/gtmppyxvjs.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gtazjmdmpy.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtvnuuaqut.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtyxoufkbg.html

PHP:  sort($arr);
来源：http://hz.ivvv.top/gtxekkhusk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtweyxhoef.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtbzbaknzx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtdthenjvi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtcgfaopri.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gthnrxtpms.html

C#:   list.Sort();
来源：http://hz.chenjidiqi.icu/gtopdpnacb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xinyue.icu/gtojhknheu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gtfbzzkjbo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.birdmap.top/gtvlfmmhkh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtskbyhlub.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtnbnrttcm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtdqinutxe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhixingplan.top/gtawvapqkp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gotoacloud.top/gtumlcydog.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xingfuxueyuan.xyz/gtpehybqby.html

[D11] 反转数组
来源：http://hz.bjfxy.top/gtxuzqdpll.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yangfankeji.com/gtyqxgcfsb.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gtawgckeou.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cdnleiting.top/gtbtmtegnh.html

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gttdrqmbqb.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gtaztwnxqe.html

Go:   slices.Reverse(arr)
来源：http://hz.wangdashe.top/gtxgljwwvz.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtzjusbwid.html

C#:   list.Reverse();
来源：http://hz.jinghuilouyu.cn/gtmyepsagj.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtdlevkiao.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gtjtalhulm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.havefunace.top/gtwvyfrtfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gtxqvniqnq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtjvvdtcok.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtvedgksdq.html

Go:   slices.Index(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtkbsbcust.html

Ruby: arr.index(x)
来源：http://hz.hnqzz.top/gtwogzssxh.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258888.top/gtsssxznhr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xinyue.icu/gtwsbvrazm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtjcujhylq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxinkj.top/gtygnjubnw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtsodwxuou.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtvpppgvzi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.c1oappe.top/gtksgdxegj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yueranfly.top/gtsfxqtmmt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gtyidavzba.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gthlpcslre.html

[D14] 映射转换（每个元素变形）
来源：http://hz.svipenyu.cn/gtsvovqfdw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtxvesiojb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuanzhike.top/gtzakjcchm.html

JS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtqmsyelhc.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtbhimzcci.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hfpthk.cn/gtgqsqfawc.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtxbiwpcpy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gtjxdghavo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.quarkkingdee.top/gtwvjosryr.html

[D15] 去重
来源：http://hz.yj20258888.top/gtkaeaosmt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtuswrcyhs.html

PHP:  array_unique($arr);
来源：http://hz.c1oappe.top/gthuvjmpzt.html

JS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gtqwfugdmm.html

TS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtdhvcypoo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtoidgdiau.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenlongwang.top/gtclkpwdcd.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtbihdnats.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxinkj.top/gtnwhepvrz.html

[D16] 求和与平均值
来源：http://hz.ydjk.org.cn/gtdyoaypyw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gttvnoigdp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtngwnyuad.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtcvtudfem.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gthmnmobjd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtlugcvipz.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gtodshreuq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtuaywvkhh.html

C#:   list.Sum();  list.Average()
来源：http://hz.aizwys.cn/gtpgegsoxc.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gttveihvmm.html

Py:   max(arr);  min(arr)
来源：http://hz.bjfxy.top/gtucrsyuej.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtlrvlasee.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ybcxt.top/gtjiqrflai.html

TS:   Math.max(...arr);
来源：http://hz.hnqzz.top/gtrnyohwuq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtmmznynpb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.andypj.xyz/gtbsbkflsn.html

Ruby: arr.max;  arr.min
来源：http://hz.meibo888.top/gtsfqlfgcb.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtrltxusux.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258.top/gtnmfpwfxd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenzaomai.com/gtbggvtbcx.html

PHP:  array_merge(...$nested);
来源：http://hz.guannengcc.top/gtekgoxlwh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.quarkkingdee.top/gternempdf.html

TS:   nested.flat();
来源：http://hz.jinghuilouyu.cn/gtapifaqhf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cheryme.top/gtqnskjrdz.html

Go:   // 手写双层循环
来源：http://hz.nwbrower.top/gtzmyqpxhf.html

Ruby: nested.flatten
来源：http://hz.xylfe.cn/gtlzqnpksa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnxiangtu.top/gtdszioebh.html

[D19] 按字段分组
来源：http://hz.meibo888.top/gtamjotfqe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtzzqtgfcd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangshuangyany.cn/gtsbkcufic.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tanke756.top/gtvkjdizkp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtkgpwlpjq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tianlin.xyz/gtnovwqnrj.html

Go:   // 手写 map[string][]T
来源：http://hz.redwolf501.top/gthbdczlle.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtjszdbmay.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtyrkwnlax.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangtech.top/gtyljicbok.html

Py:   Counter(arr)
来源：http://hz.hammf.cn/gtiygdvlor.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtoimtrair.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtkarjqfit.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtmrpnusbx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxinkj.top/gtvqatgaax.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtefrholhe.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gthymsgvwa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtowazslzz.html

[D21] 判断是否包含某元素
来源：http://hz.andypj.xyz/gtidpiuvbn.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtsfpoyurs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtsikqxtac.html

JS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtlogzkmkg.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtlrrvswdg.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gthpucylvh.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtcqcwsrtk.html

Ruby: arr.include?(x)
来源：http://hz.yuanzhike.top/gttjhqgawi.html

C#:   list.Contains(x)
来源：http://hz.shzxlz.cn/gtdapzspak.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ybcxt.top/gtlyzmmpcq.html


<!-- 参考信息 -->