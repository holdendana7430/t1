代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtzufkambo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtuirsoldm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuanzx.com/gtfrwzwtui.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jianghu66.top/gtsjlehwgk.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtwpwjchft.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtzpqbpxlk.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtsipglxue.html

[C05] 返回多个值
来源：http://hz.hywenlv.cn/gtdvpudnvh.html

Py:   return a, b
来源：http://hz.daria6918.cn/gtxmjfbfnt.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtchiepjop.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fengsongda.top/gtnlhenqyj.html

TS:   return { a, b };
来源：http://hz.xziqi.cn/gtnmmezcgs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtdbyglojg.html

Go:   return a, b
来源：http://hz.daxiang520.top/gttxqatnwm.html

Ruby: return a, b
来源：http://hz.jqgfzy.top/gtfoupllvu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gttwaiucea.html

[C06] 匿名函数 / lambda
来源：http://hz.meibo888.top/gtktqmedte.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtxfdnsrzx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtcuitypan.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gtiebopwvu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sufxvd.cn/gtyqknnlol.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtkpnrivvn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shangyingyoupin.top/gtuttttmgb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gtckiacqvb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtyuqnolqz.html

[C07] 把函数作为参数传入
来源：http://hz.svipenyu.cn/gtxaurwtyc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yongpay.top/gtxonjsype.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aizwys.cn/gtokrykonf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guannengcc.top/gtphuwiwml.html

TS:   arr.map(String)
来源：http://hz.zhengqikj.top/gtkbetutib.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.svipenyu.cn/gtoiyajuke.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydzc1.top/gtmkwesemz.html

Ruby: arr.map(&:upcase)
来源：http://hz.guannengcc.top/gtdiuxqbtg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtepdpfkbk.html

[C08] 闭包
来源：http://hz.ehwqpu.com/gtxrvqyixc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtnmezmetb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gtfpyxexay.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtdohvdder.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtpwzypknn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinghuilouyu.cn/gtwxwesywm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.feifeiyinyue.top/gthtgizleo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj202588.top/gtosqftorc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtqrgydbwx.html

[C09] 递归
来源：http://hz.shangyingyoupin.top/gtuqnhnvxc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yueranfly.top/gtmennxqyg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gtmoxurbed.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtnxdijlnw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtefapvyou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gtmscqlpmy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gogol.net.cn/gttozizivx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnqzz.top/gtxzcvjnxu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtaygkqlaw.html

[C10] 变量作用域
来源：http://hz.fzhhl.top/gttrkpguph.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenlongwang.top/gtunmpxsws.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gtoazhtwgx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuxming.cn/gtvlqtrxaj.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gteenxpnoo.html

Java: 方法内为块级作用域
来源：http://hz.daria6918.cn/gthsmlqunk.html

Go:   花括号块级作用域
来源：http://hz.quarkkingdee.top/gtcjcjwbfe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hywenlv.cn/gtmxfwmcmu.html

C#:   块级作用域
来源：http://hz.316326.xyz/gtrqtwzqxf.html

[C11] 模块导入与导出
来源：http://hz.0kj1m.cn/gtvksbnbyz.html

Py:   from module import func
来源：http://hz.wangshuangyany.cn/gtjvnltnni.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtokosnwsf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtfyhzkkai.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtwbyiexzm.html

Java: import java.util.List;
来源：http://hz.jyoumei.cn/gtvpkwjrdi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtecuoprzk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtfynwyuza.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gteftkksyp.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtzsiqlplv.html

Py:   (lambda: print("run"))()
来源：http://hz.hammf.cn/gtwufhpdqo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenlongwang.top/gtjpsdemff.html

JS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtrsaofsxe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtvftzsmui.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhengqikj.top/gttfijfxsf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenjidiqi.icu/gtotbdtadv.html

Ruby: -> { puts "run" }.call
来源：http://hz.daxiang520.top/gtpbqwvxkk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guannengcc.top/gttdpmmmqr.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnqzz.top/gtuduvwhpj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenjidiqi.icu/gtgehpkfub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gtmdnanchc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtmpbphdnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gttchawkyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtsneeckdn.html

Go:   func add(a, b int) int
来源：http://hz.52xcode.cn/gtdnmhpxar.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.andypj.xyz/gtzdsgkwrd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zycfv.cn/gtcjxnxzst.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtkvxwwbvd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtmdernpvn.html

PHP:  // 无泛型
来源：http://hz.cdnleiting.top/gtxgnklkya.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtfrvqaxal.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtfbjtkgux.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pengpengdd.cyou/gtkrmrssci.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtfpxtbnjh.html

Ruby: # 无泛型
来源：http://hz.dashuyun.cn/gtvjwpgizv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtxmqtuxji.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtndxxecsw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gthasauscb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gtpdvvdyqh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtgnhtysvd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinyuanbaomall.cn/gthtmdlqln.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtmgtopyhp.html

Go:   // 无解构
来源：http://hz.ydzc1.top/gtuzrqjhjx.html

Ruby: a, b = pair
来源：http://hz.svipenyu.cn/gtcgsretig.html

C#:   var (a, b) = pair;
来源：http://hz.yueranfly.top/gtvqybsaut.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtcspamdzq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fzhhl.top/gtmyczguqs.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtvgdxjjkh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhiwuduotai.top/gttrxdmjjl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zycfv.cn/gtrdffbgpp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.meibo888.top/gtkjtiwejk.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gtxlcbecoc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtaaofbzyq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gzhubu.top/gturdpyqmu.html

================================================================================
来源：http://hz.ybcxt.top/gtbgibbeij.html

D. 数组 / 列表 / 集合
来源：http://hz.0kj1m.cn/gtmpwuramd.html

================================================================================
来源：http://hz.cheryme.top/gtkpicpavs.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gtjlsdmuuq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hysaishi.cn/gtnkndakxx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnqzz.top/gtndrwjits.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258888.top/gtfkzedfpb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.quarkkingdee.top/gtlyymozng.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtdtcurrbn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daxiang520.top/gtteqxdefq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hfpthk.cn/gttrwqmkzx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuxming.cn/gtfqcxnmkn.html

[D02] 追加元素到末尾
来源：http://hz.cqqwz.cn/gtvovjlsqz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtbqqwxgtt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtocwzobmy.html

JS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtyvianatv.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtgpiwnjdj.html

Java: list.add(4);
来源：http://hz.yj202588.top/gtmlmculxi.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gttymuxnwk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cdnleiting.top/gtrtryyzir.html

C#:   list.Add(4);
来源：http://hz.xuetiantiany.cn/gtfkgloihd.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gtqjxtudem.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtdgmwyqht.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yangfankeji.com/gtrfwphqju.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sufxvd.cn/gtlqkavnmv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hammf.cn/gtnwakfvvg.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gtkhmdmlcz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtufzoyuur.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gtetphmzwx.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gtfekpzfcw.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtvlyesstn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtqivkkpjf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtlvwimoqd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtvdkkscac.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtdhhopkjb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuanzx.com/gtbepkonym.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gtpiszgnpm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.bjfxy.top/gtymrnuexc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yongpay.top/gthrtjbsmv.html

[D05] 访问与修改元素
来源：http://hz.daxiang520.top/gthtldudpt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtjdqvwpga.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtqjyurlcm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.haohaochexian.top/gtwzhgatdv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydjk.org.cn/gtihzagrwh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tian-w.cn/gtkxycpwaj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtynlnfglx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtlblnadpm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fzhhl.top/gtbwacsizq.html

[D06] 数组长度
来源：http://hz.jqgufenzy.top/gtfouszwug.html

Py:   len(arr)
来源：http://hz.fzhhl.top/gtfcaocekl.html

PHP:  count($arr);
来源：http://hz.jinyuanbaomall.cn/gtlihohnqs.html

JS:   arr.length
来源：http://hz.snrcjt.cn/gtswgppbyj.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtkvehnurl.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtmxjutecz.html

Go:   len(arr)
来源：http://hz.zhixingplan.top/gthprfiklc.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtbrifmfbu.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtbpifoazt.html

[D07] 切片 / 取子数组
来源：http://hz.cdnleiting.top/gthkttiszp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ehwqpu.com/gtlqtmjqkx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtylkifcxe.html

JS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtxylfujvs.html

TS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gtkrsutqjg.html

Java: list.subList(1, 4);
来源：http://hz.jinqigfzy.top/gtadqjxhvx.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtfjmhnmnk.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtfcmknfll.html

C#:   list.GetRange(1, 3);
来源：http://hz.52xcode.cn/gtptbrutgw.html

[D08] 合并两个数组
来源：http://hz.0kj1m.cn/gtacytgfyt.html

Py:   a + b;  a.extend(b)
来源：http://hz.svipenyu.cn/gthiltnysy.html

PHP:  array_merge($a, $b);
来源：http://hz.jianghu66.top/gtlpolafxd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtdqxgsqha.html

TS:   [...a, ...b];
来源：http://hz.dianchejie.cn/gtixozsyjw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gotoacloud.top/gtcxceqdeq.html

Go:   append(a, b...)
来源：http://hz.daxiang520.top/gtucsbkrnl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtfexwglgd.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangtech.top/gtpskhxloh.html

[D09] 排序（升序）
来源：http://hz.xingfuxueyuan.xyz/gtxmipjxbh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtvjcrlhla.html

PHP:  sort($arr);
来源：http://hz.dashuyun.cn/gtfmihfvpn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuanzhike.top/gtbhsqgiko.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gtwmhesxpj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258888.top/gtxxgqjxxt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.smart0.xyz/gtnawwhvbm.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtpghqkype.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gtjnwrwfsp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ybcxt.top/gtyuyrlppn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtyovclmad.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtcvvxctmj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gthpwhxghv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gttvreilic.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258888.top/gtehryxzxx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtqoyjjyra.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zycfv.cn/gtmqdvkebr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gtevlfxgnh.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtwwiwyhsi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.kuanghao11.cn/gtytskilrv.html

PHP:  array_reverse($arr);
来源：http://hz.dianchejie.cn/gtazolhjai.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258.top/gtaxxsmcrp.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtvuychctl.html

Java: Collections.reverse(list);
来源：http://hz.ehwqpu.com/gtzpdxlqgy.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtatiayega.html

Ruby: arr.reverse
来源：http://hz.ydzc1.top/gtioxbbprj.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtyxfwsdxt.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtpnwwgnzl.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gthulofjpb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yvedp.cn/gtlicrvyrt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtqamckwfi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtlszurems.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigfzy.top/gtiwkmzyuq.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtbidjejzw.html

Ruby: arr.index(x)
来源：http://hz.snrcjt.cn/gtojsdgsuz.html

C#:   list.IndexOf(x);
来源：http://hz.guowangkeji.top/gtichgdjto.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnqzz.top/gtohgrctpz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cucudq.cn/gtbnkmncej.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gtguzopyfn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gthlzddeha.html

TS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtyawgjkyv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gtvtoesgdd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tian-w.cn/gtnmffzxox.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.52xcode.cn/gtsxtgvgla.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtuqtkwvwk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xinyue.icu/gtypzvvkiu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gtqcnyjklz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shzxlz.cn/gtraneqzyz.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtxokghrpd.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtipsmeyya.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhixingplan.top/gtrbowlvdy.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtewozbibd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtzthedane.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangdashe.top/gtuyttmsoi.html

[D15] 去重
来源：http://hz.fzhhl.top/gtggowiktb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtjunbofct.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtdgskudrk.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtqkywkbre.html

TS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtuvurighw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gtajangque.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtkuumtdcw.html

Ruby: arr.uniq
来源：http://hz.daria6918.cn/gtsgcfojss.html

C#:   list.Distinct().ToList()
来源：http://hz.mhx1999.top/gttfbqldzd.html

[D16] 求和与平均值
来源：http://hz.fengsongda.top/gtoyxqpbos.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtdrayyzoj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gtyxxdsibm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.feifeiyinyue.top/gtarnjvknw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtpcunusuu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtxdkldntf.html

Go:   // 手写循环累加
来源：http://hz.bjfxy.top/gtqunfltoy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.52xcode.cn/gtedjwkoir.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtbchbrohq.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtpsfptsao.html

Py:   max(arr);  min(arr)
来源：http://hz.yj202588.top/gtrlkarpin.html

PHP:  max($arr);  min($arr);
来源：http://hz.jianghu66.top/gtafqxracn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guannengcc.top/gtbnsrioof.html

TS:   Math.max(...arr);
来源：http://hz.sweek.top/gtrpjokhnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtcxttqowq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtdfmgpokr.html

Ruby: arr.max;  arr.min
来源：http://hz.gaohongyu789.top/gtslkafeae.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtbayzusfb.html

[D18] 扁平化嵌套数组
来源：http://hz.ydjk.org.cn/gttszddgao.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pycfn.com/gtnsmsmlep.html

PHP:  array_merge(...$nested);
来源：http://hz.vqdsnc.cn/gtgkltsnxt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtusnkrjlc.html

TS:   nested.flat();
来源：http://hz.zhengqikj.top/gturctyenz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtararnuum.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtaacynpwd.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gtleqjqpsr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtpejcpyfa.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtnowwmlbr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pycfn.com/gtmubtcnra.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gttcinruep.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtijuutmen.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtgngzinec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gtbjghjday.html

Go:   // 手写 map[string][]T
来源：http://hz.guannengcc.top/gtklwkmpbi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nwbrower.top/gtfjfgheik.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtbxayjelo.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtepcumiqk.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gtdubznjre.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258888.top/gtkgsrsdgb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nwbrower.top/gtqjqhvfgc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtrvarfrvp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hnxiangtu.top/gtmvypffms.html

Go:   // 手写 map[T]int
来源：http://hz.dianchejie.cn/gtblqvlylc.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtzybyqkjl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.mhx1999.top/gtxrcxjqnj.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtiparwmej.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtfdaizpse.html


<!-- 参考信息 -->