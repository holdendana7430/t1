代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtbxqokbak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtmwtsbwdm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtusriagvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtsstjtjuj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gtzvajejcp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangshuangyany.cn/gtvgsykgpo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtclocwwef.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtmakoalee.html

[C02] 默认参数
来源：http://hz.jqgufenzy.top/gtperpofcm.html

Py:   def greet(name="World"): return name
来源：http://hz.hfpthk.cn/gtsrfvpbqo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sysykeji.top/gtxjraotot.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shzxlz.cn/gtcjtkegra.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtmzjrqdzc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dianchejie.cn/gtiafstrgc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sysykeji.top/gtpvbvydcb.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtfpjpafjj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtqiegupvn.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtymxduhqi.html

Py:   def total(*args): return sum(args)
来源：http://hz.cashguo.top/gtozfhyomo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jiagoushi.top/gttaasevvq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtvjemrcuq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtbiklnavb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shuidangran.top/gtqrfyuxsm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xylfe.cn/gtubwxphcn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daria6918.cn/gtrpkathmp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtcgztedql.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtssrmqfxd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtcloenjwz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtynkrqvmi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtcnjbamjr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxinkj.top/gtdwmtyyhm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gtbhlshlrm.html

Go:   // 无：用配置结构体参数
来源：http://hz.hywenlv.cn/gtgsmdrvmc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtoamvuekz.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gtocuaqagu.html

[C05] 返回多个值
来源：http://hz.yangfankeji.com/gtqbpkvbol.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gthjastuls.html

PHP:  return [$a, $b];
来源：http://hz.feifeiyinyue.top/gtkoxlquxg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtsymwogzn.html

TS:   return { a, b };
来源：http://hz.tianlin.xyz/gtrcmypwtf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ivvv.top/gtuysudlug.html

Go:   return a, b
来源：http://hz.hammf.cn/gtaexbauui.html

Ruby: return a, b
来源：http://hz.shzxlz.cn/gtejihjbby.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zycfv.cn/gtsyubtzwq.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtronkxvbb.html

Py:   square = lambda x: x * x
来源：http://hz.haohaochexian.top/gtiaafefzj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnxiangtu.top/gtutsuxhal.html

JS:   const square = x => x * x;
来源：http://hz.mhx1999.top/gtrwjfihtw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxuanxn.top/gttkkpqtpi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shuidangran.top/gtbanzuads.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.0kj1m.cn/gtouzubsin.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhoulong.xyz/gtqwaqcezg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gtygwxsirs.html

[C07] 把函数作为参数传入
来源：http://hz.havefunace.top/gtyymuylrr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gzhubu.top/gtvgulefel.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.smart0.xyz/gttzjoqpkk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydzc1.top/gtfmupvfks.html

TS:   arr.map(String)
来源：http://hz.ywan-chungtsiang.top/gtvxsmlate.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenjidiqi.icu/gtzmouldjq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cheryme.top/gtfrdzvvir.html

Ruby: arr.map(&:upcase)
来源：http://hz.shuidangran.top/gtawoxohyh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xingfuxueyuan.xyz/gtptvccsuq.html

[C08] 闭包
来源：http://hz.hywenlv.cn/gtmxtsofpq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fzhhl.top/gtllmkzdsi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.kuanghao11.cn/gtvtequlyq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtxxvjtygr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtqfkrauic.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gzhubu.top/gtgefbbgtp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xylfe.cn/gtkzycjymt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gturhpysxz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtvwaqczhe.html

[C09] 递归
来源：http://hz.gotoacloud.top/gtcuvurgxl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtofrukaow.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yueranfly.top/gtbtegxcbl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtikssslot.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtzhdjvsgt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shanyushiyangkeji.top/gtiyaiaizw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ehwqpu.com/gthdkebnjg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigufen.top/gttzcbznuc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtpinblgyv.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtwqajgswz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jianghu66.top/gtoaaiqqoo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pycfn.com/gthkztbsjt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtejiatbam.html

TS:   同 JS
来源：http://hz.sweek.top/gtnaafqfyl.html

Java: 方法内为块级作用域
来源：http://hz.daria6918.cn/gtwnnazluy.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtrdbrldcb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xingfuxueyuan.xyz/gtdyrfhuow.html

C#:   块级作用域
来源：http://hz.fzhhl.top/gtqvkhohvr.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtcbvvnqjt.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtnwnambky.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.316326.xyz/gtolmgisob.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtorplnmun.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhongyouzk.top/gtyzobizva.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtqimrfmvn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yanxiufei.cn/gtmvroymse.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yongpay.top/gtkehmyuyg.html

C#:   using System.Text;
来源：http://hz.jinyuanbaomall.cn/gtonuqrsob.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtoudhlfbu.html

Py:   (lambda: print("run"))()
来源：http://hz.cucudq.cn/gtoruxfpas.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yueranfly.top/gtvoqgipeh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gttcjjtaaf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtqmertcwc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hongshengwenyu.top/gtvkujypqz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtnlkqcclu.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnxiangtu.top/gtbwfmtjsj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gotoacloud.top/gtpkedxnto.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinqigufen.top/gtzpfjimer.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fzhhl.top/gtzkcveqgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtolgyaysu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangtech.top/gtxhhswgtg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtrheupzkd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtauxtfazm.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtgnfgkeuz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.smart0.xyz/gtsmfmykwj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtewlefwal.html

[C14] 泛型函数
来源：http://hz.gotoacloud.top/gtphjgwfit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtlszylnio.html

PHP:  // 无泛型
来源：http://hz.tianlin.xyz/gtimoeqxxz.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtbesdztfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jyoumei.cn/gtudlsraeu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.c1oappe.top/gtqykbxxtg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtvfngdlgh.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtpvbnihwg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenjidiqi.icu/gtqrpymdoc.html

[C15] 解构 / 展开参数
来源：http://hz.zhongyouzk.top/gteewfkxhk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangkeji.top/gtuodeczon.html

PHP:  [$a, $b] = $pair;
来源：http://hz.quarkkingdee.top/gtmwwrzbrh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtxeaesmpg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xingfuxueyuan.xyz/gtqeehbuzj.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gtbfudyfnb.html

Go:   // 无解构
来源：http://hz.gzhubu.top/gtanpicggq.html

Ruby: a, b = pair
来源：http://hz.dashuyun.cn/gtqnqtqqjo.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gtlqliiwcw.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtdmmgqdqb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fzhhl.top/gtbafhmwch.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtslosyfrs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtsmriwabu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgfzy.top/gtvxfinzpw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gtvnsjgojb.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gtngkutnwf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydzc1.top/gtwrwlwxdh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtzpejalcf.html

================================================================================
来源：http://hz.9152youxi.cn/gtuhznofpn.html

D. 数组 / 列表 / 集合
来源：http://hz.havefunace.top/gthwspniqi.html

================================================================================
来源：http://hz.yangfankeji.com/gthfidnoxd.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtufcicdxh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hfpthk.cn/gtgoqktdte.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gotoacloud.top/gtlwapxtjw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gtrpazmxbt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jlsjyb.cn/gtprnxkfal.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pycfn.com/gtygrdnqmn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hongshengwenyu.top/gtwkdksuqx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtgqvnfyzk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jiagoushi.top/gtsmewzglo.html

[D02] 追加元素到末尾
来源：http://hz.feifeiyinyue.top/gtelyfyrvb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hammf.cn/gtpoblaeny.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtuiawcrga.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtyxnivkyy.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtvozytzdf.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtssadkhgq.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtsolsvphb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnxiangtu.top/gtngpyfhna.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtbqmauzxg.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gttrronqst.html

Py:   arr.insert(0, 0)
来源：http://hz.wangshuangyany.cn/gtacoasxwl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dashuyun.cn/gtqzcbvvzf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj202588.top/gtixubfnwv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gtigjdujzv.html

Java: list.add(0, 0);
来源：http://hz.yangfankeji.com/gttwhlziqr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtrgbqhrfu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.smart0.xyz/gtagetutck.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtxzxszgnx.html

[D04] 删除元素
来源：http://hz.gzhubu.top/gtoymcqzuw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dashuyun.cn/gtwttytjla.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gtbzgcuelu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ybcxt.top/gtslqnfgap.html

TS:   arr.splice(0, 1);
来源：http://hz.xylfe.cn/gtwfutfmbs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnqzz.top/gtfzqjztxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtdbhjugvj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtglrzsbto.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtphtkyyvs.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtdiuvtknm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtgnieogkz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.dashuyun.cn/gthhiudzar.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gtbmkkqqzo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jiagoushi.top/gtsagzschc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj202588.top/gthbgrqgfm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.redwolf501.top/gtumdshrjo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtqakzasrj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtioknfcjy.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtttlwgfbu.html

Py:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtngybhykz.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtuyokjmbr.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtlclrnlfh.html

TS:   arr.length
来源：http://hz.ydzc1.top/gtyrdjdamo.html

Java: list.size();
来源：http://hz.jyoumei.cn/gthzbsqspw.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gtnvfhbguh.html

Ruby: arr.length; arr.size
来源：http://hz.mhx1999.top/gtwxqypfhf.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtqcmujfws.html

[D07] 切片 / 取子数组
来源：http://hz.cqqwz.cn/gtihbklfxb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtgrpzlawa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtvfvzveyy.html

JS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtqhimytxi.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtranajfez.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtumozwufy.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtgptevqmt.html

Ruby: arr[1, 3]
来源：http://hz.chenjidiqi.icu/gtzvmgtshv.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtmsbdvfzj.html

[D08] 合并两个数组
来源：http://hz.yj20258888.top/gtaqelmexd.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangdashe.top/gtnuiyders.html

PHP:  array_merge($a, $b);
来源：http://hz.birdmap.top/gtqqhotfpf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xylfe.cn/gtvjxsbdja.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtiromvywm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtxqwjwqbp.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtphjjkrkm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jyoumei.cn/gtokepwwqq.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gttjrtpown.html

[D09] 排序（升序）
来源：http://hz.gogol.net.cn/gtxjinzvth.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtsyysxbtw.html

PHP:  sort($arr);
来源：http://hz.zhoulong.xyz/gtbvjxygah.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ehwqpu.com/gtsdhegsbf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigfzy.top/gtrwpybmju.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtdcgizpsj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gturiahewl.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtgfqbkfqy.html

C#:   list.Sort();
来源：http://hz.jqgfzy.top/gtduxzgbgz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gtzsemsdjg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtkxhioscs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dashuyun.cn/gtryyoodzw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtmmrasbcn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtfgvicrgj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ybcxt.top/gthpgduoky.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gtpubdbesg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtcjcoloqo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sweek.top/gtnqjyjwta.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gthhsqetax.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gaohongyu789.top/gtylxqhwwk.html

PHP:  array_reverse($arr);
来源：http://hz.chenjidiqi.icu/gtztsxbpmk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ywan-chungtsiang.top/gttlktydfq.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtroecsvkh.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gtgecotqru.html

Go:   slices.Reverse(arr)
来源：http://hz.pengpengdd.cyou/gtnyvmzibo.html

Ruby: arr.reverse
来源：http://hz.bjfxy.top/gtajwvuhno.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtonnpmjtv.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtiyayfjnb.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gtkoekwato.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtbftzmwjn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gtnzddlysr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtbdxhceoc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sysykeji.top/gtaktpgjce.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gttersyioq.html

Ruby: arr.index(x)
来源：http://hz.redwolf501.top/gtmcugjori.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtqpgqmmey.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ybcxt.top/gtvnfksina.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gthwbgdwtc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtqbgyouae.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtlcrbndct.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtqbpeuhmf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dianchejie.cn/gtmifsrrwv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sxryk.cn/gtolrbklvu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cdnleiting.top/gtqooektyn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yangfankeji.com/gtoytdfqmd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.redwolf501.top/gtmdyuwzko.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtqwlfuzjm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gttthhlcge.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gthpcnwabe.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtndqfalho.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gteawyqucg.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtvcjyrnzt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtqjjprznl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhijiandao.cn/gtcfiutepz.html

[D15] 去重
来源：http://hz.chenzaomai.com/gttbjpzqgm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtcgzsyavm.html

PHP:  array_unique($arr);
来源：http://hz.yueranfly.top/gtwqbbnnko.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtispcqkbj.html

TS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtwgnchiod.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtvknwvqor.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtwturlzby.html

Ruby: arr.uniq
来源：http://hz.gzhubu.top/gtdzqpzalo.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gtgwjstsam.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtukpulair.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtxaszmskj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtacetyzfc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtyksneyax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gteeuuxkmw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj202588.top/gtebxavzqx.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtvkykzkzd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yongpay.top/gtvxxwndhk.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gthqivvkww.html

[D17] 最大值与最小值
来源：http://hz.yvedp.cn/gtmbwdfcvy.html

Py:   max(arr);  min(arr)
来源：http://hz.zhengqikj.top/gtlcmfjwkn.html

PHP:  max($arr);  min($arr);
来源：http://hz.fzhhl.top/gtyqqtelpe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtzvbhusgs.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gtkjnimrvd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gttcnagvqt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gturjvkrwm.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtuzbwocpn.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtleanmnwp.html

[D18] 扁平化嵌套数组
来源：http://hz.zhaomingkeji.xyz/gtqgxzyasu.html


<!-- 参考信息 -->