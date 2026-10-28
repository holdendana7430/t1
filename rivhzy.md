代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.snrcjt.cn/gtlnukfxtg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtpybabjcr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gtohvsrbvm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shuidangran.top/gtghnfbdge.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtubqrbqqb.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gthghntjtk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gtxvfiqrbl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xingfuxueyuan.xyz/gtjforibrm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.birdmap.top/gtgipsqsek.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtqiqwanuo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gttosefryh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gogol.net.cn/gtdyksqieo.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhaomingkeji.xyz/gtbzxbaqrb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daria6918.cn/gtfsnikaiu.html

[C08] 闭包
来源：http://hz.yangfankeji.com/gtupcfklos.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinyuanbaomall.cn/gtbpgixidt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gtuqkiaqie.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtadgxihoq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtwncghhuc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gtrkdhyhby.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.andypj.xyz/gthegfhkbm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhijiandao.cn/gtapikifly.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtrsdzzrgv.html

[C09] 递归
来源：http://hz.wangdashe.top/gtzmxwebhu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258888.top/gtozsdwimr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guannengcc.top/gtrabvthgj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtrumcnfuv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtkzsotzil.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aibaodan.cn/gtgnlqkvaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxinkj.top/gtcurnrkew.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.havefunace.top/gtalzujfpa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtkgxxoigo.html

[C10] 变量作用域
来源：http://hz.ivvv.top/gtnlccyomh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dianchejie.cn/gtuuilsksl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.mhx1999.top/gtrbbbejbs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtqhjaporu.html

TS:   同 JS
来源：http://hz.ivvv.top/gteqrzmvut.html

Java: 方法内为块级作用域
来源：http://hz.sufxvd.cn/gtlcyvxjxa.html

Go:   花括号块级作用域
来源：http://hz.yuxming.cn/gtidnynjxp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yongpay.top/gtasstyrfc.html

C#:   块级作用域
来源：http://hz.cqqwz.cn/gtjxqihcir.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtxvdxzcwu.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gtgeafasen.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shangyingyoupin.top/gtnagwuewn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ivvv.top/gtklvpkqgb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxinkj.top/gtilgkqdnl.html

Java: import java.util.List;
来源：http://hz.cucudq.cn/gtnzkdfiti.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtwiecxilk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtwmvfofrs.html

C#:   using System.Text;
来源：http://hz.dianchejie.cn/gtcxfokzxf.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtrwcwxecu.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gtytmvzast.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtgvilhvor.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtgemlrgqr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtexnbivfn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hammf.cn/gtsjxjshud.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtjuufzagz.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gttnjumdmo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtjnlakjbf.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhengqikj.top/gtvbipphnk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenjidiqi.icu/gtbgexlhpk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtueublyfs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtcqtxudyw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtvwqfoyyp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtuwwzbfwh.html

Go:   func add(a, b int) int
来源：http://hz.redwolf501.top/gtucrgqzsw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yanxiufei.cn/gtwdvgbash.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gtrcmuxpai.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gtgpxvlltk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gtvrzwqaki.html

PHP:  // 无泛型
来源：http://hz.zdqjudy.top/gtqsrxsbvu.html

JS:   // 无泛型
来源：http://hz.sysykeji.top/gtqkhrwdgw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cdnleiting.top/gthlsqfwwd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sxryk.cn/gtcsxyejfw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gtdccwcqob.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtujnnvewl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.iojbl.cn/gtjtasohql.html

[C15] 解构 / 展开参数
来源：http://hz.cheryme.top/gtjellvbxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gtiviximzi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.svipenyu.cn/gtsixoyxzb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtwnfqsnnd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.andypj.xyz/gtrqhjdvxg.html

Java: // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtkcwdmriq.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtzbtsmnid.html

Ruby: a, b = pair
来源：http://hz.yj202588.top/gtlugoigop.html

C#:   var (a, b) = pair;
来源：http://hz.chenlongwang.top/gtzqdlcqxi.html

[C16] 函数 / 方法重载
来源：http://hz.hfpthk.cn/gtdsixqrfc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gtctqakxwj.html

PHP:  // 无重载
来源：http://hz.zdqjudy.top/gtnxvgipfx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtvakhnduy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtjimonhmq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydjk.org.cn/gtxutqonxk.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtvwxkhvid.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuetiantiany.cn/gtngnzvzyb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shuidangran.top/gtugyjjdzc.html

================================================================================
来源：http://hz.yj202588.top/gtztgaszoc.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtiqitjjps.html

================================================================================
来源：http://hz.jyoumei.cn/gtmxydtcnr.html

[D01] 创建数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtbeeivssb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gzhubu.top/gtipjrbwaq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhijiandao.cn/gtfsxlovjg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xziqi.cn/gthzernqvs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtkrggnivu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gzhubu.top/gtcvijdtgk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ehwqpu.com/gtjevimjoy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gaohongyu789.top/gtcohvswcd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yanxiufei.cn/gtbdibqflp.html

[D02] 追加元素到末尾
来源：http://hz.meibo888.top/gtvhfkictt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinyuanbaomall.cn/gtqlhmaosv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xziqi.cn/gtptmexqde.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtqsgmucdo.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtyfaijseu.html

Java: list.add(4);
来源：http://hz.gzhubu.top/gtkfdokjsj.html

Go:   arr = append(arr, 4)
来源：http://hz.gotoacloud.top/gtbzjfnxbm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydzc1.top/gticnavzho.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gtavniuhhr.html

[D03] 在指定位置插入元素
来源：http://hz.yvedp.cn/gtcyrxuvwc.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtltvnjdlz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtjlwymwfa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258888.top/gtfymfvsku.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtufhqonaz.html

Java: list.add(0, 0);
来源：http://hz.hywenlv.cn/gtoziymfvf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtyulxysfr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtvshcqeka.html

C#:   list.Insert(0, 0);
来源：http://hz.gogol.net.cn/gtocrcicxq.html

[D04] 删除元素
来源：http://hz.gotoacloud.top/gtonknxdkq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtfapdapxn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gthfenjyim.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydzc1.top/gtvvoapngi.html

TS:   arr.splice(0, 1);
来源：http://hz.dianchejie.cn/gteqomvvhi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtbefxrnor.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhaomingkeji.xyz/gtnourbvyn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gttqegydfz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gthpjyyftg.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtloceqolc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtbuxwbnkk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuanzx.com/gtpvccwodj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtnkgmvcgw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhixingplan.top/gtolirmmac.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jiagoushi.top/gtllnjkznc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtiunoohwu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtpwzryzut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gtqifriudl.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtqxlciokn.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtmbhnelyd.html

PHP:  count($arr);
来源：http://hz.guannengcc.top/gtghrnedrr.html

JS:   arr.length
来源：http://hz.sysykeji.top/gtmvflxrnz.html

TS:   arr.length
来源：http://hz.smart0.xyz/gtdsiwtdiq.html

Java: list.size();
来源：http://hz.zdqjudy.top/gttckihpwl.html

Go:   len(arr)
来源：http://hz.havefunace.top/gthevybvxy.html

Ruby: arr.length; arr.size
来源：http://hz.jianghu66.top/gtrnekiadb.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gtivwxjgci.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gtikzqvcmf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tian-w.cn/gtjzvbltjx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhixingplan.top/gtjiwimsox.html

JS:   arr.slice(1, 4);
来源：http://hz.daxiang520.top/gtswgsqhbn.html

TS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtxmljkuue.html

Java: list.subList(1, 4);
来源：http://hz.bjfxy.top/gtnxioogvx.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtgkihbibt.html

Ruby: arr[1, 3]
来源：http://hz.cdnleiting.top/gtuoryinhg.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtahyygawy.html

[D08] 合并两个数组
来源：http://hz.yj20258888.top/gtwmackjyb.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtongyxojz.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtglkkceuu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtdcoxjixe.html

TS:   [...a, ...b];
来源：http://hz.yvedp.cn/gtnvjxijea.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtxvqfyryy.html

Go:   append(a, b...)
来源：http://hz.yj20258888.top/gtkhblhmpi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangkeji.top/gteublfgtm.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhixingplan.top/gtzfluubji.html

[D09] 排序（升序）
来源：http://hz.xylfe.cn/gtczfreljr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gthkrkvqwm.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtvwcsxfit.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gzhubu.top/gtdrvevacp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenzaomai.com/gtdlxxfbsx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtswlxcrln.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xziqi.cn/gttwcdtsuq.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtbodedzte.html

C#:   list.Sort();
来源：http://hz.zhijiandao.cn/gtmgsdjnqh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gthycniobr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhixingplan.top/gtjzowmiyg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dashuyun.cn/gtcnrvzbvd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtlpxzrodv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtwhaazwtg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xinyue.icu/gtgcwydbkm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtijrcvyeq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigfzy.top/gtiosejjfw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtixotxokc.html

[D11] 反转数组
来源：http://hz.hywenlv.cn/gtudgepcgk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhongyouzk.top/gtqjduwdhe.html

PHP:  array_reverse($arr);
来源：http://hz.birdmap.top/gtvloygcvf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.quarkkingdee.top/gtelcamlwe.html

TS:   [...arr].reverse();
来源：http://hz.xziqi.cn/gtyhuxurtt.html

Java: Collections.reverse(list);
来源：http://hz.aibaodan.cn/gtjmwnvdqe.html

Go:   slices.Reverse(arr)
来源：http://hz.vqdsnc.cn/gtfzkgumpy.html

Ruby: arr.reverse
来源：http://hz.cqqwz.cn/gtdfjbjwqn.html

C#:   list.Reverse();
来源：http://hz.pycfn.com/gtdlzkilwd.html

[D12] 查找元素下标
来源：http://hz.chenzaomai.com/gtgqozacsr.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtojdcjzlo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cucudq.cn/gtdozkerss.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtqqgzmkgp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtvxgpnvbt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinyuanbaomall.cn/gtfojtgxwx.html

Go:   slices.Index(arr, x)
来源：http://hz.quarkkingdee.top/gtqtsrgfpv.html

Ruby: arr.index(x)
来源：http://hz.cashguo.top/gtgniybqjf.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gttvezamke.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinghuilouyu.cn/gttxczlfdo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jianghu66.top/gtewepkuxc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtcayecutq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtsujzmkmz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gthggcwqqu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gtxfwzbvax.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtbsyaowjs.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xziqi.cn/gtnshekpnw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ehwqpu.com/gtrkscwmgy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pengpengdd.cyou/gtjiwbtftq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xinyue.icu/gtygsitsmd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhijiandao.cn/gttahxlwjf.html

JS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtjrmatahv.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtuoymicqd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.quarkkingdee.top/gtcyckobqn.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtjxnzvlcf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtvexwaexb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.0kj1m.cn/gtrgiwbzdk.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtscnxssay.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtwbnhjley.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtlkubgxuu.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtelilxmnl.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtewhplkor.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gtfnrymwyk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxuanxn.top/gtkdxhsutv.html

Ruby: arr.uniq
来源：http://hz.chenjidiqi.icu/gtlnpwymzt.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtpjbnrigv.html

[D16] 求和与平均值
来源：http://hz.yuanzhike.top/gtkmbqewis.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhixingplan.top/gthznvvpbc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ybcxt.top/gtrutrkcpx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtzzadkxvb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtyhfcpswh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhixingplan.top/gtyzwatxzc.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtlmhibqfy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxinkj.top/gtbiyqecgs.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtohccdpms.html

[D17] 最大值与最小值
来源：http://hz.c1oappe.top/gtobivmhwp.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gtimdyhghf.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnxiangtu.top/gtjobrlown.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhixingplan.top/gtmwlhvcqh.html

TS:   Math.max(...arr);
来源：http://hz.9152youxi.cn/gtnqnlioal.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtgmqlgeji.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gtbcnffwwt.html

Ruby: arr.max;  arr.min
来源：http://hz.meibo888.top/gtyzhdjkhy.html

C#:   list.Max();  list.Min()
来源：http://hz.dianchejie.cn/gtlafwwoeu.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtissugjro.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.9152youxi.cn/gtchrsqtkx.html

PHP:  array_merge(...$nested);
来源：http://hz.yanxiufei.cn/gtflovdmck.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtmmtkbcau.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtdlnteyih.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ppjwa.cn/gtmmozcjem.html

Go:   // 手写双层循环
来源：http://hz.zhijiandao.cn/gthqisvafv.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gthqzxalvm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtznmafhtq.html

[D19] 按字段分组
来源：http://hz.jianghu66.top/gtbisurmuv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gtsvgdhvfx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtbtkbwbjp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuetiantiany.cn/gtmdcqweps.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gtjwcyrpjo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nwbrower.top/gtdmlkidpr.html

Go:   // 手写 map[string][]T
来源：http://hz.xziqi.cn/gthdklqmqm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.smart0.xyz/gtbbtewhdd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jianghu66.top/gtihaewmah.html

[D20] 统计每个元素出现次数
来源：http://hz.jiagoushi.top/gtdtwwowtg.html

Py:   Counter(arr)
来源：http://hz.sufxvd.cn/gtkvvekuto.html

PHP:  array_count_values($arr);
来源：http://hz.hammf.cn/gtuukrsacy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtjycjlvqn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtyvysxudo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.mhx1999.top/gtavouxjsa.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtcaghbgna.html

Ruby: arr.tally
来源：http://hz.jinghuilouyu.cn/gtjghuespj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dashuyun.cn/gttwsmxirn.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gtfitntigp.html

Py:   x in arr
来源：http://hz.yj20258.top/gtnnkksojm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhengqikj.top/gtalysdmac.html

JS:   arr.includes(x)
来源：http://hz.tanke756.top/gtaorjqubk.html

TS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtqikadgqs.html

Java: list.contains(x)
来源：http://hz.tanke756.top/gtcbdrxmpl.html

Go:   slices.Contains(arr, x)
来源：http://hz.yueranfly.top/gtbgnfcjxm.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gttooedmvg.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtvygagppl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangdashe.top/gtdpeldlpp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtgkjvxcik.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtrxbdkeno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.haohaochexian.top/gtakvbrmbn.html

TS:   [...arr];
来源：http://hz.ppjwa.cn/gtyhnsihqq.html

Java: new ArrayList<>(list);
来源：http://hz.daria6918.cn/gtnwilivbz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtdufemcxf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtbdfsvcxg.html

C#:   new List<int>(list);
来源：http://hz.nwbrower.top/gtyqwmmogk.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gthizvqeax.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gtbyfmcwkj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gtkunqrgir.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtazedkiik.html


<!-- 参考信息 -->