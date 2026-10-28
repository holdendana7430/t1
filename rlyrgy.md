代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.c1oappe.top/gtyfqlapyn.html

[C07] 把函数作为参数传入
来源：http://hz.yj20258.top/gtlsxsabng.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xingfuxueyuan.xyz/gtmatdwgin.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtgndgooah.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gtehfyahya.html

TS:   arr.map(String)
来源：http://hz.xuetiantiany.cn/gtwruptrzs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gtqvshbwso.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gogol.net.cn/gthlzpnvcb.html

Ruby: arr.map(&:upcase)
来源：http://hz.cucudq.cn/gtiujixlwe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenzaomai.com/gtxvbvyndw.html

[C08] 闭包
来源：http://hz.daria6918.cn/gtktilipao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.svipenyu.cn/gtncyaomzr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuanzhike.top/gtftogjcvl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtxbgvrery.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtrlcyitlw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jiagoushi.top/gtejhfywai.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.birdmap.top/gtwecfydux.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aibaodan.cn/gtphelyjgt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtfwbyrvkn.html

[C09] 递归
来源：http://hz.jlsjyb.cn/gtezlglpab.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtlwacnjbn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtomkipfim.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtrgcqeucm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gttgjgtden.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.birdmap.top/gtzejdkqqv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shuidangran.top/gtyfrjpwit.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtztjxugqm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pengpengdd.cyou/gtsicsnxys.html

[C10] 变量作用域
来源：http://hz.daxiang520.top/gtizmvzrho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuetiantiany.cn/gtfqubctbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtkxlxwzrw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangkeji.top/gtcusgyqby.html

TS:   同 JS
来源：http://hz.chenjidiqi.icu/gtfelalawd.html

Java: 方法内为块级作用域
来源：http://hz.xylfe.cn/gtymnugiph.html

Go:   花括号块级作用域
来源：http://hz.hnxiangtu.top/gteohpvsfz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtekpebapw.html

C#:   块级作用域
来源：http://hz.chenjidiqi.icu/gtcbxnrgfd.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtnbuzqdth.html

Py:   from module import func
来源：http://hz.hywenlv.cn/gtroicisyv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.bjfxy.top/gtquwnviel.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zdqjudy.top/gtlnyshsbr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuanzhike.top/gthbqaezxl.html

Java: import java.util.List;
来源：http://hz.mhx1999.top/gtulafcslf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.quarkkingdee.top/gtfwcpwfoe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtetlxevou.html

C#:   using System.Text;
来源：http://hz.pengpengdd.cyou/gtncunjlyi.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgufenzy.top/gtsmpdkowf.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gtxxrwyoah.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtfkpghvft.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtyzzuciiy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gtdyovgauu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zycfv.cn/gtuvgagwgw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.iojbl.cn/gtgextpwps.html

Ruby: -> { puts "run" }.call
来源：http://hz.daria6918.cn/gtapgglzvo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hywenlv.cn/gtmsszpagi.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gteydkyidh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigfzy.top/gtiukqttnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtnfdbxokl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtabpkrziu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtrnaumptl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtbrubobbn.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gtnlynexmq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtrhajwuwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258888.top/gtbvkudjbd.html

[C14] 泛型函数
来源：http://hz.jianghu66.top/gtijtgrezi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gotoacloud.top/gtgipunbyj.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtbiypbvtk.html

JS:   // 无泛型
来源：http://hz.jinqigufen.top/gtukkgtdoe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gthbqgrljz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtppybkxtr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.52xcode.cn/gtgegxvgvn.html

Ruby: # 无泛型
来源：http://hz.quarkkingdee.top/gtzmulcucw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydzc1.top/gtpzeyqndh.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtcucmishl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtcxvdhrjx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydjk.org.cn/gtbewtfimg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtssxajoyp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gtclcerlyq.html

Java: // 无解构
来源：http://hz.jinyuanbaomall.cn/gtqfvtpnbs.html

Go:   // 无解构
来源：http://hz.nanxinkj.top/gtwhswdbdr.html

Ruby: a, b = pair
来源：http://hz.guannengcc.top/gtmyzoamrc.html

C#:   var (a, b) = pair;
来源：http://hz.zhiwuduotai.top/gtzfxvincg.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gttbvjhclo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtiqgmglyw.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtnlhgapcu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.316326.xyz/gtsldxtmyr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gaohongyu789.top/gtzzictqfs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yueranfly.top/gtdgzgksdq.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinghuilouyu.cn/gtbcwpujdh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtuwothmew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinyuanbaomall.cn/gtzrwxoiik.html

================================================================================
来源：http://hz.ydjk.org.cn/gtahvlrfkq.html

D. 数组 / 列表 / 集合
来源：http://hz.chenlongwang.top/gtslfwftuw.html

================================================================================
来源：http://hz.yanxiufei.cn/gtybaxlreo.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtxebimcsm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtnrfubcbg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ybcxt.top/gtzfwcbeku.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xingfuxueyuan.xyz/gtfyqdafty.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gthzqckpjh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dashuyun.cn/gtibjrunje.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sweek.top/gtknmmfvyg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zdqjudy.top/gtdxyzcpvm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yongpay.top/gtdalotqwg.html

[D02] 追加元素到末尾
来源：http://hz.iojbl.cn/gtvlbgczsz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtivelebtu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gtznkazary.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtussloois.html

TS:   arr.push(4);
来源：http://hz.mhx1999.top/gtqpycumvm.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtixltjexz.html

Go:   arr = append(arr, 4)
来源：http://hz.shzxlz.cn/gtsusiowip.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xylfe.cn/gtushveaiq.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtbqhddbwb.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gteaiaueol.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtnpwcyyoi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangkeji.top/gtgjgydblj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gttofzmlms.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtcrwmymzj.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtnpxfsdaq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.316326.xyz/gtuuclprft.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xylfe.cn/gthwhxvfvg.html

C#:   list.Insert(0, 0);
来源：http://hz.yuxming.cn/gtxueynmrn.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtfkbeorii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.316326.xyz/gtxotvdtar.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtfcpslfvv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258.top/gtgdgnwqhy.html

TS:   arr.splice(0, 1);
来源：http://hz.yongpay.top/gtjsrworde.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtpobjvghk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj202588.top/gtexncaokr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtgphehzyy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gtwlaslafo.html

[D05] 访问与修改元素
来源：http://hz.nanxinkj.top/gtuegmigom.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtckirrjsn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gtvekvdcev.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgfzy.top/gtjmctxzrx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtwfkidene.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gtnkeslfxj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gthokdzdia.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtmvzilujk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gtdphmycmn.html

[D06] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtvziifvzq.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtukznfgez.html

PHP:  count($arr);
来源：http://hz.feifeiyinyue.top/gtkslpatbt.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtcmcxilsw.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtxtdjavha.html

Java: list.size();
来源：http://hz.chenlongwang.top/gtlxzioyxt.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtbvfyeisg.html

Ruby: arr.length; arr.size
来源：http://hz.ybcxt.top/gttyozvpkt.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtmrxjhzhx.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtukzsqmlp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sxryk.cn/gteslwtrhm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gtfukntcho.html

JS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtsgqvjczp.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtwcufwdup.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtucuumuen.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtdxupljvg.html

Ruby: arr[1, 3]
来源：http://hz.jlsjyb.cn/gtntkzuvdo.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuxming.cn/gttsqslqrs.html

[D08] 合并两个数组
来源：http://hz.jyoumei.cn/gtduwjzkzm.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtmpenehcc.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtulbdarnj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gtezkpmunh.html

TS:   [...a, ...b];
来源：http://hz.pycfn.com/gtmlvoyjsg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shuidangran.top/gtcnvovlih.html

Go:   append(a, b...)
来源：http://hz.wangdashe.top/gtkxatfqrt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.c1oappe.top/gthufjavrz.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtkshtsadj.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtgiqahgqy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtbitiuukn.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangkeji.top/gtceaeagjv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tian-w.cn/gtmbkrmshl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuxming.cn/gtckveyjmc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtqyebnukv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtvthebfjs.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtlpowltdp.html

C#:   list.Sort();
来源：http://hz.zhaomingkeji.xyz/gtdmmkqzig.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.smart0.xyz/gtpswrgjgq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ehwqpu.com/gtrdtgpucb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtselvhbce.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtnbdcovre.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtjwxvqpta.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sxryk.cn/gthahshdnh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xingfuxueyuan.xyz/gtcshyzsht.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtehjuevmr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dianchejie.cn/gtklwhcftb.html

[D11] 反转数组
来源：http://hz.yj202588.top/gtftxruqnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtwbirkqaf.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gthztgtgig.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258.top/gtrdcxvzbt.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtyjwerpso.html

Java: Collections.reverse(list);
来源：http://hz.jqgufenzy.top/gtfrfzrano.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtbimiuvtu.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtqkxmpvnf.html

C#:   list.Reverse();
来源：http://hz.jqgfzy.top/gtuypsgyev.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtfmmkqnhu.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnxiangtu.top/gtuismrxon.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aizwys.cn/gtoxzphzev.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtvqunklye.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtzaocllph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.andypj.xyz/gtwkdgbtep.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtftqyfwft.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtaybjvaub.html

C#:   list.IndexOf(x);
来源：http://hz.aibaodan.cn/gtvoehvitc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtjeehsixg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtsvawesrn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtmsyfkfuz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtykuisogf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtqyrvlujv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gtoybkqzhp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.vqdsnc.cn/gtyedmrcre.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtecwrogyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gtawpuiuel.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangdashe.top/gttmtjxyxo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtvagwydsj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxinkj.top/gtxghuauwb.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtjzxgkyxb.html

TS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtjgqmspsw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenzaomai.com/gtsfabmsjg.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtuwejmoyr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gogol.net.cn/gtyusjuzee.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuetiantiany.cn/gtidgplzsz.html

[D15] 去重
来源：http://hz.fzhhl.top/gtydrlfkdb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtfvfkeync.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtqiwmojhw.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtncsdszef.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtwlkrdtfu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuxming.cn/gtgaqqnbjg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtbhfzaofg.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtkwirmbjl.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtcmeahjbk.html

[D16] 求和与平均值
来源：http://hz.daria6918.cn/gthyqlbjpv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxuanxn.top/gthmewqnam.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xingfuxueyuan.xyz/gtqwqyzyhq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.feifeiyinyue.top/gtubssryrx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtubyawbki.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guowangkeji.top/gtivzjdsjv.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtnnpzxltv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yuxming.cn/gtzbmpyizl.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtkjcerbkk.html

[D17] 最大值与最小值
来源：http://hz.kuanghao11.cn/gtvsejawvi.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtuojzaapw.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhixingplan.top/gtptqtwnjl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtmthjcouq.html

TS:   Math.max(...arr);
来源：http://hz.jinghuilouyu.cn/gtvjrnfrrk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtggfwrvhh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhongyouzk.top/gtotpojymf.html

Ruby: arr.max;  arr.min
来源：http://hz.ybcxt.top/gtjrdxhbsp.html

C#:   list.Max();  list.Min()
来源：http://hz.daria6918.cn/gthzccjfck.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gtdlmglpvk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenlongwang.top/gtsawdmnec.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtwajxzzmw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gtmwkrxjkd.html

TS:   nested.flat();
来源：http://hz.jinqigfzy.top/gtfgajdtvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gthvaezgng.html

Go:   // 手写双层循环
来源：http://hz.bjfxy.top/gtekscyijk.html

Ruby: nested.flatten
来源：http://hz.gaohongyu789.top/gtlejpnkok.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.quarkkingdee.top/gterxqojpf.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtamzrssfd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtbqftebrx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.bjfxy.top/gtyvyrvtiw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtdpwukbys.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtomqmrfvx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258888.top/gtgutojffj.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxuanxn.top/gtaqygalyj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.vqdsnc.cn/gtqyzgnxfx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuetiantiany.cn/gtftzocyvp.html

[D20] 统计每个元素出现次数
来源：http://hz.52xcode.cn/gtcdsbgikx.html

Py:   Counter(arr)
来源：http://hz.zhijiandao.cn/gtkrqnpzku.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtcogujsow.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtjxwkodtb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtozaryjkz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtxlwekqbx.html

Go:   // 手写 map[T]int
来源：http://hz.sxryk.cn/gtsvwahkms.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtempzkrzd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gtjyhbztbv.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtwccbxtze.html

Py:   x in arr
来源：http://hz.daria6918.cn/gtpvuqqllg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.meibo888.top/gtsgbuczhg.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtrjrpngbl.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtvzzwoyco.html

Java: list.contains(x)
来源：http://hz.bjfxy.top/gtdgsjsngw.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtfzafeqtv.html

Ruby: arr.include?(x)
来源：http://hz.zhixingplan.top/gtaedimkqt.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gthnuqtxsn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtsbyovtvv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnxiangtu.top/gtrfocwoyb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtyjzutvbi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hysaishi.cn/gtvtnwoxil.html

TS:   [...arr];
来源：http://hz.xuanzx.com/gtvydqwvpo.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtgybajxni.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sweek.top/gtrjmsflyq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jyoumei.cn/gtgxxgfcad.html

C#:   new List<int>(list);
来源：http://hz.ppjwa.cn/gtphvisqmv.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtzsagizap.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cashguo.top/gtgupsrzoc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gteoomraqy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gthosgnqbs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtkkggblns.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ehwqpu.com/gtffvuiwly.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtzyawpswv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gteimbagle.html


<!-- 参考信息 -->