代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtmirhrfnc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.9152youxi.cn/gtqrmhciwz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxinkj.top/gtetjbszgs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.havefunace.top/gtbrmjyqxz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtzesdvlxl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gthrfpkkff.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhiwuduotai.top/gtmonqucmc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yongpay.top/gtzbqsnuwu.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnxiangtu.top/gtszehopcz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtcgkbhkps.html

C#:   f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtipsolywa.html

[C05] 返回多个值
来源：http://hz.ppjwa.cn/gttxvjesky.html

Py:   return a, b
来源：http://hz.shangyingyoupin.top/gtsfyjjukq.html

PHP:  return [$a, $b];
来源：http://hz.cheryme.top/gtypfvxxpu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgfzy.top/gtliioarld.html

TS:   return { a, b };
来源：http://hz.haohaochexian.top/gthufgtqrv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtcvddmiug.html

Go:   return a, b
来源：http://hz.birdmap.top/gttmmkokzn.html

Ruby: return a, b
来源：http://hz.nanxinkj.top/gtnwrccpuu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ywan-chungtsiang.top/gtsnojvstc.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtpdevwkoq.html

Py:   square = lambda x: x * x
来源：http://hz.zhaomingkeji.xyz/gtnxvnmphj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xziqi.cn/gtctepxpnz.html

JS:   const square = x => x * x;
来源：http://hz.tian-w.cn/gtqxqfqwhh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.andypj.xyz/gttabbuctp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtyhnqhpyx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gtdmlzzhqy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgufenzy.top/gtvxgalkpz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuanzx.com/gtnpqbfzmw.html

[C07] 把函数作为参数传入
来源：http://hz.jqgfzy.top/gtyolnclra.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daxiang520.top/gtxilqlwae.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.birdmap.top/gthbswfabf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtgdkwjljf.html

TS:   arr.map(String)
来源：http://hz.zhixingplan.top/gtkgzjyhdz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.smart0.xyz/gtbhawrloa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtkjnmcpgt.html

Ruby: arr.map(&:upcase)
来源：http://hz.gaohongyu789.top/gtlmvwjmfr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.haohaochexian.top/gtmnxldjrs.html

[C08] 闭包
来源：http://hz.jyoumei.cn/gtvlcpepuk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daxiang520.top/gtrlwtuifw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tianlin.xyz/gtlmpcriph.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtqprzrvne.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtxeykfzqa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gttglznmle.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.daxiang520.top/gtetduujko.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuanzhike.top/gtspxzwarj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtumgkjfod.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gtmrhnwmwz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sxryk.cn/gtzanftnte.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtcryuslox.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtpaxvlvvm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtsunddxth.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dianchejie.cn/gtdqsstudg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxinkj.top/gtnvtzthbk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtwstqbpcv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fengsongda.top/gtseeitdan.html

[C10] 变量作用域
来源：http://hz.yueranfly.top/gtmqgnmueh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtjrassaye.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gogol.net.cn/gtkbevpveo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuxming.cn/gtelavbbaj.html

TS:   同 JS
来源：http://hz.gzhubu.top/gtvtejjvpd.html

Java: 方法内为块级作用域
来源：http://hz.jyoumei.cn/gtgpgxzwbq.html

Go:   花括号块级作用域
来源：http://hz.wangshuangyany.cn/gthoxerofw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shanyushiyangkeji.top/gtwiwmtjll.html

C#:   块级作用域
来源：http://hz.yj20258888.top/gtegngtdks.html

[C11] 模块导入与导出
来源：http://hz.iojbl.cn/gtitymfqeb.html

Py:   from module import func
来源：http://hz.zhiwuduotai.top/gtvnulrhpa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.iojbl.cn/gtdlwuqwol.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtfjurqgkd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgufenzy.top/gtmbgfibfz.html

Java: import java.util.List;
来源：http://hz.yuanzhike.top/gtasnrlhdx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hywenlv.cn/gtijbjzrxi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nwbrower.top/gtruvtwxmk.html

C#:   using System.Text;
来源：http://hz.zhaomingkeji.xyz/gtsndwhjps.html

[C12] 立即执行函数 IIFE
来源：http://hz.sweek.top/gtqrrrvcrx.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gtfhyqxtps.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jianghu66.top/gtfeghmbav.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtfxkpbaki.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtlqaboeyt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tianlin.xyz/gthemmmfjb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gtpiifbkzh.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtrbbkmomp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtwooykpyz.html

[C13] 类型声明 / 类型注解
来源：http://hz.c1oappe.top/gtmadwzezq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtohivqycf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtrfcbmsxl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jiagoushi.top/gtqnqnsdmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gticdqtzpb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtfrtatmpd.html

Go:   func add(a, b int) int
来源：http://hz.52xcode.cn/gtjbjgnoit.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtrudiqfah.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ybcxt.top/gtjjimrhcp.html

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gtydphbvdl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cdnleiting.top/gtazhpjwbk.html

PHP:  // 无泛型
来源：http://hz.zycfv.cn/gtjajbtgor.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtnyzhhuqh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhiwuduotai.top/gtdhwunfwf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtvnpfaxnw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cheryme.top/gtxhyzqewa.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtcdrudohw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xziqi.cn/gturyhyfxk.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gtowbalyjr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.haohaochexian.top/gtzkdehanq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtqvrlznua.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtnsscfumt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigufen.top/gtlfxktwyu.html

Java: // 无解构
来源：http://hz.jinqigufen.top/gtiiwyyujp.html

Go:   // 无解构
来源：http://hz.sufxvd.cn/gtbanjvhvb.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtnfkmbmdm.html

C#:   var (a, b) = pair;
来源：http://hz.ybcxt.top/gtpkjwlbwu.html

[C16] 函数 / 方法重载
来源：http://hz.nanxuanxn.top/gtbqjmyjhm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cheryme.top/gtbqqkmcdj.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gtdxgcsuuh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zycfv.cn/gtbqjwnivh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtmdemusak.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zdqjudy.top/gtsxgrlowx.html

Go:   // 无重载：用不同函数名
来源：http://hz.iojbl.cn/gtjrqavwrx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhengqikj.top/gtaxgvllyz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.svipenyu.cn/gtpaqbvxse.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjsvlezda.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtqfbsnggv.html

================================================================================
来源：http://hz.0kj1m.cn/gtptmxubkt.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtmzhowtlh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gtalxtyxtb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtyuxcvbgr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ywan-chungtsiang.top/gtlevpynvs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtiziufitt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.mhx1999.top/gtxrrkwzag.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.meibo888.top/gtpchblobm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xingfuxueyuan.xyz/gttqwslupe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dashuyun.cn/gtjelwbfna.html

[D02] 追加元素到末尾
来源：http://hz.jlsjyb.cn/gtfjokhyvo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtxyhcimad.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtjxdpzrsb.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtsvinpbti.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtkpmdzwsi.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtimaqxuiz.html

Go:   arr = append(arr, 4)
来源：http://hz.tian-w.cn/gtptsxuuua.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtxqcwixjy.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gteqssrqcw.html

[D03] 在指定位置插入元素
来源：http://hz.0kj1m.cn/gtuxezepki.html

Py:   arr.insert(0, 0)
来源：http://hz.ybcxt.top/gtbvfevptv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhiwuduotai.top/gtvcibmmmv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ywan-chungtsiang.top/gtrtkrnedm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhaomingkeji.xyz/gtchlyaciu.html

Java: list.add(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtobpsjxmv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtugfojidw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtwimwshld.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gtvozoeuzs.html

[D04] 删除元素
来源：http://hz.cucudq.cn/gtijcbdfwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtmilvxrcg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guannengcc.top/gthmhjldye.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.c1oappe.top/gtefhsqxja.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gthuktfhqx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258.top/gtivfflxsy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sxryk.cn/gttqfmlymo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtqefoymqn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtblcyaxmp.html

[D05] 访问与修改元素
来源：http://hz.316326.xyz/gtmnioejuv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtkdoecprf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtnwruextn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258888.top/gtvkjyqmht.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhaomingkeji.xyz/gtchydolwt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtaclikdck.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtycklojed.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtcfmyxzsw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgufenzy.top/gtcoxryiip.html

[D06] 数组长度
来源：http://hz.zhoulong.xyz/gttblnikvp.html

Py:   len(arr)
来源：http://hz.zhiwuduotai.top/gtgzwmkvfa.html

PHP:  count($arr);
来源：http://hz.aibaodan.cn/gtolgzxwga.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtkvjtwygg.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gtjexdaump.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtcvhnnhid.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtrroskhqd.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gtiblvqvke.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtxxixnikb.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gtoowrzepc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangkeji.top/gtzsahdcxn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenjidiqi.icu/gthietgqyy.html

JS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtcnscatee.html

TS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtmgyfintn.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gtqtkmaseb.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtngnxljmr.html

Ruby: arr[1, 3]
来源：http://hz.jlsjyb.cn/gtqncqbaho.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangdashe.top/gtdiexrclf.html

[D08] 合并两个数组
来源：http://hz.gzhubu.top/gtorifoxjc.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gthxlpykmg.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxuanxn.top/gtsswznxoi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhoulong.xyz/gtxzhhotgc.html

TS:   [...a, ...b];
来源：http://hz.cheryme.top/gtwzkuwscm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gtupbqpeym.html

Go:   append(a, b...)
来源：http://hz.svipenyu.cn/gtfoniypmn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtmakupzst.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtkosiyhpi.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtgzifhyun.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtyghxfxlu.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtlbybfdff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gttdilgpmr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gtgwpdeiku.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258888.top/gtjwabzxgq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtdnlsiqyi.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtppxgqqgv.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtckhugxwe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtzcsvcrkf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtduegnkqg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtvrzorvqf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gttjntzkmc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtopdyebhn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnxiangtu.top/gtadncwafj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtrvzteuoo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xingfuxueyuan.xyz/gtwxgwylzg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtsmcmutds.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gtmcrjnino.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xingfuxueyuan.xyz/gtpolgitsd.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtosmaslsj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ybcxt.top/gtteehciwz.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtsvjrxzql.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtjkiciyqw.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gtonlihrdq.html

Ruby: arr.reverse
来源：http://hz.sweek.top/gtlrizplne.html

C#:   list.Reverse();
来源：http://hz.xingfuxueyuan.xyz/gtjbhwzxnh.html

[D12] 查找元素下标
来源：http://hz.daxiang520.top/gtwetradcw.html

Py:   arr.index(x);  x in arr
来源：http://hz.cdnleiting.top/gtsgfevpce.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtbvbcmzll.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtoakdugub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtqnwjqslm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtitempozb.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtdshvcozb.html

Ruby: arr.index(x)
来源：http://hz.sxryk.cn/gtmvuzysnf.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gtkgsizmrx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cashguo.top/gtlnvrazja.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtwgggevti.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj202588.top/gtczsedcoe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gttraqilpz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtwfdhtzvm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtkcrmqxun.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.snrcjt.cn/gtycdlxwsc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtllataehd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtskkdzcgi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yvedp.cn/gtkhbxxbcu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtioxfiges.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtiujngfxc.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtpottxqec.html

TS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtvuzaoelc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.svipenyu.cn/gtobpanccw.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtubmvtwti.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gttmbdpcjm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtnhjknjnu.html

[D15] 去重
来源：http://hz.jianghu66.top/gtuyhmdfji.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtncrzkean.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtrwqspsop.html

JS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtwyujnupl.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtkgornher.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hongshengwenyu.top/gtvkevgdwr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtbodyrtiw.html

Ruby: arr.uniq
来源：http://hz.fzhhl.top/gttualgjlt.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtkoigmesa.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangkeji.top/gtxjcuyjxy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnqzz.top/gtowgvowju.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sweek.top/gtvtfvzeno.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtsqlwskfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtaersncho.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtonvxyklx.html

Go:   // 手写循环累加
来源：http://hz.ywan-chungtsiang.top/gtixodzmcb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtfvcnrcfq.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtvagpzdyc.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gtwqohartm.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtstjekteo.html

PHP:  max($arr);  min($arr);
来源：http://hz.vqdsnc.cn/gthlgiwbdu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shangyingyoupin.top/gtzfdovwnk.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtmgttrucp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.mhx1999.top/gtitbioenm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gtvpqlydyr.html

Ruby: arr.max;  arr.min
来源：http://hz.ywan-chungtsiang.top/gtibdqqekc.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtzqfqwlbb.html

[D18] 扁平化嵌套数组
来源：http://hz.jiagoushi.top/gtsslatyzn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtsdemolhq.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtwaeowtxh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtihsudyxe.html

TS:   nested.flat();
来源：http://hz.jinqigfzy.top/gtlhrtzbwz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.svipenyu.cn/gtffptmass.html

Go:   // 手写双层循环
来源：http://hz.sysykeji.top/gtcomilhaq.html

Ruby: nested.flatten
来源：http://hz.sufxvd.cn/gtwufxqown.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sysykeji.top/gtowgluivv.html

[D19] 按字段分组
来源：http://hz.jlsjyb.cn/gtzyexygcz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hysaishi.cn/gtmcklzoac.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtxgapvatu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxuanxn.top/gtlhsydujj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtwfqkteeg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guowangkeji.top/gtgmhfbyfx.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtdqujqaac.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydjk.org.cn/gtrznceksa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtpzrvjlqd.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtlsghanym.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtxgitxuhj.html

PHP:  array_count_values($arr);
来源：http://hz.xuanzx.com/gtuzhvazjd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtqymmruok.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtqeqfysit.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.kuanghao11.cn/gtjwetejpf.html

Go:   // 手写 map[T]int
来源：http://hz.daria6918.cn/gtfroymzmj.html


<!-- 参考信息 -->