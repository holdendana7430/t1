代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gttcalcrvt.html

TS:   arr.map(String)
来源：http://hz.hysaishi.cn/gtmiscplbb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ppjwa.cn/gtxyxeenkc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtbljadrod.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinqigufen.top/gtuzcvmbzs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gtrlnijdia.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtmwjibjus.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tian-w.cn/gtlttvidzx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnxiangtu.top/gtbwyzwigf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtheaawdwe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtfhyrpwho.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenjidiqi.icu/gtvamosukj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.kuanghao11.cn/gtgcscivsg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgufenzy.top/gtwwdjbtta.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtmyxhdruz.html

[C09] 递归
来源：http://hz.sysykeji.top/gtrmlnsbzf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtrqtaexnr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtexkyhjrj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtldqgylgj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtyiafcjwk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtaglaskhj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gttvafklgw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtagcnmziu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jiagoushi.top/gttuvuvvqw.html

[C10] 变量作用域
来源：http://hz.sxryk.cn/gtabpmnabx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.mhx1999.top/gtmtdizlzk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.quarkkingdee.top/gtgmsgsznb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.haohaochexian.top/gtamcnbbdy.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gttzwbcanv.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtjekofbhd.html

Go:   花括号块级作用域
来源：http://hz.aibaodan.cn/gtdwnsqdbt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guannengcc.top/gtbttwllbr.html

C#:   块级作用域
来源：http://hz.birdmap.top/gtqcchfvib.html

[C11] 模块导入与导出
来源：http://hz.aizwys.cn/gtcrbuhalz.html

Py:   from module import func
来源：http://hz.316326.xyz/gtpkgvomhd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydzc1.top/gtorxcmdti.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hfpthk.cn/gtalycpljh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhongyouzk.top/gtzecezkbx.html

Java: import java.util.List;
来源：http://hz.yongpay.top/gtodocnmva.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.quarkkingdee.top/gtfgbpmabe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hfpthk.cn/gtlclrjrfw.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtxuampmyg.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gtdwoglwwi.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtowbhdlss.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinghuilouyu.cn/gtwcggylhp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gttndxgxzr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtajzpiker.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtnwcfmhay.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guannengcc.top/gtcdwnvjlv.html

Ruby: -> { puts "run" }.call
来源：http://hz.jianghu66.top/gtttrwyhue.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuanzx.com/gtdorkqkjv.html

[C13] 类型声明 / 类型注解
来源：http://hz.hfpthk.cn/gtiwocchdv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yongpay.top/gtuwcukzho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtglngrvol.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj202588.top/gtpatgojse.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtahedlqko.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtgrqbztaw.html

Go:   func add(a, b int) int
来源：http://hz.gaohongyu789.top/gtvbrvoacg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dianchejie.cn/gtoxwajknm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gtgxfrbcwx.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtikxecvcq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxinkj.top/gtsyxkwgsl.html

PHP:  // 无泛型
来源：http://hz.redwolf501.top/gtrdgzsvrh.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gteqagfufy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.0kj1m.cn/gtlsemfxrr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtvhtnebjg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gttejxolcn.html

Ruby: # 无泛型
来源：http://hz.jinyuanbaomall.cn/gtmnitrkcm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guannengcc.top/gtnjnwiqoo.html

[C15] 解构 / 展开参数
来源：http://hz.zhixingplan.top/gtgjrmxuez.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydzc1.top/gtsqyyldwm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtkwumspwg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydjk.org.cn/gtughrbvqf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgfzy.top/gtzeqxgwra.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtvcuwghtv.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtdpihqeze.html

Ruby: a, b = pair
来源：http://hz.yj20258888.top/gtowbffzyu.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtyfaawepi.html

[C16] 函数 / 方法重载
来源：http://hz.fengsongda.top/gtzkdyldyj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xingfuxueyuan.xyz/gtmrlmxlbi.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gttygbvofp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.kuanghao11.cn/gtecwyooqr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtdykyyomb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtlxfqrjyx.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenjidiqi.icu/gtfzsrbhvd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtsosneckf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cheryme.top/gtcsehpfmw.html

================================================================================
来源：http://hz.svipenyu.cn/gtjtpcfhnv.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtkmeflclj.html

================================================================================
来源：http://hz.ivvv.top/gtuxezzcah.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gtlqynpocc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtpaejtjke.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtejnnbona.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.meibo888.top/gthrjpaipa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ydzc1.top/gtfitmqlzd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangtech.top/gtvfhilclf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ybcxt.top/gtbiummzch.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtbsupypwj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ppjwa.cn/gtwftdzwky.html

[D02] 追加元素到末尾
来源：http://hz.jinqigufen.top/gtlkhnzkts.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cheryme.top/gtffahvnlf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tian-w.cn/gttbpshxcy.html

JS:   arr.push(4);
来源：http://hz.yonumen.top/gtzahcwrla.html

TS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtmlrjqcbx.html

Java: list.add(4);
来源：http://hz.shangyingyoupin.top/gtgrokffjx.html

Go:   arr = append(arr, 4)
来源：http://hz.yanxiufei.cn/gtgflgfnsu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.9152youxi.cn/gtudumllpf.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gtnzsmyuvw.html

[D03] 在指定位置插入元素
来源：http://hz.hfpthk.cn/gtbdipqhrv.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtnfknwgkw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtgxwqnjkx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenlongwang.top/gtyirdevnb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gttwchqpcm.html

Java: list.add(0, 0);
来源：http://hz.quarkkingdee.top/gtstyscoib.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtlkwcqaqc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gtzrmfnijx.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgufenzy.top/gtyndkegsb.html

[D04] 删除元素
来源：http://hz.ywan-chungtsiang.top/gtuqvaopje.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gttjciihxn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgfzy.top/gtjgsmqfpj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ywan-chungtsiang.top/gtgwsotxmf.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gteytewlol.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtdsllnlvy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhixingplan.top/gtasifaclz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhixingplan.top/gtirkqekej.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhixingplan.top/gtafvmeapf.html

[D05] 访问与修改元素
来源：http://hz.xziqi.cn/gttckhxnyl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtaplptixx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhongyouzk.top/gttuphloce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhengqikj.top/gtcofnfjer.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhijiandao.cn/gtrbuqwgkf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtwzsqccnl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtarxcibhx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtlhshkzzj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtnplmflpf.html

[D06] 数组长度
来源：http://hz.tian-w.cn/gthaohcvjt.html

Py:   len(arr)
来源：http://hz.wangdashe.top/gtrmnanmdz.html

PHP:  count($arr);
来源：http://hz.jyoumei.cn/gtyyuswthv.html

JS:   arr.length
来源：http://hz.kuanghao11.cn/gtkpfswsmu.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtolhwwjdr.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtzrcomcjg.html

Go:   len(arr)
来源：http://hz.c1oappe.top/gtushlzqnt.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtnwalzvth.html

C#:   list.Count;
来源：http://hz.yonumen.top/gtaviyikbt.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtlomaltdt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xylfe.cn/gtktpjtosx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtxcwnoaln.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtiyesielh.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtaxjvlgst.html

Java: list.subList(1, 4);
来源：http://hz.jinqigfzy.top/gtrazpmuox.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtepdeauuq.html

Ruby: arr[1, 3]
来源：http://hz.gotoacloud.top/gtfxqhcwcj.html

C#:   list.GetRange(1, 3);
来源：http://hz.316326.xyz/gtpbwktule.html

[D08] 合并两个数组
来源：http://hz.kuanghao11.cn/gtsdmvjlrh.html

Py:   a + b;  a.extend(b)
来源：http://hz.andypj.xyz/gtuubymndl.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtkcnlzzdg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yvedp.cn/gtrpsqlzwx.html

TS:   [...a, ...b];
来源：http://hz.tanke756.top/gtaxuuihlu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhijiandao.cn/gtbaxjbqky.html

Go:   append(a, b...)
来源：http://hz.chenzaomai.com/gthryrxpxn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ybcxt.top/gthqqzgzlp.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gtmkuhbkab.html

[D09] 排序（升序）
来源：http://hz.9152youxi.cn/gtaudgopkj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtsbentpje.html

PHP:  sort($arr);
来源：http://hz.tian-w.cn/gtjoydwsil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtcpbvimtd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigfzy.top/gtqxntedwq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtlwwxkzgq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtpvjxpvui.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtozvajihu.html

C#:   list.Sort();
来源：http://hz.hnxiangtu.top/gtiyqjodaz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aizwys.cn/gthkipxyhf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.feifeiyinyue.top/gtciaxlhsh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhaomingkeji.xyz/gtmifnbubc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtadbfohep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtqrvclimj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtzsikwysq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnxiangtu.top/gtrmdoklbp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.snrcjt.cn/gtuvexvvfx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.316326.xyz/gttisbebne.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtkeakreto.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj20258.top/gtrnzxafbk.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtvttjvknb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.andypj.xyz/gtagohpvyk.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangkeji.top/gtllgmcyks.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtjbuvnfua.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtxbrzpxdk.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gtlnjmyrhb.html

C#:   list.Reverse();
来源：http://hz.shangyingyoupin.top/gtgscjnhbp.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtihnimsuh.html

Py:   arr.index(x);  x in arr
来源：http://hz.zdqjudy.top/gtkojltmqt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hysaishi.cn/gtvjtmjjlt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtjgvnslmq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtepwrmaha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtvmqhkwko.html

Go:   slices.Index(arr, x)
来源：http://hz.316326.xyz/gtlzblhctf.html

Ruby: arr.index(x)
来源：http://hz.pycfn.com/gtqlsdxrle.html

C#:   list.IndexOf(x);
来源：http://hz.jiagoushi.top/gtzlsvaonw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenzaomai.com/gtvexwgzla.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtkrcrydll.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtixexestk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtopotxcij.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtxuvtgaow.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgufenzy.top/gtgmenzjmv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guowangkeji.top/gtvoebmbsa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtgfziincc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtqllsiajn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jlsjyb.cn/gtgqskelri.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtqfwnrtde.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dashuyun.cn/gtvnrvtvvy.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtddtguhbx.html

TS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtjidvzonw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtkekjmedd.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtjpwmjdys.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtxwmorsso.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cashguo.top/gtltvznmte.html

[D15] 去重
来源：http://hz.meibo888.top/gtenszkkpk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tian-w.cn/gtnjzydolk.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtvciamkvl.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtngbdvvbe.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtevefxlst.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xziqi.cn/gtjacnycjp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dashuyun.cn/gtlyhuvnaf.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gtbndfqrqp.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxinkj.top/gtvyieusha.html

[D16] 求和与平均值
来源：http://hz.nanxinkj.top/gtlidxjjno.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pengpengdd.cyou/gtujaermpe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xziqi.cn/gthsneedku.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gttqbfbwme.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtcmafzprn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtqqvpxgna.html

Go:   // 手写循环累加
来源：http://hz.smart0.xyz/gtjorekqef.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sxryk.cn/gtktzigjsm.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtxymevbqw.html

[D17] 最大值与最小值
来源：http://hz.jinqigufen.top/gtunnzechm.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxinkj.top/gtescxjson.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtzpjmxyic.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xinyue.icu/gtsqqaqfsi.html

TS:   Math.max(...arr);
来源：http://hz.zhaomingkeji.xyz/gtmhjaidlj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtbdlgblgw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtephnhyju.html

Ruby: arr.max;  arr.min
来源：http://hz.chenjidiqi.icu/gtqgakdtok.html

C#:   list.Max();  list.Min()
来源：http://hz.nwbrower.top/gtjvxcoemu.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtpijrdovp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtyjbpufqh.html

PHP:  array_merge(...$nested);
来源：http://hz.hammf.cn/gtvunozbxv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gtjjnhrclo.html

TS:   nested.flat();
来源：http://hz.zhijiandao.cn/gtvgznqfja.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtuuzzdjxh.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtmwpnoaif.html

Ruby: nested.flatten
来源：http://hz.yangfankeji.com/gtbkyxyqgl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtmwlymugj.html

[D19] 按字段分组
来源：http://hz.jinghuilouyu.cn/gtqslfkymi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtkychjwmw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ybcxt.top/gtaswwpawt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtatcxlvnc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gteaahftdp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtnkkveick.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtwchzlgby.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daxiang520.top/gtrtpubgxf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtuthuucue.html

[D20] 统计每个元素出现次数
来源：http://hz.zhengqikj.top/gthqoqjnfd.html

Py:   Counter(arr)
来源：http://hz.gogol.net.cn/gtmvypmrln.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtstoiqkux.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtauipsgwt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtvkfjrprx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zycfv.cn/gteyueulqq.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtbpoexsnw.html

Ruby: arr.tally
来源：http://hz.nwbrower.top/gtugjanwmx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtjdzcvpka.html

[D21] 判断是否包含某元素
来源：http://hz.quarkkingdee.top/gtnpvrrdyg.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gtmeazyokp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gtdjdpboyr.html

JS:   arr.includes(x)
来源：http://hz.hammf.cn/gtzoihxzbz.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtemvswqia.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtztumhaas.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtlneehntm.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangkeji.top/gtifncxgsu.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gtqgwndqbh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtojhaztmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtmcjbggvw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtlgjonmwt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtunjcdoxj.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtlnjmptev.html

Java: new ArrayList<>(list);
来源：http://hz.shangyingyoupin.top/gtgwtebtyu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtjfviespy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.haohaochexian.top/gtjjlznrbs.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtjkwfjmkg.html

[D23] reduce 累积计算
来源：http://hz.zdqjudy.top/gtfygynobf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shuidangran.top/gtddpbaeau.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.havefunace.top/gtqcxsrjvq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtiazbpshd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtobhygyiw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtllzbgmws.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtuuyiwufj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daxiang520.top/gtbogoyncs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.pycfn.com/gtgmzojxqe.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gttuzcocsg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtwpzfciek.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtmtnxakzh.html


<!-- 参考信息 -->