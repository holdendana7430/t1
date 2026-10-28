代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.jinghuilouyu.cn/gtmwshiyrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtrpvhvblh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtcpevrjrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtvkwztijb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtqeqewlgt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daxiang520.top/gtwiafptcd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnqzz.top/gtyduwttxl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtrntzfukq.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gtbuzbxkqe.html

Py:   def greet(name="World"): return name
来源：http://hz.cucudq.cn/gtdzlpkbva.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xinyue.icu/gtyesqtwln.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtdrytdbto.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gtjtgrngzw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhijiandao.cn/gtekmnhunp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fzhhl.top/gtykjywbfh.html

Ruby: def greet(name = "World") = name
来源：http://hz.iojbl.cn/gtwnaeivwu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhongyouzk.top/gtdnslgddr.html

[C03] 可变参数
来源：http://hz.316326.xyz/gtitstvcyc.html

Py:   def total(*args): return sum(args)
来源：http://hz.guowangkeji.top/gttlioglep.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gaohongyu789.top/gtdttvpuuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtwymwdval.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gthjultdut.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtiobaswlt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gtvovlysws.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtdbeduxne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ppjwa.cn/gtuytrsctq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.birdmap.top/gtvlxwseod.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangtech.top/gtxbqwuibm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtmrqopzhx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtdoamxozf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtzlkrlrjh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.iojbl.cn/gtnmjveyrp.html

Go:   // 无：用配置结构体参数
来源：http://hz.jlsjyb.cn/gtvuyqxilo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtdcfdterp.html

C#:   f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtqeduihqe.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtpgyewffi.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtyofltkmg.html

PHP:  return [$a, $b];
来源：http://hz.jinyuanbaomall.cn/gtekhnpita.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.0kj1m.cn/gtxoqnlfax.html

TS:   return { a, b };
来源：http://hz.xziqi.cn/gtdcwoyfox.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.52xcode.cn/gtpohqvbsw.html

Go:   return a, b
来源：http://hz.wangdashe.top/gtavugqmpq.html

Ruby: return a, b
来源：http://hz.zycfv.cn/gtdfgcofeu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yuanzhike.top/gtubekxyav.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtbegbngzd.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangtech.top/gtsuphpjhf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtemdktlki.html

JS:   const square = x => x * x;
来源：http://hz.gzhubu.top/gtgfrekora.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gthennyqcz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yuxming.cn/gtvrfkyczm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydzc1.top/gtwpiderpx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cheryme.top/gtwznkrvca.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gogol.net.cn/gtlyneflay.html

[C07] 把函数作为参数传入
来源：http://hz.yj20258.top/gtwlsczjsj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tanke756.top/gtfzjorhik.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtiagllozk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gttfdhxmey.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtxzhuexnr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinghuilouyu.cn/gtqijoarqr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtulpcfmqg.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtskrnjptb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dianchejie.cn/gtcyudynxl.html

[C08] 闭包
来源：http://hz.jinghuilouyu.cn/gtnffsmelj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.snrcjt.cn/gtmnretplc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtcrrvhakp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtutvyerxv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtqvvgoetf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xziqi.cn/gtfqfidacx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnxiangtu.top/gtlhdoyaps.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangkeji.top/gtcpcwurxw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtgralktwb.html

[C09] 递归
来源：http://hz.zdqjudy.top/gtrcohljmi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtjfyvtzxz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.52xcode.cn/gtucgxgjwm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtohxvlreh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gtuznboxrc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dianchejie.cn/gthtlbziup.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guannengcc.top/gtfvrseoiq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigufen.top/gthwsegqfv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guannengcc.top/gttxkrwxqp.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtfpzizxtj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtofuiflxm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yonumen.top/gtvavrnfjb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuanzhike.top/gtpbisnqow.html

TS:   同 JS
来源：http://hz.havefunace.top/gtlvaibens.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gtxalquumv.html

Go:   花括号块级作用域
来源：http://hz.aibaodan.cn/gtzdfizygo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jlsjyb.cn/gtfmkbpgbz.html

C#:   块级作用域
来源：http://hz.sweek.top/gtfjroeekp.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtqawhzoxm.html

Py:   from module import func
来源：http://hz.nanxuanxn.top/gtcjruqozv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ywan-chungtsiang.top/gtyrwhzngo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtnxsyjzbu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtiinlvggl.html

Java: import java.util.List;
来源：http://hz.zdqjudy.top/gtxenejamx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ehwqpu.com/gtadsuwend.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hammf.cn/gtaibyqugd.html

C#:   using System.Text;
来源：http://hz.shangyingyoupin.top/gtdxncqvhh.html

[C12] 立即执行函数 IIFE
来源：http://hz.guowangkeji.top/gtmbutncwh.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gtoptjwcwq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gogol.net.cn/gthkppxnvq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtyzecrdpx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gogol.net.cn/gtqennasho.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtnhxmqixp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgfzy.top/gtbotfiypi.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgufenzy.top/gtjfjgdibx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtsbxcxmqy.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtrxhgalkk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtfzpxqtpq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gthqqmipgr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhongyouzk.top/gtxdexbpqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtdciqrupk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtrkhmrwmh.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtmbhqpeup.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtonyudtsr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gtfxtmbgpp.html

[C14] 泛型函数
来源：http://hz.gotoacloud.top/gtfymxxmgf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ivvv.top/gtykhxgwlk.html

PHP:  // 无泛型
来源：http://hz.jinghuilouyu.cn/gtjkkyhpbt.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gtzexdmuwh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gtdjnvfzwg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtuolofnbe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtjxfshmxb.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gtgjedwbbc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtgylvwfqp.html

[C15] 解构 / 展开参数
来源：http://hz.havefunace.top/gteoalskty.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hammf.cn/gtyuftawwy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gtpdwzowkn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtuxdicohm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gtezzhbjyn.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtxijtnlmn.html

Go:   // 无解构
来源：http://hz.ppjwa.cn/gtjivrgyzk.html

Ruby: a, b = pair
来源：http://hz.nanxuanxn.top/gtnnfumxxj.html

C#:   var (a, b) = pair;
来源：http://hz.nanxinkj.top/gtjpmkudzt.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gtlhzgvtev.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtjfucrbis.html

PHP:  // 无重载
来源：http://hz.yj20258.top/gtlxaqwerh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangdashe.top/gtcpexzxxr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cucudq.cn/gtvknnlfyv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtsrogpquk.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydjk.org.cn/gtvjbckyha.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydjk.org.cn/gtnypnzfcq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gttdelfxhm.html

================================================================================
来源：http://hz.cheryme.top/gtlxqlnlkl.html

D. 数组 / 列表 / 集合
来源：http://hz.feifeiyinyue.top/gtdsexowbq.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkwyzndca.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtpvfsgynv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenzaomai.com/gtxxhckyyl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.haohaochexian.top/gtdmvudhnj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guannengcc.top/gtyizpoozb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pengpengdd.cyou/gtrtjrpgqq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtvmgzkjwl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sysykeji.top/gtzoneiusf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtzwxknsmu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtwzcgjlxp.html

[D02] 追加元素到末尾
来源：http://hz.hammf.cn/gtaxhomznf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gtokmizwgc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtpuvrfddb.html

JS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtulabtesv.html

TS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtpkrascfk.html

Java: list.add(4);
来源：http://hz.ppjwa.cn/gtjivowbhc.html

Go:   arr = append(arr, 4)
来源：http://hz.guannengcc.top/gtjtsjvmyy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenlongwang.top/gtlleyqidi.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gteopwekzx.html

[D03] 在指定位置插入元素
来源：http://hz.cucudq.cn/gtznawiwdu.html

Py:   arr.insert(0, 0)
来源：http://hz.vqdsnc.cn/gtsrhdvsat.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhaomingkeji.xyz/gtqgwcqbsr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxuanxn.top/gtbetnpmma.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gtawhfgptv.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gtuvxmfzgx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtfxbxkkju.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtktaepgpb.html

C#:   list.Insert(0, 0);
来源：http://hz.quarkkingdee.top/gtnglgrkkn.html

[D04] 删除元素
来源：http://hz.kuanghao11.cn/gtqnejnluz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tian-w.cn/gtcuphmhkq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtvnogtpwg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.0kj1m.cn/gtzblqiwzv.html

TS:   arr.splice(0, 1);
来源：http://hz.pengpengdd.cyou/gtkwpdlcrf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtikfgeahn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtfxzzqcgt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cashguo.top/gtfvseifcv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gtidyedkaq.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangtech.top/gtpzfcrypv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtvlstwdqy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtzeyfopos.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gogol.net.cn/gtahyjrsqt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigufen.top/gtnmoqwqle.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gogol.net.cn/gtqkpvjuwm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shuidangran.top/gtkmdefxan.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtjasviqow.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtljkuaxmy.html

[D06] 数组长度
来源：http://hz.zycfv.cn/gttoquiaax.html

Py:   len(arr)
来源：http://hz.fengsongda.top/gteydtdbjq.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtxxmrtukq.html

JS:   arr.length
来源：http://hz.guannengcc.top/gtgtiozidn.html

TS:   arr.length
来源：http://hz.shzxlz.cn/gtjxptjufo.html

Java: list.size();
来源：http://hz.quarkkingdee.top/gtrfehdaqf.html

Go:   len(arr)
来源：http://hz.yvedp.cn/gtgskdlhug.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtmonghadi.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gthyezuapv.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtsenodqdt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangtech.top/gtedolixce.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gthxnuodze.html

JS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtiabgikgf.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtxpiuhrku.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtgjuuaanb.html

Go:   arr[1:4]
来源：http://hz.daria6918.cn/gtggzytnyr.html

Ruby: arr[1, 3]
来源：http://hz.gaohongyu789.top/gtznkvqrcl.html

C#:   list.GetRange(1, 3);
来源：http://hz.hysaishi.cn/gtcozgggsi.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gtsbbdrkvk.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258.top/gtobvalesy.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtrpizppdd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aibaodan.cn/gtxhbgfcfa.html

TS:   [...a, ...b];
来源：http://hz.cdnleiting.top/gtbkegzzer.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.316326.xyz/gtdtyuuxwx.html

Go:   append(a, b...)
来源：http://hz.ivvv.top/gtctevspgy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtmqkswisg.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtppccrtpg.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtyizxqwaz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtnbmossvu.html

PHP:  sort($arr);
来源：http://hz.cqqwz.cn/gtigzuwwoh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtauufpsvs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtmuzpncsd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtgfoqkgsd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guannengcc.top/gtonkbrjol.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtfiodjnxv.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtcsdywvxf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtmzdkrqxm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.mhx1999.top/gtyuqgkzdy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gotoacloud.top/gtzbxkcspu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtlymkmcve.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtfilflwxu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtmcuohrax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtendtpyyv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jiagoushi.top/gtnjltnmbx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jqgfzy.top/gtupnwcvvs.html

[D11] 反转数组
来源：http://hz.vqdsnc.cn/gtvqzrffsx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fzhhl.top/gtjyqwmzny.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtyntwhfyn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtiikrjyet.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtjsiinpvi.html

Java: Collections.reverse(list);
来源：http://hz.smart0.xyz/gtscwpaxsn.html

Go:   slices.Reverse(arr)
来源：http://hz.shuidangran.top/gtsqednwhq.html

Ruby: arr.reverse
来源：http://hz.tanke756.top/gtmkhstfrx.html

C#:   list.Reverse();
来源：http://hz.xuanzx.com/gtolegrbpe.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtgxunxini.html

Py:   arr.index(x);  x in arr
来源：http://hz.shzxlz.cn/gtokcmtuda.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhengqikj.top/gtdsopospl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtyumzqroe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtanfxyzaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gtfwnjuzij.html

Go:   slices.Index(arr, x)
来源：http://hz.dianchejie.cn/gtnlodrnub.html

Ruby: arr.index(x)
来源：http://hz.316326.xyz/gtrdjckknd.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gterjzxkma.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gtupeqbajn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtsideghoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtemcxyxzy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtycdvhhxg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtybgdsfui.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgufenzy.top/gtyhilpebu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cucudq.cn/gtutuzdosu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gtrzmmfmhn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gthmgreyse.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yonumen.top/gtunxjsomn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhengqikj.top/gtbbqfastb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtlkpdcowk.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gthfqxkzxm.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtskaqllmx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtkezwpayz.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtswvssuxq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtjbtdvhgm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtjycohutr.html

[D15] 去重
来源：http://hz.cheryme.top/gtuqpoekpg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtytlsvyja.html

PHP:  array_unique($arr);
来源：http://hz.chenlongwang.top/gtmbudilij.html

JS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtkgwgmedx.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtwjsgmxtg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtqkbhmtwq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtsvfcwxdt.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtxlteglis.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtsswulsjo.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtwkzwdaja.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.haohaochexian.top/gtnwoxazlz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cucudq.cn/gtdhrxpqgf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gtjioxwstk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtwsxzsere.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yangfankeji.com/gtkgbriyhf.html

Go:   // 手写循环累加
来源：http://hz.hnxiangtu.top/gtiuofeqiz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtmlhbralx.html

C#:   list.Sum();  list.Average()
来源：http://hz.jlsjyb.cn/gtfnwcvlov.html

[D17] 最大值与最小值
来源：http://hz.jianghu66.top/gtjyzprgek.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtxvombnqv.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gtfhghfugf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yvedp.cn/gtyigercud.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtdcifauiz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.haohaochexian.top/gtnjxxbleq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cashguo.top/gtqqyaompc.html

Ruby: arr.max;  arr.min
来源：http://hz.zhixingplan.top/gttzhwvcpx.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtogkjzrbe.html

[D18] 扁平化嵌套数组
来源：http://hz.zycfv.cn/gttkzepnmi.html


<!-- 参考信息 -->