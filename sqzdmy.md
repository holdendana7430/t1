代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtczlzbjyy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtkhgboyaq.html

[C08] 闭包
来源：http://hz.zhongyouzk.top/gtixgabtoe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.316326.xyz/gtojlzweue.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydzc1.top/gtzzgeddlr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtmathyaod.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtforrsumn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zycfv.cn/gttmyyqpnw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhiwuduotai.top/gtizcqvicj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtqhdhdcev.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtmjzuxaok.html

[C09] 递归
来源：http://hz.yj202588.top/gtmmlbctmt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtludmqwsl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhijiandao.cn/gtfqgrmfqi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtkbzjguiu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtbushmuxz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gotoacloud.top/gtckkkwkrm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ehwqpu.com/gtrfqtrjsg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtmsvjzcfz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gotoacloud.top/gtcduvesmh.html

[C10] 变量作用域
来源：http://hz.jinghuilouyu.cn/gtvfcklhay.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pycfn.com/gtxpsxgvgp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.316326.xyz/gtqbzdqifb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daria6918.cn/gtadaxkkga.html

TS:   同 JS
来源：http://hz.mhx1999.top/gtdkthopdy.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtdolhohnr.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtckpvaosa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuetiantiany.cn/gtxfpskuqu.html

C#:   块级作用域
来源：http://hz.havefunace.top/gthpijklhf.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtlbemnkvd.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtzweaofux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydzc1.top/gtesyywlgn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hammf.cn/gtsouqabbt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sweek.top/gtsmdgfsxm.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtuyencema.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yonumen.top/gtklgbsnav.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtoazbnrlt.html

C#:   using System.Text;
来源：http://hz.jqgufenzy.top/gtlrlgazzd.html

[C12] 立即执行函数 IIFE
来源：http://hz.sweek.top/gtnbegmlqw.html

Py:   (lambda: print("run"))()
来源：http://hz.hysaishi.cn/gtdssxmuta.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gtktkfeyos.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtnyoxmehg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtkxslpvia.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtqxyglxfc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtonplgjdp.html

Ruby: -> { puts "run" }.call
来源：http://hz.ybcxt.top/gtxzhsknrv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gtuffbcyto.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtodlvcdzu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.mhx1999.top/gtfsznztre.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtflzijdfa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtpavtlbnx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtdxvvdqbi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtqfopoiqd.html

Go:   func add(a, b int) int
来源：http://hz.meibo888.top/gtwdgwwkpn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sweek.top/gthuevqsec.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtzsvfppqk.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gtuqwutubf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xylfe.cn/gtxwejoxba.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gtkrwuskru.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtchunhtzr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtsqqsjuzb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gthnyygtgy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtuukgcuut.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtywllztic.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgfzy.top/gtpdtsiigr.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtvrpkepnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtbrdeluba.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daxiang520.top/gtacwhxnpd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtuxgzmvch.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtvmdqggbt.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtalfxaogt.html

Go:   // 无解构
来源：http://hz.sxryk.cn/gtnahtrmet.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gthiaarzrj.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258.top/gtqydxmrfc.html

[C16] 函数 / 方法重载
来源：http://hz.meibo888.top/gtlpmukyds.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtsjftnusx.html

PHP:  // 无重载
来源：http://hz.zycfv.cn/gtmzqybjpd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtbwfgpgat.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigufen.top/gtsnnyyugh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtkckqtwqx.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhongyouzk.top/gtoobvgjpr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtkltxcgfz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gtdcwkcmot.html

================================================================================
来源：http://hz.sxryk.cn/gtkddaffwi.html

D. 数组 / 列表 / 集合
来源：http://hz.shangyingyoupin.top/gtezrtbijw.html

================================================================================
来源：http://hz.sweek.top/gtfdccumnv.html

[D01] 创建数组 / 列表
来源：http://hz.jqgufenzy.top/gtqvzkwljf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gtltsjstzn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtsxwuizkb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtwtsyyedf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daria6918.cn/gtcaeyxywm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhixingplan.top/gtufexhwtx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.316326.xyz/gtmublquvl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tanke756.top/gtipururef.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtsmrgwvqr.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtiguchdsj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtutvbrssr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtcyyrztoj.html

JS:   arr.push(4);
来源：http://hz.316326.xyz/gtpbefadvt.html

TS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtdntqajyp.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtfwyeucvl.html

Go:   arr = append(arr, 4)
来源：http://hz.cdnleiting.top/gtbwaocmzs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtzdftzodt.html

C#:   list.Add(4);
来源：http://hz.ehwqpu.com/gtvdozjvvg.html

[D03] 在指定位置插入元素
来源：http://hz.jyoumei.cn/gtqarusuwg.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtdmkbidtq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jyoumei.cn/gtpqibpyff.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.feifeiyinyue.top/gtacvelrrh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.52xcode.cn/gtssglmfmf.html

Java: list.add(0, 0);
来源：http://hz.bjfxy.top/gtdxcromet.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.iojbl.cn/gthglcyygm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sxryk.cn/gtjrqezalb.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigufen.top/gtvostbipa.html

[D04] 删除元素
来源：http://hz.yj20258888.top/gtaoiccgkp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hfpthk.cn/gtjoadodjf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gtsiawbael.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtorjllokx.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtmxocvbgr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenzaomai.com/gtssmtgbhg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj202588.top/gtpyaeypjn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtgkcqkfoh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydjk.org.cn/gtsvkwnodt.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtjwzhamoi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtsaimkbiy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtcttdkysw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jlsjyb.cn/gtrmgpbtqe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.snrcjt.cn/gtbawfifmc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangtech.top/gtulugrnrl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtgwgwffir.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtqxxbkaql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtmajorzsm.html

[D06] 数组长度
来源：http://hz.cqqwz.cn/gtypyzdtjt.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtpzzasung.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtgviryjxf.html

JS:   arr.length
来源：http://hz.zhoulong.xyz/gttqrhdnst.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtjdwqwtls.html

Java: list.size();
来源：http://hz.wangdashe.top/gtkynyzfdl.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtpjfzyagl.html

Ruby: arr.length; arr.size
来源：http://hz.nanxuanxn.top/gtcuwmgsee.html

C#:   list.Count;
来源：http://hz.quarkkingdee.top/gtzcveavxs.html

[D07] 切片 / 取子数组
来源：http://hz.svipenyu.cn/gthyybqozz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtxrzkfrqb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nwbrower.top/gtkcpdudht.html

JS:   arr.slice(1, 4);
来源：http://hz.aizwys.cn/gtxkmbqnzt.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtkkeqejpx.html

Java: list.subList(1, 4);
来源：http://hz.jlsjyb.cn/gttxjqaowk.html

Go:   arr[1:4]
来源：http://hz.guannengcc.top/gtapzvjrwj.html

Ruby: arr[1, 3]
来源：http://hz.ivvv.top/gtfvdvnevf.html

C#:   list.GetRange(1, 3);
来源：http://hz.jyoumei.cn/gthhkkcyur.html

[D08] 合并两个数组
来源：http://hz.jqgfzy.top/gtdvrhgnew.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangkeji.top/gtftjaiyii.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtopnknbxr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xylfe.cn/gtkazqfzrw.html

TS:   [...a, ...b];
来源：http://hz.tian-w.cn/gtksiygwpx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fengsongda.top/gtvldnpwvg.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtlgqvbkpj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtldoecunz.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinyuanbaomall.cn/gtbnsrvdjg.html

[D09] 排序（升序）
来源：http://hz.yongpay.top/gtfkwqrqpi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtqskvsmvn.html

PHP:  sort($arr);
来源：http://hz.0kj1m.cn/gtcocrolar.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuanzx.com/gtqdlnuwfb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtplqdcnpm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhoulong.xyz/gtcfnlmpev.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yvedp.cn/gtimggwncd.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gthhusaiul.html

C#:   list.Sort();
来源：http://hz.feifeiyinyue.top/gtwnyqpxbz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.redwolf501.top/gtlvhgdrus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtyywseoza.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtizoomwfm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtqazomgzv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtxleoetks.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtjnthvsqp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtvprzfhlu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigfzy.top/gtydaaeoky.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.havefunace.top/gtrmfgwzcp.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtniupkekj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj202588.top/gtxlzqehyp.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtsfpuqvot.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhiwuduotai.top/gtmhloboir.html

TS:   [...arr].reverse();
来源：http://hz.ivvv.top/gtjoavwcoy.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtqrgarncm.html

Go:   slices.Reverse(arr)
来源：http://hz.0kj1m.cn/gtfhwenaku.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtdoddiphv.html

C#:   list.Reverse();
来源：http://hz.shangyingyoupin.top/gtcppsbvfs.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtxqomahkv.html

Py:   arr.index(x);  x in arr
来源：http://hz.xingfuxueyuan.xyz/gtpjttdqad.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnxiangtu.top/gtqzfqinxr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtfailtppc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtwgmkkaxt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gtvvkcjqmx.html

Go:   slices.Index(arr, x)
来源：http://hz.0kj1m.cn/gtjabwdxzo.html

Ruby: arr.index(x)
来源：http://hz.chenzaomai.com/gtxilyzyyf.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtripgaolt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhixingplan.top/gtzbqfscuq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yanxiufei.cn/gtpvndwbtn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnqzz.top/gtspoxzlai.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtxliuuvik.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtsiphwual.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtavbgryju.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gtyvrjgiau.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtpayfeyny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtfmlampez.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenjidiqi.icu/gtiqmbfynm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtcrvgshyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnxiangtu.top/gtrqivqcqb.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gthsgkuiby.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtqwolbnls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtxkhrmtcn.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gttxbydgqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.quarkkingdee.top/gtfutsgeyu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gthjuvewju.html

[D15] 去重
来源：http://hz.jqgufenzy.top/gtmysrfqqa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnqzz.top/gtkmkktdtv.html

PHP:  array_unique($arr);
来源：http://hz.ydzc1.top/gtoowvllfk.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtbnsxomca.html

TS:   [...new Set(arr)]
来源：http://hz.9152youxi.cn/gtimeplqwj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hfpthk.cn/gtcrkdypdq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigfzy.top/gtmlznxvod.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtzjktlkfw.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtvihtyaxa.html

[D16] 求和与平均值
来源：http://hz.sufxvd.cn/gthehuzkvb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zycfv.cn/gthjerndmr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtcwfwvwmv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtslgrstjl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtvxankwoz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtrdorbhte.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtxxhwsdba.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gthqhfcsdi.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gtwabenuon.html

[D17] 最大值与最小值
来源：http://hz.9152youxi.cn/gtixnksulx.html

Py:   max(arr);  min(arr)
来源：http://hz.ydjk.org.cn/gthajpywkp.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangdashe.top/gtyzkrpmno.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.feifeiyinyue.top/gtqkrvpcvm.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gtaiznbgqu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtbnrkybnq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gtuepweyeu.html

Ruby: arr.max;  arr.min
来源：http://hz.dashuyun.cn/gtdljtjhnu.html

C#:   list.Max();  list.Min()
来源：http://hz.vqdsnc.cn/gtwtvqcvud.html

[D18] 扁平化嵌套数组
来源：http://hz.wangshuangyany.cn/gtxfliwpwl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sxryk.cn/gtornitgyv.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtrzsnaqgz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtkmsqmmbr.html

TS:   nested.flat();
来源：http://hz.dashuyun.cn/gtsgrkambz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ppjwa.cn/gthcgmodur.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gtbfprtlqv.html

Ruby: nested.flatten
来源：http://hz.yj20258888.top/gtkzmvvzuy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtlqrcitvb.html

[D19] 按字段分组
来源：http://hz.sweek.top/gtusllajid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ppjwa.cn/gttciagzmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtygcczkzm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtzszzsxgg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xylfe.cn/gtabhisnne.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgufenzy.top/gtcyeqfjds.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigufen.top/gtnyodtiyg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtplevsoxv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jianghu66.top/gtdozxjdvn.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtucvbuson.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtswxgewhg.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtabbxgjzt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtarbpmnhs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gthnbhxoeh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.mhx1999.top/gtsybippfu.html

Go:   // 手写 map[T]int
来源：http://hz.yueranfly.top/gtfebzjslh.html

Ruby: arr.tally
来源：http://hz.zhongyouzk.top/gtauwbnzlz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhengqikj.top/gtmxgdykws.html

[D21] 判断是否包含某元素
来源：http://hz.jyoumei.cn/gtkqgwtsam.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gthsxwsktb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.vqdsnc.cn/gtoqnoedgu.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtcdnjzouw.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtteiqixyb.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gthajxwbin.html

Go:   slices.Contains(arr, x)
来源：http://hz.cashguo.top/gtyuqnsdoo.html

Ruby: arr.include?(x)
来源：http://hz.jyoumei.cn/gtglesxydz.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtlvnlqblw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tianlin.xyz/gttcrozrri.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tanke756.top/gtivdlosqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtixsbovyl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yonumen.top/gtjfwsrhwv.html

TS:   [...arr];
来源：http://hz.jinghuilouyu.cn/gthinuppue.html

Java: new ArrayList<>(list);
来源：http://hz.chenzaomai.com/gtrlfrmdor.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtrbbcpfcd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.kuanghao11.cn/gthbxkiqtk.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gtnsvtwjsj.html

[D23] reduce 累积计算
来源：http://hz.meibo888.top/gtmgmdofay.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.kuanghao11.cn/gtsyfkjpvw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sweek.top/gtwachmjny.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtdahxhphg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtxpmisjqu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtgzinmcmg.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtcjpicvbv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtboxerhum.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtnyhtauxw.html

[D24] 字典 / Map 基本操作
来源：http://hz.pengpengdd.cyou/gtzplzdckq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.daria6918.cn/gtdjlisiaz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtaaboazsk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtrwatkweo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gticlfajkr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtuotyvqvi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gtpducqhno.html


<!-- 参考信息 -->