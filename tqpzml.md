代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.vqdsnc.cn/gtklocrmly.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtxrqpzgkg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shangyingyoupin.top/gttbrdewhm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xziqi.cn/gtmntmkagq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.0kj1m.cn/gthelfiwnk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtvuqixrlm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtdjrfwabr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.birdmap.top/gtyagohmtu.html

Go:   // 无：用配置结构体参数
来源：http://hz.daxiang520.top/gtfxythokj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtvgjarzsk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gteryenamu.html

[C05] 返回多个值
来源：http://hz.zhijiandao.cn/gtddxithgs.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtrewvgcfz.html

PHP:  return [$a, $b];
来源：http://hz.dianchejie.cn/gtbnsiyizz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.quarkkingdee.top/gtpyxokvnj.html

TS:   return { a, b };
来源：http://hz.aizwys.cn/gtavcukquq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gtomxqbfgg.html

Go:   return a, b
来源：http://hz.fengsongda.top/gttyrdtttm.html

Ruby: return a, b
来源：http://hz.tian-w.cn/gtdbfptneo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtjxszyhyd.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtuumwyplm.html

Py:   square = lambda x: x * x
来源：http://hz.jianghu66.top/gtyngcerfi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtttbrjzbw.html

JS:   const square = x => x * x;
来源：http://hz.shuidangran.top/gtfbcggzul.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.0kj1m.cn/gtkwfmxkjm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gzhubu.top/gtfubtoeic.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhiwuduotai.top/gtwaofvgtq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtnnnyzniv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nwbrower.top/gtnykcsfiv.html

[C07] 把函数作为参数传入
来源：http://hz.shangyingyoupin.top/gtvvpnezvr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xziqi.cn/gtinmwkmdu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ivvv.top/gtrzfxhasl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cheryme.top/gtcrakqjyj.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtuvkwgpkl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.iojbl.cn/gtwermpqtv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhijiandao.cn/gtuykbhmel.html

Ruby: arr.map(&:upcase)
来源：http://hz.meibo888.top/gtayfexila.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shuidangran.top/gtzieqcbld.html

[C08] 闭包
来源：http://hz.guannengcc.top/gtfasbdfwj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtekysivfb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.9152youxi.cn/gttivsbpwt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtxtjunthm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtfghikprx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtfhbrlewu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xinyue.icu/gtyezibuoq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.c1oappe.top/gtaducgjen.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtfdhtkabl.html

[C09] 递归
来源：http://hz.guowangkeji.top/gtiitjjjik.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtdywdugli.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jianghu66.top/gttqtsjrki.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtwenwifkj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtrwtjggoc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jlsjyb.cn/gtqpbhznfm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yongpay.top/gteevjekkk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtitfgckob.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtcljbyndz.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtznozuqgx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgfzy.top/gtpyuqpkjs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtwkvfptrz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daxiang520.top/gtwchtozxg.html

TS:   同 JS
来源：http://hz.yangfankeji.com/gtmcadydyh.html

Java: 方法内为块级作用域
来源：http://hz.zycfv.cn/gtjqalsnsm.html

Go:   花括号块级作用域
来源：http://hz.guannengcc.top/gtgyptbfcw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hfpthk.cn/gtnnyhadsq.html

C#:   块级作用域
来源：http://hz.guowangkeji.top/gteqlehieq.html

[C11] 模块导入与导出
来源：http://hz.yvedp.cn/gtfztxluuy.html

Py:   from module import func
来源：http://hz.xylfe.cn/gtbxhnwdnu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ybcxt.top/gtcpenaehn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.svipenyu.cn/gtwaepgbin.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtflgtqzgy.html

Java: import java.util.List;
来源：http://hz.bjfxy.top/gtxvwhwniw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtphsqumej.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ybcxt.top/gtpthmnkiq.html

C#:   using System.Text;
来源：http://hz.havefunace.top/gtgucmljzz.html

[C12] 立即执行函数 IIFE
来源：http://hz.havefunace.top/gtviwvzmje.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtfvoivtoi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtppaaqdbw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gthrdnnhxe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtfmzpdike.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yvedp.cn/gtuwvmggwu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gotoacloud.top/gtxpbhnkwl.html

Ruby: -> { puts "run" }.call
来源：http://hz.hywenlv.cn/gtmlabmdcw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtxtqswcrb.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gtfbzycmkv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.bjfxy.top/gtyltbjrzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtmiaelzfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ehwqpu.com/gtfmodmnxb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gthollcvwc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtsgdvsltr.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtnfijqkqy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnqzz.top/gtmkfpnbqb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtwevycieq.html

[C14] 泛型函数
来源：http://hz.mhx1999.top/gtysgtuheh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenjidiqi.icu/gtvidarebx.html

PHP:  // 无泛型
来源：http://hz.wangdashe.top/gtnknotsiw.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtzokffnfq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.birdmap.top/gtjplvlxro.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtmiiuvnqx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hammf.cn/gtgpuptmiu.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtqxpmrpqy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtomvhrahn.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtvxjcnoha.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtnilvktan.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gthtcsopbc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtvsjxxgbn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yongpay.top/gtsfaiabkl.html

Java: // 无解构
来源：http://hz.andypj.xyz/gtxdwrkvhx.html

Go:   // 无解构
来源：http://hz.c1oappe.top/gtnzixosgl.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gtwaiwpxnf.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtjitctjcl.html

[C16] 函数 / 方法重载
来源：http://hz.birdmap.top/gtbpqhwxgt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuanzhike.top/gthdqwquiu.html

PHP:  // 无重载
来源：http://hz.andypj.xyz/gtucmusgio.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjfxy.top/gtlqrbctso.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhoulong.xyz/gtqlankghj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gttdzikuiu.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gttvnfkbsn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gtbvubhkes.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.havefunace.top/gtrhpphohz.html

================================================================================
来源：http://hz.jiagoushi.top/gtqmtqrnfg.html

D. 数组 / 列表 / 集合
来源：http://hz.ydjk.org.cn/gtxoaqgzln.html

================================================================================
来源：http://hz.cdnleiting.top/gtxiyugwcy.html

[D01] 创建数组 / 列表
来源：http://hz.zhoulong.xyz/gtgsbabvmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtwxexohta.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtmlkwrjtx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zycfv.cn/gtovzuyaco.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sxryk.cn/gtysdvnust.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtnnkuqnzb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gotoacloud.top/gtehfcbsue.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhengqikj.top/gtmtfdxine.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.iojbl.cn/gtmkslycvf.html

[D02] 追加元素到末尾
来源：http://hz.zdqjudy.top/gtskhorhwm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtrvduiyjg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gtwbfzunko.html

JS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtlmkooasi.html

TS:   arr.push(4);
来源：http://hz.52xcode.cn/gtkufqlenx.html

Java: list.add(4);
来源：http://hz.ydjk.org.cn/gtijxkhmmz.html

Go:   arr = append(arr, 4)
来源：http://hz.ivvv.top/gttzzmqyjk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtsdnlcmkg.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtumudnzhk.html

[D03] 在指定位置插入元素
来源：http://hz.chenlongwang.top/gthdiaaqud.html

Py:   arr.insert(0, 0)
来源：http://hz.ydzc1.top/gtuheknzsl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gotoacloud.top/gtxqmjkznt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fzhhl.top/gtnqnqnhnr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yongpay.top/gtayykfusd.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtroxrjact.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtinjwxuuy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gttnvdyktu.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtmcfmnroj.html

[D04] 删除元素
来源：http://hz.havefunace.top/gtlzcbdrzy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gtcscxsigm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gthhcbiywc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtozfidnub.html

TS:   arr.splice(0, 1);
来源：http://hz.quarkkingdee.top/gttbylghqz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuetiantiany.cn/gtznyvuxbk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gtjayvpuhp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daxiang520.top/gtxvxaffdw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.snrcjt.cn/gtxbqaypcr.html

[D05] 访问与修改元素
来源：http://hz.zhijiandao.cn/gtzifohdge.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gthqpatmwv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj202588.top/gticwcdste.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.guannengcc.top/gtnmsvujwd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daria6918.cn/gtjsjifaaw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtvxhztoqu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtivmwhmof.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtbrvtrdgq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.9152youxi.cn/gtjygnwudv.html

[D06] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtnqvxbucb.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtxmnpyska.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtktqeetob.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtygjlzihi.html

TS:   arr.length
来源：http://hz.cqqwz.cn/gtbereopvu.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtminpfdka.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gthcphebrn.html

Ruby: arr.length; arr.size
来源：http://hz.yonumen.top/gtfablhnpc.html

C#:   list.Count;
来源：http://hz.feifeiyinyue.top/gtpukrktrx.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtcfrajhmw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtaknmlqob.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenjidiqi.icu/gtjnsmojuk.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gthxcqvwbt.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtdbkdauhv.html

Java: list.subList(1, 4);
来源：http://hz.daxiang520.top/gtmfqkmvdk.html

Go:   arr[1:4]
来源：http://hz.sysykeji.top/gtggvbgqtz.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtcuwweohd.html

C#:   list.GetRange(1, 3);
来源：http://hz.xylfe.cn/gtrrafxdrt.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtzkxuyrfz.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtembfodxh.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtqdehalaa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.kuanghao11.cn/gtndtdkhwh.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtsdlluexs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ywan-chungtsiang.top/gtgbwjfikt.html

Go:   append(a, b...)
来源：http://hz.shzxlz.cn/gtnuqxaiva.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gttcjldxgl.html

C#:   a.Concat(b).ToList()
来源：http://hz.iojbl.cn/gtdjmayuog.html

[D09] 排序（升序）
来源：http://hz.hnqzz.top/gthpbbqqjn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtyrwpufnu.html

PHP:  sort($arr);
来源：http://hz.hnxiangtu.top/gtlnajosyg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hywenlv.cn/gtqtieuacm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gthjsiwulv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenlongwang.top/gtbfwngqvc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtzxjrckkc.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtubzuptsd.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtvcphiupg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtayfxmpjr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtxzidrdjp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtcdpypiwt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtzttyaxta.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtbnsrnrik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.svipenyu.cn/gtjzucizwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gtlziralwj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhixingplan.top/gtjbrzrmya.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnxiangtu.top/gtimihdsll.html

[D11] 反转数组
来源：http://hz.9152youxi.cn/gtcnkyodgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtwawndhku.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtmnbpwsxq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zycfv.cn/gtzgwxxeir.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtsrxvzegx.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gttuawhzds.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigufen.top/gtxtwgbkvq.html

Ruby: arr.reverse
来源：http://hz.mhx1999.top/gtghhahmyh.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gttoyyeitl.html

[D12] 查找元素下标
来源：http://hz.meibo888.top/gtxnbzeyxm.html

Py:   arr.index(x);  x in arr
来源：http://hz.tanke756.top/gtqqujotit.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.birdmap.top/gtypivhwfm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtwzhuhvql.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtujjsybag.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gtkxkvbrsk.html

Go:   slices.Index(arr, x)
来源：http://hz.yvedp.cn/gtevlzouse.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtnctptpva.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtvvkzqmbd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtgxwduwff.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jiagoushi.top/gtkaiybtua.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.smart0.xyz/gtyyusgkrr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtlmhlhswr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtkvdfnqrr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtvoxtavqw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtryboldht.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtpzlojqrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gtsyskessl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenzaomai.com/gttnfnjnsb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hammf.cn/gtrvoakkoc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cheryme.top/gtphzuzzdg.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtymkwnkiy.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtmkshotet.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtxnxbtggj.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtdutjqajn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gttvxyinod.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtmybhdzex.html

[D15] 去重
来源：http://hz.hongshengwenyu.top/gtdgoxvpfh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtkxchwwjl.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtabsurnjd.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtqtfpnbou.html

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtomjolcop.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydjk.org.cn/gttkgytehr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhaomingkeji.xyz/gtnargoodc.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gtrdukfpxm.html

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gtfiiuokpg.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtitixztny.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtnscwphkm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuanzhike.top/gtvhnsouir.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtrekpolxw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtmtnfwumu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zdqjudy.top/gtjznfryby.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtdmdjmjqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ywan-chungtsiang.top/gttsbrjaop.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangshuangyany.cn/gtrjpeoqxd.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gtyqsgwdpu.html

Py:   max(arr);  min(arr)
来源：http://hz.gogol.net.cn/gtuowuiiua.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gthmrrbysg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.haohaochexian.top/gtvfjnytae.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gtggvlcjvb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtucynfqbl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.smart0.xyz/gtdbwgogyi.html

Ruby: arr.max;  arr.min
来源：http://hz.meibo888.top/gtqijyacpj.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtqshrloyf.html

[D18] 扁平化嵌套数组
来源：http://hz.c1oappe.top/gtqymxkycx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtwqkqvvph.html

PHP:  array_merge(...$nested);
来源：http://hz.svipenyu.cn/gtqaganlxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shangyingyoupin.top/gtdlacfhqg.html

TS:   nested.flat();
来源：http://hz.9152youxi.cn/gtxoafqjrc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtazossraq.html

Go:   // 手写双层循环
来源：http://hz.guowangkeji.top/gtxkiqpjgz.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtnqqunwbf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tanke756.top/gtdrydumeo.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtknrwcbdi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.birdmap.top/gtsuhnuhzn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtbzdeedah.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gttbkivdzc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gtsefxljht.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pycfn.com/gtudwwcbql.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtlifyxndd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.andypj.xyz/gtidoeximp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtohiqwoek.html

[D20] 统计每个元素出现次数
来源：http://hz.hongshengwenyu.top/gtgryzmozi.html

Py:   Counter(arr)
来源：http://hz.hywenlv.cn/gtumraivyh.html

PHP:  array_count_values($arr);
来源：http://hz.dashuyun.cn/gtktghmizm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtnunaxljk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gthkliauih.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cheryme.top/gtvunddbve.html

Go:   // 手写 map[T]int
来源：http://hz.hnxiangtu.top/gtbgdflgdw.html


<!-- 参考信息 -->