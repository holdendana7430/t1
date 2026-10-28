代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtiyxtlhnp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.meibo888.top/gtfzihhpbx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gotoacloud.top/gtjjmqqrio.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuanzx.com/gtqywospfz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yangfankeji.com/gtlypylccu.html

[C03] 可变参数
来源：http://hz.gaohongyu789.top/gtkbmlptzl.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gtwxndkiuu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gtynjjmreo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtctxtqjgy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtbxfveoej.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.vqdsnc.cn/gtvdjnnmjy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtvvwnmujb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuxming.cn/gtnlhhjidm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hfpthk.cn/gtkmjvxfxd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yanxiufei.cn/gtsgrzkcbv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtzxjfpweq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.0kj1m.cn/gtqfzqpole.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgufenzy.top/gtoixbvgth.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuanzhike.top/gtxuzvrlyi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xziqi.cn/gtbjavegsh.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gtowikailx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtjzqohoab.html

C#:   f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtqpgyfdvy.html

[C05] 返回多个值
来源：http://hz.hongshengwenyu.top/gtfaxogcza.html

Py:   return a, b
来源：http://hz.fengsongda.top/gtqodcgoxp.html

PHP:  return [$a, $b];
来源：http://hz.jianghu66.top/gtuamfnxgn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.52xcode.cn/gtqrjsivct.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtldfbukvm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hywenlv.cn/gtkfypcqtt.html

Go:   return a, b
来源：http://hz.hysaishi.cn/gtqyxovlne.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtmurmteqb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.havefunace.top/gtfeagilou.html

[C06] 匿名函数 / lambda
来源：http://hz.vqdsnc.cn/gtziicmlbm.html

Py:   square = lambda x: x * x
来源：http://hz.yvedp.cn/gtvfkiyzsb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhengqikj.top/gtjiqakocw.html

JS:   const square = x => x * x;
来源：http://hz.yongpay.top/gtjotnclcf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gotoacloud.top/gttlqglmrk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtgmjhwmzz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.bjfxy.top/gtcwkktaif.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ivvv.top/gtzpqxqtpw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gogol.net.cn/gtkvxecilb.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtcqkyujku.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gzhubu.top/gtiklgcrmg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gtbbjtlfqt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhaomingkeji.xyz/gtttmkygog.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtrrtkkwxd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gtdzniwdbb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dianchejie.cn/gthofrkldj.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhoulong.xyz/gtrcjqpnuf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jyoumei.cn/gtwwabztam.html

[C08] 闭包
来源：http://hz.jyoumei.cn/gtgzrrmblb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuanzhike.top/gtennsisfu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shangyingyoupin.top/gtwmutgxrk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtnbnpkmve.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtfwdljqjb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gtzebjsmjz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtnbbsjlqd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtzzlapjyw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtrujkseqr.html

[C09] 递归
来源：http://hz.sweek.top/gtvhiwhxrp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtsaiqpwqv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.nwbrower.top/gtewltvhar.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtqbqxaatv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtbmlqejll.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.iojbl.cn/gtjyevcmqj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jyoumei.cn/gttatexawn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258.top/gthguhelpb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtjfivlecb.html

[C10] 变量作用域
来源：http://hz.zhongyouzk.top/gtfndqjmmq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zycfv.cn/gtqvlalpru.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtgujmxqjo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ppjwa.cn/gtsitlllmg.html

TS:   同 JS
来源：http://hz.shanyushiyangkeji.top/gtoxaugfql.html

Java: 方法内为块级作用域
来源：http://hz.hysaishi.cn/gtopigozls.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtdbfcmclg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigfzy.top/gtbqecjucz.html

C#:   块级作用域
来源：http://hz.yongpay.top/gtmfgbotwt.html

[C11] 模块导入与导出
来源：http://hz.52xcode.cn/gtdahugjql.html

Py:   from module import func
来源：http://hz.quarkkingdee.top/gtsoosdhpt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinghuilouyu.cn/gtgkqlmdmb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ybcxt.top/gtordhendc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cdnleiting.top/gtittxtpft.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtbjtrbvtw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gaohongyu789.top/gtpgisxmia.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtddefeomy.html

C#:   using System.Text;
来源：http://hz.tian-w.cn/gtmsjtlpmm.html

[C12] 立即执行函数 IIFE
来源：http://hz.gogol.net.cn/gtsigmpitp.html

Py:   (lambda: print("run"))()
来源：http://hz.pycfn.com/gtvioudpjn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gttfkzbzyl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtmyguzyjx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtyfesahhw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gtlwdxullr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtgzwqgfva.html

Ruby: -> { puts "run" }.call
来源：http://hz.ybcxt.top/gthfwqirun.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuetiantiany.cn/gtusdtzrfq.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtscsaduuy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gtdsxumbpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtfpzxssko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtjvenhhra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtwmvhjwvn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtoqncyihe.html

Go:   func add(a, b int) int
来源：http://hz.jqgfzy.top/gtfjfhgukz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtdkiauoer.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtteepghdk.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gtmdrzwxnj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shzxlz.cn/gtfgejznhq.html

PHP:  // 无泛型
来源：http://hz.kuanghao11.cn/gtcggskmgg.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gteflojwvx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.kuanghao11.cn/gtltkpksxv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhijiandao.cn/gtintlnurj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gtiltilprg.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtvmxxjowr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gtstwfwjdu.html

[C15] 解构 / 展开参数
来源：http://hz.hnxiangtu.top/gtlmhiwejk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aizwys.cn/gthrvnxxuy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtkwctziwb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtjwatoqwe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jiagoushi.top/gtrbiqvbdz.html

Java: // 无解构
来源：http://hz.bjfxy.top/gtyczymrtg.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gtmezapwbv.html

Ruby: a, b = pair
来源：http://hz.aibaodan.cn/gtfzrrpcsh.html

C#:   var (a, b) = pair;
来源：http://hz.chenzaomai.com/gtuzetsusd.html

[C16] 函数 / 方法重载
来源：http://hz.fengsongda.top/gtghbsvpka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gtxvmifxkj.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gtcnffwbfj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangtech.top/gtcsciynnb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtwpzkosov.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtpwsnfkrm.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gtriknixdx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.316326.xyz/gtfovysyak.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtmmhwxhug.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjcobdbnu.html

D. 数组 / 列表 / 集合
来源：http://hz.chenlongwang.top/gtujcfxvon.html

================================================================================
来源：http://hz.havefunace.top/gtwoujpomb.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtbfjckkqs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtvbbybwht.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jianghu66.top/gtwlusmamo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtsspyjcyc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tian-w.cn/gtypbvktse.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gtpdopvtxj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gthoehghcu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yvedp.cn/gtjptmwvmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gtxfeqwnag.html

[D02] 追加元素到末尾
来源：http://hz.yvedp.cn/gtqgfgcgvr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yonumen.top/gttyxjsrvj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tian-w.cn/gtldhkazjy.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtcpvtacua.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtdmfeqkjx.html

Java: list.add(4);
来源：http://hz.jinyuanbaomall.cn/gtshfmvaba.html

Go:   arr = append(arr, 4)
来源：http://hz.xinyue.icu/gtdysifnlz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hfpthk.cn/gtobybccjk.html

C#:   list.Add(4);
来源：http://hz.ydzc1.top/gtbexqfqug.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtwhayaqoz.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtzzbkxhvz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yongpay.top/gtsofvsmcy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.kuanghao11.cn/gtpoppible.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtfrldrovq.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gtufntdign.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtfpxaunro.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhengqikj.top/gtevuvadmw.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gthpbmloah.html

[D04] 删除元素
来源：http://hz.smart0.xyz/gtyivrqzoe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.feifeiyinyue.top/gtlpdhmqsq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sxryk.cn/gtxgsvivcz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangdashe.top/gtygtzqyhm.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gtacqlaksj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gtrekqobqs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gttnqhbisy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ivvv.top/gtewhvuyjb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxinkj.top/gtzcuaqjiz.html

[D05] 访问与修改元素
来源：http://hz.zhiwuduotai.top/gtrmzoqmyb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtmzsbkfxl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtnkxljnxs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuxming.cn/gtcdpdtffq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yuxming.cn/gtwywaokrg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gtdkehpniv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtedvwbuss.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtzkkemjtu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtaduphura.html

[D06] 数组长度
来源：http://hz.snrcjt.cn/gtucwpmaco.html

Py:   len(arr)
来源：http://hz.nanxinkj.top/gttfersfau.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtjtcqfeop.html

JS:   arr.length
来源：http://hz.guannengcc.top/gtumopbain.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtrgzvexwi.html

Java: list.size();
来源：http://hz.316326.xyz/gtmhwjmkyz.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gtjwcprrzm.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gtkmwucvvv.html

C#:   list.Count;
来源：http://hz.chenjidiqi.icu/gtstdkwhel.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtvyltbtbm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.quarkkingdee.top/gtknfptrmu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.andypj.xyz/gtssdphmmd.html

JS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtvgmczedl.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtwobryzex.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtdfnxkery.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtkilhrrrs.html

Ruby: arr[1, 3]
来源：http://hz.gogol.net.cn/gtpalkqhbt.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenlongwang.top/gtlhcgfutw.html

[D08] 合并两个数组
来源：http://hz.zhoulong.xyz/gtsmiwndgj.html

Py:   a + b;  a.extend(b)
来源：http://hz.yanxiufei.cn/gtdddmdudl.html

PHP:  array_merge($a, $b);
来源：http://hz.ybcxt.top/gtopsmchnz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gtqgrhgjki.html

TS:   [...a, ...b];
来源：http://hz.yj20258888.top/gtcslatqqw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtvhqtoizx.html

Go:   append(a, b...)
来源：http://hz.jyoumei.cn/gthrpkifdi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtxpjwtvnp.html

C#:   a.Concat(b).ToList()
来源：http://hz.fzhhl.top/gtspjwpmpo.html

[D09] 排序（升序）
来源：http://hz.dashuyun.cn/gtuvqgpjcw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtoczlmcsr.html

PHP:  sort($arr);
来源：http://hz.xingfuxueyuan.xyz/gtlytijwog.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtvlpdixkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daria6918.cn/gtvlhbtxto.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gtatnarcas.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuanzx.com/gtvyzqueeh.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtnkoiwkoc.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gtdllvcvys.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtymmisbkv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtvaygnper.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnqzz.top/gtwzaluaqi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtrpnhdveb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtyihmpgpw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtvxgmdvld.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yanxiufei.cn/gtonkwsmiw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtrsbyxhqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gtsfjvtjid.html

[D11] 反转数组
来源：http://hz.gotoacloud.top/gtqiwvwgjj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtwvrjhvkc.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtjxtvhcnj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daria6918.cn/gtdxhslppi.html

TS:   [...arr].reverse();
来源：http://hz.yvedp.cn/gtyiyrbfwl.html

Java: Collections.reverse(list);
来源：http://hz.shzxlz.cn/gtahtxxtyj.html

Go:   slices.Reverse(arr)
来源：http://hz.havefunace.top/gtxcqrnfhr.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtqokgqekg.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gttfrcpdpk.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtbjlnsrrc.html

Py:   arr.index(x);  x in arr
来源：http://hz.yueranfly.top/gtvwdfhklp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gthsdhrabu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gttcmfbegx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtvtpkcgyv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aibaodan.cn/gtblylskld.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtjnceujjs.html

Ruby: arr.index(x)
来源：http://hz.ydjk.org.cn/gtocmmkurv.html

C#:   list.IndexOf(x);
来源：http://hz.redwolf501.top/gtaemiiwcv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtvryeyjld.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangdashe.top/gtyehkmuxj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtidlqmwdt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtgremzsjd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtgfwygurs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gtirxjvjze.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtsuapszin.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.meibo888.top/gtoanbxcjv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.feifeiyinyue.top/gtfntystsa.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtofbhgody.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.smart0.xyz/gtrhfpxwal.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gttcejmsuo.html

JS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtpgbnlqiy.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtwnevoscg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnxiangtu.top/gtqsumlsxu.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtfbrrugkr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtrktqwwmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtwibdxivr.html

[D15] 去重
来源：http://hz.ehwqpu.com/gtvrngttgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtmpcztnef.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtodnpgtvc.html

JS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtwdhmpmta.html

TS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtkedgdeea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtepnjierw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gttqthezyh.html

Ruby: arr.uniq
来源：http://hz.jinqigfzy.top/gteleooqiw.html

C#:   list.Distinct().ToList()
来源：http://hz.zdqjudy.top/gtwldzbvwl.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtkojiywnm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sweek.top/gtoxrynagw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtsyuspvcb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtxfeebwjy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtilicpyee.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtlrqarqij.html

Go:   // 手写循环累加
来源：http://hz.daxiang520.top/gtstyalwiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtilzioiup.html

C#:   list.Sum();  list.Average()
来源：http://hz.redwolf501.top/gtbhsfjovu.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtvngfvtkp.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtrfgiogim.html

PHP:  max($arr);  min($arr);
来源：http://hz.shangyingyoupin.top/gtdbsojhwu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtxcgbjuuy.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtixpfajcj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtqmwrzcdh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtywxqvgvu.html

Ruby: arr.max;  arr.min
来源：http://hz.jinyuanbaomall.cn/gtbyjicpot.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtrjbuixhj.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtpxuqhdoi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jiagoushi.top/gtngcabmeo.html

PHP:  array_merge(...$nested);
来源：http://hz.shuidangran.top/gtulkazmjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuetiantiany.cn/gtocpbgjvg.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gteubaiicq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtanwlsjpv.html

Go:   // 手写双层循环
来源：http://hz.gaohongyu789.top/gtlaisimao.html

Ruby: nested.flatten
来源：http://hz.kuanghao11.cn/gtvuzpnzat.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtdyrbrvby.html

[D19] 按字段分组
来源：http://hz.chenzaomai.com/gtrbrqksli.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gthfkdhjji.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangdashe.top/gtmufhxumy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gogol.net.cn/gtmrkrrybl.html


<!-- 参考信息 -->