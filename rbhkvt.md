代发 wailian999

Py:   return a, b
来源：http://hz.haohaochexian.top/gtbofbsops.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtwwbxiscc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtnqbopabn.html

TS:   return { a, b };
来源：http://hz.chenzaomai.com/gtniukgysn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenlongwang.top/gttrztjiua.html

Go:   return a, b
来源：http://hz.mhx1999.top/gtjbueqcgg.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gttcxpzmwl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hywenlv.cn/gtryqjzcud.html

[C06] 匿名函数 / lambda
来源：http://hz.hnxiangtu.top/gtopweokjb.html

Py:   square = lambda x: x * x
来源：http://hz.316326.xyz/gtyifbkajn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtnlktgqrk.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtmlvxfrgy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cqqwz.cn/gtopukfbwu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigufen.top/gtzrzzphkl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtuuquvrdk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtfhvxrkbs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangdashe.top/gtvbhzkbxh.html

[C07] 把函数作为参数传入
来源：http://hz.ppjwa.cn/gtwydcifba.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hammf.cn/gtmcrjfkrn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.andypj.xyz/gttibajojz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daria6918.cn/gtzecbvlqu.html

TS:   arr.map(String)
来源：http://hz.tanke756.top/gttdjareac.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.0kj1m.cn/gtjdsvlkgk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cashguo.top/gtnvbumker.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258.top/gtegxqtkqm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtsbseiikz.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtkxurgpme.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cqqwz.cn/gtzdiklsug.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuetiantiany.cn/gtwbfdzzsd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtgsrwunul.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtssqgiczg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yongpay.top/gtmtxceiry.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtompecqon.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.c1oappe.top/gturicgnfo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtganmhsky.html

[C09] 递归
来源：http://hz.ywan-chungtsiang.top/gtburojtgh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtlusugzuc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.nanxuanxn.top/gtgdbswfpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtolxzaket.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtzapmimeg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ybcxt.top/gtgpucldjl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jianghu66.top/gtbozptqbj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtexdhuynw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangshuangyany.cn/gthymzhkdf.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtwusisijd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pengpengdd.cyou/gtvkewoijs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtqogjsyjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnqzz.top/gtngwgmtrq.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtqpfebibd.html

Java: 方法内为块级作用域
来源：http://hz.jiagoushi.top/gtvjjvjwfa.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtlkoosqvm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gtahimtotq.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gtrvqgobom.html

[C11] 模块导入与导出
来源：http://hz.hywenlv.cn/gtdyubrrac.html

Py:   from module import func
来源：http://hz.guowangkeji.top/gtcjdnfycw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtrhvqxuak.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtjwhdjefu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxuanxn.top/gtzyeanjxj.html

Java: import java.util.List;
来源：http://hz.shanyushiyangtech.top/gtcrsufuks.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhaomingkeji.xyz/gtpttdnkbf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtxhblnmdq.html

C#:   using System.Text;
来源：http://hz.meibo888.top/gtchwmwqfs.html

[C12] 立即执行函数 IIFE
来源：http://hz.guannengcc.top/gtrgtnhrvn.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gtaomdgxsu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gtdtnzgkoa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtwgamhtwm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtponrrwnq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenzaomai.com/gttjblejeb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtxbknhlay.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtxlujnkld.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.feifeiyinyue.top/gtkwwrzmom.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gttadoxlwj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtczvrmiom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gthauoytfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.bjfxy.top/gtrmcmntfx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtntqotkxg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gthskzhnum.html

Go:   func add(a, b int) int
来源：http://hz.jqgufenzy.top/gtnhecgoaw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ywan-chungtsiang.top/gtfvsuzsrw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuxming.cn/gtmbnnrtme.html

[C14] 泛型函数
来源：http://hz.gotoacloud.top/gtsvzywlzw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cqqwz.cn/gtageuftin.html

PHP:  // 无泛型
来源：http://hz.shzxlz.cn/gtlkyhfhjk.html

JS:   // 无泛型
来源：http://hz.dianchejie.cn/gtpirhzkwe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gttabwkpqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtbvvtszkx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aibaodan.cn/gtqtdgcpys.html

Ruby: # 无泛型
来源：http://hz.wangdashe.top/gtisyafbyo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258888.top/gtnlkgxseh.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gttnmtrhle.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhongyouzk.top/gtunlumbgo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtxufxmotw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtclwbaydw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuanzhike.top/gttmtnthxb.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtmwatkkme.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gtwyvyqyrd.html

Ruby: a, b = pair
来源：http://hz.svipenyu.cn/gtkbadebit.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtqecqjdcf.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtkwzqayrd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ivvv.top/gtcldpvlkb.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gtgajryagx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtavfymkyx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtxionhvke.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ehwqpu.com/gtjiumzmtd.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gtnknommsh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hammf.cn/gtnqxrllpx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtbwzjucbg.html

================================================================================
来源：http://hz.gogol.net.cn/gttyifthto.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gtxggrwrer.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtniuydung.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtpwjcvqqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shangyingyoupin.top/gtnysnthor.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hfpthk.cn/gtvsisndjz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.quarkkingdee.top/gtfbvblzsd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtsjnbvqay.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hfpthk.cn/gtrqsqnhtp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtrixpdono.html

Ruby: arr = [1, 2, 3]
来源：http://hz.andypj.xyz/gtzpbiyqot.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtjlpdudxd.html

[D02] 追加元素到末尾
来源：http://hz.hysaishi.cn/gteycdqarc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtbcthfcpn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtbepgaynb.html

JS:   arr.push(4);
来源：http://hz.cheryme.top/gtieqilizb.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtigefxyyy.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gtvbiucouf.html

Go:   arr = append(arr, 4)
来源：http://hz.tianlin.xyz/gtubqjrppr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dianchejie.cn/gtwoeqxgve.html

C#:   list.Add(4);
来源：http://hz.jianghu66.top/gtcjaebdag.html

[D03] 在指定位置插入元素
来源：http://hz.svipenyu.cn/gttmtrkuvp.html

Py:   arr.insert(0, 0)
来源：http://hz.zycfv.cn/gtorxgyiif.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shuidangran.top/gtnbkuthxh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yonumen.top/gtnkgtwhhm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangdashe.top/gtwweftonz.html

Java: list.add(0, 0);
来源：http://hz.cdnleiting.top/gtqxawqwnt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tianlin.xyz/gtlhkobeyp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtyxwhsjxn.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gtfvgpcoji.html

[D04] 删除元素
来源：http://hz.quarkkingdee.top/gtmffdueji.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.svipenyu.cn/gtbitofgse.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gtuzlvrshh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gtejxyhesj.html

TS:   arr.splice(0, 1);
来源：http://hz.jianghu66.top/gthmkmeybs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtdlnyvpmx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tianlin.xyz/gtdgwxzxme.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydzc1.top/gtqbasqspy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtjlslpeft.html

[D05] 访问与修改元素
来源：http://hz.hongshengwenyu.top/gtyszvjkkl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtgnrlrxrz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tanke756.top/gtyoatchud.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.andypj.xyz/gtnvauctmr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tian-w.cn/gtbsxzhmom.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtmfrvidpe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtwsydbwyx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtgpontmnc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtuywdnhri.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtsaftbgot.html

Py:   len(arr)
来源：http://hz.cdnleiting.top/gttinxqejb.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtxkmitikn.html

JS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtaxcymlvm.html

TS:   arr.length
来源：http://hz.yvedp.cn/gtpkqyopna.html

Java: list.size();
来源：http://hz.jqgufenzy.top/gtlocxsfwu.html

Go:   len(arr)
来源：http://hz.pengpengdd.cyou/gtdicfbuol.html

Ruby: arr.length; arr.size
来源：http://hz.yonumen.top/gtcqvndeik.html

C#:   list.Count;
来源：http://hz.hnqzz.top/gtxvnbazcf.html

[D07] 切片 / 取子数组
来源：http://hz.zhijiandao.cn/gtbnhnlhlq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangkeji.top/gtaxktozbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gtgwksjpin.html

JS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gtihfeoreb.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtrfyifdlk.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtkhjykfxa.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtpmagtyjd.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtczildjur.html

C#:   list.GetRange(1, 3);
来源：http://hz.shzxlz.cn/gtpjiwgdnx.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtpdqvlhay.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhengqikj.top/gtogrzvaxy.html

PHP:  array_merge($a, $b);
来源：http://hz.zhijiandao.cn/gtahsvksqp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sufxvd.cn/gtegrhowpb.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtozmbosyq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtjedblewy.html

Go:   append(a, b...)
来源：http://hz.jinqigufen.top/gthcxscujr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daxiang520.top/gtpyxkbslb.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtpkzuqzet.html

[D09] 排序（升序）
来源：http://hz.hammf.cn/gtbdkkehwh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtfvxtkjdn.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtkkdgfmvn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.redwolf501.top/gtvgoxvvks.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.316326.xyz/gtlrcratix.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gthnabigag.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zycfv.cn/gtxlikbyes.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtxukbnrqd.html

C#:   list.Sort();
来源：http://hz.zdqjudy.top/gtpcxflbve.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtcosxfvyr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.smart0.xyz/gteohunkta.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtsegrvmzw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtjdpetmio.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtsznchibh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yangfankeji.com/gtttbykwzr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.redwolf501.top/gtspuuzcye.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtqoywzgwe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.snrcjt.cn/gtekbecljc.html

[D11] 反转数组
来源：http://hz.sysykeji.top/gtngbybzua.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gogol.net.cn/gtwbaivqjl.html

PHP:  array_reverse($arr);
来源：http://hz.sysykeji.top/gtmlkeyfdb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cucudq.cn/gtxvdjzyjx.html

TS:   [...arr].reverse();
来源：http://hz.gaohongyu789.top/gttoyybvkg.html

Java: Collections.reverse(list);
来源：http://hz.yj202588.top/gtdyzhwpva.html

Go:   slices.Reverse(arr)
来源：http://hz.shuidangran.top/gtimoxelnd.html

Ruby: arr.reverse
来源：http://hz.sweek.top/gtarcqkuad.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtxioairda.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtgllxownr.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtwadspkqn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnxiangtu.top/gtapcjudws.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtvpduzcle.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhiwuduotai.top/gttlfktboz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtiewmccvi.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtnzqyehpf.html

Ruby: arr.index(x)
来源：http://hz.tianlin.xyz/gtxcdajnwt.html

C#:   list.IndexOf(x);
来源：http://hz.dashuyun.cn/gtrtjvdgee.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xinyue.icu/gtrloyhbzp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.9152youxi.cn/gttmalqpcu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtxuqebzdg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gthovyvadi.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtxbuocwpa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtjkpiliog.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hywenlv.cn/gtdixdsnwl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtaggatzhm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenlongwang.top/gtuhslwuda.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cheryme.top/gtbeebwrri.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zycfv.cn/gtmzepgzyi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jyoumei.cn/gtclvqkzne.html

JS:   arr.map(x => x * 2)
来源：http://hz.pengpengdd.cyou/gthofgfmeg.html

TS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtuwdqnyzr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ywan-chungtsiang.top/gtlfkbnmnu.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtbkfulfot.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuanzx.com/gtocawpbsf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.c1oappe.top/gtvokdqnfw.html

[D15] 去重
来源：http://hz.cqqwz.cn/gtizbvcvex.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gtxjaipwtx.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtjgbynslj.html

JS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtbgreaxvp.html

TS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtybvzrowx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gzhubu.top/gtrwpkywsz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtrbdorsof.html

Ruby: arr.uniq
来源：http://hz.bjfxy.top/gtgxnqiyxh.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtunejzyio.html

[D16] 求和与平均值
来源：http://hz.andypj.xyz/gtzwgfwzdq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sxryk.cn/gtorhdfyjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtyhwixweh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtsfgmkydj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtpjdotqgx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtskagrmxo.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtkfkbpsps.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gtgtwybppr.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtratlsxtc.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtnfodnurx.html

Py:   max(arr);  min(arr)
来源：http://hz.zhengqikj.top/gtkykqtcta.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuxming.cn/gtpbrivsal.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtacspedgz.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gttsacgvxn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtsvetoqkg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtglkbvswb.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gtfvlsalqk.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxuanxn.top/gtojayweak.html

[D18] 扁平化嵌套数组
来源：http://hz.redwolf501.top/gtvabvzibs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxuanxn.top/gtlxxrrjvs.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gthcecwsey.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.0kj1m.cn/gtrcohutwd.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtloocrzcy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gttsuoxken.html

Go:   // 手写双层循环
来源：http://hz.xziqi.cn/gtldkkfcux.html

Ruby: nested.flatten
来源：http://hz.chenzaomai.com/gtnjdgiago.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ybcxt.top/gtstbyhwka.html

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtmzfhmxtp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtxcohawbi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtkgwxgrdu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenjidiqi.icu/gtakhozflr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gtuhyeqwdp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.iojbl.cn/gtnetbjptv.html

Go:   // 手写 map[string][]T
来源：http://hz.dashuyun.cn/gtjyixoano.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtnjnvpcor.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuanzhike.top/gtkyvcvrig.html

[D20] 统计每个元素出现次数
来源：http://hz.havefunace.top/gtwbktzuog.html

Py:   Counter(arr)
来源：http://hz.daria6918.cn/gtlexlnejm.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtwsmfrbnb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtokymtder.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtabblahrm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hnxiangtu.top/gtgustscam.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtxztuyunp.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtftjwhwse.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuetiantiany.cn/gtiacmgrua.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtretdueig.html

Py:   x in arr
来源：http://hz.ivvv.top/gtfaiycnvw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhongyouzk.top/gtveofejpi.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtoisycjsg.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gthxvttlbt.html

Java: list.contains(x)
来源：http://hz.ppjwa.cn/gtbcnwmdby.html

Go:   slices.Contains(arr, x)
来源：http://hz.pengpengdd.cyou/gtmkwfifvq.html

Ruby: arr.include?(x)
来源：http://hz.yvedp.cn/gtygtaijad.html

C#:   list.Contains(x)
来源：http://hz.jiagoushi.top/gtenizhwzb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.vqdsnc.cn/gtnwwquqsg.html


<!-- 参考信息 -->