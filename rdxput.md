代发 wailian999

Py:   return a, b
来源：http://hz.svipenyu.cn/gttnzsltgp.html

PHP:  return [$a, $b];
来源：http://hz.jiagoushi.top/gtszvwpuhv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gthwhuzymn.html

TS:   return { a, b };
来源：http://hz.yangfankeji.com/gtiarwkbyi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtjkpntuzd.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gtenhiyckj.html

Ruby: return a, b
来源：http://hz.xuanzx.com/gtnjmaucop.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.andypj.xyz/gtgtjtmwog.html

[C06] 匿名函数 / lambda
来源：http://hz.xinyue.icu/gttvitwlry.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtrmdjdvug.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jianghu66.top/gtlmpvrohx.html

JS:   const square = x => x * x;
来源：http://hz.316326.xyz/gtvmssrjnz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ivvv.top/gtajxbgcjb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.bjfxy.top/gtsxrsfytf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.0kj1m.cn/gtvaezqvzj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gtoqwcqvhy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cheryme.top/gtgktptiie.html

[C07] 把函数作为参数传入
来源：http://hz.hongshengwenyu.top/gtxxinfamv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sweek.top/gtxafrvnsc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.feifeiyinyue.top/gtjptrnqim.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangshuangyany.cn/gtvqpepdng.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtibxfqpaj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cucudq.cn/gtefqbzbpd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnxiangtu.top/gtpofbgefe.html

Ruby: arr.map(&:upcase)
来源：http://hz.dianchejie.cn/gtiydnsppz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hywenlv.cn/gtxsinjcrl.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtctdytkgw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhiwuduotai.top/gtecsewlrl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guowangkeji.top/gtoimrpnrv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtjzsyyfqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtwhkdsqoq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zdqjudy.top/gtyfilutkh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtjatglmpb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtsjwkhpnf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtdzkelzkw.html

[C09] 递归
来源：http://hz.zhengqikj.top/gtibdaiyhd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.mhx1999.top/gtqvqwnbki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.c1oappe.top/gtlmdpqbtp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtsochxqsy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gttwkdzcxs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtjkvzryjb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgufenzy.top/gtyqcccire.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cheryme.top/gtwtmdxyrh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtaibypmhj.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gttjzkabfy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.52xcode.cn/gtwaxybbmf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.svipenyu.cn/gtbwcbywvu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.vqdsnc.cn/gtfmyxurtz.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtpcdppvss.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtpokjxcym.html

Go:   花括号块级作用域
来源：http://hz.52xcode.cn/gtnrshdirh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtxaovjlbq.html

C#:   块级作用域
来源：http://hz.yanxiufei.cn/gtblgtkkph.html

[C11] 模块导入与导出
来源：http://hz.hfpthk.cn/gtnlyyptns.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtimvsvpra.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gotoacloud.top/gttcrncfav.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gogol.net.cn/gtnlkkxxws.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtdgyumhis.html

Java: import java.util.List;
来源：http://hz.yuanzhike.top/gtcxhhkvum.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hfpthk.cn/gtkcppujab.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtqrylcruy.html

C#:   using System.Text;
来源：http://hz.tian-w.cn/gtyguzbwqt.html

[C12] 立即执行函数 IIFE
来源：http://hz.fzhhl.top/gtbfclvufo.html

Py:   (lambda: print("run"))()
来源：http://hz.ydjk.org.cn/gtedcjitxj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xinyue.icu/gtzmrnuvla.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtlynmfkoe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtezzyjflz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtcrbdltnb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtjssuqrom.html

Ruby: -> { puts "run" }.call
来源：http://hz.yangfankeji.com/gtbqdjviqw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tanke756.top/gtspeprugj.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhixingplan.top/gtqxrggwqa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pycfn.com/gtzmihydod.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtfzavzlpc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.andypj.xyz/gtoiglkxbg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtimkaospc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtwbuwltun.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtxhusupmn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.mhx1999.top/gtfxioepyq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtbobagmah.html

[C14] 泛型函数
来源：http://hz.hfpthk.cn/gtkljjzcpc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigufen.top/gtoemcighv.html

PHP:  // 无泛型
来源：http://hz.cucudq.cn/gtaqohxcop.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gtwzkoldvd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gtznwevpfh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gotoacloud.top/gtnkswgutr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daxiang520.top/gtpbtppcvx.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gtmnfluwsh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtsxtjlslw.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtzebpjebz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtkiljdcaa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtbagcoqsz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtwsnmhqlj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenzaomai.com/gtiuskiedg.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtuwmqzegz.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtkrchnijo.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtduzdppha.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtrkjsejia.html

[C16] 函数 / 方法重载
来源：http://hz.dashuyun.cn/gtbcfbmwfl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.316326.xyz/gtwszbewsp.html

PHP:  // 无重载
来源：http://hz.feifeiyinyue.top/gtcktjyqxy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.redwolf501.top/gtunljpndo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.52xcode.cn/gteygzdvlg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sweek.top/gtcszdydrh.html

Go:   // 无重载：用不同函数名
来源：http://hz.bjfxy.top/gtnwdnbdgq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.9152youxi.cn/gtkjhxbrxl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtoedtvqqn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjfsdyzwe.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtciiqupfz.html

================================================================================
来源：http://hz.sweek.top/gtmphmhegn.html

[D01] 创建数组 / 列表
来源：http://hz.sweek.top/gtzemkyiiy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtyceeesee.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tanke756.top/gtignusynx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zycfv.cn/gtyvjkrudw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtbekgrvbn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtnaodocxb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangshuangyany.cn/gtshyvkguj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gogol.net.cn/gtdneteurc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangdashe.top/gtrmjknftp.html

[D02] 追加元素到末尾
来源：http://hz.guowangkeji.top/gtjyyxnvuf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gttoqqanrd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuxming.cn/gtrvysgmyf.html

JS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtmbmqmkep.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtjolhfqlm.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gtvjoslcug.html

Go:   arr = append(arr, 4)
来源：http://hz.cheryme.top/gtfstjlpln.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xziqi.cn/gtkcxizyom.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gtcgvvywbf.html

[D03] 在指定位置插入元素
来源：http://hz.mhx1999.top/gtcqfeuhwy.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtjaklyims.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dashuyun.cn/gtqrcsdhpq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtvtecqhat.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pengpengdd.cyou/gtvxzenfns.html

Java: list.add(0, 0);
来源：http://hz.zdqjudy.top/gtwfhemwfk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gogol.net.cn/gtnfnpdmeg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tian-w.cn/gtalpdiukv.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtwrshkfll.html

[D04] 删除元素
来源：http://hz.shangyingyoupin.top/gticysizun.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhaomingkeji.xyz/gtiljgtlii.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daria6918.cn/gtaojbxycu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gttswibrcn.html

TS:   arr.splice(0, 1);
来源：http://hz.vqdsnc.cn/gtjtlerbvk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.9152youxi.cn/gtqpeczjyq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ehwqpu.com/gtqrmaziqa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cqqwz.cn/gthalxrpwy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gthcapycxs.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gthmvhyosc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtqclgigzd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtkyanekor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.c1oappe.top/gtmkxyhjep.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtkiiesxry.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gtaeuqbidy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtftiarhhw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtiradsmuq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhiwuduotai.top/gtqataesza.html

[D06] 数组长度
来源：http://hz.aibaodan.cn/gtgbpdtzad.html

Py:   len(arr)
来源：http://hz.dashuyun.cn/gtlfxcxjzq.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtquygmlmk.html

JS:   arr.length
来源：http://hz.bjfxy.top/gtarqovcih.html

TS:   arr.length
来源：http://hz.hfpthk.cn/gtmsntaaac.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtiomdqxea.html

Go:   len(arr)
来源：http://hz.fzhhl.top/gtuanbmsew.html

Ruby: arr.length; arr.size
来源：http://hz.hfpthk.cn/gtyeyvigrt.html

C#:   list.Count;
来源：http://hz.andypj.xyz/gtjkuxklnb.html

[D07] 切片 / 取子数组
来源：http://hz.zhaomingkeji.xyz/gtkyahlkke.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gotoacloud.top/gtlgmznjre.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtpbmunbek.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtkqrvfpoi.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtifckctrf.html

Java: list.subList(1, 4);
来源：http://hz.kuanghao11.cn/gtvvpvmehi.html

Go:   arr[1:4]
来源：http://hz.vqdsnc.cn/gtsfowlcjr.html

Ruby: arr[1, 3]
来源：http://hz.zhengqikj.top/gtrvcrsons.html

C#:   list.GetRange(1, 3);
来源：http://hz.sufxvd.cn/gthnfgsvzz.html

[D08] 合并两个数组
来源：http://hz.meibo888.top/gtxacqsxsz.html

Py:   a + b;  a.extend(b)
来源：http://hz.fengsongda.top/gtzktegcmr.html

PHP:  array_merge($a, $b);
来源：http://hz.vqdsnc.cn/gtpfvxgmtr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnqzz.top/gtdlrdrtyc.html

TS:   [...a, ...b];
来源：http://hz.chenjidiqi.icu/gttmarllcn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtvyfbxwct.html

Go:   append(a, b...)
来源：http://hz.jinghuilouyu.cn/gtflqybsio.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtyrscsstv.html

C#:   a.Concat(b).ToList()
来源：http://hz.kuanghao11.cn/gtnnvctzzw.html

[D09] 排序（升序）
来源：http://hz.zdqjudy.top/gtvjiaqwwd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtyylcyqea.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtkglkaedm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shangyingyoupin.top/gtnrpxjgrm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.bjfxy.top/gtdgbzgkao.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtyohmobug.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtnzwstcix.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtnvligysw.html

C#:   list.Sort();
来源：http://hz.birdmap.top/gtunedawhw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuxming.cn/gtldvpwwbx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtxwfvvvrj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gotoacloud.top/gtknkxxhgf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtvepkmvig.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtilxkosgx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dianchejie.cn/gtrgspfjnl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ehwqpu.com/gtzgcxbnpi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gogol.net.cn/gthqxqzkla.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtelygddhj.html

[D11] 反转数组
来源：http://hz.fengsongda.top/gtbruindus.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinghuilouyu.cn/gtxzzfqfbc.html

PHP:  array_reverse($arr);
来源：http://hz.guannengcc.top/gtkfnlsrgk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gthrgmnspp.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtptmitebf.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtetxiefsm.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gthvaxkvmy.html

Ruby: arr.reverse
来源：http://hz.sufxvd.cn/gttqhqoesm.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtgehurykq.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gthdjblqtd.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gtrgaierek.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxinkj.top/gtzxcwqftl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtdwneafzn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtxnlzhnww.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gtxjmuimff.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gteuvshpht.html

Ruby: arr.index(x)
来源：http://hz.shangyingyoupin.top/gtimzlnyzf.html

C#:   list.IndexOf(x);
来源：http://hz.gzhubu.top/gthmdwqhzu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtaacfosel.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fzhhl.top/gtmlgoxwzo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigufen.top/gtupyqnmer.html

JS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtufbxheto.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtbsaudihq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtzhybfgxx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtzzvltubb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtaxcbnnmx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuxming.cn/gtjwpmzgvs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtxrlsjoew.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtqgzxscvi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtucmjykdg.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtdneeyicz.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtrvoubzif.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtemldmsqa.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gteexlosss.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtdxhcyynf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sxryk.cn/gtbaiupjbr.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtmsuvzjpe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtgexfospm.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtswujxanl.html

JS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtuqbxrkci.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtpjqmnxor.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhaomingkeji.xyz/gtijbospok.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuetiantiany.cn/gtndbbmzvb.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gtgwuynkzw.html

C#:   list.Distinct().ToList()
来源：http://hz.hongshengwenyu.top/gtbaifmuyx.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtrhnhegck.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gtgcxajhtd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhoulong.xyz/gtahhfgzwo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtoncwelvc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gtwnyxdebx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtwcpnbkay.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gthatficzj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtahgmywzl.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtgceenlxx.html

[D17] 最大值与最小值
来源：http://hz.dianchejie.cn/gtafixzrxy.html

Py:   max(arr);  min(arr)
来源：http://hz.gzhubu.top/gtgmdmeixh.html

PHP:  max($arr);  min($arr);
来源：http://hz.smart0.xyz/gtxxovpdqz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yongpay.top/gtdcewaiwo.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtesdnaqca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtcsztvxws.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.9152youxi.cn/gtrmrelhvc.html

Ruby: arr.max;  arr.min
来源：http://hz.kuanghao11.cn/gtgspzdhtu.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtfgktozge.html

[D18] 扁平化嵌套数组
来源：http://hz.vqdsnc.cn/gtxpnebvle.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pycfn.com/gtizkvcwde.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtbbeeahur.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.kuanghao11.cn/gtfvdqrknc.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtwwqkvxjt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jlsjyb.cn/gtchgzvzhz.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gthctvloic.html

Ruby: nested.flatten
来源：http://hz.iojbl.cn/gtwdiwkole.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtsmyivurg.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gtownizvbh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gtsfihizdi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangdashe.top/gtpnwnznvu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sufxvd.cn/gtdbfpmvab.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtwomdymlg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.0kj1m.cn/gtduoblhbl.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtwwcwmwwr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.svipenyu.cn/gtqlnyrbjx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtmehwwzrm.html

[D20] 统计每个元素出现次数
来源：http://hz.redwolf501.top/gtebthoisw.html

Py:   Counter(arr)
来源：http://hz.xingfuxueyuan.xyz/gtolrxaprs.html

PHP:  array_count_values($arr);
来源：http://hz.tianlin.xyz/gtdjolxchn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtrsvjhffq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtggmobgvn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.havefunace.top/gtmynkinih.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtsyyfmnsz.html

Ruby: arr.tally
来源：http://hz.guannengcc.top/gtxukhbtoy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.andypj.xyz/gtvzfdpbdv.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangkeji.top/gtowpulzrc.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gthbzfyeyv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtjqcteexy.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtisguyogl.html

TS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtzsfmerkg.html

Java: list.contains(x)
来源：http://hz.pengpengdd.cyou/gtevqspjoy.html

Go:   slices.Contains(arr, x)
来源：http://hz.havefunace.top/gtslztwrac.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtslehoymu.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtrpmdxonz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.feifeiyinyue.top/gtkplspsmt.html


<!-- 参考信息 -->