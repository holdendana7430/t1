代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.xziqi.cn/gtghqmnxtz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtkqsteeop.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangkeji.top/gtwerhvixm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gtfaonrbix.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.9152youxi.cn/gtpnndyurw.html

[C07] 把函数作为参数传入
来源：http://hz.zhaomingkeji.xyz/gtohemwtkf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangkeji.top/gtggdlpvxo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gtmrtjaqyf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.pycfn.com/gtkgjfvgfr.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtlaivpnds.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangshuangyany.cn/gtcyrpehsy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gtxvneaskf.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangkeji.top/gtgafucfyl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgfzy.top/gtokxdxzod.html

[C08] 闭包
来源：http://hz.316326.xyz/gtweqvqpuq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xziqi.cn/gtskojiwij.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fzhhl.top/gtpbgfmxgz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtsrhzfpwx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtlqvlwofl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtsphbqydw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxuanxn.top/gtvzcqkjkz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangdashe.top/gtjcytfbok.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtjnuosihc.html

[C09] 递归
来源：http://hz.yonumen.top/gtnbqbdcmx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtdkilxkwo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gtsowgtrtf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtcacwrxtc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtkjvhlsed.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtvbvzkvwf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.iojbl.cn/gtfgugcnnx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yueranfly.top/gthjghyovg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.52xcode.cn/gtanjpbwph.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtftvqkbqo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtbfjhcjac.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.fengsongda.top/gtaefchedm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtuyqwtouc.html

TS:   同 JS
来源：http://hz.chenlongwang.top/gthssjydam.html

Java: 方法内为块级作用域
来源：http://hz.yuxming.cn/gtzzfejgxj.html

Go:   花括号块级作用域
来源：http://hz.hongshengwenyu.top/gtyekxffsn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gzhubu.top/gtvynnbzva.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtourqobti.html

[C11] 模块导入与导出
来源：http://hz.c1oappe.top/gthnftmxte.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtzmbcfmag.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hammf.cn/gtsmucoamu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtvivnturs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtdwwsjnha.html

Java: import java.util.List;
来源：http://hz.pengpengdd.cyou/gttvqzdyxg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtpwkchfsq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gtftlexepq.html

C#:   using System.Text;
来源：http://hz.sufxvd.cn/gtddybtmcd.html

[C12] 立即执行函数 IIFE
来源：http://hz.pycfn.com/gtquxwygqf.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtgscdrqzu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtsfgfeqiq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtnvqmbftt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtucirafgh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenzaomai.com/gtmffendpy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.mhx1999.top/gtmjpdafjs.html

Ruby: -> { puts "run" }.call
来源：http://hz.gogol.net.cn/gtycjplsll.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtxcrfelzq.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gtibariyjs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gthmzvqstb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtrhkzzrzx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtygncctjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hongshengwenyu.top/gthfrfcjdc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtwawfsdpd.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtprzfqvkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtcqjhtomm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangtech.top/gtbduragub.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtyjjjepst.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtcygeywtg.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtcugswocr.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtpcqfuicc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fzhhl.top/gtbzybdtxi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fengsongda.top/gtzdcxeifc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtnsyubegs.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gtgwbveojb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tanke756.top/gtvklphcyv.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gttwbykhue.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtrnldxsmv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gthvbfjzbw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtnarwoizf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gtaognfjjh.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gttfdkdwme.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gthtnwcalo.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtqcnlwfrn.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gtpllymazj.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtmnyseeld.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.0kj1m.cn/gtjkaxnmhv.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtgpuyrneg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtzggardex.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cheryme.top/gtdyktrqgb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gturhvehex.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxinkj.top/gtnpkkidro.html

Ruby: # 无重载：靠动态参数
来源：http://hz.svipenyu.cn/gtqpxpfsvt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tianlin.xyz/gtntvxxlsb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrwxstawn.html

D. 数组 / 列表 / 集合
来源：http://hz.daria6918.cn/gtmxywwgbk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtoeanwotu.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gthdofjapo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.iojbl.cn/gtffewpogu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daxiang520.top/gtnxgjukfj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtefgtbzjb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuanzx.com/gtjtsyglon.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtngepxyvi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jiagoushi.top/gtixlpfmjh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtosfalxdm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtmejiezfm.html

[D02] 追加元素到末尾
来源：http://hz.fzhhl.top/gttpiveymq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xinyue.icu/gtexwtwsnk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xziqi.cn/gtcojhoelb.html

JS:   arr.push(4);
来源：http://hz.yuanzhike.top/gtpqnbfqqd.html

TS:   arr.push(4);
来源：http://hz.zhixingplan.top/gtbtvrylvf.html

Java: list.add(4);
来源：http://hz.wangshuangyany.cn/gtyuhbcidx.html

Go:   arr = append(arr, 4)
来源：http://hz.52xcode.cn/gttykuxwkj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258888.top/gtazgjlbrn.html

C#:   list.Add(4);
来源：http://hz.zhoulong.xyz/gtpivoiqqh.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gtjhruivoq.html

Py:   arr.insert(0, 0)
来源：http://hz.pengpengdd.cyou/gtaosibrmg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenjidiqi.icu/gtfgxxbjso.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gtczkykwqm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yongpay.top/gteslogklp.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gteprowocg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgufenzy.top/gtacivxlbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shangyingyoupin.top/gtzmwenymt.html

C#:   list.Insert(0, 0);
来源：http://hz.yueranfly.top/gtexrxpxwp.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gttaizxzrq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sufxvd.cn/gtunxgafjo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daria6918.cn/gtwatgdgct.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhiwuduotai.top/gtzhtkealo.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtcqzqsdsh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtjurezutk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daxiang520.top/gtcrtmuuok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenzaomai.com/gthdeatnhq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtuoruufld.html

[D05] 访问与修改元素
来源：http://hz.yvedp.cn/gtmyivfwkq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtiksxnfim.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtazxsjzdm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtbfocvmic.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.haohaochexian.top/gtvmcvsipx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtggyscovm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtalyhhdrl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtsuoumgon.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.iojbl.cn/gtrauwvrqp.html

[D06] 数组长度
来源：http://hz.aizwys.cn/gtfbtspmop.html

Py:   len(arr)
来源：http://hz.yongpay.top/gtjuskbprw.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtgcpdcyjt.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtiynkxhwt.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gtruaekgkz.html

Java: list.size();
来源：http://hz.pycfn.com/gtliavcmbt.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtwatxpypx.html

Ruby: arr.length; arr.size
来源：http://hz.cdnleiting.top/gtxfgkdomn.html

C#:   list.Count;
来源：http://hz.ydjk.org.cn/gtnhrzumau.html

[D07] 切片 / 取子数组
来源：http://hz.yanxiufei.cn/gtqumngoie.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtwfcnqlih.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gtoxvdmjsf.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtnbdgzybt.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gthcxdknpe.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtdwodajqf.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtatcdbvzy.html

Ruby: arr[1, 3]
来源：http://hz.zycfv.cn/gtzubsnjmk.html

C#:   list.GetRange(1, 3);
来源：http://hz.hfpthk.cn/gtghixdgpp.html

[D08] 合并两个数组
来源：http://hz.jiagoushi.top/gtenyvqtpn.html

Py:   a + b;  a.extend(b)
来源：http://hz.gaohongyu789.top/gtkidqvkya.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtzvbmeazw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenjidiqi.icu/gtpoedqghp.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtttrpeayk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xinyue.icu/gtrphrtdvj.html

Go:   append(a, b...)
来源：http://hz.hywenlv.cn/gtehytdcsl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cashguo.top/gtadxomukp.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtmxdaofbr.html

[D09] 排序（升序）
来源：http://hz.jinyuanbaomall.cn/gtrlszswwh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gteldkzupu.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtktyvakai.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hfpthk.cn/gtvwqywwpo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.birdmap.top/gtxvwosuhq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtswwyrwht.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtavpqwsbl.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtvcudxzem.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtddcnjxrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinyuanbaomall.cn/gtptogvjtd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtxnzdlgjd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gtizkhtydt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtgsuqnrag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtyqdqcqgs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtcrblnnlb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hywenlv.cn/gtlmlfqghw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtlievobuj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtagtcoihi.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtoialwuee.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nwbrower.top/gtkkslsnce.html

PHP:  array_reverse($arr);
来源：http://hz.yanxiufei.cn/gtkwklmcjr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtzvjlktqq.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtjjnrivin.html

Java: Collections.reverse(list);
来源：http://hz.cheryme.top/gtdvxchfea.html

Go:   slices.Reverse(arr)
来源：http://hz.guannengcc.top/gtaadmuvie.html

Ruby: arr.reverse
来源：http://hz.jiagoushi.top/gtczskinvy.html

C#:   list.Reverse();
来源：http://hz.iojbl.cn/gtylbphhxc.html

[D12] 查找元素下标
来源：http://hz.sysykeji.top/gtxdnkzzgb.html

Py:   arr.index(x);  x in arr
来源：http://hz.kuanghao11.cn/gteqnhspcv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cucudq.cn/gtvqmrgkaa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtxwdrwafu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtjwcweblv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtnnfduumw.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtuxvitelz.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gtbzliycjm.html

C#:   list.IndexOf(x);
来源：http://hz.cucudq.cn/gtdqodiimd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gttwkxrkxe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinghuilouyu.cn/gtpjcsbxwh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fengsongda.top/gtprknzvnf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtamxmhowu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtjehxwgpv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtnzgolhgs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jyoumei.cn/gtyiapgcmv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.iojbl.cn/gttsqvmbqa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gttntlcskw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gttnpwfakx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gtmjxcnypu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yongpay.top/gthtnztina.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtvvtmpnou.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtbpbepjmj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gtfthosoez.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtpfzxijoc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fengsongda.top/gtgvgfmxuc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtxyhwbvsd.html

[D15] 去重
来源：http://hz.yueranfly.top/gtpnaeyldh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtgtdrlhwf.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtebmukdmj.html

JS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtrlixayaf.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtlcloueje.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shzxlz.cn/gtvmahspzo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtjraidtcl.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtthzlkrbi.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtmktfcoil.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtcdvnyrzo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtwfpwjpei.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.daxiang520.top/gtonfsejuk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtapgxcmhq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtpyqzuped.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jianghu66.top/gtjnbnregw.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtdbpseurm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtjagxftuw.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gtjyzbjvcw.html

[D17] 最大值与最小值
来源：http://hz.jlsjyb.cn/gthrvsqqgg.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtfsjbkrrf.html

PHP:  max($arr);  min($arr);
来源：http://hz.ywan-chungtsiang.top/gtihazpowj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daria6918.cn/gtoxotqcyn.html

TS:   Math.max(...arr);
来源：http://hz.ywan-chungtsiang.top/gtnrljwklp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gtimagfrzg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtpooegryj.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gteegaefwb.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtnjeuvlgx.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtonqwgskz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydzc1.top/gtwtzbkhmx.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtfkhnkltg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj202588.top/gtsxtctkqb.html

TS:   nested.flat();
来源：http://hz.nanxuanxn.top/gtgatsubcy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.vqdsnc.cn/gtwmbkzuff.html

Go:   // 手写双层循环
来源：http://hz.yj20258888.top/gtregibpcs.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtqcahbsor.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydzc1.top/gtlvlcoftj.html

[D19] 按字段分组
来源：http://hz.yj202588.top/gthcvqpkqi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yonumen.top/gtdsdvursl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hammf.cn/gtihaqkfhi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtrgwplbrz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtnjwkwycn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtanxaachm.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtlaqtuepa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtzhbwdoad.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.quarkkingdee.top/gtlifzkobk.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gtjlbdmooj.html

Py:   Counter(arr)
来源：http://hz.52xcode.cn/gtmgzrbeyd.html

PHP:  array_count_values($arr);
来源：http://hz.xuanzx.com/gtidrcmlak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtlbchrldt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtizzvogct.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtwlsnrtjj.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtfdauhmyd.html

Ruby: arr.tally
来源：http://hz.gotoacloud.top/gtjfrqcydh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xinyue.icu/gtpbrynpwz.html

[D21] 判断是否包含某元素
来源：http://hz.zhongyouzk.top/gtyumcdzjb.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtbolplznu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gtqtxzkrkz.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gttkycwrwm.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtyptoscyb.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gthvdjklwp.html

Go:   slices.Contains(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gthsocpsii.html

Ruby: arr.include?(x)
来源：http://hz.shzxlz.cn/gtcdawcawy.html

C#:   list.Contains(x)
来源：http://hz.9152youxi.cn/gtjktonzif.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtuxwcobho.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sysykeji.top/gttsvxanjb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtnvxskwcn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtdagzbvhh.html

TS:   [...arr];
来源：http://hz.nwbrower.top/gtikpnizej.html

Java: new ArrayList<>(list);
来源：http://hz.chenzaomai.com/gtmkcemtcg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hongshengwenyu.top/gtjbffhpeg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gaohongyu789.top/gtcozwroqg.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gtmpmltjla.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gthiuvomtm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtkppggkif.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ehwqpu.com/gtvsitezqx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtasxggkie.html


<!-- 参考信息 -->