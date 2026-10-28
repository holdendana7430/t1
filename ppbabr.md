代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shuidangran.top/gtuumieqxe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtpbqqvryb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtqrcgrjsi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fengsongda.top/gtharygebz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.meibo888.top/gtyvxglbwi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gthhqlgbke.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtwkrqlpiq.html

[C09] 递归
来源：http://hz.chenjidiqi.icu/gtrgewoivk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.havefunace.top/gtwvsozgau.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgufenzy.top/gtsndznnfc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtjozbofau.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gthcsssapn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtisbwwfey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gogol.net.cn/gtscxbzxrf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gttilnofae.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhongyouzk.top/gtijgdmvop.html

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtgmkvkbax.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtbglvthed.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtmtsfdcnj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jiagoushi.top/gtzetcbnwp.html

TS:   同 JS
来源：http://hz.yongpay.top/gtladrqafs.html

Java: 方法内为块级作用域
来源：http://hz.aizwys.cn/gtuddqzrmu.html

Go:   花括号块级作用域
来源：http://hz.zhixingplan.top/gtjwwkffks.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.haohaochexian.top/gtlwwbcjwh.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gttmlpwseh.html

[C11] 模块导入与导出
来源：http://hz.nanxuanxn.top/gtpkjoniwg.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtsgsyioav.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gtzprldshd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhijiandao.cn/gthwhckppw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhoulong.xyz/gttdwwcbca.html

Java: import java.util.List;
来源：http://hz.wangdashe.top/gthkweznpo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.iojbl.cn/gtwkoinoxe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yangfankeji.com/gtpozploab.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtfmsyptts.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigfzy.top/gtmtiuifdq.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gtegbzeaqh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtqcyqhifh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtxwoarchj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtpgsowibd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hfpthk.cn/gtkxhmdood.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtlwydtuqi.html

Ruby: -> { puts "run" }.call
来源：http://hz.iojbl.cn/gtzmkqhzjf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gtelyizipc.html

[C13] 类型声明 / 类型注解
来源：http://hz.aibaodan.cn/gtjviahgiy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.quarkkingdee.top/gtalgarykp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtidijoteb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtpvnscexa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aizwys.cn/gtsruwpedh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtkqxzigez.html

Go:   func add(a, b int) int
来源：http://hz.zhongyouzk.top/gtwksaraxe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shuidangran.top/gtpwuclvuw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hongshengwenyu.top/gtqrttbzar.html

[C14] 泛型函数
来源：http://hz.gogol.net.cn/gtkgvhetsh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.mhx1999.top/gtehdxwdcp.html

PHP:  // 无泛型
来源：http://hz.cqqwz.cn/gtdbahvtkf.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtyhyegzpu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydzc1.top/gtpiatjzeo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtgqbwuudc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtvwdavumb.html

Ruby: # 无泛型
来源：http://hz.dianchejie.cn/gtkeggmani.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgufenzy.top/gtvckhagee.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtwsqqtirf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.0kj1m.cn/gtuikchknt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cucudq.cn/gtyzxmvtsj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gttstjndsl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.iojbl.cn/gtmyclqnug.html

Java: // 无解构
来源：http://hz.0kj1m.cn/gtoszfefja.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gtqvzsvnef.html

Ruby: a, b = pair
来源：http://hz.xingfuxueyuan.xyz/gtrlnbfxci.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gtmbwvxpcr.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtrfoclksi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhaomingkeji.xyz/gtoezicigf.html

PHP:  // 无重载
来源：http://hz.hnxiangtu.top/gtwymkdsya.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gttjtsohln.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gthirdlnkx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtssyvaiem.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangdashe.top/gthpmjxtfl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.meibo888.top/gthfcxzueo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhengqikj.top/gtsgogmrbj.html

================================================================================
来源：http://hz.gotoacloud.top/gtecmbfubr.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtkzicoogp.html

================================================================================
来源：http://hz.cqqwz.cn/gtzyssutco.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtaalbkfej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258.top/gtyojuisjf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtmzllglgr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtkgbahops.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtatqeqitu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtyxawxvbw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258.top/gtkphnsfib.html

Ruby: arr = [1, 2, 3]
来源：http://hz.kuanghao11.cn/gtjpgunctl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhiwuduotai.top/gtsxyoltbu.html

[D02] 追加元素到末尾
来源：http://hz.zhiwuduotai.top/gtwzslxqfi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jiagoushi.top/gtnxriiwky.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenlongwang.top/gtusgnffqv.html

JS:   arr.push(4);
来源：http://hz.hongshengwenyu.top/gtowdmfuck.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtvdnluict.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtdqqzhjfi.html

Go:   arr = append(arr, 4)
来源：http://hz.cashguo.top/gtjdsmqvjt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yangfankeji.com/gtdqimivta.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtioybxdcw.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtrbbrxwua.html

Py:   arr.insert(0, 0)
来源：http://hz.aizwys.cn/gtzzzrsywc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aibaodan.cn/gtgwizktzv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gtzbnhqdkp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gtlmbavtth.html

Java: list.add(0, 0);
来源：http://hz.shuidangran.top/gtmsiwvedb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtevqfrkec.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yonumen.top/gtfmknqxpb.html

C#:   list.Insert(0, 0);
来源：http://hz.sxryk.cn/gtibbnawob.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gthjxpmoug.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtrlnotjlg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtuluoeoqi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xylfe.cn/gtbointxsl.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxuanxn.top/gtindncdlg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guannengcc.top/gtphpeirah.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtgbwiypcr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gtiisjtllt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shzxlz.cn/gtmaorcicj.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gttehrnpwf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtdnbkhzso.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtgnlkqmya.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtyvgirrwc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnqzz.top/gtvtrikakv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtlbwbgdls.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fengsongda.top/gtdpfbgruk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtxgyfytgb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gttuqgtnzd.html

[D06] 数组长度
来源：http://hz.svipenyu.cn/gtqvdisbzn.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gttghaeero.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gtbtuuorgg.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtvztaavzn.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtafquyftd.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtqbrjxkxk.html

Go:   len(arr)
来源：http://hz.gogol.net.cn/gtrosplgno.html

Ruby: arr.length; arr.size
来源：http://hz.xingfuxueyuan.xyz/gtrcggircw.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gtxirqbaei.html

[D07] 切片 / 取子数组
来源：http://hz.xuanzx.com/gtfhodvgfl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gttelgenwo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.wangdashe.top/gthetbquqa.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtecynbokn.html

TS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtqiygpkij.html

Java: list.subList(1, 4);
来源：http://hz.zycfv.cn/gtlsoowcyd.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtqxisxcta.html

Ruby: arr[1, 3]
来源：http://hz.yvedp.cn/gthxrumwxs.html

C#:   list.GetRange(1, 3);
来源：http://hz.guowangkeji.top/gtkxscdujx.html

[D08] 合并两个数组
来源：http://hz.svipenyu.cn/gthvxggkax.html

Py:   a + b;  a.extend(b)
来源：http://hz.jiagoushi.top/gtxswomcmd.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtharszheh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtyhnjaovm.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gtdszytycn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtvaxxvipk.html

Go:   append(a, b...)
来源：http://hz.0kj1m.cn/gtjpzqeueu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtasmszikj.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtseuoxkox.html

[D09] 排序（升序）
来源：http://hz.aizwys.cn/gtfhsgwcte.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtffshuffg.html

PHP:  sort($arr);
来源：http://hz.sweek.top/gtqyumtaek.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnqzz.top/gtgsfdhmgx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ydzc1.top/gttbcogodn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtzksekdyr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtusmjzrbc.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtpkxgdfqh.html

C#:   list.Sort();
来源：http://hz.svipenyu.cn/gtqzwgvwrx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinyuanbaomall.cn/gtxbnjdeyb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.mhx1999.top/gticcuortx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtyxeyiwbf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtxixzxvhi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtpiiigvlf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.52xcode.cn/gtkgxjvsec.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guannengcc.top/gtbyvlrnjw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtdhvetkxp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dianchejie.cn/gtkzouacuh.html

[D11] 反转数组
来源：http://hz.tanke756.top/gtycdvsbce.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigfzy.top/gtidqjtggz.html

PHP:  array_reverse($arr);
来源：http://hz.chenzaomai.com/gtcpdefpup.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtfigvasij.html

TS:   [...arr].reverse();
来源：http://hz.guannengcc.top/gtnfnfpypj.html

Java: Collections.reverse(list);
来源：http://hz.gaohongyu789.top/gtpurddkao.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gteepuhynf.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gtuwkbjdsz.html

C#:   list.Reverse();
来源：http://hz.andypj.xyz/gtlfubtlag.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtppycjhvq.html

Py:   arr.index(x);  x in arr
来源：http://hz.shzxlz.cn/gtfbbffamv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sysykeji.top/gtazaqeihm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtynlflpzi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gttvzbbvpo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gtvsvwwrag.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtrenauplh.html

Ruby: arr.index(x)
来源：http://hz.daxiang520.top/gtixgpmvfi.html

C#:   list.IndexOf(x);
来源：http://hz.havefunace.top/gtrnsvaoth.html

[D13] 过滤（保留满足条件的）
来源：http://hz.bjfxy.top/gtgqldlgxk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinqigufen.top/gtxordfhzk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtyutdsdkz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtrprnluqu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtfoqfdwyf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtbrmtndhs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nwbrower.top/gtlgmrzyrp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuxming.cn/gtoaictjce.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gtkmiwcqfn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aizwys.cn/gtbpgzgmed.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtphftakdm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtieagghke.html

JS:   arr.map(x => x * 2)
来源：http://hz.xuanzx.com/gtsgzxyroc.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtpkkrnkod.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhixingplan.top/gtzlcvmafa.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gthnyevjig.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daxiang520.top/gtjtgtvlqg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtmryrscwb.html

[D15] 去重
来源：http://hz.yueranfly.top/gthbtrnbuk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtsronfcwo.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtyyroxneo.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtybuvjzbz.html

TS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtfkrwkxqf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtmqmdhgja.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtjstrdfwm.html

Ruby: arr.uniq
来源：http://hz.andypj.xyz/gttyyfdqye.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgufenzy.top/gttpvjueig.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtlralcucw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangshuangyany.cn/gtdybcwwuk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtpmsptmho.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gtzgfpvijw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtzvcrvkel.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtnulpxnef.html

Go:   // 手写循环累加
来源：http://hz.bjfxy.top/gtlavlwimw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.snrcjt.cn/gtsjxnkzuc.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtjnuybtje.html

[D17] 最大值与最小值
来源：http://hz.shzxlz.cn/gtlazopzgj.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtywwgdrba.html

PHP:  max($arr);  min($arr);
来源：http://hz.ehwqpu.com/gtchoysthf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gtrskoicle.html

TS:   Math.max(...arr);
来源：http://hz.xuanzx.com/gtdhdpeyiz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtkublonyj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnqzz.top/gtwvgjbglt.html

Ruby: arr.max;  arr.min
来源：http://hz.jyoumei.cn/gtseodwqdh.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtmgfofdje.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtfgxkywua.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zdqjudy.top/gtcuqctbpg.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtnzzrizmr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gttkbqhpud.html

TS:   nested.flat();
来源：http://hz.jinqigfzy.top/gtblczxgnz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xuanzx.com/gtgqluxeiu.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtffeqglwi.html

Ruby: nested.flatten
来源：http://hz.haohaochexian.top/gtnyswlojg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.meibo888.top/gtjwgljmix.html

[D19] 按字段分组
来源：http://hz.yuanzhike.top/gtgcbmvufl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtehkkouuo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gtdkpbrrnl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtgrxhaskv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gttyftomrk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cqqwz.cn/gtlzyxqyem.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtsxyjfqbx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangdashe.top/gtbemnposj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtnepdtnem.html

[D20] 统计每个元素出现次数
来源：http://hz.hfpthk.cn/gteweyevvp.html

Py:   Counter(arr)
来源：http://hz.cqqwz.cn/gtndpmxhdc.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gthcdzwixz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtbgrfbirk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtntjgcfnc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtgtolujye.html

Go:   // 手写 map[T]int
来源：http://hz.0kj1m.cn/gtnhqxnkan.html

Ruby: arr.tally
来源：http://hz.xingfuxueyuan.xyz/gtlkfcksce.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ivvv.top/gtmwbjbrlr.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtxtdladah.html

Py:   x in arr
来源：http://hz.yuxming.cn/gtrnxrsadw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtxawulkkx.html

JS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtrjtmwvbl.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtxgdbkyog.html

Java: list.contains(x)
来源：http://hz.xinyue.icu/gtcrdgezlx.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtlctluehc.html

Ruby: arr.include?(x)
来源：http://hz.tianlin.xyz/gtrazdoogu.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gtgzkmlfuq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhijiandao.cn/gtsvrfxflb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtzxmgromg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gtqwqhmgkt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sweek.top/gtqctmimli.html

TS:   [...arr];
来源：http://hz.shzxlz.cn/gtfpvjucmo.html

Java: new ArrayList<>(list);
来源：http://hz.zhoulong.xyz/gtonvuwacv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtotxnveoi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gzhubu.top/gtscfqxanz.html

C#:   new List<int>(list);
来源：http://hz.cheryme.top/gtmemdgjou.html

[D23] reduce 累积计算
来源：http://hz.yuanzhike.top/gtejxfqyvj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gthsapkvmz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.mhx1999.top/gtkznhpjjl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtgqehfhbg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtmrxgcukz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtjwxjufgw.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtfutqnvbc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtqvhjalsi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhaomingkeji.xyz/gtfgudmnnj.html

[D24] 字典 / Map 基本操作
来源：http://hz.shuidangran.top/gtgzyhshwc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtewbbtxzd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xylfe.cn/gtggrxysnq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gthtkqdufn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gthtzvawzf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pengpengdd.cyou/gtpwsadqru.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtzyjtygsr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xziqi.cn/gttutquscm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtinvrdgvk.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtckmmzaxg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtgxhpgpwq.html


<!-- 参考信息 -->