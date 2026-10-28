代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.xuetiantiany.cn/gtwmckxijs.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtluzvfdit.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.havefunace.top/gtnpzsinal.html

JS:   const square = x => x * x;
来源：http://hz.daria6918.cn/gtgphfrotc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.tianlin.xyz/gtajyfrdag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gttboajvue.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pengpengdd.cyou/gtvsrjpfda.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hammf.cn/gtowatkryn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shangyingyoupin.top/gtuzoryuby.html

[C07] 把函数作为参数传入
来源：http://hz.zhijiandao.cn/gtvmozzzun.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxuanxn.top/gtlzlqtvkm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gthyxzrzzb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhiwuduotai.top/gtfpjeptiv.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gteyoihxqh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.kuanghao11.cn/gthltbcgje.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gogol.net.cn/gtoefamkre.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxinkj.top/gtyalxhtqf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nwbrower.top/gtooedkqny.html

[C08] 闭包
来源：http://hz.tanke756.top/gtlwfhvgog.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtenphhmjz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinyuanbaomall.cn/gtglwyuheq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gttrzpmxhe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtktpbncuc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cdnleiting.top/gtxxptkthq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.birdmap.top/gtfkcbhbki.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtdnfweluu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtrljimxqe.html

[C09] 递归
来源：http://hz.tanke756.top/gtuobuzopn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtgpqnlpgv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258.top/gtqvmxdxst.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daria6918.cn/gtxxmkmzmg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtyxqfcwnz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.0kj1m.cn/gtjbsozder.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtyvugblmi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gteoiwhpiv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinghuilouyu.cn/gtvcophjxt.html

[C10] 变量作用域
来源：http://hz.zhoulong.xyz/gtzaddlqjp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtelwehubg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gaohongyu789.top/gtmnogiyfl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jlsjyb.cn/gtgnbelfam.html

TS:   同 JS
来源：http://hz.shangyingyoupin.top/gtvdgxbocp.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtcipbvncd.html

Go:   花括号块级作用域
来源：http://hz.jyoumei.cn/gtjanonaee.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ybcxt.top/gtmfrowmri.html

C#:   块级作用域
来源：http://hz.sxryk.cn/gtfqxrhnie.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtuidxlajg.html

Py:   from module import func
来源：http://hz.yonumen.top/gtkdggexda.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zdqjudy.top/gtjqfuukmh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnxiangtu.top/gtatqgtycc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxuanxn.top/gtrcepylkm.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtaagmlfza.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtlgopogwp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hongshengwenyu.top/gtyhuhmayp.html

C#:   using System.Text;
来源：http://hz.nanxinkj.top/gtbvdwehla.html

[C12] 立即执行函数 IIFE
来源：http://hz.yueranfly.top/gtxynlomub.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtjydzffws.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxinkj.top/gtwwakskro.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtkvioigbq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtizefqyao.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtpuomqokr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtgereopjt.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gtjmkoxlfd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtrnwrqqeg.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhongyouzk.top/gtyfubjtbs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtvvgnmdcj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtdjmfedds.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigfzy.top/gthfdiazqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtguxqhqoa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtwvtidzll.html

Go:   func add(a, b int) int
来源：http://hz.quarkkingdee.top/gtjrnaiewg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangtech.top/gtzijdmzzy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtzfdhhvrl.html

[C14] 泛型函数
来源：http://hz.ivvv.top/gtjciwilcb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtiiecnbkl.html

PHP:  // 无泛型
来源：http://hz.shzxlz.cn/gtoohynojp.html

JS:   // 无泛型
来源：http://hz.aizwys.cn/gtylkabjrq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gogol.net.cn/gtxhuodgnm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.smart0.xyz/gthqmaubyv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.iojbl.cn/gtsqybiula.html

Ruby: # 无泛型
来源：http://hz.shangyingyoupin.top/gtsfzibwau.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenlongwang.top/gtvptbilim.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangtech.top/gtdpsoirhc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtsorkseuv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtcfgsxkfq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtwbfsgvus.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtnbmdfsex.html

Java: // 无解构
来源：http://hz.52xcode.cn/gtexurcxxa.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtsfhltcyg.html

Ruby: a, b = pair
来源：http://hz.xingfuxueyuan.xyz/gtqsrsqdwa.html

C#:   var (a, b) = pair;
来源：http://hz.cucudq.cn/gtoimdwyao.html

[C16] 函数 / 方法重载
来源：http://hz.yuxming.cn/gtddyflkrr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtstckxjgt.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gthdefcapf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtjhmlkktw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cashguo.top/gtxllzbgul.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinghuilouyu.cn/gtmaocedue.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigfzy.top/gtchsgmmsn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydjk.org.cn/gtqheubzug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shuidangran.top/gtrcknwehm.html

================================================================================
来源：http://hz.redwolf501.top/gtorcaykhb.html

D. 数组 / 列表 / 集合
来源：http://hz.zhixingplan.top/gthzineedi.html

================================================================================
来源：http://hz.zhongyouzk.top/gtaqvezpht.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtspyovxjp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtclbkpvyv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gotoacloud.top/gtutuzvqsi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hywenlv.cn/gtrocgzrmv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.vqdsnc.cn/gthzvcjlth.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tanke756.top/gtmiabubsi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.quarkkingdee.top/gtswxntpfm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtxcltllfq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtxuynjxmj.html

[D02] 追加元素到末尾
来源：http://hz.fengsongda.top/gtciduhkxm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gtrslmjvtm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangdashe.top/gtlsmmurxd.html

JS:   arr.push(4);
来源：http://hz.andypj.xyz/gtcfrwxryi.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtdwdceauq.html

Java: list.add(4);
来源：http://hz.chenjidiqi.icu/gteecurtwr.html

Go:   arr = append(arr, 4)
来源：http://hz.daria6918.cn/gtkyqdaazc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yangfankeji.com/gttodwvdjs.html

C#:   list.Add(4);
来源：http://hz.chenzaomai.com/gtaarvjqjy.html

[D03] 在指定位置插入元素
来源：http://hz.ydjk.org.cn/gtnnzyufbl.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtbetswbat.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhiwuduotai.top/gtxvscpruo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gaohongyu789.top/gtprfwcfli.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fzhhl.top/gtbkfpqhyj.html

Java: list.add(0, 0);
来源：http://hz.jyoumei.cn/gthemratjg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gtpqqxiele.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.c1oappe.top/gtvpepvdwn.html

C#:   list.Insert(0, 0);
来源：http://hz.sxryk.cn/gtuvubbwtk.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gtroxiqthw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuetiantiany.cn/gtfudzwiao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtzdknppxe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gteyceouik.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtycwxadfo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuetiantiany.cn/gtnvpgrwkw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtjyqgoyoq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gtqgkpqecc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtnhgwfniu.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtmlqgqelf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gticnljrst.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuanzx.com/gtdphyyknu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtqtzmfxil.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtthonpaei.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtylxkoens.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gttrvwkxsv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtgquyoacy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtherjgmnp.html

[D06] 数组长度
来源：http://hz.nwbrower.top/gtdhytyxwm.html

Py:   len(arr)
来源：http://hz.xuetiantiany.cn/gtlsruuslx.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtwkxazrar.html

JS:   arr.length
来源：http://hz.zdqjudy.top/gtguexingo.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gtkcmqzuks.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtjerrspxu.html

Go:   len(arr)
来源：http://hz.snrcjt.cn/gtsrvwbpdt.html

Ruby: arr.length; arr.size
来源：http://hz.jinghuilouyu.cn/gtbyyhopmb.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtmlokispu.html

[D07] 切片 / 取子数组
来源：http://hz.sufxvd.cn/gtlqbhszrh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtozbxyuyh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuanzhike.top/gtbrqqtbzj.html

JS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gtyftrtire.html

TS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtpseauydo.html

Java: list.subList(1, 4);
来源：http://hz.zycfv.cn/gtkgjxanjo.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtfafmfinw.html

Ruby: arr[1, 3]
来源：http://hz.vqdsnc.cn/gtwgjueyct.html

C#:   list.GetRange(1, 3);
来源：http://hz.ppjwa.cn/gtlncdlkpj.html

[D08] 合并两个数组
来源：http://hz.iojbl.cn/gtfqzlmwum.html

Py:   a + b;  a.extend(b)
来源：http://hz.yanxiufei.cn/gtsnmrfvaq.html

PHP:  array_merge($a, $b);
来源：http://hz.daria6918.cn/gtiuimhiut.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtcexipqgl.html

TS:   [...a, ...b];
来源：http://hz.ydzc1.top/gtvzellpep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxinkj.top/gtqynxaqjp.html

Go:   append(a, b...)
来源：http://hz.iojbl.cn/gtyuxqyclj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xylfe.cn/gtpjknrxnv.html

C#:   a.Concat(b).ToList()
来源：http://hz.c1oappe.top/gtqrngclvq.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtoadppifm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtqawzgpio.html

PHP:  sort($arr);
来源：http://hz.andypj.xyz/gtfnjjvnum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258888.top/gtccfmwuan.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.andypj.xyz/gtvjxhsaeq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gtkjrjdagp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtzotfsrex.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtwxsxfeiz.html

C#:   list.Sort();
来源：http://hz.52xcode.cn/gtynhmqaar.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gtqafapqun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtwyjugbbv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtubctrggc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtgpkmeltz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtbaabfghh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xylfe.cn/gtkabkmnyl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sweek.top/gthpiyskdi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtwyufymci.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.iojbl.cn/gtzqypebwo.html

[D11] 反转数组
来源：http://hz.zhijiandao.cn/gtgattepcy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.vqdsnc.cn/gtqkmjcpix.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gthticrbad.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtkafpiwnr.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtwhcpyvsy.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtziybkeua.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangkeji.top/gtwzkgivof.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtfwwjjmsm.html

C#:   list.Reverse();
来源：http://hz.gzhubu.top/gtkpcpseti.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtlesgnofy.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gtokzkukwe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sweek.top/gtsibhuebe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtbwuwebxp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtsurixkcf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gttbchxgsu.html

Go:   slices.Index(arr, x)
来源：http://hz.shanyushiyangtech.top/gtqqurjxpp.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtopnayaqa.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtptkzfynd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ybcxt.top/gthvnmyrii.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtmugukpcu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gzhubu.top/gtxyccgcrk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtedrvyylu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gttcbprwrs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtmgbqcrca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenzaomai.com/gtvblyzfvv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sysykeji.top/gtjmytzkga.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gteeagrhde.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shzxlz.cn/gtgxdfmhze.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangdashe.top/gtsrbguxdz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtxpymdjxe.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtzrqgxwmx.html

TS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtjabzsldv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhijiandao.cn/gtzfrbkmye.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtzaqxtbtf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtfliryubu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hywenlv.cn/gtrraiyzxi.html

[D15] 去重
来源：http://hz.xingfuxueyuan.xyz/gtuesaglcm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtsugtzeis.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtdrjvwmvp.html

JS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtmijcoixc.html

TS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtkfdchnyt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhengqikj.top/gtuiixyplo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtknjmenfs.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtxtjsnuya.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtlksriryx.html

[D16] 求和与平均值
来源：http://hz.c1oappe.top/gtlwjffzgg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtsgnqugmn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtbcxguiok.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtzwrgjphn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtcissndjz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtwwibonwj.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gtqjisslzg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtnovxmdyo.html

C#:   list.Sum();  list.Average()
来源：http://hz.jlsjyb.cn/gtjclwpdmo.html

[D17] 最大值与最小值
来源：http://hz.c1oappe.top/gtppzckncy.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtnlvhhajh.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gtxikylyuk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.316326.xyz/gtwqwspepg.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtakrgfxar.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtwosxodnt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtevpbxpbe.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gtnplovpkq.html

C#:   list.Max();  list.Min()
来源：http://hz.gaohongyu789.top/gtveocsgks.html

[D18] 扁平化嵌套数组
来源：http://hz.yangfankeji.com/gtncwtpoeb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtukmnhhtt.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtrvmbukmf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jlsjyb.cn/gtzarztofw.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtajxwucmj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daria6918.cn/gtvdwrqosk.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gthmuszndc.html

Ruby: nested.flatten
来源：http://hz.chenlongwang.top/gtlzgzahmc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jqgfzy.top/gtrgnezyqi.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtwoamjxro.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hywenlv.cn/gtamhrzgkd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hywenlv.cn/gttlfhabbl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenzaomai.com/gtdtucorev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gtyzmmxczq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gtciwlxryf.html

Go:   // 手写 map[string][]T
来源：http://hz.zhongyouzk.top/gttziwvxmt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tanke756.top/gtchmznszk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daria6918.cn/gtcufsrmbk.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtzgaxwkkw.html

Py:   Counter(arr)
来源：http://hz.zycfv.cn/gttvbqztmo.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtihhcvdct.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtsfgunvpj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtkldpkvvw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxinkj.top/gtqvuwbqme.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtzhqkfuja.html

Ruby: arr.tally
来源：http://hz.52xcode.cn/gtklyilmdl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtjqgxxwfu.html

[D21] 判断是否包含某元素
来源：http://hz.zhiwuduotai.top/gtylrklvoc.html

Py:   x in arr
来源：http://hz.cqqwz.cn/gtiawfvsjm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hywenlv.cn/gtzyeaziii.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtrhcduwfo.html

TS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gtoelyuwiq.html

Java: list.contains(x)
来源：http://hz.zhengqikj.top/gtwpypjilv.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtzgryoylb.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtarbcjpvb.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtkoeysnpq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtvowdqxml.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtxzfyypyu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ehwqpu.com/gtisfqcofn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtcqsxqmeg.html

TS:   [...arr];
来源：http://hz.zhengqikj.top/gtmlanytgz.html

Java: new ArrayList<>(list);
来源：http://hz.yueranfly.top/gtxocnpifq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtklgxbukk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fengsongda.top/gtfvzvmxmz.html

C#:   new List<int>(list);
来源：http://hz.yonumen.top/gtwqtczskk.html


<!-- 参考信息 -->