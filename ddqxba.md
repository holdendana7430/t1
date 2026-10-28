代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtimmzpkfs.html

Go:   return a, b
来源：http://hz.ppjwa.cn/gtkcpvpwvq.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtukdayufh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtecxqcqux.html

[C06] 匿名函数 / lambda
来源：http://hz.cashguo.top/gtscpweymc.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtuuvxiqbj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gttieglivw.html

JS:   const square = x => x * x;
来源：http://hz.nanxinkj.top/gtvexcbirg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgufenzy.top/gtjvskgzau.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.redwolf501.top/gtvgskdjae.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.bjfxy.top/gtpybcrwmr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.haohaochexian.top/gthlpqvvtn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gtjqbjpskz.html

[C07] 把函数作为参数传入
来源：http://hz.shangyingyoupin.top/gtrnczchgu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtzikiizif.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.kuanghao11.cn/gthuwpggig.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258888.top/gteeqdpxsq.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtdfsmxcuo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nwbrower.top/gtgwnektro.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgfzy.top/gtsopdmskx.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydjk.org.cn/gtfobcijwp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.iojbl.cn/gtquuuxlgl.html

[C08] 闭包
来源：http://hz.yuanzhike.top/gthzdddjaq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuanzhike.top/gtaakpcllr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zdqjudy.top/gtvjswkgwr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtxuwovpfm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtathpcufe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtwtechnpt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yangfankeji.com/gtubohlane.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenjidiqi.icu/gtgnkdmzdg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtgpoezkos.html

[C09] 递归
来源：http://hz.xinyue.icu/gtfodxhqlf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxuanxn.top/gtokgtmawf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hfpthk.cn/gtextpkymv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtebacmoqq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtewnlmyxi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shuidangran.top/gtuoaoifxg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ivvv.top/gtymectkaw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nwbrower.top/gttwypbesv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nwbrower.top/gtasndpnnc.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtugsxenbe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ehwqpu.com/gtjdnkzhhv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtabwebibc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtqovelgsa.html

TS:   同 JS
来源：http://hz.zhaomingkeji.xyz/gtfbwtspbq.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtxuyyennr.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtwwqcemkf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuanzx.com/gtioziakgn.html

C#:   块级作用域
来源：http://hz.meibo888.top/gtryxwnbvx.html

[C11] 模块导入与导出
来源：http://hz.guowangkeji.top/gtfcgbogkn.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtxknjducj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtzszttjdh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daria6918.cn/gtikqiiaxi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xziqi.cn/gtyxhmipqj.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtefyiipju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtnaefcjjm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hysaishi.cn/gtnttipnaw.html

C#:   using System.Text;
来源：http://hz.c1oappe.top/gtovqbsbmr.html

[C12] 立即执行函数 IIFE
来源：http://hz.316326.xyz/gtsxmmqeea.html

Py:   (lambda: print("run"))()
来源：http://hz.yonumen.top/gtvwhguhvb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yongpay.top/gtpibkplts.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtsbjxivmt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtedodceym.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gttfqzylvf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhongyouzk.top/gtyvsatwor.html

Ruby: -> { puts "run" }.call
来源：http://hz.vqdsnc.cn/gtjomxnbnb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yanxiufei.cn/gtlziemnjq.html

[C13] 类型声明 / 类型注解
来源：http://hz.aibaodan.cn/gtcwjlqilc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtcsuzmvgu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtkchiinil.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtmvthntof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtfvnedjll.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtqiblkpnx.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtbmrxqkby.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtppjhagqb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tanke756.top/gttmmnfnjz.html

[C14] 泛型函数
来源：http://hz.yvedp.cn/gtrpslmcdp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yonumen.top/gtcmyhiayx.html

PHP:  // 无泛型
来源：http://hz.tianlin.xyz/gtljdqihfn.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtyndpbkmm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtojcowekz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hywenlv.cn/gtnvsvrvue.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ywan-chungtsiang.top/gttyelzxcd.html

Ruby: # 无泛型
来源：http://hz.dashuyun.cn/gtjuemenzw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hongshengwenyu.top/gtydmjbhmg.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtjhrwtrjs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtxpgvyjqf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guowangkeji.top/gtjrnwsnpg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhoulong.xyz/gtjldyctda.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gtawncrgxu.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gteiihwdof.html

Go:   // 无解构
来源：http://hz.c1oappe.top/gtwkexgixb.html

Ruby: a, b = pair
来源：http://hz.zhijiandao.cn/gtzstxwgzc.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gthfgueqzs.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gtnznzxltv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gthgdzepxo.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gttntbsnac.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtzsyxamdt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gzhubu.top/gtctdsjymg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gtjobucdet.html

Go:   // 无重载：用不同函数名
来源：http://hz.sweek.top/gtrdtavdze.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhengqikj.top/gttnxynqyo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hammf.cn/gtnsvujbto.html

================================================================================
来源：http://hz.yj20258.top/gteveztqtv.html

D. 数组 / 列表 / 集合
来源：http://hz.birdmap.top/gtfkyyjipy.html

================================================================================
来源：http://hz.tian-w.cn/gtsopusmxv.html

[D01] 创建数组 / 列表
来源：http://hz.dianchejie.cn/gtteoxrpxx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shangyingyoupin.top/gterqirsym.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gtxepdoqdw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhiwuduotai.top/gtadtodicn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gzhubu.top/gtmhzpzblq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtvmjlyatl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yanxiufei.cn/gtrjncytns.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigfzy.top/gtyiwvkafs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guannengcc.top/gtgyrakqkx.html

[D02] 追加元素到末尾
来源：http://hz.daria6918.cn/gtcojlqxez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gttlsumkiv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtcylsiyti.html

JS:   arr.push(4);
来源：http://hz.chenzaomai.com/gthenhgtbu.html

TS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtqmbosgvk.html

Java: list.add(4);
来源：http://hz.vqdsnc.cn/gtwtiecjes.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gtjuuhrzpg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxinkj.top/gtzvlvceoc.html

C#:   list.Add(4);
来源：http://hz.haohaochexian.top/gtphcwtvrn.html

[D03] 在指定位置插入元素
来源：http://hz.hongshengwenyu.top/gtmkoswvfq.html

Py:   arr.insert(0, 0)
来源：http://hz.yonumen.top/gtjodswvdf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shangyingyoupin.top/gtvrfxywvj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.quarkkingdee.top/gtagiziupf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtnvaeiuth.html

Java: list.add(0, 0);
来源：http://hz.jyoumei.cn/gtsffabhad.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangdashe.top/gtkovbkpwx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daria6918.cn/gtfytabexk.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtkvptzmmu.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtjiiuuton.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.c1oappe.top/gtikxrkdvo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtwvgxbtke.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtpdlcjcsd.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gtvtwtlewy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnqzz.top/gtukzjprez.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tianlin.xyz/gtwvcvxgap.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxuanxn.top/gtzvzgyerk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtbbzkkmli.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtbaqyirny.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtdehftmpy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtuvbjtnfe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtvdlrmtnz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sweek.top/gtehtcifra.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtrmjbxrlb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtbdzsvelj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtjsjgjnxw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtrwucxhqg.html

[D06] 数组长度
来源：http://hz.redwolf501.top/gtiwpsrbfb.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtqntpptve.html

PHP:  count($arr);
来源：http://hz.haohaochexian.top/gtfajcsklf.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtgiinpvsh.html

TS:   arr.length
来源：http://hz.vqdsnc.cn/gtbqpcfqai.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtyhwcbtqe.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtmiyirufl.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gtwqyevukl.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtkfwxpeyg.html

[D07] 切片 / 取子数组
来源：http://hz.sxryk.cn/gtnuszxglh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gotoacloud.top/gtrzwcvftr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xylfe.cn/gtkhydtcru.html

JS:   arr.slice(1, 4);
来源：http://hz.aizwys.cn/gtlojtpmso.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtgixnvjne.html

Java: list.subList(1, 4);
来源：http://hz.zhijiandao.cn/gtpeceuawr.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtaawjyzif.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gtxgvnhall.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtkxycgtvb.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtkdfqzioj.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtlferwewd.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtxhlyjrqo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gturzyhkek.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtlffhzzcz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtrclizwho.html

Go:   append(a, b...)
来源：http://hz.chenjidiqi.icu/gtoernijhl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtmkeupmgs.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gtsxokevdt.html

[D09] 排序（升序）
来源：http://hz.guannengcc.top/gtysqsmdyh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtamarxlri.html

PHP:  sort($arr);
来源：http://hz.kuanghao11.cn/gtbsnlntqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenjidiqi.icu/gtgvwrjsps.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtasxvkfkg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenzaomai.com/gthubppjmt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtfecvkxrg.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtalzvatsy.html

C#:   list.Sort();
来源：http://hz.redwolf501.top/gtsvhnfbvy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtrpsdmqkj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gttimzufxk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtgbsgrbdi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtdaatpiem.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gttjdndpxx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtiebzwsvs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jiagoushi.top/gtyqxvdcks.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.iojbl.cn/gthsmvbpnf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhongyouzk.top/gtoapfqtvm.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtgekjadoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtjgdiqrhi.html

PHP:  array_reverse($arr);
来源：http://hz.zhengqikj.top/gtvwqmglan.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gthervvugy.html

TS:   [...arr].reverse();
来源：http://hz.shzxlz.cn/gtemnygduv.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtrxzauksc.html

Go:   slices.Reverse(arr)
来源：http://hz.cdnleiting.top/gtiothxjqc.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gttsyphiej.html

C#:   list.Reverse();
来源：http://hz.tianlin.xyz/gtossxihyo.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtppfmtppe.html

Py:   arr.index(x);  x in arr
来源：http://hz.guowangkeji.top/gtlupsymch.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gtryaqvxir.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtixyeazuf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtegvrhhaf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtvaieueti.html

Go:   slices.Index(arr, x)
来源：http://hz.yangfankeji.com/gtgbvdoiju.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gthrfmspoo.html

C#:   list.IndexOf(x);
来源：http://hz.zhixingplan.top/gtdlikblmw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cdnleiting.top/gtdqubfloc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zycfv.cn/gtqcmgrmvz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gtbdiytvpi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtnawhhydb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtdvnizcpn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cheryme.top/gtgjeezqge.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtybsftisq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hammf.cn/gtmzqflgdv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydjk.org.cn/gtuadhobdk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangtech.top/gtsdqodjof.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenzaomai.com/gtskazowym.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhiwuduotai.top/gtlaovwluw.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtzbcczcvt.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtcqhptuyo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gthtqndqxl.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gthuxtjxbd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gogol.net.cn/gtwlnxyglo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fengsongda.top/gtnysskdjc.html

[D15] 去重
来源：http://hz.zycfv.cn/gtynvfhmkr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtcdmejrkz.html

PHP:  array_unique($arr);
来源：http://hz.316326.xyz/gtxluvnqbm.html

JS:   [...new Set(arr)]
来源：http://hz.birdmap.top/gtsxisayjj.html

TS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtbouezjea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xingfuxueyuan.xyz/gtyexlvmnc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gaohongyu789.top/gtlpgjguet.html

Ruby: arr.uniq
来源：http://hz.ivvv.top/gtyiiksvnh.html

C#:   list.Distinct().ToList()
来源：http://hz.guowangkeji.top/gtztgqcxvd.html

[D16] 求和与平均值
来源：http://hz.zdqjudy.top/gtnktgyvsq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258.top/gtoufxctst.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtsnfiiotz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtmocxntmy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtdwtplcli.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtpkcgaiaq.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtiosdffpp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtmefijhab.html

C#:   list.Sum();  list.Average()
来源：http://hz.ywan-chungtsiang.top/gtxxrkslue.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtjvludpdc.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangkeji.top/gtggypvzys.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gthgnpposk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtdmjqdkky.html

TS:   Math.max(...arr);
来源：http://hz.9152youxi.cn/gtfeqqbfrk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sysykeji.top/gthnuitykx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtiwiyigcg.html

Ruby: arr.max;  arr.min
来源：http://hz.quarkkingdee.top/gtecboyxzb.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtvxkwsgey.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtiaudsyua.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gtxnmfjzqi.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gtaybsxngh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nanxinkj.top/gtnyuifqzf.html

TS:   nested.flat();
来源：http://hz.quarkkingdee.top/gteyivhzev.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhengqikj.top/gtgipdjnsh.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtdekhqyws.html

Ruby: nested.flatten
来源：http://hz.yanxiufei.cn/gtvclqyezm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtyabthfdq.html

[D19] 按字段分组
来源：http://hz.xuanzx.com/gtlbjfltpm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gtczxgajye.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yanxiufei.cn/gtnfcozwcm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xylfe.cn/gtayxbntkf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gttryxjycw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pycfn.com/gtpttflxai.html

Go:   // 手写 map[string][]T
来源：http://hz.ppjwa.cn/gtkegbdwzj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258.top/gtmlxwfrty.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtxwkeqipa.html

[D20] 统计每个元素出现次数
来源：http://hz.jlsjyb.cn/gtcczsdjlf.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtqfokhtck.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtoasvvgff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtpkhzdjbz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtqlgdpkzt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.svipenyu.cn/gtkratthou.html

Go:   // 手写 map[T]int
来源：http://hz.hnqzz.top/gthokxbbrt.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtqbrnuaai.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yanxiufei.cn/gtcelofwqk.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gtrtwxmxoq.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtqhnipduk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shanyushiyangtech.top/gtwkbugrfy.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtevnpzrtm.html

TS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtbqqxndst.html

Java: list.contains(x)
来源：http://hz.havefunace.top/gtkgljajfz.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtntibnftx.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtznnwobdu.html

C#:   list.Contains(x)
来源：http://hz.chenzaomai.com/gtsgbevmnu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtotxrvccz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnxiangtu.top/gtjaqemxne.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtkrfwztys.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hysaishi.cn/gtnltmsiqa.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtegtywyuc.html


<!-- 参考信息 -->