代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtndckltfh.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gtmsppcncq.html

Ruby: return a, b
来源：http://hz.birdmap.top/gtpcncuwhl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hywenlv.cn/gtdzfcclwl.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gtnxilnieb.html

Py:   square = lambda x: x * x
来源：http://hz.zhoulong.xyz/gtkrikhwwh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shuidangran.top/gtwqrfjiiq.html

JS:   const square = x => x * x;
来源：http://hz.yanxiufei.cn/gtcdhjcypa.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ywan-chungtsiang.top/gtxxrjqahh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtpjwywdqo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gtukoqabcv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gtuysrfsgr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.0kj1m.cn/gthrkkbzjv.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtezyeawec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gaohongyu789.top/gtgtjrokrv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gotoacloud.top/gtoojptlvc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydjk.org.cn/gtysuvtbfe.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtxctudgxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yangfankeji.com/gtiixbkgtp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuetiantiany.cn/gtpvnklgds.html

Ruby: arr.map(&:upcase)
来源：http://hz.quarkkingdee.top/gtzrrlyneb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigfzy.top/gtfgpnjqua.html

[C08] 闭包
来源：http://hz.cucudq.cn/gtlomodzuw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xylfe.cn/gtolnokdps.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jyoumei.cn/gthpppcujx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtenayqxqm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtnchrwebu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtdecwsnaz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhoulong.xyz/gtevhwjpqy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.mhx1999.top/gtppmkrhdz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtccfdpdqa.html

[C09] 递归
来源：http://hz.0kj1m.cn/gtxdfjjfck.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hfpthk.cn/gttrtcffqs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aizwys.cn/gtbmucukud.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gtvictwqpr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gttgxjrugr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtdcrvdyas.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtjvftxmrm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtxecgxybs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.bjfxy.top/gtdcmhlanh.html

[C10] 变量作用域
来源：http://hz.cucudq.cn/gtikkwznai.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.snrcjt.cn/gtggpviept.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtwobbstxj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dashuyun.cn/gtkunfhbwd.html

TS:   同 JS
来源：http://hz.nwbrower.top/gtynooozwa.html

Java: 方法内为块级作用域
来源：http://hz.c1oappe.top/gtyzxmxymv.html

Go:   花括号块级作用域
来源：http://hz.nanxinkj.top/gtzspibksx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxuanxn.top/gtqkzxydeu.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtmijbbtke.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtfurczdvv.html

Py:   from module import func
来源：http://hz.zycfv.cn/gtjwhcbreq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gaohongyu789.top/gtwhzjqxcf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.mhx1999.top/gtlyjtupyg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sweek.top/gtxiawbslz.html

Java: import java.util.List;
来源：http://hz.smart0.xyz/gtwohlfacj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gtjssocppi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gotoacloud.top/gtzxjyzvyp.html

C#:   using System.Text;
来源：http://hz.52xcode.cn/gtymzpdiuj.html

[C12] 立即执行函数 IIFE
来源：http://hz.xinyue.icu/gtoivptjow.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gtbkonzzyd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangkeji.top/gtwlhxdmcr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gzhubu.top/gtusxlygqu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtjllsbvwe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ybcxt.top/gttisqzxdn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hysaishi.cn/gtghzsvsij.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gtcbshueir.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hysaishi.cn/gtqtugvvta.html

[C13] 类型声明 / 类型注解
来源：http://hz.sufxvd.cn/gtbyxgnimo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gttdlkdspq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtroxunzvv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtuqcjxciw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gthibyrbue.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtgoimcmai.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtfiriodbz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtfxdgvpqs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtscylmojd.html

[C14] 泛型函数
来源：http://hz.mhx1999.top/gtauszubpl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtanmghras.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtjzkkjltv.html

JS:   // 无泛型
来源：http://hz.jyoumei.cn/gtagvomzhr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gtatprxvij.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gtbypruytp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gttfwegbll.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gtcrzeympg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gtgzupeddy.html

[C15] 解构 / 展开参数
来源：http://hz.nanxuanxn.top/gtbuobtxtf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xinyue.icu/gtfuuoqtfw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sufxvd.cn/gtglzppyhp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtsqvpwqnd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fengsongda.top/gtcrvvkjrj.html

Java: // 无解构
来源：http://hz.yj202588.top/gttbjljwhz.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtvjviftzp.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtkerqtbzw.html

C#:   var (a, b) = pair;
来源：http://hz.yvedp.cn/gtgvpsipmk.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtctmwpitd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gtsbmtnepo.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gtkxznsjri.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtlpzujjlp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtjcksayrg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtutkbtysh.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtjvxgozro.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtsaptbmlw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yvedp.cn/gtzmictoqy.html

================================================================================
来源：http://hz.sxryk.cn/gtqkxisvxz.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtrsaljakx.html

================================================================================
来源：http://hz.iojbl.cn/gtctclnxgq.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtzajsqmwv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtvixzknhx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtrxonfcng.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ivvv.top/gtchwtyyob.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtncuzuiof.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtenaaulnd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtzflhqraf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxinkj.top/gtfjtaruhc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gtztywutom.html

[D02] 追加元素到末尾
来源：http://hz.fzhhl.top/gttoqwreke.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtrzlmnruz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gtvnzfzvpk.html

JS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gttndnijul.html

TS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtrdjiggww.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtahcftqmh.html

Go:   arr = append(arr, 4)
来源：http://hz.vqdsnc.cn/gtozwpqoth.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hysaishi.cn/gtjtpogutc.html

C#:   list.Add(4);
来源：http://hz.cucudq.cn/gtwgtgnekh.html

[D03] 在指定位置插入元素
来源：http://hz.guowangkeji.top/gtqljfjyod.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtvubnmsea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtfapophvo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aizwys.cn/gtlpmhsimt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigufen.top/gthgviqgsi.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gtyqoocqhd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hfpthk.cn/gtvnbfpcgs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenzaomai.com/gtvmdlfswp.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigfzy.top/gtmuljkfei.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gthwyrjsvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuetiantiany.cn/gtzqczilki.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtuxcumqwi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtgxwvizuw.html

TS:   arr.splice(0, 1);
来源：http://hz.ywan-chungtsiang.top/gteeivpync.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shanyushiyangtech.top/gtjwqonmgx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.vqdsnc.cn/gtjpnpvpij.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gzhubu.top/gtguhhnxtt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gttqasseup.html

[D05] 访问与修改元素
来源：http://hz.jiagoushi.top/gtcjpjmajs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtuozfsrws.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtflgwkyvm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtzlcrfevz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtkllwkloi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shangyingyoupin.top/gtbbcwahvs.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtssiwdrpy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtnrzimfno.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tianlin.xyz/gtjgpejoad.html

[D06] 数组长度
来源：http://hz.fzhhl.top/gtwlpiawxq.html

Py:   len(arr)
来源：http://hz.xylfe.cn/gtycponuir.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gticksmcsr.html

JS:   arr.length
来源：http://hz.birdmap.top/gtlvgzhxan.html

TS:   arr.length
来源：http://hz.hnxiangtu.top/gtvxqxskbd.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtbipnpeka.html

Go:   len(arr)
来源：http://hz.fzhhl.top/gtyjqrxnwo.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtlgajbaqa.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtjlwhnwrl.html

[D07] 切片 / 取子数组
来源：http://hz.hammf.cn/gtsudygmxm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtkqatlrho.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.birdmap.top/gtwyralygi.html

JS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtpnexrngn.html

TS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtonxtwsnx.html

Java: list.subList(1, 4);
来源：http://hz.daria6918.cn/gtlaeryhuu.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtmjthrjkk.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtjtjfcgqo.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtdsffcxdw.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtejvocznu.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnqzz.top/gtclfpsloa.html

PHP:  array_merge($a, $b);
来源：http://hz.quarkkingdee.top/gtuzkocgdw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtpwywwqth.html

TS:   [...a, ...b];
来源：http://hz.nanxinkj.top/gtdllegyjf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtsneegxvc.html

Go:   append(a, b...)
来源：http://hz.sweek.top/gteksfvscf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtbknsiixo.html

C#:   a.Concat(b).ToList()
来源：http://hz.aizwys.cn/gtajmlhvpa.html

[D09] 排序（升序）
来源：http://hz.yueranfly.top/gtdieimrbg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtufdssdye.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtdtlqlaog.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xylfe.cn/gtjgcvobwm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtjmscxsey.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtomuvolup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtnfbjblzv.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtwjhifcyn.html

C#:   list.Sort();
来源：http://hz.kuanghao11.cn/gtogfpynhb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydjk.org.cn/gthauvolxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.vqdsnc.cn/gttjaqgmti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtsbdaixwq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtahhhunnk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gtftcprucq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtahvemtvu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtslulbtfg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnxiangtu.top/gtebfwcnjm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtyhmvuwym.html

[D11] 反转数组
来源：http://hz.fengsongda.top/gtuipoudib.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigufen.top/gthzpsopme.html

PHP:  array_reverse($arr);
来源：http://hz.9152youxi.cn/gtgnhgkksh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cdnleiting.top/gtruzhvikf.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtfrduwnrr.html

Java: Collections.reverse(list);
来源：http://hz.daria6918.cn/gtmelvbxwp.html

Go:   slices.Reverse(arr)
来源：http://hz.aizwys.cn/gtsvkeummo.html

Ruby: arr.reverse
来源：http://hz.316326.xyz/gtsjmpeagy.html

C#:   list.Reverse();
来源：http://hz.yueranfly.top/gtjlbnxnml.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtyfplcqkw.html

Py:   arr.index(x);  x in arr
来源：http://hz.sufxvd.cn/gtdyvmnjus.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtiguepqlj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtzsfbnwyz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtitiivamx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.kuanghao11.cn/gtcrshvygg.html

Go:   slices.Index(arr, x)
来源：http://hz.meibo888.top/gtirnnbmtv.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtasssmbra.html

C#:   list.IndexOf(x);
来源：http://hz.feifeiyinyue.top/gtbsuwggcd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtuknmovxj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtqtynbgbg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtklpcyzld.html

JS:   arr.filter(x => x > 3)
来源：http://hz.wangshuangyany.cn/gttcnfkcco.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtmtnvscxo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gtqzswfxqt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daria6918.cn/gtqyllhcef.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pengpengdd.cyou/gteoasumqg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.vqdsnc.cn/gtmhtkrbnv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtxlceadbu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yueranfly.top/gtpnedilly.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guannengcc.top/gthhlvzmrk.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gttwgmvvgp.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtoorqblyl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cqqwz.cn/gtvbjcayjn.html

Go:   // 手写循环
来源：http://hz.shuidangran.top/gtqlmyzubf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.svipenyu.cn/gttiemngnx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gtcupyoqft.html

[D15] 去重
来源：http://hz.xziqi.cn/gtidjnrjtv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtfzfozuog.html

PHP:  array_unique($arr);
来源：http://hz.nwbrower.top/gtvgqokxhj.html

JS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gthbhiamcy.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtkszqhvql.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gteeerpkue.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtkzwmbgly.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtygbppfod.html

C#:   list.Distinct().ToList()
来源：http://hz.aizwys.cn/gtvgqvrldy.html

[D16] 求和与平均值
来源：http://hz.yueranfly.top/gtueeclngt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yonumen.top/gtimwhyetj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtsqxxdlfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gthgojipux.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtichtyakv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.9152youxi.cn/gtfybpwwid.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangtech.top/gtcdddddkm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fzhhl.top/gtkidvhaer.html

C#:   list.Sum();  list.Average()
来源：http://hz.dashuyun.cn/gtalbvmaqh.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gtdgwkvjfx.html

Py:   max(arr);  min(arr)
来源：http://hz.tianlin.xyz/gtllcinati.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhijiandao.cn/gtzgixipxe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj202588.top/gtevpfrdpo.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtvdmrzyeh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtvmncknxc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shzxlz.cn/gthivrpkza.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtpspkkxgg.html

C#:   list.Max();  list.Min()
来源：http://hz.yanxiufei.cn/gtwyqrxfxr.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtgdgztqpn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtdmnonxnp.html

PHP:  array_merge(...$nested);
来源：http://hz.zycfv.cn/gtpbjrwmca.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtfuywfeyc.html

TS:   nested.flat();
来源：http://hz.bjfxy.top/gtuxyrjdtr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gtivhtttde.html

Go:   // 手写双层循环
来源：http://hz.jinghuilouyu.cn/gttbbnamld.html

Ruby: nested.flatten
来源：http://hz.jqgufenzy.top/gtjyfwgdvh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.mhx1999.top/gtjrvcqhfr.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtluhetsqu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhongyouzk.top/gtphrqoztr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtzttzpzee.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhoulong.xyz/gtxkldhsfm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtrlejfwij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtkqfkpgcn.html

Go:   // 手写 map[string][]T
来源：http://hz.chenlongwang.top/gtesqdoyyb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtwpopekcu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtxvepvkcb.html

[D20] 统计每个元素出现次数
来源：http://hz.ehwqpu.com/gtehzmwqul.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtdkrljbvt.html

PHP:  array_count_values($arr);
来源：http://hz.sysykeji.top/gtplmtgtdi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtkoroggqx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtuyyxgwwn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cheryme.top/gtzobtbxzd.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtbpyztvzu.html

Ruby: arr.tally
来源：http://hz.jiagoushi.top/gtiaufchpi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tanke756.top/gtdkiyizcz.html

[D21] 判断是否包含某元素
来源：http://hz.wangshuangyany.cn/gtfyvxdyqc.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtzclstxbx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guannengcc.top/gtqveqsmds.html

JS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtadyulfyf.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtxxlwdldx.html

Java: list.contains(x)
来源：http://hz.hammf.cn/gtzjhqgbim.html

Go:   slices.Contains(arr, x)
来源：http://hz.hywenlv.cn/gtkxedwgkw.html

Ruby: arr.include?(x)
来源：http://hz.jiagoushi.top/gtoaoeihrm.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtglxmvjzp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtqlorqqao.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtcvnfhumh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtwucibfaf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ehwqpu.com/gtznoytsbp.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtforslqnz.html


<!-- 参考信息 -->