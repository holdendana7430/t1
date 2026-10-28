代发 wailian999

Java: if (data == null) return;
来源：http://hz.kuanghao11.cn/gtounoinel.html

Go:   if data == nil { return }
来源：http://hz.xziqi.cn/gtidzptmoy.html

Ruby: return if data.nil?
来源：http://hz.ehwqpu.com/gtpunlvczb.html

C#:   if (data == null) return;
来源：http://hz.daria6918.cn/gtiyjytbeo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttaiblttq.html

C. 函数与作用域
来源：http://hz.316326.xyz/gtzbjlfyjc.html

================================================================================
来源：http://hz.aizwys.cn/gttyllqiul.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gthjrhoazy.html

Py:   def add(a, b): return a + b
来源：http://hz.hammf.cn/gtuvromkyv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gttzwqlioh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenlongwang.top/gtlaqstfsr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtlngzbbpq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtdoavlmjg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtdysbgprr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ppjwa.cn/gttdkrcnim.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtfxffnplf.html

[C02] 默认参数
来源：http://hz.0kj1m.cn/gtjgwhukmt.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxuanxn.top/gtfbzlpigf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtiksbokog.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtpnjasdzj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gtqepvitod.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.pycfn.com/gtchlwvjng.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shangyingyoupin.top/gtzjjomuhm.html

Ruby: def greet(name = "World") = name
来源：http://hz.gotoacloud.top/gtfzfeeaow.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.vqdsnc.cn/gtdgflsnsy.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtxwdqecjd.html

Py:   def total(*args): return sum(args)
来源：http://hz.cashguo.top/gtyqfxkwal.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.c1oappe.top/gtsmjjynjc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gthsxcjyoe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtqdalfryq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangkeji.top/gtadumynro.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ehwqpu.com/gtgrsjklaf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dianchejie.cn/gtzsykqjwx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhijiandao.cn/gtksdlqfzx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.feifeiyinyue.top/gtjzdwnsxp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.bjfxy.top/gtefthjijx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ppjwa.cn/gtmoyjtiec.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtholhkwiw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shangyingyoupin.top/gtvbozvryi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sweek.top/gtkuvahbyw.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtakusspsm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtaacfhdan.html

C#:   f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gttudsjmed.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtbdswdenb.html

Py:   return a, b
来源：http://hz.chenjidiqi.icu/gtqntyofat.html

PHP:  return [$a, $b];
来源：http://hz.shzxlz.cn/gtkrvganlg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.bjfxy.top/gtqnpzhmzj.html

TS:   return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtbeaegjgt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.snrcjt.cn/gtawoazqnl.html

Go:   return a, b
来源：http://hz.zhoulong.xyz/gtlfixgehu.html

Ruby: return a, b
来源：http://hz.hammf.cn/gtqlwblpeq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jianghu66.top/gttphjibpj.html

[C06] 匿名函数 / lambda
来源：http://hz.xingfuxueyuan.xyz/gtcpdegykm.html

Py:   square = lambda x: x * x
来源：http://hz.yj202588.top/gtwtvxjvlb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinghuilouyu.cn/gtdqwucugz.html

JS:   const square = x => x * x;
来源：http://hz.yanxiufei.cn/gtygwvnuwh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jyoumei.cn/gtggdhajop.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gzhubu.top/gtmuvorjja.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zycfv.cn/gtcwpqpmwt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtyelcmrms.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenlongwang.top/gtyospdnjy.html

[C07] 把函数作为参数传入
来源：http://hz.aizwys.cn/gtxmknxuua.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenzaomai.com/gtsxhnyhns.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yangfankeji.com/gtwadlqgkm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtpamlesjv.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtlogazavp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jiagoushi.top/gtdmaveasa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daria6918.cn/gtnbrdrfyn.html

Ruby: arr.map(&:upcase)
来源：http://hz.gogol.net.cn/gtvfhzolza.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuxming.cn/gteojpwpvz.html

[C08] 闭包
来源：http://hz.andypj.xyz/gtcwirkehh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenlongwang.top/gtievnlxxh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtobvfzetp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtavwthqhe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtzgllecty.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuxming.cn/gthikffnyf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.meibo888.top/gtlfnsfqua.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gthfcztsnh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gteafldgxc.html

[C09] 递归
来源：http://hz.jqgufenzy.top/gtckhrlmwl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.c1oappe.top/gttrxomgee.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.birdmap.top/gttxdqqpau.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtcoeezjic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtqesvqclp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtfxllmarq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtmbrkntyf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daria6918.cn/gtlhnjflry.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.andypj.xyz/gtzlrttimi.html

[C10] 变量作用域
来源：http://hz.cucudq.cn/gtkqtxeved.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sysykeji.top/gtxzysyqbu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtoylqrhzw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtwbvpkbva.html

TS:   同 JS
来源：http://hz.yuanzhike.top/gtjxogkrsr.html

Java: 方法内为块级作用域
来源：http://hz.ybcxt.top/gtsefjkwhg.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtzvlhdblm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangdashe.top/gtanujdwsb.html

C#:   块级作用域
来源：http://hz.zhijiandao.cn/gtpeddnwlz.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtnxdwdvpz.html

Py:   from module import func
来源：http://hz.chenzaomai.com/gtryyculxq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gtdmdmctkz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj202588.top/gtzbfiekoe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtubauzxqj.html

Java: import java.util.List;
来源：http://hz.feifeiyinyue.top/gtuqwhsnwq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtbpkbxkem.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtpmmtpvxu.html

C#:   using System.Text;
来源：http://hz.shzxlz.cn/gtftwjhmsf.html

[C12] 立即执行函数 IIFE
来源：http://hz.fengsongda.top/gtfdoycghw.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtobokcbbn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ybcxt.top/gtkklrnxkd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtjchfsrpd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtzdahsnkh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnxiangtu.top/gtxovdqlaj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pycfn.com/gtyotcxlfp.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtkzqumxjk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gtwhfbmnfg.html

[C13] 类型声明 / 类型注解
来源：http://hz.redwolf501.top/gthxmbcuvo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sufxvd.cn/gtdcfulhva.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtwllevzoh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtfaitvzzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtjlezfird.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtmpsvcdbg.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gtnmqkxuqi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtstdlemvp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhongyouzk.top/gtylgkhtvr.html

[C14] 泛型函数
来源：http://hz.quarkkingdee.top/gtgzlunemg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhongyouzk.top/gtgjujtoqo.html

PHP:  // 无泛型
来源：http://hz.jqgfzy.top/gtkrzdzfwj.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtybiqcuwf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.9152youxi.cn/gtbhdkdiug.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtgihfscmq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtypynotsf.html

Ruby: # 无泛型
来源：http://hz.sufxvd.cn/gtrtvuqljd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xylfe.cn/gtokwltjeq.html

[C15] 解构 / 展开参数
来源：http://hz.wangshuangyany.cn/gttadggngd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guannengcc.top/gtjspnpnxi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtsnaaycdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtlexgonxp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ivvv.top/gtjclpkwzf.html

Java: // 无解构
来源：http://hz.meibo888.top/gtljovuoji.html

Go:   // 无解构
来源：http://hz.meibo888.top/gtiducpfsh.html

Ruby: a, b = pair
来源：http://hz.tian-w.cn/gtulqjqusa.html

C#:   var (a, b) = pair;
来源：http://hz.jyoumei.cn/gtgbflcbhi.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtjsptccou.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pycfn.com/gtvgcjhihe.html

PHP:  // 无重载
来源：http://hz.yuanzhike.top/gtmlrxerwp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuanzhike.top/gtvkwlzevb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gticvtzurv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hysaishi.cn/gtzdtsjqcc.html

Go:   // 无重载：用不同函数名
来源：http://hz.havefunace.top/gthxkdoyem.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtvxmwvovp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cdnleiting.top/gtzcchrhbi.html

================================================================================
来源：http://hz.tianlin.xyz/gtvfwtfuxm.html

D. 数组 / 列表 / 集合
来源：http://hz.guannengcc.top/gtbpeuwymx.html

================================================================================
来源：http://hz.pycfn.com/gtqamfcrmo.html

[D01] 创建数组 / 列表
来源：http://hz.c1oappe.top/gtircigxmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258888.top/gtjynovnck.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuetiantiany.cn/gtuvcuqbmb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtcideaitl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gtaklonuak.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.mhx1999.top/gtwthhycfe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.haohaochexian.top/gtgxsshnch.html

Ruby: arr = [1, 2, 3]
来源：http://hz.svipenyu.cn/gtmzgkkrbm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtxpzxocdg.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gtursubbvn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnqzz.top/gtwieczmjh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtvvosdrjf.html

JS:   arr.push(4);
来源：http://hz.hongshengwenyu.top/gthelgikuu.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtxsgdnlqn.html

Java: list.add(4);
来源：http://hz.sxryk.cn/gtlgwrfjmt.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gtaeacnvoz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtqhcfreuf.html

C#:   list.Add(4);
来源：http://hz.yvedp.cn/gtqbzjulnq.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gtsgrtvdbq.html

Py:   arr.insert(0, 0)
来源：http://hz.hysaishi.cn/gtlngewvbd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gzhubu.top/gtkebyoxrj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yanxiufei.cn/gtomjeynpk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.iojbl.cn/gtlxtellyd.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtlbxxrhlm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.0kj1m.cn/gtweoosnhi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xuetiantiany.cn/gtqoblamfn.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtygwyoriu.html

[D04] 删除元素
来源：http://hz.ehwqpu.com/gtgbljtkhu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtwppfawzx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtzonmyksa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gotoacloud.top/gtpntzxrwu.html

TS:   arr.splice(0, 1);
来源：http://hz.guannengcc.top/gtfxvbaxys.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtansuofzs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gttvrsbvar.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ivvv.top/gtwyzdytka.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aizwys.cn/gtaustbzgw.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtzydhnpda.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtjycntrqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hammf.cn/gtluljtqdl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yongpay.top/gtwzfnqkpx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hywenlv.cn/gtydgnbzvg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gotoacloud.top/gtsnauspsn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtumocjifv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ivvv.top/gtgptwjqor.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258888.top/gtgzarbtir.html

[D06] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtcrbxhpcw.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtxrfmttnu.html

PHP:  count($arr);
来源：http://hz.jinyuanbaomall.cn/gtrdjezxiv.html

JS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtkktfnmkw.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtnibokkfq.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtgcczxchp.html

Go:   len(arr)
来源：http://hz.birdmap.top/gtvqxscppp.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtumtjakuw.html

C#:   list.Count;
来源：http://hz.sxryk.cn/gtjysibsjg.html

[D07] 切片 / 取子数组
来源：http://hz.shzxlz.cn/gtyrcuquyr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dianchejie.cn/gtuatfksqd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenjidiqi.icu/gthwinfzug.html

JS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtyolmuwrm.html

TS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtqyeohihn.html

Java: list.subList(1, 4);
来源：http://hz.guannengcc.top/gtclrwooso.html

Go:   arr[1:4]
来源：http://hz.tian-w.cn/gtklxnjscn.html

Ruby: arr[1, 3]
来源：http://hz.daxiang520.top/gtnikwvahp.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtitexzwul.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtbznlxioz.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtcedydcjl.html

PHP:  array_merge($a, $b);
来源：http://hz.guannengcc.top/gtbznfsipi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtixsrodey.html

TS:   [...a, ...b];
来源：http://hz.pycfn.com/gtmkhfnzzt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cdnleiting.top/gtamvqkruu.html

Go:   append(a, b...)
来源：http://hz.xinyue.icu/gtjupohkia.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gotoacloud.top/gtafkqhawd.html

C#:   a.Concat(b).ToList()
来源：http://hz.gaohongyu789.top/gtqraousgk.html

[D09] 排序（升序）
来源：http://hz.yuanzhike.top/gtfxpmcznm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zycfv.cn/gtfmfyrcfn.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtddrmccml.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtaugiaggi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtghtdrvxz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinghuilouyu.cn/gtzqeuvmfr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtnxyveiuc.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtgybmqrdj.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gtzcggzvws.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtkoeybvnd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtkiihxjsz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhixingplan.top/gthkfrzsfn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tanke756.top/gtfphpyogw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtdpnvbvox.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtcptpdlpp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtvcbanaqp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yangfankeji.com/gtajdljapw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtaennsqeo.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtqsprsdsg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.c1oappe.top/gttnjolapa.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtvvtrdamo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gthfjyqdox.html

TS:   [...arr].reverse();
来源：http://hz.cashguo.top/gtuicemaoh.html

Java: Collections.reverse(list);
来源：http://hz.wangdashe.top/gtmgdnmsjf.html

Go:   slices.Reverse(arr)
来源：http://hz.ivvv.top/gtwejurrni.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtdkccotam.html

C#:   list.Reverse();
来源：http://hz.pengpengdd.cyou/gtquxbgjjk.html

[D12] 查找元素下标
来源：http://hz.wangdashe.top/gtrmcbyefx.html

Py:   arr.index(x);  x in arr
来源：http://hz.jyoumei.cn/gtlejglwpq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.havefunace.top/gtskvtcgqo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtbnpcfzwi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtvcfjmspr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhongyouzk.top/gtehzohwfu.html

Go:   slices.Index(arr, x)
来源：http://hz.chenzaomai.com/gtadxjwnon.html

Ruby: arr.index(x)
来源：http://hz.xylfe.cn/gtruocaqst.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtqjnbkvkv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtxrvjopii.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtekwylhoh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gttizdzlup.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtoalprxyq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtontofklr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jianghu66.top/gtoplszvxz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.smart0.xyz/gtxbaebstt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtxdrtqcbd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtfdnhglzd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtufocmsep.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtwtrhcogz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gaohongyu789.top/gtxsqpycby.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtgcpjbgad.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtnrshnspn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gtfevwxgdr.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gteohyehpq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gtbworoghg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gogol.net.cn/gtllmfzfng.html

[D15] 去重
来源：http://hz.hongshengwenyu.top/gtrikegfzc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gttsithihq.html

PHP:  array_unique($arr);
来源：http://hz.vqdsnc.cn/gtsfsmnyjh.html

JS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtrjcsupll.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtmzoiczcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gtnsmvvqnr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtblwjdkaj.html

Ruby: arr.uniq
来源：http://hz.hysaishi.cn/gtzbtposxd.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtchafttem.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtxjzjlzom.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtgnxlpfyb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gtxbrgdxml.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtfhoqccuk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtpuqhnkbm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtmvimvefv.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtarukrxax.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydjk.org.cn/gtcxralqyl.html

C#:   list.Sum();  list.Average()
来源：http://hz.hywenlv.cn/gtujirroma.html

[D17] 最大值与最小值
来源：http://hz.bjfxy.top/gtgsuorpfi.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtspaxffgn.html


<!-- 参考信息 -->