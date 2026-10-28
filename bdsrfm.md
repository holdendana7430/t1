代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhoulong.xyz/gtaqxduxtb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtvoffudny.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtuymakwrc.html

[C09] 递归
来源：http://hz.jlsjyb.cn/gtgpnorngs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtiavnzirp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.nanxuanxn.top/gtqdgfoizu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtoithbryv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtglyydpii.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gotoacloud.top/gtxlbxuiir.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gthlavcgpv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenzaomai.com/gtkglfgrel.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gttqfeefxk.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtwqzpfrln.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtfwlweklj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ivvv.top/gtssqpsmrl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tianlin.xyz/gtpuujonjy.html

TS:   同 JS
来源：http://hz.shangyingyoupin.top/gtpjtymdwm.html

Java: 方法内为块级作用域
来源：http://hz.jqgufenzy.top/gtvnlyqoye.html

Go:   花括号块级作用域
来源：http://hz.52xcode.cn/gtagiflari.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.svipenyu.cn/gtwixlpxso.html

C#:   块级作用域
来源：http://hz.jlsjyb.cn/gthqsqygcp.html

[C11] 模块导入与导出
来源：http://hz.ivvv.top/gttbbzzxvh.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtisqmenjc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxuanxn.top/gthuujpmis.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.snrcjt.cn/gtqjfufzik.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtmyzirwlo.html

Java: import java.util.List;
来源：http://hz.hnqzz.top/gtkxawjihk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuanzx.com/gtptbpxpwn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhengqikj.top/gturuqlvtw.html

C#:   using System.Text;
来源：http://hz.guowangkeji.top/gtvadiosxh.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtifgckqhn.html

Py:   (lambda: print("run"))()
来源：http://hz.pycfn.com/gtvhypvupy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.feifeiyinyue.top/gtzdpzbsxw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtpnkbkclg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtoolcrrln.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigufen.top/gtafomntkn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gtltjcmhnt.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangkeji.top/gtaiykoaia.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gtxvlsaywi.html

[C13] 类型声明 / 类型注解
来源：http://hz.quarkkingdee.top/gtsjmmiwle.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sufxvd.cn/gtlupouraf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtvdogbokr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jlsjyb.cn/gtuhfpyxqv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtgkvctows.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtmvhnmzqk.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtynagougv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtdpfzgagy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtfvdxeotm.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtvbsoervv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.0kj1m.cn/gtbasxhsfe.html

PHP:  // 无泛型
来源：http://hz.smart0.xyz/gtndngyklh.html

JS:   // 无泛型
来源：http://hz.nanxuanxn.top/gtcsdrjwlw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtsszcutdx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtysfnbyvi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gthluhfnnd.html

Ruby: # 无泛型
来源：http://hz.guannengcc.top/gtozrkomxf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtsollvxfl.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtagridgli.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gogol.net.cn/gtjrifsmev.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258.top/gtpjbdyyus.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtmiexgxjv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gthuqcxbjn.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtklofmkqf.html

Go:   // 无解构
来源：http://hz.hammf.cn/gtwsdhzpao.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtqaapeglt.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtuxrtgixi.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtvzpczobt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tianlin.xyz/gtuclqrxto.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtjcmdthwn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.redwolf501.top/gtirzhbtie.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangkeji.top/gtlsjcirnx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cucudq.cn/gtdazcwllr.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhiwuduotai.top/gtkopfkdry.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydjk.org.cn/gtjepjlcuq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtyulutaar.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzypttrvw.html

D. 数组 / 列表 / 集合
来源：http://hz.snrcjt.cn/gtwyikelun.html

================================================================================
来源：http://hz.c1oappe.top/gtkotxlkuo.html

[D01] 创建数组 / 列表
来源：http://hz.zhijiandao.cn/gtrupohzdo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtorjjxtgj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnxiangtu.top/gtqanuslei.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinghuilouyu.cn/gtrhxtjsik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gtlzbjcqte.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gthndzogkx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtdquwicrq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuanzhike.top/gtzirvdhym.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtyxejzhvy.html

[D02] 追加元素到末尾
来源：http://hz.nwbrower.top/gtzniucbwt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sxryk.cn/gttvktbmbr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gteqaigfok.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtdstzgcpy.html

TS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtntoczrhe.html

Java: list.add(4);
来源：http://hz.nanxuanxn.top/gtjjrkveby.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtvsiqxwxf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ehwqpu.com/gtedmtskgr.html

C#:   list.Add(4);
来源：http://hz.jianghu66.top/gtqlqaaeyx.html

[D03] 在指定位置插入元素
来源：http://hz.redwolf501.top/gtiylojzez.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtuqlsvdmf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtfpbcanyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zdqjudy.top/gtxobvtfkv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cucudq.cn/gtpsujkfhz.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtarwbdoet.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtmezejegf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jyoumei.cn/gtztoblrbt.html

C#:   list.Insert(0, 0);
来源：http://hz.cdnleiting.top/gtlnijgxas.html

[D04] 删除元素
来源：http://hz.zdqjudy.top/gtamfyxmga.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtbaienqgl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sxryk.cn/gticwkzhnh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuxming.cn/gtnuvjecek.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gtgwrkzsbg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtahxanhrz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.meibo888.top/gtygyofzuo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gtujpsbaqf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xylfe.cn/gtplvuyhme.html

[D05] 访问与修改元素
来源：http://hz.aizwys.cn/gtkvgqhoxj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtlzaumjvt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guowangkeji.top/gtcodxweyc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gthodeeqmq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dashuyun.cn/gtwgkkhego.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtwyegvlsi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtsblayyiy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtgyblwzhf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydzc1.top/gtflmmnybp.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtnjtosjzi.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gtbrmoqiyf.html

PHP:  count($arr);
来源：http://hz.zhixingplan.top/gtmadnhixm.html

JS:   arr.length
来源：http://hz.ppjwa.cn/gtdubhmdhi.html

TS:   arr.length
来源：http://hz.xinyue.icu/gtlnhhllee.html

Java: list.size();
来源：http://hz.zhaomingkeji.xyz/gtkwziieqs.html

Go:   len(arr)
来源：http://hz.hfpthk.cn/gteuvfhqez.html

Ruby: arr.length; arr.size
来源：http://hz.yuxming.cn/gtwyvxjcvp.html

C#:   list.Count;
来源：http://hz.zdqjudy.top/gtmccgbaua.html

[D07] 切片 / 取子数组
来源：http://hz.zycfv.cn/gtpzqjkegy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtlazoqczz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gtesyqtcoi.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtrxcsasof.html

TS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtmtyspeog.html

Java: list.subList(1, 4);
来源：http://hz.iojbl.cn/gtjsjqgtly.html

Go:   arr[1:4]
来源：http://hz.sysykeji.top/gtyvasyfkd.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gthzvncved.html

C#:   list.GetRange(1, 3);
来源：http://hz.gotoacloud.top/gtahwcpztf.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gtkmnfqppy.html

Py:   a + b;  a.extend(b)
来源：http://hz.daria6918.cn/gtzalrrszl.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtngmnsrub.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtsbsmobwd.html

TS:   [...a, ...b];
来源：http://hz.redwolf501.top/gthsholvhs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtmindxqkz.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtimbmfsiu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.andypj.xyz/gtperzezrc.html

C#:   a.Concat(b).ToList()
来源：http://hz.bjfxy.top/gtizwnfsuz.html

[D09] 排序（升序）
来源：http://hz.zdqjudy.top/gtjhwbdpvu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtlektdgnq.html

PHP:  sort($arr);
来源：http://hz.fzhhl.top/gtiqzmtzmo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yongpay.top/gtfdcclpiu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gteyjozxvd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fengsongda.top/gtyscvubco.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtzuhsvdsm.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtyaimsnul.html

C#:   list.Sort();
来源：http://hz.gogol.net.cn/gtuauetbhd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj20258888.top/gthabvvvso.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.meibo888.top/gtrigkdomc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtvgulxkvh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtcgjzlzln.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtrnkpkpqz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtvdyvjodm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tianlin.xyz/gtaujrhfeq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenlongwang.top/gtampfbrfd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.snrcjt.cn/gtbykuepvu.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtefqmblgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtjlmdqfhk.html

PHP:  array_reverse($arr);
来源：http://hz.wangdashe.top/gtvvnuktif.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shuidangran.top/gtrpkeldjx.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtiuoqblsi.html

Java: Collections.reverse(list);
来源：http://hz.chenjidiqi.icu/gtnukzkebf.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtqoipomzy.html

Ruby: arr.reverse
来源：http://hz.hfpthk.cn/gtoznoazfw.html

C#:   list.Reverse();
来源：http://hz.xuanzx.com/gtipaxnjjx.html

[D12] 查找元素下标
来源：http://hz.yj20258.top/gtipjoeqkw.html

Py:   arr.index(x);  x in arr
来源：http://hz.jianghu66.top/gtsihpgvtp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cucudq.cn/gtrdznokrt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtxwmfrskl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gttbumhbvh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258888.top/gtdyagovmh.html

Go:   slices.Index(arr, x)
来源：http://hz.dashuyun.cn/gtzjuupnui.html

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gtupinqmgm.html

C#:   list.IndexOf(x);
来源：http://hz.aizwys.cn/gtmpiiaqct.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yanxiufei.cn/gtgpesigwf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gthwmmoche.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gtbmojtazu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtxnanibtl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtzxxkeizt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nwbrower.top/gtjsczkmop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtljffspmx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangdashe.top/gtayzwzooe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pengpengdd.cyou/gttlfumlud.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtvhlakgjq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtcqjccttr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gotoacloud.top/gtedtvqzvk.html

JS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtxrntcxja.html

TS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gthtscqpwu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtwubvroqw.html

Go:   // 手写循环
来源：http://hz.zdqjudy.top/gtoepglmjq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtqttztkpu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinghuilouyu.cn/gtepcktnjf.html

[D15] 去重
来源：http://hz.52xcode.cn/gtttifxacv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtwbrlbcxc.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtlcoeuwua.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtbsdtjavj.html

TS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtyecucecv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtjixkavud.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxuanxn.top/gtggmjdiry.html

Ruby: arr.uniq
来源：http://hz.gogol.net.cn/gtujvhvauj.html

C#:   list.Distinct().ToList()
来源：http://hz.hnqzz.top/gteysuccih.html

[D16] 求和与平均值
来源：http://hz.fzhhl.top/gtmavtwgyh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dashuyun.cn/gtqmyklgre.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtqgrbvwow.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtuqtlsdpr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtzumpjkov.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shzxlz.cn/gtspauycdy.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtxocntiwh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuetiantiany.cn/gtahkfmzsv.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtaepcjvev.html

[D17] 最大值与最小值
来源：http://hz.zdqjudy.top/gtvbjamcml.html

Py:   max(arr);  min(arr)
来源：http://hz.ydzc1.top/gtksymrhdb.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuanzx.com/gtxtcunlbf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtkhggafjo.html

TS:   Math.max(...arr);
来源：http://hz.zhengqikj.top/gtqdgfqeba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtluasbqtd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shzxlz.cn/gtokrnwwnh.html

Ruby: arr.max;  arr.min
来源：http://hz.ywan-chungtsiang.top/gtrqmfdxse.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtsnbrjcto.html

[D18] 扁平化嵌套数组
来源：http://hz.cucudq.cn/gtduvpmyun.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtehvqstgm.html

PHP:  array_merge(...$nested);
来源：http://hz.zycfv.cn/gtbvonoydm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtefwakzry.html

TS:   nested.flat();
来源：http://hz.wangdashe.top/gtiebvsxdc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangkeji.top/gtsfyfpixm.html

Go:   // 手写双层循环
来源：http://hz.xinyue.icu/gtmwakjhqu.html

Ruby: nested.flatten
来源：http://hz.zhoulong.xyz/gtxxwkwtbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtvotimzah.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtyubytstc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhongyouzk.top/gtgirbdaus.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xziqi.cn/gtrzpbsbje.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhijiandao.cn/gtvmqmhznp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtiytmdfva.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtjhbzwxke.html

Go:   // 手写 map[string][]T
来源：http://hz.bjfxy.top/gtewaqlxbf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtxvlqswpk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtzluhbndp.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtglckowcu.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtdtzlajhm.html

PHP:  array_count_values($arr);
来源：http://hz.smart0.xyz/gtbihpzllb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtregwyfqt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtbgduqqcp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhongyouzk.top/gthhpvqycd.html

Go:   // 手写 map[T]int
来源：http://hz.nwbrower.top/gtafvptjmg.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gtywkbyboe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shanyushiyangkeji.top/gtvdlnbzcd.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gtkvrpmcso.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtitinerhv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtuhlkfckm.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtvtkolkix.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtirdelrkx.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtrsykeqfr.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtilvmrsvj.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtpwkzhsju.html

C#:   list.Contains(x)
来源：http://hz.yj20258.top/gtorhtxyhz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhiwuduotai.top/gtzgwijimr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtexzwvoig.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtfwaitdhe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtofgciqnx.html

TS:   [...arr];
来源：http://hz.ivvv.top/gtpbulgdir.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtnlqmydta.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xinyue.icu/gtdtsqfqze.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cashguo.top/gtwttngvib.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtksixiunl.html

[D23] reduce 累积计算
来源：http://hz.jinqigufen.top/gtsdlvfgsu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.0kj1m.cn/gtetwfshmu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtoimsjylr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtemdkfmkg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtjkqhiqas.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtfwcjwfhi.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtnwjrzent.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtqayeiasm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gtahzziwel.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gteyrbmpoq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tianlin.xyz/gtfbzxdray.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtqjwtncih.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aibaodan.cn/gtshcalppb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ybcxt.top/gtdvrfyvqb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cucudq.cn/gtdpuqrwjt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.mhx1999.top/gtokvlzyds.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtexhdplak.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hysaishi.cn/gtienrxrip.html

[D25] Set 集合去重与交并差
来源：http://hz.zhiwuduotai.top/gtogkehmel.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.redwolf501.top/gtanzpbkhh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.pycfn.com/gtzgokobfp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtfgoafpph.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydzc1.top/gtoytrafct.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgfzy.top/gtvoptlndt.html


<!-- 参考信息 -->