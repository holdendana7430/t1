代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gteomkqbly.html

Py:   square = lambda x: x * x
来源：http://hz.pengpengdd.cyou/gtpcmrolxq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gtmkiypnep.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtgskchons.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.svipenyu.cn/gtbxdnbvao.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shuidangran.top/gtpfffpqed.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hfpthk.cn/gthnguayoy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhaomingkeji.xyz/gtwvhwrgsu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxinkj.top/gttgvurmnb.html

[C07] 把函数作为参数传入
来源：http://hz.snrcjt.cn/gtwjafklye.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hongshengwenyu.top/gtdbeehhpe.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtpqasxldl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tianlin.xyz/gtasubepnu.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtzzbjqxzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.316326.xyz/gtcbcnpnfy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ehwqpu.com/gtxpmialqs.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnxiangtu.top/gtgecdgsoz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cheryme.top/gtofqojhhk.html

[C08] 闭包
来源：http://hz.feifeiyinyue.top/gthhpfvljb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnxiangtu.top/gtfryxjvex.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinyuanbaomall.cn/gtcebrhgfw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtnrqdyrpk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gthdoczkqx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yongpay.top/gtuqnreisp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtzflljazo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pycfn.com/gtmmxumxpj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gticldoatk.html

[C09] 递归
来源：http://hz.ywan-chungtsiang.top/gtdqmsiojn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yueranfly.top/gtoasqfgjx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fzhhl.top/gttrknctjm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtzabrvuln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtducuteau.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yanxiufei.cn/gtxxeqwzqt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shanyushiyangkeji.top/gtysnmmvba.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nwbrower.top/gtddzedgcd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtaktlnmxz.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtyfxnqqvs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cqqwz.cn/gtsvntgcnt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gtxmlraafy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gtjkpswcvw.html

TS:   同 JS
来源：http://hz.sweek.top/gtrnjxlitv.html

Java: 方法内为块级作用域
来源：http://hz.dianchejie.cn/gtfgyjzlbk.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtjccolygz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daria6918.cn/gtficaqnvj.html

C#:   块级作用域
来源：http://hz.zhengqikj.top/gtvvstjfjf.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtptnsxncq.html

Py:   from module import func
来源：http://hz.gzhubu.top/gtltfnunnz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gtqtuucqjx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtjmzegpwm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.wangdashe.top/gtxdqunkky.html

Java: import java.util.List;
来源：http://hz.zhoulong.xyz/gthyyekfbs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gtzqnobpnd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtjmiycxhw.html

C#:   using System.Text;
来源：http://hz.tianlin.xyz/gtltqxqnlx.html

[C12] 立即执行函数 IIFE
来源：http://hz.cqqwz.cn/gtucmkyumh.html

Py:   (lambda: print("run"))()
来源：http://hz.xingfuxueyuan.xyz/gtjkvlsabq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gtczobyrxr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtdillcxaj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtsvsrywrg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gtpftbpjsf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shuidangran.top/gthgrdprhp.html

Ruby: -> { puts "run" }.call
来源：http://hz.ivvv.top/gtfsvvflle.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinyuanbaomall.cn/gtzqrniohy.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxuanxn.top/gtxvjmajbd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtvpcbdtzy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtxqshgdab.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtrvemjhez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtpxgufuza.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtmnamkmtu.html

Go:   func add(a, b int) int
来源：http://hz.yj202588.top/gtiwqrywbc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gttoivuwrg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gtskbuircs.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gteumilbxg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hywenlv.cn/gtbwbxqclz.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtsozxhjmf.html

JS:   // 无泛型
来源：http://hz.0kj1m.cn/gtnxehrzds.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtnbptrgrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gtrjlvxsnn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuxming.cn/gtywwfyeja.html

Ruby: # 无泛型
来源：http://hz.aizwys.cn/gtmkhzaxgv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.bjfxy.top/gtbiefbsyx.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtfdwxgwls.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daria6918.cn/gtocvuobts.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydzc1.top/gtniywfayf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtrqnznhjc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.quarkkingdee.top/gtzqtvfsfa.html

Java: // 无解构
来源：http://hz.jinghuilouyu.cn/gtxvtgrpfr.html

Go:   // 无解构
来源：http://hz.aizwys.cn/gtzpndoxdp.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtkqisptqa.html

C#:   var (a, b) = pair;
来源：http://hz.cucudq.cn/gtrjnzqind.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtgvyheqdz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.9152youxi.cn/gtsbyrmlrt.html

PHP:  // 无重载
来源：http://hz.gogol.net.cn/gtublpyklr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sufxvd.cn/gtllpadivu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtzpgfjjbl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtdlgaexzx.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtakkkjaut.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgufenzy.top/gtunkwxzek.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.haohaochexian.top/gtdelpljqe.html

================================================================================
来源：http://hz.jqgfzy.top/gtxjikkbim.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gtusmrucvi.html

================================================================================
来源：http://hz.yuxming.cn/gtudrkgajq.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gthawcxzdx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hongshengwenyu.top/gthobrbbcn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.snrcjt.cn/gtnaakhgen.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuanzx.com/gtmjomhaxt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xylfe.cn/gtlqnqrree.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gthuljwwmk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.52xcode.cn/gtauwflsoj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtwkghqxsa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtixmwahgr.html

[D02] 追加元素到末尾
来源：http://hz.jiagoushi.top/gtbwmqtfnb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtfyfkzqau.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.52xcode.cn/gtceiwjguz.html

JS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtlcuwpbpm.html

TS:   arr.push(4);
来源：http://hz.hammf.cn/gtlxvvbrii.html

Java: list.add(4);
来源：http://hz.tanke756.top/gthkitbfhc.html

Go:   arr = append(arr, 4)
来源：http://hz.xuetiantiany.cn/gtvxousbeu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dashuyun.cn/gtakqvwmjv.html

C#:   list.Add(4);
来源：http://hz.jinqigfzy.top/gtnuuvfqkv.html

[D03] 在指定位置插入元素
来源：http://hz.fengsongda.top/gtqwlenmak.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtyanexmac.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.iojbl.cn/gtpovlotsc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtwtskjaoq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gttgcxpwbl.html

Java: list.add(0, 0);
来源：http://hz.jiagoushi.top/gtmgjhpfqm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tian-w.cn/gtkquhqlyz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangtech.top/gtsizwvgqh.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gttigjdaor.html

[D04] 删除元素
来源：http://hz.havefunace.top/gtdhehlnmt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.redwolf501.top/gtqhbpjxnw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtfghkckhy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.0kj1m.cn/gtjrrmduny.html

TS:   arr.splice(0, 1);
来源：http://hz.c1oappe.top/gtyfnloldg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gtmqwpzwyg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daxiang520.top/gthgxjopfc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gtyowpjgni.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sysykeji.top/gtjlvqzfyn.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtpovustqs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gthdskvafu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtdyffidil.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtcwxpsheq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtdsbiipdz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gttmqsyifu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gttuukgbhi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtxtealqgm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hysaishi.cn/gtfuiqqljq.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gtcjazdric.html

Py:   len(arr)
来源：http://hz.tian-w.cn/gtuthbwclr.html

PHP:  count($arr);
来源：http://hz.zycfv.cn/gtcpsmbzda.html

JS:   arr.length
来源：http://hz.cheryme.top/gtslsarfih.html

TS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtsfclglaq.html

Java: list.size();
来源：http://hz.chenzaomai.com/gtxgubgxqq.html

Go:   len(arr)
来源：http://hz.guowangkeji.top/gtwdnoqdeu.html

Ruby: arr.length; arr.size
来源：http://hz.nanxinkj.top/gtdsjksbbn.html

C#:   list.Count;
来源：http://hz.zhixingplan.top/gtxqaefmjq.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gtuhwouudf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtbvkwxjrh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnxiangtu.top/gtxhrojrkm.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtyrfxhbac.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtsbjrelby.html

Java: list.subList(1, 4);
来源：http://hz.feifeiyinyue.top/gtcvfqlwzu.html

Go:   arr[1:4]
来源：http://hz.kuanghao11.cn/gtuupvpdek.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtiiyzbpxg.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gtelotjrna.html

[D08] 合并两个数组
来源：http://hz.zhengqikj.top/gtmoqxfxgb.html

Py:   a + b;  a.extend(b)
来源：http://hz.52xcode.cn/gttghxmiqg.html

PHP:  array_merge($a, $b);
来源：http://hz.havefunace.top/gtxfooqrsd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gotoacloud.top/gtabjqrilh.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtahqgzlrc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.52xcode.cn/gtsfuxqhle.html

Go:   append(a, b...)
来源：http://hz.nanxinkj.top/gtwuzkboda.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtnxxvdyef.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtdrtvgpyv.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtykpcducq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtnirgcsxh.html

PHP:  sort($arr);
来源：http://hz.yonumen.top/gtbegeggpj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtgpaqiwsu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gteacxpewg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtjwxvcpjk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuanzx.com/gtnholwszy.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtttwmixta.html

C#:   list.Sort();
来源：http://hz.9152youxi.cn/gtttebpsjv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fengsongda.top/gtndcxwffl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtfpgmtylp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtaogyjfap.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtnzbveanz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtwgcsaase.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtebmqagcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jyoumei.cn/gtrmpupnpi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gtjstafpqg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtbpaccxfh.html

[D11] 反转数组
来源：http://hz.zhongyouzk.top/gtmskdhife.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtexlwfdue.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gttoffrjnt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gtxkzddnmz.html

TS:   [...arr].reverse();
来源：http://hz.gaohongyu789.top/gtmayfzclf.html

Java: Collections.reverse(list);
来源：http://hz.hywenlv.cn/gtgxlbrqnu.html

Go:   slices.Reverse(arr)
来源：http://hz.havefunace.top/gtgyrffvpq.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtegoympgn.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtcckkphez.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtbmosndfy.html

Py:   arr.index(x);  x in arr
来源：http://hz.52xcode.cn/gtctaaqogn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hfpthk.cn/gtkuouueox.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtjgtikopg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtylxtpyqw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shangyingyoupin.top/gtrjnlvhwy.html

Go:   slices.Index(arr, x)
来源：http://hz.gzhubu.top/gtnozbqzju.html

Ruby: arr.index(x)
来源：http://hz.meibo888.top/gtsurcajyf.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gtowsyucem.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gtriqgdnhi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangtech.top/gtyuxfkans.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtclbgysun.html

JS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtmkpqxmgt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtcqgothdz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tian-w.cn/gtsettsdse.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shuidangran.top/gttwabmyqz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.birdmap.top/gtduhdeqqa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtflofzphn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zycfv.cn/gtxxzvyrrn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtmkhofjnu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtsauxpdxo.html

JS:   arr.map(x => x * 2)
来源：http://hz.xuetiantiany.cn/gtxyxnfmyg.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtkhmfjqqa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gtiwkywupa.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtsjdqrwae.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sweek.top/gtzsfjfhnc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtuscjecgr.html

[D15] 去重
来源：http://hz.yj202588.top/gtlrmxntkf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtcvguwktf.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtfuybiibh.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gteuhqhiuc.html

TS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtnfrnjnhv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cheryme.top/gtkqedmpju.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtovoaddeu.html

Ruby: arr.uniq
来源：http://hz.tian-w.cn/gtpacicpzb.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtmuyotkye.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtxdkgfjgu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ivvv.top/gtwdjyrybp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtuhtictfr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtrzckezzr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtvrwtwnms.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtzqhcqnhh.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangtech.top/gtkzpcpsce.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gaohongyu789.top/gtogxsndzm.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtqsmfmpnj.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtbltopnmi.html

Py:   max(arr);  min(arr)
来源：http://hz.zhongyouzk.top/gtmzgrxlka.html

PHP:  max($arr);  min($arr);
来源：http://hz.havefunace.top/gtlefbdujs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.feifeiyinyue.top/gtczxrjbht.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtrppqoljt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenlongwang.top/gtlhpxwoya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sufxvd.cn/gthugatmet.html

Ruby: arr.max;  arr.min
来源：http://hz.gaohongyu789.top/gtptyymwsc.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtklhzuowh.html

[D18] 扁平化嵌套数组
来源：http://hz.feifeiyinyue.top/gtwkaidsjs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.0kj1m.cn/gtwvvborsx.html

PHP:  array_merge(...$nested);
来源：http://hz.aibaodan.cn/gtiireqnsm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtmqttqiuo.html

TS:   nested.flat();
来源：http://hz.hammf.cn/gtellpaeft.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258.top/gtrssbkazn.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtgmsonnwn.html

Ruby: nested.flatten
来源：http://hz.cheryme.top/gtvqmproxr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daria6918.cn/gtyfqolifw.html

[D19] 按字段分组
来源：http://hz.chenjidiqi.icu/gtbqzlkhac.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtbksqayci.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258888.top/gtieqydzyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.mhx1999.top/gtbypmnnoq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtqxihipqm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtukhuqics.html

Go:   // 手写 map[string][]T
来源：http://hz.gaohongyu789.top/gtgkelvobt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jiagoushi.top/gtyyoqnxgp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtyjgdbhjr.html

[D20] 统计每个元素出现次数
来源：http://hz.yangfankeji.com/gtqsdirmkp.html

Py:   Counter(arr)
来源：http://hz.ybcxt.top/gtmaraanag.html

PHP:  array_count_values($arr);
来源：http://hz.quarkkingdee.top/gtaowymhra.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtrvoahokf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtyisymuzp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.havefunace.top/gtksqdlpto.html

Go:   // 手写 map[T]int
来源：http://hz.havefunace.top/gtlgrroryy.html

Ruby: arr.tally
来源：http://hz.gaohongyu789.top/gtjfolqtyj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hywenlv.cn/gtbmqjgmov.html

[D21] 判断是否包含某元素
来源：http://hz.zdqjudy.top/gtbtbccgzl.html

Py:   x in arr
来源：http://hz.tianlin.xyz/gtsnyrtlep.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hywenlv.cn/gtxqbdmbbj.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtsqmsyyfv.html

TS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtyqpinsfa.html

Java: list.contains(x)
来源：http://hz.52xcode.cn/gtaulwaygy.html

Go:   slices.Contains(arr, x)
来源：http://hz.cheryme.top/gtjkkwvosx.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtfqpixzet.html

C#:   list.Contains(x)
来源：http://hz.hammf.cn/gtlthubmqn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shuidangran.top/gtuubnhduy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtssibjzlo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangshuangyany.cn/gtilsubhsw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cqqwz.cn/gttrymexhg.html

TS:   [...arr];
来源：http://hz.fzhhl.top/gtknnbfjto.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangkeji.top/gtbvdmsrdp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gtulydhktw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtucbgmcxv.html

C#:   new List<int>(list);
来源：http://hz.nwbrower.top/gtiubxdagn.html


<!-- 参考信息 -->