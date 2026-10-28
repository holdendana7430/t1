代发 wailian999

Py:   return a, b
来源：http://hz.tianlin.xyz/gtglaokjmw.html

PHP:  return [$a, $b];
来源：http://hz.guowangkeji.top/gthzzonozt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jyoumei.cn/gtwmhkjvyi.html

TS:   return { a, b };
来源：http://hz.cdnleiting.top/gtoiqtyukk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhixingplan.top/gtvleuedwi.html

Go:   return a, b
来源：http://hz.meibo888.top/gtcvojxdhj.html

Ruby: return a, b
来源：http://hz.zdqjudy.top/gtqjnhitbf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhixingplan.top/gtxpgzhepe.html

[C06] 匿名函数 / lambda
来源：http://hz.xingfuxueyuan.xyz/gtrwdjmjxc.html

Py:   square = lambda x: x * x
来源：http://hz.jqgufenzy.top/gtjnaimfoe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yvedp.cn/gtirfvxhzx.html

JS:   const square = x => x * x;
来源：http://hz.shuidangran.top/gtdcdzkumh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgfzy.top/gtuptwtmoq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtcspwqxcp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtixzuiihm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtfmudyfgw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhongyouzk.top/gtyhydyjao.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtpjgviykw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tianlin.xyz/gttnzfxmfk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zdqjudy.top/gtruwzwdff.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gtzfwhxkjz.html

TS:   arr.map(String)
来源：http://hz.hywenlv.cn/gtdaqnrvmg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenjidiqi.icu/gttbyzjbku.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cashguo.top/gtultuxono.html

Ruby: arr.map(&:upcase)
来源：http://hz.aizwys.cn/gtsnkjndur.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj202588.top/gtvwsoqpnp.html

[C08] 闭包
来源：http://hz.tanke756.top/gtbaxrhaxj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtestfnztj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yanxiufei.cn/gturqrarcf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtrerxetpv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtijvrssvh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydjk.org.cn/gthgmtydai.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.daria6918.cn/gtizwegkuc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daria6918.cn/gtedamgamw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtycqxxwaz.html

[C09] 递归
来源：http://hz.ydjk.org.cn/gtjcwiqcws.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cqqwz.cn/gtdoutytzk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shanyushiyangtech.top/gtufexsggg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtfldbnnok.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtqwzxojad.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuanzhike.top/gtgutotnha.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yonumen.top/gttqiipuin.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtjipcgccn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.kuanghao11.cn/gtvbzmxvji.html

[C10] 变量作用域
来源：http://hz.gogol.net.cn/gtqiqnmbyr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daria6918.cn/gticdqenfn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xylfe.cn/gtpagszous.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhixingplan.top/gtrjmzlvht.html

TS:   同 JS
来源：http://hz.chenzaomai.com/gthormlhqd.html

Java: 方法内为块级作用域
来源：http://hz.0kj1m.cn/gthgxvkenl.html

Go:   花括号块级作用域
来源：http://hz.shzxlz.cn/gtsshnlhvf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtkoyelxvn.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtcgouoxsk.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtgubrnqzo.html

Py:   from module import func
来源：http://hz.zhaomingkeji.xyz/gtlxrnparh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jianghu66.top/gtswuljspt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gtlruyvssm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hammf.cn/gthwrnojhx.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gtqbskjgkp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgfzy.top/gtyvtgaknt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gteyggqlhw.html

C#:   using System.Text;
来源：http://hz.xziqi.cn/gtpesvlmdh.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtovzcxrzv.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtraezqynn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.redwolf501.top/gtdcahidvf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gttfesaksq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtlysgpewf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtjndcdkcj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.haohaochexian.top/gtowldctml.html

Ruby: -> { puts "run" }.call
来源：http://hz.redwolf501.top/gtlxouqiey.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258888.top/gttpbtxeau.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtvtmaellw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtdhokdiyk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtwvbcfrwz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigfzy.top/gtzfypxcrn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtwvuqedwg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gthcnwssqp.html

Go:   func add(a, b int) int
来源：http://hz.sxryk.cn/gtvtyacevh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ywan-chungtsiang.top/gtwzejmpcr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gtslekzvdi.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtfwsvtscd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gthpyqyocv.html

PHP:  // 无泛型
来源：http://hz.chenzaomai.com/gttmnzkndo.html

JS:   // 无泛型
来源：http://hz.snrcjt.cn/gtofzplfnq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gthgjnweef.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtrjlcmolj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guowangkeji.top/gttauibcgz.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtprzpakou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gtyuzunade.html

[C15] 解构 / 展开参数
来源：http://hz.ehwqpu.com/gttogwmjmu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gtjnciorel.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258.top/gtvuqamhgx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgufenzy.top/gtuxjwjgty.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hywenlv.cn/gtlonwcugn.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtsmodbvoj.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtknuhsogx.html

Ruby: a, b = pair
来源：http://hz.0kj1m.cn/gtaicquirb.html

C#:   var (a, b) = pair;
来源：http://hz.guowangkeji.top/gtelnlipdn.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtxeyihhre.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtosfbamsw.html

PHP:  // 无重载
来源：http://hz.zhoulong.xyz/gttsyomxqg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinghuilouyu.cn/gtbopdnhls.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.quarkkingdee.top/gttdiztyyn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinqigfzy.top/gtbufsuxoq.html

Go:   // 无重载：用不同函数名
来源：http://hz.gogol.net.cn/gtqtlbugko.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtlsvmjjqg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.iojbl.cn/gtswubqbdr.html

================================================================================
来源：http://hz.316326.xyz/gtoldkzyxp.html

D. 数组 / 列表 / 集合
来源：http://hz.hnqzz.top/gtvoepekip.html

================================================================================
来源：http://hz.wangdashe.top/gtbkhzosqx.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtbtgixlur.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtcxmkpwva.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnqzz.top/gtkkqtqqpx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj202588.top/gttoayfdgm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtnzzxsnse.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtswfcvcdz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gtcnfbiawg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ppjwa.cn/gtpiohauoq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cashguo.top/gtvngpepeo.html

[D02] 追加元素到末尾
来源：http://hz.pycfn.com/gteclpdbah.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.haohaochexian.top/gtcyqgifsm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cdnleiting.top/gtiouutbow.html

JS:   arr.push(4);
来源：http://hz.sxryk.cn/gtnorzntsv.html

TS:   arr.push(4);
来源：http://hz.hysaishi.cn/gtrzvecugd.html

Java: list.add(4);
来源：http://hz.xziqi.cn/gtueerogto.html

Go:   arr = append(arr, 4)
来源：http://hz.zhongyouzk.top/gtwypphzpx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sufxvd.cn/gtjxxgxoou.html

C#:   list.Add(4);
来源：http://hz.xuanzx.com/gtlvqoaynj.html

[D03] 在指定位置插入元素
来源：http://hz.yonumen.top/gttjlmbzln.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtuxbgossf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.meibo888.top/gtmbaamval.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtdzemepsv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.snrcjt.cn/gtkzhxofin.html

Java: list.add(0, 0);
来源：http://hz.aizwys.cn/gtpfutxtcy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhixingplan.top/gthrxuvans.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gtozppmexy.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtaxxefbaj.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtiwzmmvxd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.vqdsnc.cn/gtduiuupuy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ivvv.top/gtcdgsohvf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtqcjsnjrp.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gtsyrgxzkk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sufxvd.cn/gtvyaosbbi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.snrcjt.cn/gthmgicveb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.smart0.xyz/gtntynletx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sysykeji.top/gtrmxyexxx.html

[D05] 访问与修改元素
来源：http://hz.meibo888.top/gtfwzphoph.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtzttgvink.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gotoacloud.top/gtiszkxtth.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gaohongyu789.top/gthrnrraoi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.mhx1999.top/gtvtxkekhu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.vqdsnc.cn/gtqwkchinj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtdqpmzpvd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gttbjjenej.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hongshengwenyu.top/gthmzplcer.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gtjozeqvbt.html

Py:   len(arr)
来源：http://hz.9152youxi.cn/gtrlflvviq.html

PHP:  count($arr);
来源：http://hz.cucudq.cn/gtxnsngdpv.html

JS:   arr.length
来源：http://hz.xuanzx.com/gtsdmowkwu.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtdbsjbdvd.html

Java: list.size();
来源：http://hz.xylfe.cn/gtcsxlyqzc.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtqxjfzpou.html

Ruby: arr.length; arr.size
来源：http://hz.yj20258888.top/gtkhpvtlyt.html

C#:   list.Count;
来源：http://hz.hnxiangtu.top/gteybffwsw.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtqfrkjuty.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.kuanghao11.cn/gtamdgddvm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigfzy.top/gtfzqkwpqp.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtuzeqgnym.html

TS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtdwpaefip.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtzbbwrmrs.html

Go:   arr[1:4]
来源：http://hz.guowangkeji.top/gttsflbent.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtlgvqqraa.html

C#:   list.GetRange(1, 3);
来源：http://hz.hammf.cn/gtagnxxhcl.html

[D08] 合并两个数组
来源：http://hz.ivvv.top/gtjbrugpck.html

Py:   a + b;  a.extend(b)
来源：http://hz.ybcxt.top/gtvxwnzcpp.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gtyotqwksh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj202588.top/gtqrtkkjwy.html

TS:   [...a, ...b];
来源：http://hz.kuanghao11.cn/gtzpokaoyd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.mhx1999.top/gtslmzgmse.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtkzkarygz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yanxiufei.cn/gtyaeovydd.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgfzy.top/gtjwmwands.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtvhkoqvow.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtlabdcduq.html

PHP:  sort($arr);
来源：http://hz.ydjk.org.cn/gtpzbfsnrz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yangfankeji.com/gtpjvpqmkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nanxuanxn.top/gthkxzoxyk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gthlugibdr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.andypj.xyz/gtlozoqsuw.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtkcmkgpcl.html

C#:   list.Sort();
来源：http://hz.shuidangran.top/gtqrevjcgl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cheryme.top/gtvfolfpaf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuanzx.com/gtehcaxevi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtkbzddfvp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gttcxxdaec.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtjgkkdopf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtcffemxem.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xinyue.icu/gtkvwpsmmv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ppjwa.cn/gtgapezgzp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gtyzyviifs.html

[D11] 反转数组
来源：http://hz.daxiang520.top/gtsxlcvafo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ehwqpu.com/gtotxyuudn.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtmvyfdehi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtfbwyslyz.html

TS:   [...arr].reverse();
来源：http://hz.zhengqikj.top/gtnvpnbavn.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtygikasfy.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gtfrsigpau.html

Ruby: arr.reverse
来源：http://hz.daria6918.cn/gtfxndvmfa.html

C#:   list.Reverse();
来源：http://hz.cqqwz.cn/gtcodonrqt.html

[D12] 查找元素下标
来源：http://hz.yonumen.top/gtbusyopvf.html

Py:   arr.index(x);  x in arr
来源：http://hz.kuanghao11.cn/gtkqdjexit.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtfxfhgrbx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtfdpbvmmj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtuyqbwywk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtprpmrbuy.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtidycycpt.html

Ruby: arr.index(x)
来源：http://hz.cucudq.cn/gtqlgalsma.html

C#:   list.IndexOf(x);
来源：http://hz.dashuyun.cn/gtpfsgltls.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtunkrobov.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cqqwz.cn/gtmvokikuk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yangfankeji.com/gtassdtpxz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtvdyxayar.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtbcspjkyh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.pycfn.com/gthngdmkdk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258.top/gtjobxjrps.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtizcjqocg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj202588.top/gtxhaqnxua.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtedcqbswv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinghuilouyu.cn/gtanzjsqld.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtbskezgpr.html

JS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtoyqlwkkh.html

TS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtrichknew.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtgdnshofw.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtdchcmwwu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cqqwz.cn/gtrigpaxzq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cashguo.top/gtggncxpyl.html

[D15] 去重
来源：http://hz.jinqigfzy.top/gtcuxudnzk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtewxfunej.html

PHP:  array_unique($arr);
来源：http://hz.nanxinkj.top/gtaeozkzku.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtxdlqplsm.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtchspwsrq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xinyue.icu/gtkkhzytqk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guowangkeji.top/gtjtusgdmy.html

Ruby: arr.uniq
来源：http://hz.tian-w.cn/gtfbwsdzaj.html

C#:   list.Distinct().ToList()
来源：http://hz.gotoacloud.top/gtoaqililz.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gttrrppdwc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gthfwitxze.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtofbaoudy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtymrqvcgi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtqeeheclt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtlqlfgdqs.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gtpvghkfbz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gttcvuprfd.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtllqatdbn.html

[D17] 最大值与最小值
来源：http://hz.pycfn.com/gtbzabrfwp.html

Py:   max(arr);  min(arr)
来源：http://hz.cheryme.top/gtmgowpolh.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtfesftbeo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jianghu66.top/gtgzskdhvs.html

TS:   Math.max(...arr);
来源：http://hz.hnqzz.top/gtbqhncfqu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtpxxinqwr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinghuilouyu.cn/gtabdlosef.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtsmtqugzb.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtbgvmxjui.html

[D18] 扁平化嵌套数组
来源：http://hz.sufxvd.cn/gtunshriqn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.52xcode.cn/gtzeozrlsd.html

PHP:  array_merge(...$nested);
来源：http://hz.daria6918.cn/gtwfcrzmdx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnqzz.top/gtqomptumz.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtbbeupivq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gthanhqiff.html

Go:   // 手写双层循环
来源：http://hz.havefunace.top/gtoytwplgw.html

Ruby: nested.flatten
来源：http://hz.bjfxy.top/gtdcugtgva.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtkpgbvyfz.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtswfynnwu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtowekmyok.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtnkkbqipw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydzc1.top/gtoodmqamh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258888.top/gtntbqqsjd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtcsfodbgo.html

Go:   // 手写 map[string][]T
来源：http://hz.pycfn.com/gtqlizihka.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtjuhlzwbs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuanzx.com/gtxajapgxd.html

[D20] 统计每个元素出现次数
来源：http://hz.zhijiandao.cn/gtkqfpizbx.html

Py:   Counter(arr)
来源：http://hz.sufxvd.cn/gtlwobyllh.html

PHP:  array_count_values($arr);
来源：http://hz.fengsongda.top/gtfjfrijlj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtvzhbquod.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gttefghsxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gtfgpwoabs.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtekmuzgjm.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtwlsnnwsq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtqxbpinga.html

[D21] 判断是否包含某元素
来源：http://hz.zhiwuduotai.top/gtpldwrhbw.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtjwwbmgyf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtxtjwckun.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtdmwwldme.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtacmhghvk.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtdaxrxqyi.html

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gtolfaxnea.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gttdqcvnal.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gtbznrbucg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gogol.net.cn/gtpcjuxwth.html


<!-- 参考信息 -->