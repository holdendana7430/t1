代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtvtdebdca.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtfpiajxre.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinyuanbaomall.cn/gtkgeygdlf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sweek.top/gtviyhyfma.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtxfgeebce.html

TS:   arr.map(String)
来源：http://hz.mhx1999.top/gtuvtgaoyz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.snrcjt.cn/gtipfuswaf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yongpay.top/gtzmfoogid.html

Ruby: arr.map(&:upcase)
来源：http://hz.mhx1999.top/gtrxlazfhm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtvdomgfqu.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtrmfnvure.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinyuanbaomall.cn/gtcvwpqhhr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gtkiffpxiu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtbzjampjs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gttrcjrrie.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.snrcjt.cn/gtmviidwfa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shuidangran.top/gtqjtylgpv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gtzxxkmpth.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtoqfdyxns.html

[C09] 递归
来源：http://hz.hnqzz.top/gtlefslmsb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gzhubu.top/gtpdnsoyii.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shzxlz.cn/gtcsyaxgmc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtaonbtxpb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gttnfnvzfh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tianlin.xyz/gtnfyxfnar.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aibaodan.cn/gthcfiosll.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtdtfohyut.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sxryk.cn/gtbonzqgjg.html

[C10] 变量作用域
来源：http://hz.yangfankeji.com/gtrrxgjwpt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangkeji.top/gtwmzrmplk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daxiang520.top/gtfolaqsoz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtlmodpfsg.html

TS:   同 JS
来源：http://hz.daria6918.cn/gtjsqpukrq.html

Java: 方法内为块级作用域
来源：http://hz.chenjidiqi.icu/gtzuhigknh.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtrslqmtri.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtrapdkivu.html

C#:   块级作用域
来源：http://hz.zhixingplan.top/gtcrxxneoc.html

[C11] 模块导入与导出
来源：http://hz.pycfn.com/gtkorsagje.html

Py:   from module import func
来源：http://hz.hongshengwenyu.top/gtcigrqmvg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuanzx.com/gtpscslfxp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yonumen.top/gtnpsqtkbw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydzc1.top/gtxjhgktug.html

Java: import java.util.List;
来源：http://hz.xylfe.cn/gtmsvdnonn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hfpthk.cn/gtkgivzscp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cucudq.cn/gtbiezzrfp.html

C#:   using System.Text;
来源：http://hz.tianlin.xyz/gtzjixvfbt.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtysyutzko.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gtwkkvsquz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gtsoxaroep.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtnmjkmuna.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtczjyvipp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtqcofshfk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258.top/gtcwcfjupz.html

Ruby: -> { puts "run" }.call
来源：http://hz.mhx1999.top/gtfyjsrapp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhoulong.xyz/gtvlkllvss.html

[C13] 类型声明 / 类型注解
来源：http://hz.nwbrower.top/gtkqiksmtu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtxljvaula.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtmjwmklve.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtfpzxnqcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtuwtkorye.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtfuiqpwmy.html

Go:   func add(a, b int) int
来源：http://hz.ydzc1.top/gtawpuvhda.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.birdmap.top/gtnckuqvmb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtophnpdbs.html

[C14] 泛型函数
来源：http://hz.chenlongwang.top/gtnympbonn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gtnolxgtuj.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gtzgnunjch.html

JS:   // 无泛型
来源：http://hz.yj20258.top/gttbigooiy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hongshengwenyu.top/gtniyzkzze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtavtkvkvc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cucudq.cn/gtbtpuqrvk.html

Ruby: # 无泛型
来源：http://hz.xuetiantiany.cn/gtlccbybla.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtzmaeyutm.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gtnndrbpjv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtifkpjlwa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.c1oappe.top/gttvdurjkz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xylfe.cn/gtoeogtwcw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xylfe.cn/gtxosftdzt.html

Java: // 无解构
来源：http://hz.0kj1m.cn/gtedewphzp.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gtfkeanlfp.html

Ruby: a, b = pair
来源：http://hz.pengpengdd.cyou/gtwkshlfeo.html

C#:   var (a, b) = pair;
来源：http://hz.xziqi.cn/gtkwjywgog.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtjlnvnxvt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xingfuxueyuan.xyz/gtxdyjimte.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtcauxlfsl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenjidiqi.icu/gtgptugiii.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxinkj.top/gtcusqsirf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtpjkjtcec.html

Go:   // 无重载：用不同函数名
来源：http://hz.pengpengdd.cyou/gtgtodnxpt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtregjyrox.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gtnabnkwit.html

================================================================================
来源：http://hz.ivvv.top/gtbamqsipy.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gtldiijrvi.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmxirmlwx.html

[D01] 创建数组 / 列表
来源：http://hz.dashuyun.cn/gtxefrgthn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gtkgevnijm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.snrcjt.cn/gtkbkvxtpz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtsuooogkf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtznngsssm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dashuyun.cn/gtfpelgnas.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtdbevhfqz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenlongwang.top/gtaugykhnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.smart0.xyz/gttmxqokyq.html

[D02] 追加元素到末尾
来源：http://hz.chenjidiqi.icu/gthxmjbdwy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hysaishi.cn/gtcjmofuqq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtqnyrwrzv.html

JS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtxdauzxav.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtpbavdkij.html

Java: list.add(4);
来源：http://hz.gzhubu.top/gtioxxxwvg.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangtech.top/gtajywoopw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtckazglyj.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gthvoxgjrz.html

[D03] 在指定位置插入元素
来源：http://hz.yuxming.cn/gtmrhsecwj.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtpkrgpyzv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.wangshuangyany.cn/gtdqwjtwmg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zycfv.cn/gtyinwtidx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.guannengcc.top/gtwvdicpsb.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gthialdhpe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.feifeiyinyue.top/gtsezsrszy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ehwqpu.com/gtsyrpwobn.html

C#:   list.Insert(0, 0);
来源：http://hz.yuxming.cn/gtfymumato.html

[D04] 删除元素
来源：http://hz.zhixingplan.top/gtnhdniqab.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnqzz.top/gtscqdbbsu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtlaafkwgx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigfzy.top/gtduiewzqp.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gttrjhhcou.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtdaclciyc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtksfcrflw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.kuanghao11.cn/gtuiisvhju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xylfe.cn/gttuiobimf.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtxdaudlpb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtofmpxjnb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.c1oappe.top/gtrleplhrw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtcgfyjkpr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258.top/gtegwlstbl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gotoacloud.top/gtpozlxxan.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sxryk.cn/gtlzgbrlqt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtbrkxtlse.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtlnustrig.html

[D06] 数组长度
来源：http://hz.gogol.net.cn/gtcaxzsmjb.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtynrstujp.html

PHP:  count($arr);
来源：http://hz.haohaochexian.top/gttzuzhgsa.html

JS:   arr.length
来源：http://hz.meibo888.top/gtdeatcyuu.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtujdureij.html

Java: list.size();
来源：http://hz.shuidangran.top/gtiiqcvtls.html

Go:   len(arr)
来源：http://hz.cqqwz.cn/gtkrswhhqy.html

Ruby: arr.length; arr.size
来源：http://hz.0kj1m.cn/gthxrspcna.html

C#:   list.Count;
来源：http://hz.c1oappe.top/gtdhmmygdk.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtudkbdlij.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtvluuicbn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.birdmap.top/gtujxewkyx.html

JS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gthvnflslb.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtvkrbcsgo.html

Java: list.subList(1, 4);
来源：http://hz.yj20258888.top/gtytevidji.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtcmuenihf.html

Ruby: arr[1, 3]
来源：http://hz.jiagoushi.top/gtpooebkje.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gtsmwtrghi.html

[D08] 合并两个数组
来源：http://hz.fzhhl.top/gtacctyrih.html

Py:   a + b;  a.extend(b)
来源：http://hz.dashuyun.cn/gtceznqdvx.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtgzgnxbay.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fengsongda.top/gtgajqgsrt.html

TS:   [...a, ...b];
来源：http://hz.ydzc1.top/gtodjhdvtc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtvtyanexs.html

Go:   append(a, b...)
来源：http://hz.zhijiandao.cn/gtxbbfziax.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtxydxogcv.html

C#:   a.Concat(b).ToList()
来源：http://hz.shuidangran.top/gtpqsijaox.html

[D09] 排序（升序）
来源：http://hz.haohaochexian.top/gtqmizeapp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtnriftfwv.html

PHP:  sort($arr);
来源：http://hz.wangshuangyany.cn/gtwsjdjojp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hywenlv.cn/gtykfzplrv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtrdgaxquw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258.top/gtdsoyscse.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtgkfphzka.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtssqxfnuk.html

C#:   list.Sort();
来源：http://hz.aizwys.cn/gtupdihofm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtbblplsun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtyvmsjtec.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtbmxyunqi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtgriobmvv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtssfwqyqb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gaohongyu789.top/gtepetogst.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gtvlbiwtzx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuanzx.com/gthxkrosah.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtavgpzths.html

[D11] 反转数组
来源：http://hz.gzhubu.top/gtwpjptnmr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtxrvnndvq.html

PHP:  array_reverse($arr);
来源：http://hz.xylfe.cn/gtgmybnsym.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.svipenyu.cn/gtnihklxun.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtkkwtmjxs.html

Java: Collections.reverse(list);
来源：http://hz.hywenlv.cn/gtuplkoktb.html

Go:   slices.Reverse(arr)
来源：http://hz.sweek.top/gtendgdung.html

Ruby: arr.reverse
来源：http://hz.hfpthk.cn/gtdutesqct.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtkvmdwnyk.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtriksofzm.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtqfcgtagl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aibaodan.cn/gtoszvyanl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtouczjeph.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gttmsdowpy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtrhucagak.html

Go:   slices.Index(arr, x)
来源：http://hz.guowangkeji.top/gtysalguof.html

Ruby: arr.index(x)
来源：http://hz.snrcjt.cn/gtlyhwxjlm.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtyzpmoikf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuetiantiany.cn/gtbiqwismh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtethcsdge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxuanxn.top/gtqxfxjfby.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtzdaimfkn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtaneoczbp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yueranfly.top/gtfcpnfvmr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.316326.xyz/gtqdcneact.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tianlin.xyz/gtzbskjmpz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtytihfpli.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtsogetktb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yueranfly.top/gtviuweerk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtejwrjrhu.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtjgrdazeq.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtezeqmmxy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtjozldjuk.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtkxixfwpt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gtrrdgqfnd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aibaodan.cn/gtaaxdevyy.html

[D15] 去重
来源：http://hz.hysaishi.cn/gtkyptlowi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtfycasimw.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtejpkrxjd.html

JS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtqsbncist.html

TS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtlpfrlyia.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtzcoieyfg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gteumskpyi.html

Ruby: arr.uniq
来源：http://hz.cashguo.top/gtndrboymx.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtyxoqmiue.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtjeetahnl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtblhjdvjb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gogol.net.cn/gtwbztxkrg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtnrindzwm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtzzzqyqyw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtpnosjizk.html

Go:   // 手写循环累加
来源：http://hz.ppjwa.cn/gtljqptiud.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtitgagwbu.html

C#:   list.Sum();  list.Average()
来源：http://hz.haohaochexian.top/gtxlkvtgja.html

[D17] 最大值与最小值
来源：http://hz.yj20258.top/gtypflsxmc.html

Py:   max(arr);  min(arr)
来源：http://hz.9152youxi.cn/gtxkhgcthq.html

PHP:  max($arr);  min($arr);
来源：http://hz.feifeiyinyue.top/gtytdaxmwu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuanzx.com/gtppvyrzfj.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtbikbfqci.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gttshvvkmn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shanyushiyangkeji.top/gtxfwaczjz.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtsajyhrvi.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gthafuocfa.html

[D18] 扁平化嵌套数组
来源：http://hz.kuanghao11.cn/gtugmxgdcm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ppjwa.cn/gtwygibrym.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtnrlbloxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuetiantiany.cn/gtodcyuomf.html

TS:   nested.flat();
来源：http://hz.gaohongyu789.top/gtbdqwwumh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ybcxt.top/gtnlfcehod.html

Go:   // 手写双层循环
来源：http://hz.jyoumei.cn/gtezhxerki.html

Ruby: nested.flatten
来源：http://hz.andypj.xyz/gttcydwnuk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gtusgvadrm.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtmlhqbesp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtfjurnthw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gthwwambqq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xziqi.cn/gttvncsrbq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtbxdxkivy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtqnuetcye.html

Go:   // 手写 map[string][]T
来源：http://hz.iojbl.cn/gtekzykvmj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tianlin.xyz/gtlcydfpqv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtnjajgzcr.html

[D20] 统计每个元素出现次数
来源：http://hz.gzhubu.top/gtsmeizzkn.html

Py:   Counter(arr)
来源：http://hz.xziqi.cn/gtkuoeodyg.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtuzmeqphz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtynfqcmqw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtgvmupjki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.birdmap.top/gtkqaaqywq.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtesdhcwzm.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtnegclpww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtjqejowhr.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gtxuvoczug.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtlsloabre.html

PHP:  in_array($x, $arr, true);
来源：http://hz.0kj1m.cn/gtbelhworm.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtmvaelpcg.html

TS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gttiymlljx.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtkokyproe.html

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gtmwyupzre.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtunryyscp.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtlzqkzbpi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.vqdsnc.cn/gttujaawia.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.0kj1m.cn/gtnofplmcp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xinyue.icu/gthkpojitu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gteownyinj.html

TS:   [...arr];
来源：http://hz.redwolf501.top/gtgukwvbak.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtuamlyodi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtxhpijnfi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daxiang520.top/gtosgzrjmx.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtnddpjbax.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gtdraxcvkr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xylfe.cn/gtwqkmpxzk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtoctzxsce.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtgtethvzc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtdxhgwceu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.fengsongda.top/gtsozqcptk.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gthxthysmg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jlsjyb.cn/gtazfafusd.html


<!-- 参考信息 -->