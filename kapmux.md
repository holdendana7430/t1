代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zycfv.cn/gtjrdwgaua.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtvubapycg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtzpbaokzh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258.top/gtkgzcyfnv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cheryme.top/gtquofgstg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.52xcode.cn/gtaioaovfi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtoletfhjw.html

[C09] 递归
来源：http://hz.kuanghao11.cn/gtjnymdnyq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtdjmrukwg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuanzx.com/gtptvekyjm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtgqszhalp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtiljzomul.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydzc1.top/gtytaqjnns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gthwikqtus.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtpehrmpas.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhaomingkeji.xyz/gteuqpxbto.html

[C10] 变量作用域
来源：http://hz.gotoacloud.top/gtgquymccu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.bjfxy.top/gtzfcltkqt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pycfn.com/gtlgjvglfa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daria6918.cn/gtpxxwusyt.html

TS:   同 JS
来源：http://hz.sufxvd.cn/gthxxkngzd.html

Java: 方法内为块级作用域
来源：http://hz.daria6918.cn/gtvvkapiki.html

Go:   花括号块级作用域
来源：http://hz.quarkkingdee.top/gthxbljdcr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.smart0.xyz/gtszrteweu.html

C#:   块级作用域
来源：http://hz.jlsjyb.cn/gtlarahmlb.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtroabsead.html

Py:   from module import func
来源：http://hz.hnxiangtu.top/gtrdakvees.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gtqelcpfzx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cucudq.cn/gtfdyjxsga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.snrcjt.cn/gtcidnbemc.html

Java: import java.util.List;
来源：http://hz.jlsjyb.cn/gtvooatzpy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.feifeiyinyue.top/gticjyfpfy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenlongwang.top/gtyxbbcftb.html

C#:   using System.Text;
来源：http://hz.hywenlv.cn/gteelapmos.html

[C12] 立即执行函数 IIFE
来源：http://hz.hywenlv.cn/gtnivhjsid.html

Py:   (lambda: print("run"))()
来源：http://hz.svipenyu.cn/gtdrhatdls.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cdnleiting.top/gtwcqgkofr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtzbuyiqza.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtyosorudn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtaoticvxj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pengpengdd.cyou/gtfdzclkzi.html

Ruby: -> { puts "run" }.call
来源：http://hz.dianchejie.cn/gtlmvtyjlk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtpirnjegi.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhaomingkeji.xyz/gtbjgjbhgv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtizyvllug.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtflbrqnrz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtrhvssvcw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtamzjhpfh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtpqlrqjtq.html

Go:   func add(a, b int) int
来源：http://hz.redwolf501.top/gtfdigsjqv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gtajogazom.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gzhubu.top/gtoajpbhce.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gtfjvblgur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yanxiufei.cn/gtfdasmpmu.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtpsqdqnki.html

JS:   // 无泛型
来源：http://hz.yangfankeji.com/gtmawuarwj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxinkj.top/gtqvaunijy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtakfsjxrp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhengqikj.top/gtzmvxptrs.html

Ruby: # 无泛型
来源：http://hz.c1oappe.top/gtwcqrdyds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cqqwz.cn/gtdfmfmeic.html

[C15] 解构 / 展开参数
来源：http://hz.316326.xyz/gtbotflgxp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangshuangyany.cn/gtjbqngiaj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xinyue.icu/gtcjmezonv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guannengcc.top/gttienetiw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangkeji.top/gtscllixsc.html

Java: // 无解构
来源：http://hz.gogol.net.cn/gtujewpopo.html

Go:   // 无解构
来源：http://hz.bjfxy.top/gtsjxfteuj.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtbauyuthj.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtwaysmqtm.html

[C16] 函数 / 方法重载
来源：http://hz.c1oappe.top/gthbgessgh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhongyouzk.top/gtbjrypuxz.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtwhdvyxmf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.birdmap.top/gtmwuhtgqv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtfhrrueuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gtknihghgh.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258.top/gtbcgukzdu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guannengcc.top/gthijjvkpr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gtycwdauos.html

================================================================================
来源：http://hz.tanke756.top/gtnvresryu.html

D. 数组 / 列表 / 集合
来源：http://hz.jinghuilouyu.cn/gtptjowyrn.html

================================================================================
来源：http://hz.0kj1m.cn/gtqshpznfp.html

[D01] 创建数组 / 列表
来源：http://hz.sufxvd.cn/gtjmgacsax.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigufen.top/gtviflwezf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtrhthozlb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gzhubu.top/gtjlcblwlz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gthjdgoqnh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.vqdsnc.cn/gtfxnkjayv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtxpggldfz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gtzgwbbxzo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtksjooidn.html

[D02] 追加元素到末尾
来源：http://hz.yonumen.top/gtsuvhjhif.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtpnkujbqv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dashuyun.cn/gtjexzrsft.html

JS:   arr.push(4);
来源：http://hz.zhengqikj.top/gtjeylnpbq.html

TS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtuyhojfrv.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtouqoygsk.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangtech.top/gtwmrgvkis.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.meibo888.top/gtsjecxock.html

C#:   list.Add(4);
来源：http://hz.jyoumei.cn/gtfydplrnq.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtybmrnayd.html

Py:   arr.insert(0, 0)
来源：http://hz.zhixingplan.top/gtkxbhdjdv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gttbuiephq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hywenlv.cn/gtsmrhuoqj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangshuangyany.cn/gtvqldwmpz.html

Java: list.add(0, 0);
来源：http://hz.sxryk.cn/gtxxbmgbcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sufxvd.cn/gtobviskja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtxccaogfv.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtjxspnxgh.html

[D04] 删除元素
来源：http://hz.sxryk.cn/gteixbnwgh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jyoumei.cn/gtrubphqbt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtyrlphjxa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yanxiufei.cn/gtlhdvsmtz.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtwjobvosx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.dashuyun.cn/gtvuxqscgh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gtcjqosloa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gaohongyu789.top/gtzjbtqbox.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sxryk.cn/gtzqnxdfip.html

[D05] 访问与修改元素
来源：http://hz.9152youxi.cn/gtxqynbwcv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtyumqjuoa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gteqacstyd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gtvxxmkcuy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.feifeiyinyue.top/gtiqqtrfon.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gttivwctoc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xziqi.cn/gtfekljzhl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtuiiwfimw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dianchejie.cn/gtjhiamalj.html

[D06] 数组长度
来源：http://hz.dianchejie.cn/gtiarkgiwk.html

Py:   len(arr)
来源：http://hz.quarkkingdee.top/gtnhhtzjvn.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtmtztzoht.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtwxtaasrz.html

TS:   arr.length
来源：http://hz.sysykeji.top/gthyaulymm.html

Java: list.size();
来源：http://hz.fengsongda.top/gtlynubbdc.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtfnopgfts.html

Ruby: arr.length; arr.size
来源：http://hz.cucudq.cn/gtvkglgkmn.html

C#:   list.Count;
来源：http://hz.zhengqikj.top/gtkuanbhrh.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtaovrfgkn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gtiametdao.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenjidiqi.icu/gteekzggkg.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gttgerqkba.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtbhbnxoxk.html

Java: list.subList(1, 4);
来源：http://hz.ydjk.org.cn/gtmbdcnhdl.html

Go:   arr[1:4]
来源：http://hz.sysykeji.top/gtyyaeeayx.html

Ruby: arr[1, 3]
来源：http://hz.ywan-chungtsiang.top/gtjthzhdsd.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtsiwexbcn.html

[D08] 合并两个数组
来源：http://hz.xuetiantiany.cn/gtjovhvmbz.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gtswwhwrzl.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtqitwlngm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnqzz.top/gttnjgsuzt.html

TS:   [...a, ...b];
来源：http://hz.hnxiangtu.top/gtngsvkdfw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtecrzjggz.html

Go:   append(a, b...)
来源：http://hz.redwolf501.top/gtmjuxbwql.html

Ruby: a + b;  a.concat(b)
来源：http://hz.meibo888.top/gtpupznyja.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtkhtalwoo.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtletakwsu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtxfltfpss.html

PHP:  sort($arr);
来源：http://hz.jiagoushi.top/gtmyawqmup.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtzxbdoszq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.vqdsnc.cn/gtnauahika.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhengqikj.top/gtnmlbsdbb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnqzz.top/gtckbqvgje.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtkfkggwpv.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtduhfkekp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangkeji.top/gtqsylwowc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtzysedith.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtdcqitzzo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtbkyqylkh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtcwkhnpqx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ybcxt.top/gtgjvzfnsc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinghuilouyu.cn/gtvneneevn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtvswnifxb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daria6918.cn/gtcpubdnjn.html

[D11] 反转数组
来源：http://hz.hammf.cn/gtmqybswwl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jiagoushi.top/gtptcvywys.html

PHP:  array_reverse($arr);
来源：http://hz.zycfv.cn/gtxjhxstbl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cashguo.top/gtoybgvnvx.html

TS:   [...arr].reverse();
来源：http://hz.guannengcc.top/gtnnjpjsjp.html

Java: Collections.reverse(list);
来源：http://hz.fengsongda.top/gtiwbtcjrl.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtzbhketva.html

Ruby: arr.reverse
来源：http://hz.ydjk.org.cn/gtfkvpwlox.html

C#:   list.Reverse();
来源：http://hz.yueranfly.top/gtraitwhwb.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtidwcrwjg.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinyuanbaomall.cn/gtvqlekauz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtljidjsvb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtueirmawq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtuihrljbm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zdqjudy.top/gtpibuofzp.html

Go:   slices.Index(arr, x)
来源：http://hz.yj202588.top/gttmfedfhz.html

Ruby: arr.index(x)
来源：http://hz.yanxiufei.cn/gtnfvngyzt.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtnqmdvsbw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinyuanbaomall.cn/gtlbydtlhz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydjk.org.cn/gtiyziqwfs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtldfathgo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gthejldial.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtacoyrrjd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtdawfcvbg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gttzjyampy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtfesvmtbr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtgjlibezs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gttnpazkpx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtffhjinwv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sufxvd.cn/gtpppywqbs.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtgrmceovl.html

TS:   arr.map(x => x * 2)
来源：http://hz.xuanzx.com/gtoxiclfte.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dashuyun.cn/gtojnayobi.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtckulbsed.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhixingplan.top/gtvqlmjiyg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.redwolf501.top/gtfegbbgwe.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtwygtzmzl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtbxnznhfb.html

PHP:  array_unique($arr);
来源：http://hz.nanxuanxn.top/gtbtndbitb.html

JS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtigxiymos.html

TS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtyfggoadl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtbxquosvc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenzaomai.com/gtlnjsqqqs.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtmjvirrog.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtsmgspshw.html

[D16] 求和与平均值
来源：http://hz.hammf.cn/gtelzpsfgv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigfzy.top/gtemmroupn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtrxwbomnk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtkyskxfoz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtoemdhlro.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtbzxbepgb.html

Go:   // 手写循环累加
来源：http://hz.aibaodan.cn/gtpvjfhkvj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtjurztyhb.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtpptncbzc.html

[D17] 最大值与最小值
来源：http://hz.nwbrower.top/gtfuouygfl.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtkdxiigkd.html

PHP:  max($arr);  min($arr);
来源：http://hz.jqgufenzy.top/gtadhalxvl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yanxiufei.cn/gtrrxdoyky.html

TS:   Math.max(...arr);
来源：http://hz.smart0.xyz/gtgdvrgblg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtgftvrntu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigufen.top/gtuekgdcwb.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtfubvaota.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtqgvovmow.html

[D18] 扁平化嵌套数组
来源：http://hz.hnxiangtu.top/gtddyaundl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.vqdsnc.cn/gtcjmjuncp.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtgrcjdpob.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtidpastxo.html

TS:   nested.flat();
来源：http://hz.zhixingplan.top/gtoigstohi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hongshengwenyu.top/gtzqzizsqz.html

Go:   // 手写双层循环
来源：http://hz.vqdsnc.cn/gtlutlwiim.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtcuoswmix.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtdqzoavhd.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtcubhabze.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtbivlhmpy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnqzz.top/gtakdyaypz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hywenlv.cn/gtzvbdccsb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtigqtrkud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydjk.org.cn/gtvjzxvxbg.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gtwygcoxcr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.smart0.xyz/gtejdlndgd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.316326.xyz/gtlhhqignk.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtgxocmcgs.html

Py:   Counter(arr)
来源：http://hz.cheryme.top/gtaknycphd.html

PHP:  array_count_values($arr);
来源：http://hz.shuidangran.top/gtuibghhkd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtpkasbpwr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtirmydian.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.vqdsnc.cn/gtzutzogdc.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtlcqzfbzw.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gtelqxymnb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zdqjudy.top/gtgoqvxypk.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gttiewuouc.html

Py:   x in arr
来源：http://hz.316326.xyz/gtcvxmtwnv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jianghu66.top/gtqmyafmct.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtntxumibh.html

TS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtvwmvuhwj.html

Java: list.contains(x)
来源：http://hz.jinqigfzy.top/gtvvkbtbfq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtfxyjyfzx.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtnmrzmqvy.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtwbgvmzdg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtnxnakkhv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.quarkkingdee.top/gtuhptiozw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zycfv.cn/gtncpzpinx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangdashe.top/gtilqpoawe.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtuozwsdtx.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtfevhddom.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ywan-chungtsiang.top/gtqavrzkrv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtrndewxjt.html

C#:   new List<int>(list);
来源：http://hz.hfpthk.cn/gtvkqqvsfq.html

[D23] reduce 累积计算
来源：http://hz.316326.xyz/gtumigmwxl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtjiyygxsw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtyjsfollm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtxpolsxxw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtoyoautld.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtnxdlbife.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtkzgbspyz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gtaspbqiec.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ehwqpu.com/gtssqgezjg.html

[D24] 字典 / Map 基本操作
来源：http://hz.cucudq.cn/gtzszaovdd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tianlin.xyz/gtujmpiqop.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.316326.xyz/gttnzbrwxz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtmidiitml.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cashguo.top/gtxvnmmiwv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtgzerutyi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gtzkuezqer.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hysaishi.cn/gtrscgsygi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jiagoushi.top/gtvwrnzzmb.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gtnmxbmljm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtqlvzowvk.html


<!-- 参考信息 -->