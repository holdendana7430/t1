代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtmogvkvgf.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtyqerpgcm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinyuanbaomall.cn/gthtchbkrv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gthfgfjzev.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtsxpyblhu.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gtdvhletlw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhaomingkeji.xyz/gttyjobcjt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daria6918.cn/gtupnvvnif.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydzc1.top/gtrlgxqlag.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jianghu66.top/gtclglqvfb.html

[C08] 闭包
来源：http://hz.guowangkeji.top/gtvqpdhdjc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xuanzx.com/gtiecuaaue.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shangyingyoupin.top/gtqhzgqkkw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtlewqkzvb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtshelllvg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hywenlv.cn/gtntndbupq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gtksqzxfih.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xuanzx.com/gtvhgvjgjw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtirbfandp.html

[C09] 递归
来源：http://hz.tanke756.top/gthmmdkear.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtbzopuwbv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daxiang520.top/gtniwfxgau.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtrcxbdusc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtjtldsflx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.9152youxi.cn/gtwwrufvml.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.havefunace.top/gtyamuavtp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cucudq.cn/gtmbbsnfky.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtpfjvqrgw.html

[C10] 变量作用域
来源：http://hz.jinghuilouyu.cn/gthtklrfvf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gaohongyu789.top/gthnmaktrn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuanzhike.top/gtnzfpfwrg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhijiandao.cn/gtwofnxfwc.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtmsuwmpck.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtksshkuon.html

Go:   花括号块级作用域
来源：http://hz.yonumen.top/gtmqkgugaz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sweek.top/gtrriuwoeq.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtfrsnwtly.html

[C11] 模块导入与导出
来源：http://hz.yj20258888.top/gtsmdziiav.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gtefkufhbv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tanke756.top/gtkccchydo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hongshengwenyu.top/gtwxrmzxoa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.wangdashe.top/gtnqbxmndn.html

Java: import java.util.List;
来源：http://hz.nanxuanxn.top/gtimratfvw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxinkj.top/gtzztgqjza.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuanzx.com/gtlytprptw.html

C#:   using System.Text;
来源：http://hz.bjfxy.top/gtnjvtgzsb.html

[C12] 立即执行函数 IIFE
来源：http://hz.snrcjt.cn/gtfiylhjwo.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtncfbfpsy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtsrjqybmo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtzztnpgqs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtcpgdltrd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydjk.org.cn/gtrhnygwrb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yanxiufei.cn/gtakeiyejy.html

Ruby: -> { puts "run" }.call
来源：http://hz.mhx1999.top/gtnisnxcjn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtpgvvjcik.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gttzfokoyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.vqdsnc.cn/gthmcrpuho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtcofuqijk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.iojbl.cn/gtlgzmrtsl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtjjlxsrnq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtamztejky.html

Go:   func add(a, b int) int
来源：http://hz.hnxiangtu.top/gtnwmhigvr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigufen.top/gtuazpzomg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtooonjcsu.html

[C14] 泛型函数
来源：http://hz.yuanzhike.top/gtafherjfq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtvtwwhtmx.html

PHP:  // 无泛型
来源：http://hz.jianghu66.top/gtnluzwclu.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtobrblbyk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtkqmsmtfi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtyivxiqiu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xziqi.cn/gtuapxayhx.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gtfcnlkkeq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtgirzmkvt.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtvoniqgnk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhengqikj.top/gtvmyepufi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtvbewdgem.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtfifgvplu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtfqpahyds.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtwzcaqnps.html

Go:   // 无解构
来源：http://hz.nanxuanxn.top/gtitthmpvb.html

Ruby: a, b = pair
来源：http://hz.xinyue.icu/gtlqbrwdtw.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gtfkrzjcnc.html

[C16] 函数 / 方法重载
来源：http://hz.vqdsnc.cn/gtvjigtosb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtmwdorfbh.html

PHP:  // 无重载
来源：http://hz.vqdsnc.cn/gtuycjvslb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tianlin.xyz/gtswujumhm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtgtbjqmec.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.mhx1999.top/gtqbvpphot.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtmeiolnng.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtiqjtcrqr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.smart0.xyz/gtjrnmtfwe.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtewwzmwdd.html

D. 数组 / 列表 / 集合
来源：http://hz.zhongyouzk.top/gtlxjovxzr.html

================================================================================
来源：http://hz.yuanzhike.top/gtorneport.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigfzy.top/gttyehdzzc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtnqqahpyz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.havefunace.top/gtbwrdconq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yvedp.cn/gtklqlqtcr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtilkttjyh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gtethrrrkb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtixmmpuot.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hfpthk.cn/gtvrbgtnbn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258888.top/gtymfogmwe.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gtiofjktco.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtqbydwgqw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnqzz.top/gtjrqiiayg.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtbiirtzmn.html

TS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtiwiairaa.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtjmtedrkg.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtoerfjrke.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtkdlxkwvv.html

C#:   list.Add(4);
来源：http://hz.cheryme.top/gtcmnybmol.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtkyjvoanl.html

Py:   arr.insert(0, 0)
来源：http://hz.hfpthk.cn/gtmvrrfixg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtffhwukms.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guowangkeji.top/gtlzpfkmfj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jianghu66.top/gtvrmsezct.html

Java: list.add(0, 0);
来源：http://hz.zdqjudy.top/gtclzdpsif.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuxming.cn/gtgxsohshi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtquhbhsez.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangtech.top/gtzfkmpebe.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtxdiowdql.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangtech.top/gtdzbhslow.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cheryme.top/gtsfnqhyqh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.bjfxy.top/gtnzsclvxf.html

TS:   arr.splice(0, 1);
来源：http://hz.sysykeji.top/gtvkwmxxee.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtpgleacqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtyyeukmwv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.svipenyu.cn/gtlfdmgqfp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cdnleiting.top/gtzkricbwo.html

[D05] 访问与修改元素
来源：http://hz.xziqi.cn/gtbpepuawn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gtzqpndtxv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.birdmap.top/gtyacefzth.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtcoqvlykc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pengpengdd.cyou/gtkpgjwcid.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cashguo.top/gtwidemxuo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtevvztulw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtztvjoyfs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cdnleiting.top/gthpjqyjgj.html

[D06] 数组长度
来源：http://hz.jyoumei.cn/gtcvtcovcr.html

Py:   len(arr)
来源：http://hz.pycfn.com/gtuggmvbph.html

PHP:  count($arr);
来源：http://hz.vqdsnc.cn/gtgxfqfdsw.html

JS:   arr.length
来源：http://hz.sxryk.cn/gtltjhjdrc.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gttyckpbll.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtlrikcivg.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtlieyfuma.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtrxxkhkif.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtfnkqvjra.html

[D07] 切片 / 取子数组
来源：http://hz.ydzc1.top/gtwpsexmif.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtbhgtrhec.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnxiangtu.top/gtxxqgwwht.html

JS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtubcnfbpc.html

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtigxbulgo.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtjhrucouv.html

Go:   arr[1:4]
来源：http://hz.sufxvd.cn/gtmkcpbngu.html

Ruby: arr[1, 3]
来源：http://hz.c1oappe.top/gtvffjftrc.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtjncudtjb.html

[D08] 合并两个数组
来源：http://hz.kuanghao11.cn/gtdhhcutyz.html

Py:   a + b;  a.extend(b)
来源：http://hz.redwolf501.top/gtgdqpesrj.html

PHP:  array_merge($a, $b);
来源：http://hz.wangshuangyany.cn/gtprrxmmmn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zdqjudy.top/gtzdrodjsh.html

TS:   [...a, ...b];
来源：http://hz.jqgufenzy.top/gtozrfvjkk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtqwtybsyt.html

Go:   append(a, b...)
来源：http://hz.hfpthk.cn/gtkxociaml.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtgsxavgbb.html

C#:   a.Concat(b).ToList()
来源：http://hz.ehwqpu.com/gtyuspgqos.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtnlrmxnco.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtniimwbuw.html

PHP:  sort($arr);
来源：http://hz.hammf.cn/gturgkzvgl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gogol.net.cn/gtsizqykso.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.bjfxy.top/gtixbxigwo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtaytthfvv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.meibo888.top/gtkzvnacph.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtcggetguu.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gthlanblpb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.haohaochexian.top/gtgnpivudl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtnpatuclr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtywjykiuj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtvaghqgsx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtvgfjskqz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.feifeiyinyue.top/gtjfnfuesp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtoppvvowi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtmhcysqur.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtujkvzrpv.html

[D11] 反转数组
来源：http://hz.zhijiandao.cn/gtuhjspyug.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtebkbyzfk.html

PHP:  array_reverse($arr);
来源：http://hz.yvedp.cn/gtjguxcmyl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.meibo888.top/gtiffgilwf.html

TS:   [...arr].reverse();
来源：http://hz.vqdsnc.cn/gtrjvwzryp.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtqsnrztoj.html

Go:   slices.Reverse(arr)
来源：http://hz.zhijiandao.cn/gtjbvybtsg.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtbnxaxeyo.html

C#:   list.Reverse();
来源：http://hz.hfpthk.cn/gtmjfqdnrd.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtzyouuecc.html

Py:   arr.index(x);  x in arr
来源：http://hz.sweek.top/gtonyagpko.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jiagoushi.top/gtgdlvtjcx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtxpfnfruq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtjzecnjud.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hfpthk.cn/gtozkocjis.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtdmemxtlw.html

Ruby: arr.index(x)
来源：http://hz.jiagoushi.top/gtsxkvhwwi.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gterrrbdbx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtbjduqjbu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtzyzdujea.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenlongwang.top/gtwktvpyps.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtunaliish.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gthtskskue.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hywenlv.cn/gtpnidbfhl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtjgpeczyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.meibo888.top/gtopikrnlb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ivvv.top/gtsijssgwr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sweek.top/gtfjrmvsmw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigufen.top/gtvzlijdly.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gtrenymgdm.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtiqtwnaul.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gthlgxriel.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtvpznqoeq.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtvywnjmnh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gaohongyu789.top/gtocwlzqmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtnuwcuiea.html

[D15] 去重
来源：http://hz.aizwys.cn/gtmcemdvaa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtizxsoili.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtlbhalpqq.html

JS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtummunmji.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtwdpvlrko.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sxryk.cn/gtelqoblvw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtqnaojsgq.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtbpwfmrvo.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtcqgkgfqu.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtbymewxom.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtvlhcwjdr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jiagoushi.top/gtiokfvwno.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtcuxxkhsv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtidygjvvu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.316326.xyz/gtgyexzghz.html

Go:   // 手写循环累加
来源：http://hz.hywenlv.cn/gtbyaeszwj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhengqikj.top/gtwblzlood.html

C#:   list.Sum();  list.Average()
来源：http://hz.birdmap.top/gtskkxvtdp.html

[D17] 最大值与最小值
来源：http://hz.yongpay.top/gtlhqhcvla.html

Py:   max(arr);  min(arr)
来源：http://hz.zhaomingkeji.xyz/gtyzxlwbic.html

PHP:  max($arr);  min($arr);
来源：http://hz.cashguo.top/gtlcaxqbht.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.svipenyu.cn/gtpqjzduyk.html

TS:   Math.max(...arr);
来源：http://hz.andypj.xyz/gthvubzggb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtezwpciqf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xuetiantiany.cn/gtmlntjton.html

Ruby: arr.max;  arr.min
来源：http://hz.redwolf501.top/gtwhlnuvnn.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtamckuuxq.html

[D18] 扁平化嵌套数组
来源：http://hz.yuxming.cn/gtfqtbpejh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cashguo.top/gtjnzhzozz.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gttlwivrhp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gticdidcdl.html

TS:   nested.flat();
来源：http://hz.jinqigfzy.top/gtgirnwdgt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhengqikj.top/gtggzufsdn.html

Go:   // 手写双层循环
来源：http://hz.jqgfzy.top/gttcmwhgyc.html

Ruby: nested.flatten
来源：http://hz.gotoacloud.top/gtolukhwhj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtyvasficr.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtoijqfkho.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ywan-chungtsiang.top/gtdzekztrk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gttjmjmouy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtotovupnq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtawumytrv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigfzy.top/gtwgufczcw.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtjaamzfnz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guowangkeji.top/gtllekashp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtthfbbbbl.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gtakzuyrga.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtllvcpdje.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gtiakubimy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtcsskfmja.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtdkrtolca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ybcxt.top/gtklzpxvsn.html

Go:   // 手写 map[T]int
来源：http://hz.tianlin.xyz/gtfkyxvlhs.html

Ruby: arr.tally
来源：http://hz.redwolf501.top/gtoovzathq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guowangkeji.top/gtioaibhre.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtsolziman.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtuttraqaj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yanxiufei.cn/gtoomkdngo.html

JS:   arr.includes(x)
来源：http://hz.cashguo.top/gttzgffnoy.html

TS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gtdidzsmge.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gtshjqpjaf.html

Go:   slices.Contains(arr, x)
来源：http://hz.hongshengwenyu.top/gtlajyknku.html

Ruby: arr.include?(x)
来源：http://hz.yongpay.top/gtpuqpibcj.html

C#:   list.Contains(x)
来源：http://hz.chenlongwang.top/gtkcgvamok.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtzxvqziml.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtxgtwcyar.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtjijnpwhw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shangyingyoupin.top/gtuwldozvb.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gtuymjdygy.html

Java: new ArrayList<>(list);
来源：http://hz.yangfankeji.com/gtxgqkzgaj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tianlin.xyz/gtczjmrgtn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gtlqghylak.html

C#:   new List<int>(list);
来源：http://hz.chenjidiqi.icu/gtydbnirqu.html

[D23] reduce 累积计算
来源：http://hz.ydjk.org.cn/gtovcopdex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.0kj1m.cn/gttmrfotru.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.kuanghao11.cn/gtmzmgsdak.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtmpdiaoui.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtqvhzhyth.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtjrgaiyas.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtsriutfsw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydzc1.top/gtdobnhiwe.html


<!-- 参考信息 -->