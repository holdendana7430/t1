代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.cdnleiting.top/gtpktnbqid.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dashuyun.cn/gtjvkvyijm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yueranfly.top/gtxemohmkt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dashuyun.cn/gtosjyauhu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtbjpfucue.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtpbkbglyh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gotoacloud.top/gtbdmbcrdk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hfpthk.cn/gteeqgqhjd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.fengsongda.top/gtdzprzgrd.html

TS:   arr.map(String)
来源：http://hz.cucudq.cn/gtzvetxtfz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gtuyzwhnqi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgufenzy.top/gtzocmmnhq.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gtuquxxhxh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shanyushiyangkeji.top/gtqslvtosx.html

[C08] 闭包
来源：http://hz.zhiwuduotai.top/gtwxivcbrq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.vqdsnc.cn/gtsvjlbpva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtwmvyayff.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtcsgphdkk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtdfiqodef.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shanyushiyangtech.top/gtzvrabgal.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xinyue.icu/gtticgkquu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hongshengwenyu.top/gtaspltpat.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtpputmquh.html

[C09] 递归
来源：http://hz.jqgufenzy.top/gtmllsehgx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gtprhqfnit.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigfzy.top/gtpdohfqcg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtrwmwcghb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtrbtdrpbr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cucudq.cn/gttqvlyxxl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xingfuxueyuan.xyz/gtfdicrais.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenjidiqi.icu/gtsikoglku.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dianchejie.cn/gtsmfnbdvn.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtxqhvrlqr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gtvwjschzp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.vqdsnc.cn/gtwrjgvfbt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhaomingkeji.xyz/gtcbixnzip.html

TS:   同 JS
来源：http://hz.meibo888.top/gtufzejwuk.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gtkmzloprs.html

Go:   花括号块级作用域
来源：http://hz.zhoulong.xyz/gtjjruksoi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.havefunace.top/gtomxwbzgy.html

C#:   块级作用域
来源：http://hz.cashguo.top/gtknzzbecc.html

[C11] 模块导入与导出
来源：http://hz.sxryk.cn/gtkguglrhl.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtkdiukyfy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtznwosntx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtvloxjoxu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxinkj.top/gtkcglpzsa.html

Java: import java.util.List;
来源：http://hz.zhaomingkeji.xyz/gtpnqjnbjz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gogol.net.cn/gtmiwddnua.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinghuilouyu.cn/gtccrcdhpz.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtbpblquto.html

[C12] 立即执行函数 IIFE
来源：http://hz.aizwys.cn/gttceltxzh.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258.top/gtaougamax.html

PHP:  (function () { echo "run"; })();
来源：http://hz.316326.xyz/gtdcehmdtn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gzhubu.top/gtaoajznon.html

TS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtszxutzxj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xylfe.cn/gtkwbvzojq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhaomingkeji.xyz/gtmlkhwuzp.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtahjsxsxl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hongshengwenyu.top/gtfodiacwy.html

[C13] 类型声明 / 类型注解
来源：http://hz.sxryk.cn/gtpoocspso.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xingfuxueyuan.xyz/gtdytpnoiu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtttopcnwa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.andypj.xyz/gtvaikolfz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gthaenjcjo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtleuqvzne.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtofczyfba.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hfpthk.cn/gtxtvmlqhh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtfealtkby.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtdsxecmzo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gtianrepnm.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtostukcln.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtjrvahbxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtvosharmh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtmrybnrks.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtoqhjyqqo.html

Ruby: # 无泛型
来源：http://hz.pycfn.com/gtdmgbpbdm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gttxutfzxa.html

[C15] 解构 / 展开参数
来源：http://hz.yongpay.top/gtnkxyaynf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gtafoqhfft.html

PHP:  [$a, $b] = $pair;
来源：http://hz.52xcode.cn/gtajiwscjo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtqjkhzpaa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gthdowywml.html

Java: // 无解构
来源：http://hz.iojbl.cn/gtagqtfali.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtjoukubnw.html

Ruby: a, b = pair
来源：http://hz.xylfe.cn/gtrkkykffn.html

C#:   var (a, b) = pair;
来源：http://hz.xuanzx.com/gtvetcdajb.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtdwasdomy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtqthimlcv.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtjeytdviu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtuilzcury.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtpmdegfex.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zycfv.cn/gtwobmowpv.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtsssnnadk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtcytnzdam.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtfgdolnei.html

================================================================================
来源：http://hz.yuxming.cn/gtvrihqwen.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtcfbqaufn.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvowzpmpb.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtmukhibio.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jiagoushi.top/gtewltqftw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gthmhuvuep.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxinkj.top/gtowmbhkka.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hfpthk.cn/gtbveaygrc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cheryme.top/gtdmaykwlb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtxqvzcpht.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtcwjfjoaq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuanzhike.top/gtlphfslvx.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtbehdkope.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgfzy.top/gtcxkgwsai.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aizwys.cn/gtgjmuvrxo.html

JS:   arr.push(4);
来源：http://hz.yj20258888.top/gtnvkqyyik.html

TS:   arr.push(4);
来源：http://hz.fzhhl.top/gtxbdwlmjg.html

Java: list.add(4);
来源：http://hz.svipenyu.cn/gtkqhmwwsr.html

Go:   arr = append(arr, 4)
来源：http://hz.yj202588.top/gtsbmfiseh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxuanxn.top/gtqiyxsduq.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtamzxjdxc.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtzmtjzzti.html

Py:   arr.insert(0, 0)
来源：http://hz.52xcode.cn/gtvlgjegvj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.smart0.xyz/gtsjomqdtb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtezkljxma.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtiekdymec.html

Java: list.add(0, 0);
来源：http://hz.sysykeji.top/gtdoufelft.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangshuangyany.cn/gtpvrwglzk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.kuanghao11.cn/gtpaistcjq.html

C#:   list.Insert(0, 0);
来源：http://hz.cucudq.cn/gtiudvsjri.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtprgdylow.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zycfv.cn/gtzvswwjrh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gotoacloud.top/gtxbvqawuk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jiagoushi.top/gtobqezlwg.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gtlrvamlyt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gtitjrwykz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pengpengdd.cyou/gtjvikkpnl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtqmllqocw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gthdzkspkn.html

[D05] 访问与修改元素
来源：http://hz.cqqwz.cn/gtlqtxchxa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.bjfxy.top/gtdrkcjkcl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yongpay.top/gtnplvoyll.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtevhvjjxe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xinyue.icu/gthnieyzrb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.redwolf501.top/gttbznlqzw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtrhgodrgk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtobelpwld.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtbxqbbzid.html

[D06] 数组长度
来源：http://hz.yangfankeji.com/gtamzfleqi.html

Py:   len(arr)
来源：http://hz.yj20258.top/gtlnxpknck.html

PHP:  count($arr);
来源：http://hz.shanyushiyangtech.top/gtfsiodtsb.html

JS:   arr.length
来源：http://hz.cdnleiting.top/gtgnurdeoc.html

TS:   arr.length
来源：http://hz.guowangkeji.top/gtmdtngbhi.html

Java: list.size();
来源：http://hz.jianghu66.top/gtvgrortql.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtdoaaryeo.html

Ruby: arr.length; arr.size
来源：http://hz.ehwqpu.com/gtczlemiys.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtmnwfmeaj.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258.top/gtkjixripp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cashguo.top/gtcgzfpbwt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtilzlhotd.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtxwopahul.html

TS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtcaywaowq.html

Java: list.subList(1, 4);
来源：http://hz.cheryme.top/gtlkhakdff.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtklzwgdih.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtxtyzyecm.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtpvxvfths.html

[D08] 合并两个数组
来源：http://hz.wangshuangyany.cn/gtpuraskhx.html

Py:   a + b;  a.extend(b)
来源：http://hz.daria6918.cn/gtknlmsftg.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtaqsimefu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gtjphkecvi.html

TS:   [...a, ...b];
来源：http://hz.jlsjyb.cn/gtqubmdjtd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shuidangran.top/gtfxvsxyfi.html

Go:   append(a, b...)
来源：http://hz.tian-w.cn/gtlgqxrvve.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gthivdfymi.html

C#:   a.Concat(b).ToList()
来源：http://hz.sxryk.cn/gtyomjucpl.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtklejtneo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtejmvqapd.html

PHP:  sort($arr);
来源：http://hz.jinqigufen.top/gtxrhrctjp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtggjjdzng.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtvbfmkgaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hywenlv.cn/gtplgqbfsf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtgcatcvbs.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtcpfhecuh.html

C#:   list.Sort();
来源：http://hz.52xcode.cn/gtjfochjbm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenjidiqi.icu/gtgeteezax.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuanzx.com/gtwtklweqi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtxhglrmmx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtmbelttqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydjk.org.cn/gtjosqmdqv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.52xcode.cn/gtufqetnmb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nanxinkj.top/gttywwvdju.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtaozggqfn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtmkrzmofd.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtpfofnmlh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhaomingkeji.xyz/gteoybffjr.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtqpaatlvb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sysykeji.top/gthzktukml.html

TS:   [...arr].reverse();
来源：http://hz.nanxinkj.top/gtuwcvinhr.html

Java: Collections.reverse(list);
来源：http://hz.cheryme.top/gtjctwxelb.html

Go:   slices.Reverse(arr)
来源：http://hz.gotoacloud.top/gtgssfdhkd.html

Ruby: arr.reverse
来源：http://hz.jiagoushi.top/gthvcnxiwi.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtocnyyxgy.html

[D12] 查找元素下标
来源：http://hz.daria6918.cn/gtpmtpwypc.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtwxnxsbdr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtgucxcpgb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtlmqicqvh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtrlpyoqfx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtzaorrjsh.html

Go:   slices.Index(arr, x)
来源：http://hz.jlsjyb.cn/gtcdqxtebf.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtunszxhtx.html

C#:   list.IndexOf(x);
来源：http://hz.ivvv.top/gtpnocioxo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenzaomai.com/gtvqcnucvp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtfvddcxpt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zdqjudy.top/gtojzwdxcy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtvtlxnvlc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtgsffaptr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jianghu66.top/gtnenxqlcr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guowangkeji.top/gtayithatd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xinyue.icu/gtdoqleynh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.haohaochexian.top/gtumfvzmcj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhongyouzk.top/gtoqbdixxq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenlongwang.top/gthastyzxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.bjfxy.top/gtahkmwbhw.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtssetnhvl.html

TS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtsvgalmqk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangtech.top/gtrfuebpoa.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtekrstztg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xinyue.icu/gtrevyfpwy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.vqdsnc.cn/gtrvgqhzaa.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtupqtrarl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtdijjeaos.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtxhaaudtl.html

JS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtvywrzjid.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtophobvis.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gtdmpdaujr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daxiang520.top/gtkvfmmkkp.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtbsjpyojn.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtaukduikg.html

[D16] 求和与平均值
来源：http://hz.ydjk.org.cn/gtcfofckuw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenzaomai.com/gtktnuwlel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.haohaochexian.top/gtegykeqyz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtllctcqle.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtvlrkqpxm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnxiangtu.top/gthgiawsno.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gtwarskhjz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtnpmsxhdo.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gttcwwnjvb.html

[D17] 最大值与最小值
来源：http://hz.jinqigufen.top/gtapqavlla.html

Py:   max(arr);  min(arr)
来源：http://hz.zhoulong.xyz/gtlluwiibj.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtynwvhymw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtidxxrguv.html

TS:   Math.max(...arr);
来源：http://hz.svipenyu.cn/gtqjmmlcct.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gturidyfyn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gtixiarszu.html

Ruby: arr.max;  arr.min
来源：http://hz.cqqwz.cn/gtevfwqtlj.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtztbdgrlq.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtfkdgfecy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydjk.org.cn/gtckzidqhv.html

PHP:  array_merge(...$nested);
来源：http://hz.cheryme.top/gtmjuzgfyr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtccomzgba.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gttiusaahm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.316326.xyz/gtxlcegauf.html

Go:   // 手写双层循环
来源：http://hz.ybcxt.top/gtovjmpmct.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtkansmavq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtqnliamby.html

[D19] 按字段分组
来源：http://hz.jinqigufen.top/gtfszmzhfu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gtpxjnggkd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj202588.top/gtasjkrcht.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxuanxn.top/gtmjwndcfm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtepavpzhw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gttfabdamb.html

Go:   // 手写 map[string][]T
来源：http://hz.zycfv.cn/gtvnuhdxzm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtotkddvkx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtstcsgobw.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gttdhituzj.html

Py:   Counter(arr)
来源：http://hz.chenzaomai.com/gtlowcixxf.html

PHP:  array_count_values($arr);
来源：http://hz.jiagoushi.top/gtvqjcxtpu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtoohlxisg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtkgdqnjfn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gtxntpuzsp.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gtjgupfnzy.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtzmnxucwd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtimosfjvr.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangtech.top/gtbbcfflqo.html

Py:   x in arr
来源：http://hz.316326.xyz/gthsmzgyyl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtpauzgisx.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtealdnnjr.html

TS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtcvjtylbi.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtfmaescth.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtfiikxwku.html

Ruby: arr.include?(x)
来源：http://hz.chenlongwang.top/gtefvsuqjg.html

C#:   list.Contains(x)
来源：http://hz.9152youxi.cn/gtofdleqcb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtkmyihudk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jiagoushi.top/gtxrdvqqfi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ywan-chungtsiang.top/gtpqqdmmln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sweek.top/gtrgkqvflc.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtsoqudgwp.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtmddndzzu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ywan-chungtsiang.top/gtyqzgfpkh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xziqi.cn/gtzorrpcdy.html

C#:   new List<int>(list);
来源：http://hz.wangdashe.top/gtuzkguhgx.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtuvdrpvlp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.haohaochexian.top/gtduvxuxxu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yongpay.top/gthsqgkxyp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gthyepgjuv.html


<!-- 参考信息 -->