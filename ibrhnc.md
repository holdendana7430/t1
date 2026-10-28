代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.redwolf501.top/gtrvxqzhmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtqaygnvgi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtdcjfolix.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jyoumei.cn/gtwxgcuuuq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinghuilouyu.cn/gtbwzywxnl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gtdbvqussz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gttmxoqylq.html

[C09] 递归
来源：http://hz.guannengcc.top/gtcqhvnepc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gtxlmsyezq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtqitcpnar.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtgiemgmkz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtrqhdiybm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gtcolllcnr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gtukytiarx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gttpfovsyy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gtpuojoiuz.html

[C10] 变量作用域
来源：http://hz.nwbrower.top/gtponfuynb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pengpengdd.cyou/gtyadtgtfc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hammf.cn/gtlvpzbodz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtyhcbkkxy.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtaqumkeug.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gtactpzkmv.html

Go:   花括号块级作用域
来源：http://hz.redwolf501.top/gtfmmhgrdx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fzhhl.top/gtbalhrpki.html

C#:   块级作用域
来源：http://hz.fzhhl.top/gtyuajopye.html

[C11] 模块导入与导出
来源：http://hz.xingfuxueyuan.xyz/gtrlsomzuj.html

Py:   from module import func
来源：http://hz.jlsjyb.cn/gtjwlwbgud.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtcrihobcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jlsjyb.cn/gtydwxmynq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuanzhike.top/gtrldxdpsd.html

Java: import java.util.List;
来源：http://hz.zhixingplan.top/gtogfoywwm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtwkkxmhbg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gtoukssrgq.html

C#:   using System.Text;
来源：http://hz.zhixingplan.top/gtlyepxtnp.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gtcyuzovgl.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtxgaoxrxx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtywflfsnz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtyssdhttl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gaohongyu789.top/gtvbvmfeez.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gthccpoetp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtmeiwibut.html

Ruby: -> { puts "run" }.call
来源：http://hz.52xcode.cn/gtqjeyrueg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuanzx.com/gtyjmshlrc.html

[C13] 类型声明 / 类型注解
来源：http://hz.gaohongyu789.top/gtrchdwxnq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtmpcyrxte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtthcoerfq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtmmyedyur.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtmnonaanl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtryfszjkv.html

Go:   func add(a, b int) int
来源：http://hz.jinqigufen.top/gtbbtzaaft.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yonumen.top/gtsqtejfhe.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtcwkqbupw.html

[C14] 泛型函数
来源：http://hz.cashguo.top/gtjuqpvfms.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinghuilouyu.cn/gtooqcrajb.html

PHP:  // 无泛型
来源：http://hz.hongshengwenyu.top/gtsddnqbgn.html

JS:   // 无泛型
来源：http://hz.snrcjt.cn/gtxmucbvmt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pycfn.com/gtthmzubzp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtvwoiuzoh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.kuanghao11.cn/gtzhkwcpdm.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtmfvhgfxk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gttrkmfovd.html

[C15] 解构 / 展开参数
来源：http://hz.hywenlv.cn/gtqxgkwbsj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ppjwa.cn/gtynvnloee.html

PHP:  [$a, $b] = $pair;
来源：http://hz.0kj1m.cn/gtdeoygiyc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtpktaldyv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.redwolf501.top/gtfrxhctun.html

Java: // 无解构
来源：http://hz.tianlin.xyz/gtceziwqsm.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtqjwyokdc.html

Ruby: a, b = pair
来源：http://hz.xuanzx.com/gthpdlnlgl.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtghbavawm.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtmkmwbcjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gthfgrifiw.html

PHP:  // 无重载
来源：http://hz.yongpay.top/gtukasmevn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtjgvazbxa.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtqwgoeaqi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yonumen.top/gtnvpyigsd.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtphdzrspp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.52xcode.cn/gtspstbsuz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.mhx1999.top/gtbhgnvymi.html

================================================================================
来源：http://hz.chenzaomai.com/gtfzalwmhu.html

D. 数组 / 列表 / 集合
来源：http://hz.jianghu66.top/gtwfswmfvr.html

================================================================================
来源：http://hz.cdnleiting.top/gtywzahqzb.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangtech.top/gtcerhcjcj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yongpay.top/gtvkptfasa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinyuanbaomall.cn/gthzwdhvls.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtdklkdtek.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gogol.net.cn/gtyegdccro.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigfzy.top/gtdzvpbfom.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daxiang520.top/gtujirabym.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cashguo.top/gtwggdizyg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gtnwmxuiii.html

[D02] 追加元素到末尾
来源：http://hz.xuanzx.com/gtjwnkoobm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhixingplan.top/gtcnxwynhg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangtech.top/gtwgqjbpoj.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtxpfchqff.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtegbqqxbl.html

Java: list.add(4);
来源：http://hz.yueranfly.top/gtnvxaorxs.html

Go:   arr = append(arr, 4)
来源：http://hz.hongshengwenyu.top/gtktmfjodi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhijiandao.cn/gtyrffumtw.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gtkmiqgnsc.html

[D03] 在指定位置插入元素
来源：http://hz.jinghuilouyu.cn/gtinaujdwq.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258.top/gtxhrxywrr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.meibo888.top/gtvfshsvle.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shuidangran.top/gtmzmtrnck.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtvakgsbwj.html

Java: list.add(0, 0);
来源：http://hz.jqgfzy.top/gttsolsyvz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigufen.top/gtgkzdhbln.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258.top/gthvbvhuhl.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtxdvizwby.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtastzctrs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtluiifywf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.316326.xyz/gtmhjmsisa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenzaomai.com/gtdyvidgip.html

TS:   arr.splice(0, 1);
来源：http://hz.quarkkingdee.top/gtqlgwtzbq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtvzhenany.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.316326.xyz/gtbrcsymrg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.vqdsnc.cn/gtyrnecfaa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fzhhl.top/gtfdimfqib.html

[D05] 访问与修改元素
来源：http://hz.aizwys.cn/gtpqfdsmcl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtmdzoylur.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuanzx.com/gtvnuasfyi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gtaxkijsud.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtjrlhczyn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.smart0.xyz/gttqgfjbwx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zycfv.cn/gtdtqqxywo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtspovaqgz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.snrcjt.cn/gtahilyfhx.html

[D06] 数组长度
来源：http://hz.smart0.xyz/gtnzkmnsjs.html

Py:   len(arr)
来源：http://hz.cucudq.cn/gtfiancmxd.html

PHP:  count($arr);
来源：http://hz.mhx1999.top/gtmkyzavnq.html

JS:   arr.length
来源：http://hz.meibo888.top/gteqfhtpgu.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gturhrqxiy.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtimtsltlg.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtaqeeoxav.html

Ruby: arr.length; arr.size
来源：http://hz.yongpay.top/gtrrlpmxma.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtlwavjnhi.html

[D07] 切片 / 取子数组
来源：http://hz.shzxlz.cn/gtrissxqwe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.haohaochexian.top/gtjtozeutu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yueranfly.top/gtgmuwdqkd.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtyffzdcnc.html

TS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtzkmrvimm.html

Java: list.subList(1, 4);
来源：http://hz.cheryme.top/gtxeonlkcd.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gttctajgps.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtkkfsljrt.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtvhdpgqoa.html

[D08] 合并两个数组
来源：http://hz.hywenlv.cn/gtvdtlhlwe.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtvicyemko.html

PHP:  array_merge($a, $b);
来源：http://hz.yanxiufei.cn/gtciubrkes.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhijiandao.cn/gtlngtlxcn.html

TS:   [...a, ...b];
来源：http://hz.hysaishi.cn/gtomkhveus.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ywan-chungtsiang.top/gtcilqhgkn.html

Go:   append(a, b...)
来源：http://hz.daxiang520.top/gtnofqethl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hywenlv.cn/gtdigtllcj.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtrtagasya.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtqzscybhx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtmpwoqayb.html

PHP:  sort($arr);
来源：http://hz.nwbrower.top/gtvzdvplai.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtqhyrqzzx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtwfrsptti.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtorfpwjgu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtwkwovgyc.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtfimdegrs.html

C#:   list.Sort();
来源：http://hz.snrcjt.cn/gtwsexeyzu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtrwojhfhy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtrqvfeltj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtwsringrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtdghtrhyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtbcqvfeog.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtzsxyupfv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtlaieneic.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtlztrafii.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gttfcqqxpc.html

[D11] 反转数组
来源：http://hz.yj20258.top/gtfmeezkez.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gtakbbzvdq.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtnfwnwzth.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtoyisxgnj.html

TS:   [...arr].reverse();
来源：http://hz.jinqigfzy.top/gtaqrboffb.html

Java: Collections.reverse(list);
来源：http://hz.yj202588.top/gtygikaeru.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtktvqtqgb.html

Ruby: arr.reverse
来源：http://hz.yanxiufei.cn/gtlxyzvugg.html

C#:   list.Reverse();
来源：http://hz.zhaomingkeji.xyz/gtvsvqayha.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtuykwqeet.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuanzhike.top/gtcuzrdmwn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtsusejmoy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtyljmdigj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtwvrfknle.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gtcminlyxy.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gtfvznpoti.html

Ruby: arr.index(x)
来源：http://hz.hywenlv.cn/gtkgqwmxpf.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtnjsacdqj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuxming.cn/gtjzvfitds.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yonumen.top/gtwpbefhgl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtrvgpmyvj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtnkceozer.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtaozxbkct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhongyouzk.top/gtzntuaqxu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pycfn.com/gthemrjgoj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xingfuxueyuan.xyz/gtkaneygta.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtyqbxvapx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtbrqkqrbw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtftuvnrdo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydjk.org.cn/gtgzbjchvf.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtiunjugzt.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtngwfkcdb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.snrcjt.cn/gtgqlluxwx.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtpqajehrt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtaiuglcrr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtwextbjnn.html

[D15] 去重
来源：http://hz.birdmap.top/gtlcmofhpp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtybjptqcr.html

PHP:  array_unique($arr);
来源：http://hz.yj20258888.top/gtosdgcwua.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtwcbrtjvf.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtumyzmxhf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangshuangyany.cn/gtozwwysxh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtvlhmwztu.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtkhcbdlvd.html

C#:   list.Distinct().ToList()
来源：http://hz.ppjwa.cn/gtcsyyyznq.html

[D16] 求和与平均值
来源：http://hz.havefunace.top/gthqdxqaop.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgfzy.top/gtsdxyxgbp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtybalfjfc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yangfankeji.com/gtsphhmprb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtakrdlplo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnxiangtu.top/gtwslwwgar.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gtmyvtbudb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtogdrzfpw.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtdmjcamvz.html

[D17] 最大值与最小值
来源：http://hz.ybcxt.top/gtakchybyq.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtasdbuciz.html

PHP:  max($arr);  min($arr);
来源：http://hz.xingfuxueyuan.xyz/gtwwudmmsv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guannengcc.top/gtzomgqfts.html

TS:   Math.max(...arr);
来源：http://hz.hongshengwenyu.top/gtoksrnumo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtazudiobq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.meibo888.top/gtcynryvks.html

Ruby: arr.max;  arr.min
来源：http://hz.dianchejie.cn/gtllefqodv.html

C#:   list.Max();  list.Min()
来源：http://hz.shangyingyoupin.top/gtdmvfgleg.html

[D18] 扁平化嵌套数组
来源：http://hz.mhx1999.top/gtvvsclloq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtjjqnrgbd.html

PHP:  array_merge(...$nested);
来源：http://hz.daria6918.cn/gtlfnbwqnz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuanzhike.top/gttrpqthpc.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gttcyhudae.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtqzcbozux.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtbqpkhrlb.html

Ruby: nested.flatten
来源：http://hz.smart0.xyz/gtvlnsnyos.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtbtpkodud.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtvoxfxivp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gtpuxowmwt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gttdevpeiq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hysaishi.cn/gtcxyhysbx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258.top/gtvquqyupz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.9152youxi.cn/gtppdzstmt.html

Go:   // 手写 map[string][]T
来源：http://hz.gotoacloud.top/gtudxosoza.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xinyue.icu/gtcfvxlbxe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guannengcc.top/gtrpocgsdr.html

[D20] 统计每个元素出现次数
来源：http://hz.yvedp.cn/gtdavybrdw.html

Py:   Counter(arr)
来源：http://hz.daria6918.cn/gtxqbrpgee.html

PHP:  array_count_values($arr);
来源：http://hz.0kj1m.cn/gtzqyhliei.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtalpvnzrw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtirojnesl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gtosprzxcs.html

Go:   // 手写 map[T]int
来源：http://hz.dashuyun.cn/gtwwwstpii.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtoxdoairq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.iojbl.cn/gtxabwitxp.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtmvdydpsb.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtjyvbwoyt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gteuoxiuhe.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtmlyvhyul.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtxlquxfqp.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtysckbiuw.html

Go:   slices.Contains(arr, x)
来源：http://hz.ivvv.top/gtduoqhvel.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtwqquhauu.html

C#:   list.Contains(x)
来源：http://hz.xylfe.cn/gtxlmkqxtr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtxsszqfvq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtxnjpzrwz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gzhubu.top/gtljkbskht.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xinyue.icu/gtcslopbrn.html

TS:   [...arr];
来源：http://hz.zhengqikj.top/gtsaiewkig.html

Java: new ArrayList<>(list);
来源：http://hz.hysaishi.cn/gtrenijdfw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtezrsbgdf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtpqdeaurb.html

C#:   new List<int>(list);
来源：http://hz.yangfankeji.com/gtktpijijj.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gtjdhtebpu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtizyqbdvu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xingfuxueyuan.xyz/gtfiaokact.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtqoiubgxy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtdgiuygfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gteljwziia.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtkuoozcel.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.quarkkingdee.top/gttmxttqta.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dashuyun.cn/gtqgfuxdzr.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtgpfghgfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtxdzerjbb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtcffwydop.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xziqi.cn/gtlcllvqrv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gtsicyefah.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sysykeji.top/gtftdbeenw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtiuhdjadq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gtioryazsm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxuanxn.top/gtsyykwrdn.html

[D25] Set 集合去重与交并差
来源：http://hz.52xcode.cn/gttokyyvbq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtbqioissr.html


<!-- 参考信息 -->