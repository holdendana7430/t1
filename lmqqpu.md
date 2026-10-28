代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtnpivnuca.html

[C07] 把函数作为参数传入
来源：http://hz.pengpengdd.cyou/gtwcznukwd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gzhubu.top/gtvtgncykn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hywenlv.cn/gtdlantjxn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ppjwa.cn/gthwgizdat.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtjmawyjer.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj202588.top/gtpycjylji.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgufenzy.top/gtcegmmnjf.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinqigufen.top/gttnimyyoc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xziqi.cn/gtqwdnunsw.html

[C08] 闭包
来源：http://hz.316326.xyz/gtximbndlw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtxdkatfmt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sufxvd.cn/gtwzupskrm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtzdcwdpjj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtpbayjtdm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtzhadkqyg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj202588.top/gtxbloyibt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ivvv.top/gtvrculzcp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtmlffosmr.html

[C09] 递归
来源：http://hz.bjfxy.top/gtbuwhvafk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtznzcvnol.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.kuanghao11.cn/gtfkrtgjeb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtejvhsuvi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtyvuvzadn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhoulong.xyz/gtqkufzyjz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.andypj.xyz/gthdyyzzmi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yueranfly.top/gtketuytdt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.birdmap.top/gtdcjthtvi.html

[C10] 变量作用域
来源：http://hz.zhixingplan.top/gtytksyusf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydjk.org.cn/gtxgbaujck.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.quarkkingdee.top/gttiyusrbe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtlqpnpqno.html

TS:   同 JS
来源：http://hz.nanxinkj.top/gtjmwqhnmq.html

Java: 方法内为块级作用域
来源：http://hz.jqgufenzy.top/gtutplvvxt.html

Go:   花括号块级作用域
来源：http://hz.0kj1m.cn/gtunrghfvf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258888.top/gttymtqddu.html

C#:   块级作用域
来源：http://hz.gaohongyu789.top/gtyvvwndur.html

[C11] 模块导入与导出
来源：http://hz.sweek.top/gtymcspecz.html

Py:   from module import func
来源：http://hz.cqqwz.cn/gtjzsqzvsk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dianchejie.cn/gtqkyjhoeo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yanxiufei.cn/gtntkoqaai.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ppjwa.cn/gtlhaugpuc.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gtdedqysgs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgfzy.top/gttxrrvoot.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhiwuduotai.top/gtqawcypwh.html

C#:   using System.Text;
来源：http://hz.andypj.xyz/gttpakucwn.html

[C12] 立即执行函数 IIFE
来源：http://hz.tian-w.cn/gtowuketoe.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigufen.top/gtujxzzjeu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fzhhl.top/gtjlqspyll.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtkeqhybyi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtcplixnne.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenjidiqi.icu/gtvmwynbtz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuetiantiany.cn/gtlwerlavl.html

Ruby: -> { puts "run" }.call
来源：http://hz.ehwqpu.com/gtqtzsikki.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.dianchejie.cn/gtrkpdbxmz.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtiqqdrgie.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgufenzy.top/gtjemkeqmc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtvscrfmsm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtcpmordip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtxffxqvzs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtruslhxqv.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangkeji.top/gtrdqnyztf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtcvuymxaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sxryk.cn/gtycdatwbn.html

[C14] 泛型函数
来源：http://hz.316326.xyz/gtmefgjyef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj202588.top/gtpgvmxxca.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gtwmmgqjcf.html

JS:   // 无泛型
来源：http://hz.sxryk.cn/gtrjojmgok.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtxkyewluw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hfpthk.cn/gtyngdqjso.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.birdmap.top/gtqavboqwt.html

Ruby: # 无泛型
来源：http://hz.daxiang520.top/gtaufyawmd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.52xcode.cn/gtphkznqhq.html

[C15] 解构 / 展开参数
来源：http://hz.ehwqpu.com/gtiaqzpydd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gttkcdktyo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtdaunkjyk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cdnleiting.top/gtfclzfhgh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xziqi.cn/gtrzztuqbm.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gtfdjgilvh.html

Go:   // 无解构
来源：http://hz.kuanghao11.cn/gtdfxbiqpk.html

Ruby: a, b = pair
来源：http://hz.pengpengdd.cyou/gteqisfuay.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtrolyhrhu.html

[C16] 函数 / 方法重载
来源：http://hz.ywan-chungtsiang.top/gtjizneigx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cqqwz.cn/gtmtinddgq.html

PHP:  // 无重载
来源：http://hz.chenjidiqi.icu/gtnsegogyl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.snrcjt.cn/gtmokphbmc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgufenzy.top/gtgdjxujhb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gtxscldvuc.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtmneryxpr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.redwolf501.top/gtvnnflhcn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shzxlz.cn/gtbszkxaeq.html

================================================================================
来源：http://hz.guannengcc.top/gtbnqyduau.html

D. 数组 / 列表 / 集合
来源：http://hz.jinyuanbaomall.cn/gtkdsgytao.html

================================================================================
来源：http://hz.jiagoushi.top/gtykfpddpw.html

[D01] 创建数组 / 列表
来源：http://hz.redwolf501.top/gtpxtycmdj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhoulong.xyz/gtzbsshsui.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gtishjfodv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gtqbkmbqiy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtrlioabxt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.9152youxi.cn/gtskmfcgbu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuxming.cn/gtpdahwupw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ywan-chungtsiang.top/gtqhclwetw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydjk.org.cn/gtplepqnuf.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtyzmsrdog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gtzbihybji.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtzjdihlih.html

JS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtfrbwhpme.html

TS:   arr.push(4);
来源：http://hz.fzhhl.top/gtbxpnmukm.html

Java: list.add(4);
来源：http://hz.fengsongda.top/gtupojqibq.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gthneqikaa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jianghu66.top/gteohmloht.html

C#:   list.Add(4);
来源：http://hz.gzhubu.top/gtfwwzgsju.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtowhoetlo.html

Py:   arr.insert(0, 0)
来源：http://hz.nwbrower.top/gttotnxxrx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xylfe.cn/gtevfntpla.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.havefunace.top/gtknzccfkc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtnplrgjwl.html

Java: list.add(0, 0);
来源：http://hz.jlsjyb.cn/gtfpwxnfsy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuxming.cn/gtaeebassv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtcxxlayvb.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gtpdpjvngh.html

[D04] 删除元素
来源：http://hz.hammf.cn/gthmlwomeb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yueranfly.top/gtoiojhnxz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ppjwa.cn/gtupbbfrsv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gaohongyu789.top/gtnytouomw.html

TS:   arr.splice(0, 1);
来源：http://hz.zhongyouzk.top/gtxlrtqmhs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yangfankeji.com/gtfzcoxwdm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtvdzlnojn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sufxvd.cn/gtqzitetvk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sxryk.cn/gtfukyzowu.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtxuqpobmq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtvevnhfof.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gttxtdbvhc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtmhcuqrsa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258.top/gtzjoayaqk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yanxiufei.cn/gtqupsfyuz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gthwcsnsyq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtwboubhjg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtejvrgpiu.html

[D06] 数组长度
来源：http://hz.hysaishi.cn/gtxttdadyh.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtwnprmcom.html

PHP:  count($arr);
来源：http://hz.gogol.net.cn/gttvtkcigr.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gthsetqves.html

TS:   arr.length
来源：http://hz.jinqigufen.top/gtzjdfhsrq.html

Java: list.size();
来源：http://hz.bjfxy.top/gtjsmpjrnb.html

Go:   len(arr)
来源：http://hz.fzhhl.top/gtodrmkpcl.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtjqrwnlhq.html

C#:   list.Count;
来源：http://hz.zhaomingkeji.xyz/gtdivlypjz.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtetblrfuq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gtnczvusny.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258888.top/gtqaeikswc.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gteogohgxt.html

TS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtrvqgfydf.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gtlmkhcdpp.html

Go:   arr[1:4]
来源：http://hz.cheryme.top/gtfarsjtgz.html

Ruby: arr[1, 3]
来源：http://hz.snrcjt.cn/gtayryjhrr.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gtfaneiinf.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gthmhkevih.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtvixzwokc.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtcxscmdkb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtxvavsajt.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtnqvstdwk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gthzhwxvnw.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtaipfhabz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tian-w.cn/gtdccxszwv.html

C#:   a.Concat(b).ToList()
来源：http://hz.birdmap.top/gtzusrbvvf.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtssvkvkfe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtiimylflv.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtvgdoicfl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtdktothue.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.snrcjt.cn/gtuqdfevgy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtvdknyhet.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.andypj.xyz/gtedoiqpau.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtsvincekl.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtvpqabqcx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gttricjoop.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ehwqpu.com/gthmpvfxvf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtjhzpncwu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtiurykdyn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtexbprmaf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258.top/gtokkwlpij.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtbnewecrs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yangfankeji.com/gtweleumlg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.meibo888.top/gtyolrzblq.html

[D11] 反转数组
来源：http://hz.cqqwz.cn/gtvhsmbhoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xziqi.cn/gtlioozcmu.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigfzy.top/gtqfhuocpv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.316326.xyz/gtyjdqawqc.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gttizrelbx.html

Java: Collections.reverse(list);
来源：http://hz.xuetiantiany.cn/gtntsaivnv.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtfblrmcpc.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtueftfrdi.html

C#:   list.Reverse();
来源：http://hz.hfpthk.cn/gtvczxjkgo.html

[D12] 查找元素下标
来源：http://hz.yvedp.cn/gtdclskhis.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gtlmchezto.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhixingplan.top/gtcdmqhmbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtvjowatgj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtmqtvgprm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sysykeji.top/gtepoygfve.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtefttmuwc.html

Ruby: arr.index(x)
来源：http://hz.sxryk.cn/gtfhaexdlz.html

C#:   list.IndexOf(x);
来源：http://hz.sufxvd.cn/gtcekkjttj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daxiang520.top/gtddhiypdz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.dianchejie.cn/gtfpiszfoi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtdmhipgvz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtvvywlrnc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtyztxjmns.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtdizlxhnk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtlhnrrtyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gthzxuvwmi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtlojspnpd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhongyouzk.top/gtjczdfzxe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtcsqedauk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pengpengdd.cyou/gtunbbbgiq.html

JS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtmaxqaxqu.html

TS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtokkxhywk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtmddcpejp.html

Go:   // 手写循环
来源：http://hz.shanyushiyangtech.top/gtofwdvjsz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.dianchejie.cn/gtgpuiitks.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtdciwnegr.html

[D15] 去重
来源：http://hz.ppjwa.cn/gtltmyalrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtlfiptczi.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtcsdshslu.html

JS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gttymtntxa.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtrpsnucig.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtvnlbjqmg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtcmvpjvev.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtqzccgabs.html

C#:   list.Distinct().ToList()
来源：http://hz.hongshengwenyu.top/gthwpqcyck.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtditndrrn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhijiandao.cn/gtiaclpssd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gtcqivgrhm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtvhckpmsw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gttnwissuy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gthbtmrmjf.html

Go:   // 手写循环累加
来源：http://hz.nanxuanxn.top/gtkzicglaw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gogol.net.cn/gtpgobkeoc.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtnlqttxtb.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtlnjwdtnr.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxinkj.top/gtdehagboi.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuanzx.com/gtontzxujs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guannengcc.top/gtyhrwqjto.html

TS:   Math.max(...arr);
来源：http://hz.kuanghao11.cn/gtqalzkofx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gaohongyu789.top/gtkwdjxkxy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtmwuaozkf.html

Ruby: arr.max;  arr.min
来源：http://hz.jyoumei.cn/gtgophkhpl.html

C#:   list.Max();  list.Min()
来源：http://hz.sufxvd.cn/gtcspklwhl.html

[D18] 扁平化嵌套数组
来源：http://hz.cashguo.top/gtoxugfqvs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gtlhupbpov.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtnxfdnxaa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yongpay.top/gtojbqswbt.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtziigejcv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtdwuarzfd.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtqdvjbcgl.html

Ruby: nested.flatten
来源：http://hz.chenjidiqi.icu/gtwjtkqygq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtbybdbijz.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtzqoqddrd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtmayfbrod.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hywenlv.cn/gtsflidyab.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guowangkeji.top/gtyeunvvzf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258.top/gthvsxbzah.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gtgmpdaidp.html

Go:   // 手写 map[string][]T
来源：http://hz.aizwys.cn/gtxcqagtij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shzxlz.cn/gtyllygvaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.bjfxy.top/gtiagghrmb.html

[D20] 统计每个元素出现次数
来源：http://hz.hammf.cn/gtembvcyuv.html

Py:   Counter(arr)
来源：http://hz.jiagoushi.top/gtmamfxueu.html

PHP:  array_count_values($arr);
来源：http://hz.yueranfly.top/gtccamvjoo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtyatrhtjd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gteqittbqk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gttjovhlma.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangkeji.top/gtavdikqld.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtbavxleqz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhoulong.xyz/gtjcnzjtcz.html

[D21] 判断是否包含某元素
来源：http://hz.xuetiantiany.cn/gtordxbfvu.html

Py:   x in arr
来源：http://hz.redwolf501.top/gtuffnriod.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtxvlgdrce.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtlilgyaqp.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gthnzyccqa.html

Java: list.contains(x)
来源：http://hz.guowangkeji.top/gtqvlzjcnw.html

Go:   slices.Contains(arr, x)
来源：http://hz.gotoacloud.top/gtftzyqoct.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtpmctidtw.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtlzppmorg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhengqikj.top/gtnqyeqobq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtjoautetc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hysaishi.cn/gtaamkninz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hywenlv.cn/gtcfqcdzcm.html

TS:   [...arr];
来源：http://hz.pengpengdd.cyou/gtfldbbqmj.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtnaayeefk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sysykeji.top/gtrrmmxxup.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydzc1.top/gtdlxksblv.html

C#:   new List<int>(list);
来源：http://hz.ydjk.org.cn/gtobvlzhqv.html

[D23] reduce 累积计算
来源：http://hz.52xcode.cn/gtgoomctaf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xylfe.cn/gtxmjewjyd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtsyrqrkex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtsqtzmzzw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtmcixqfwi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jyoumei.cn/gthglfaptk.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtugjknwzp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gtkubbbtaw.html


<!-- 参考信息 -->