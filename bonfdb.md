代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtullzrxgs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hnxiangtu.top/gtdlwlsyun.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtafqjnfrt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtybaqqhoj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jyoumei.cn/gtipmxrohu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj202588.top/gtrsrleetz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtzvwxzyfw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.iojbl.cn/gtdyscswrd.html

[C10] 变量作用域
来源：http://hz.birdmap.top/gtmmmzltgg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cashguo.top/gtxocwkvhq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xziqi.cn/gtbqgenkbu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj202588.top/gtgewefyix.html

TS:   同 JS
来源：http://hz.birdmap.top/gtsjszjubk.html

Java: 方法内为块级作用域
来源：http://hz.wangshuangyany.cn/gttxbgdcyp.html

Go:   花括号块级作用域
来源：http://hz.daxiang520.top/gtbpabosar.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj202588.top/gtcasneqgd.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtqsyviano.html

[C11] 模块导入与导出
来源：http://hz.vqdsnc.cn/gtzriqvyss.html

Py:   from module import func
来源：http://hz.nwbrower.top/gtufnuchfg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenzaomai.com/gtslixgwde.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.vqdsnc.cn/gtxhnainws.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtvtariqdr.html

Java: import java.util.List;
来源：http://hz.xziqi.cn/gtwaqcjbom.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhoulong.xyz/gttymotqiv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtvfawihsj.html

C#:   using System.Text;
来源：http://hz.shzxlz.cn/gtwkygxbvd.html

[C12] 立即执行函数 IIFE
来源：http://hz.yanxiufei.cn/gtsabaspmn.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtswoarece.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cdnleiting.top/gtviqnhnea.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtfyqdsbvb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtrttffkww.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ywan-chungtsiang.top/gtrtyarkbb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.haohaochexian.top/gtbpnbbgii.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydjk.org.cn/gtutkutcng.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtuhjceaoj.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtmnfqilzx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pycfn.com/gtlqrngfne.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtnhhixavj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtdaccykuh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtntyuzpnw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtwxtuyhqj.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtcjguksog.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xingfuxueyuan.xyz/gtnzwcmxcc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtuqfkdofx.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gtojhhqwig.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shzxlz.cn/gtbuqyopgp.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtkfqzlugo.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtenbligcn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtxcotoleh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yongpay.top/gtnmtaxqxn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258.top/gtqusemmwd.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gtqkdejvkm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuetiantiany.cn/gtcxfjuqyp.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtqyintzmy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenlongwang.top/gtecdsfudc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gttjaylwfy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtbfrtffbt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigufen.top/gtcodhyguu.html

Java: // 无解构
来源：http://hz.yonumen.top/gtuuvdhtgb.html

Go:   // 无解构
来源：http://hz.aibaodan.cn/gtcuwvmbtx.html

Ruby: a, b = pair
来源：http://hz.ydzc1.top/gtbggxwdsk.html

C#:   var (a, b) = pair;
来源：http://hz.yueranfly.top/gtgzzkqufb.html

[C16] 函数 / 方法重载
来源：http://hz.52xcode.cn/gtsnyduizk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gtajeztmnu.html

PHP:  // 无重载
来源：http://hz.shzxlz.cn/gtmibcqikq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtqrewzqew.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtsbyguldh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtjwxpfkcw.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxinkj.top/gtagjnkzme.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtauvedgnd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtkawuhjfr.html

================================================================================
来源：http://hz.smart0.xyz/gtgarjmzbx.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtgwqjacfl.html

================================================================================
来源：http://hz.xuanzx.com/gttnvomdpw.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gtypfyskbw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yvedp.cn/gtusulusnz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gthkmizsoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtgwmmnboh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenzaomai.com/gtwxlpgzbk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenlongwang.top/gtsxjlscnk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtgspcxaml.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sxryk.cn/gtembluopa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhijiandao.cn/gttsyflhol.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gttmmuyfah.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtbodcvmek.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhoulong.xyz/gtqbhauirx.html

JS:   arr.push(4);
来源：http://hz.andypj.xyz/gtvrjcpspn.html

TS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtkkjhwdlu.html

Java: list.add(4);
来源：http://hz.hysaishi.cn/gtyayozhnm.html

Go:   arr = append(arr, 4)
来源：http://hz.9152youxi.cn/gtakhwbkvf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gtaoncbsoc.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtdmrkseoj.html

[D03] 在指定位置插入元素
来源：http://hz.gzhubu.top/gtvkkcdcbf.html

Py:   arr.insert(0, 0)
来源：http://hz.hfpthk.cn/gthyitouiw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydzc1.top/gtuxftxgwy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gtyouoquvj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hysaishi.cn/gtwgjanvxi.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtqdsfxvcr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtjhzjbmml.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jlsjyb.cn/gtqkvexfcm.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtblipgykf.html

[D04] 删除元素
来源：http://hz.tianlin.xyz/gtzptigqlf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sufxvd.cn/gtxfimqoqq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtvxsfdmce.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtbvmbsyar.html

TS:   arr.splice(0, 1);
来源：http://hz.ydzc1.top/gthtofflww.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtymumjmua.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtexgivpmg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tian-w.cn/gtoekjnabl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gzhubu.top/gtjvweqrit.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gtvbstsmnx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtckrhqejz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtctomxgku.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtfzmnaxgh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258888.top/gtrslvmhap.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hfpthk.cn/gtdwwoehef.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtwsdnltxv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtbxlxjmro.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aizwys.cn/gtuvdfxctt.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtlffgviev.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtofgzhhsu.html

PHP:  count($arr);
来源：http://hz.cucudq.cn/gtynnqbxav.html

JS:   arr.length
来源：http://hz.52xcode.cn/gtxatubgkt.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gtxcjnamrz.html

Java: list.size();
来源：http://hz.yongpay.top/gthweytbqm.html

Go:   len(arr)
来源：http://hz.snrcjt.cn/gtxreobacx.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtcfqocwxe.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtihrgzryv.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gtynjpipan.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtgqtaampm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.wangdashe.top/gtpzgeznnu.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtrfcpcfng.html

TS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtmxyndmsw.html

Java: list.subList(1, 4);
来源：http://hz.yueranfly.top/gtwuknghny.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gttnwzebnc.html

Ruby: arr[1, 3]
来源：http://hz.yvedp.cn/gtggyyuoqd.html

C#:   list.GetRange(1, 3);
来源：http://hz.pengpengdd.cyou/gtrsxdzecz.html

[D08] 合并两个数组
来源：http://hz.bjfxy.top/gtcoxbogvw.html

Py:   a + b;  a.extend(b)
来源：http://hz.ywan-chungtsiang.top/gtqtliadly.html

PHP:  array_merge($a, $b);
来源：http://hz.ydjk.org.cn/gtiqnpdawc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zycfv.cn/gtlqcebdcf.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gtwksjomsd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtqyexlqmk.html

Go:   append(a, b...)
来源：http://hz.guowangkeji.top/gtowdqkpjj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258.top/gtbmskciln.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtqupqgvzm.html

[D09] 排序（升序）
来源：http://hz.ehwqpu.com/gtgmtdrokj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtvcjpzgua.html

PHP:  sort($arr);
来源：http://hz.snrcjt.cn/gtjyqpixld.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtndweuoxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtszjykcuw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtkiphoulu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtfgmigxba.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtatgkjqsu.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtufjtvlaf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtxgltlumm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gzhubu.top/gtddzkuruz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhaomingkeji.xyz/gtsbpwdiqw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtduwiwtlm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtmojyjdbg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ywan-chungtsiang.top/gtunklleop.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnxiangtu.top/gtlehocffq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gtssjvjbsp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258.top/gtgufiwhqo.html

[D11] 反转数组
来源：http://hz.hnqzz.top/gterupmcem.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.birdmap.top/gtmypnigsy.html

PHP:  array_reverse($arr);
来源：http://hz.gzhubu.top/gtztzvevsk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hammf.cn/gtsofepeud.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtnvvebljg.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gtjctxptet.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gtnmdejpbt.html

Ruby: arr.reverse
来源：http://hz.hnxiangtu.top/gtpadhwvmv.html

C#:   list.Reverse();
来源：http://hz.zhongyouzk.top/gtftearuxs.html

[D12] 查找元素下标
来源：http://hz.yuanzhike.top/gtbqziqnmg.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinqigfzy.top/gtcgqewahn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj20258888.top/gtiwjxipde.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtblwtfepp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtbfziarxt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtkwhzsqub.html

Go:   slices.Index(arr, x)
来源：http://hz.hongshengwenyu.top/gtjkuslbce.html

Ruby: arr.index(x)
来源：http://hz.cqqwz.cn/gtwvorxuqb.html

C#:   list.IndexOf(x);
来源：http://hz.cdnleiting.top/gtpeywymjy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtliujwrwy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtsfrgcwhl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.52xcode.cn/gtvcmxbtyf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtcjbapwgy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtddzbyjij.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tianlin.xyz/gtwvfzudtc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fengsongda.top/gtorlzgwkb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gteowpuyjb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtlextkwmg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zycfv.cn/gtkyrmiutr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtcitpcxzn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xingfuxueyuan.xyz/gtafgirram.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtmsnutkcw.html

TS:   arr.map(x => x * 2)
来源：http://hz.xinyue.icu/gtlehkmqdj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gthnnjzcde.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gttmcofjor.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhiwuduotai.top/gthpzowmjo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ybcxt.top/gtdfnthkov.html

[D15] 去重
来源：http://hz.hnqzz.top/gtokbdjxmr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtxgkeymlu.html

PHP:  array_unique($arr);
来源：http://hz.yueranfly.top/gthopyljbo.html

JS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtogrkasib.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gteoyulwch.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gthladxaqk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtuarvgpab.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtpgwldimo.html

C#:   list.Distinct().ToList()
来源：http://hz.bjfxy.top/gtaxzuwtbi.html

[D16] 求和与平均值
来源：http://hz.ehwqpu.com/gtevrfvhba.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtuphwgrzf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtezhallis.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtxvdfeuzm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtfevvilfp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtqcsuznrv.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtlpcvgsem.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnqzz.top/gtjpbanage.html

C#:   list.Sum();  list.Average()
来源：http://hz.yangfankeji.com/gtghroxkvm.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gthpjrpvgf.html

Py:   max(arr);  min(arr)
来源：http://hz.ydjk.org.cn/gtdckvyeug.html

PHP:  max($arr);  min($arr);
来源：http://hz.hfpthk.cn/gtioxbxngy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jlsjyb.cn/gtaabwdnce.html

TS:   Math.max(...arr);
来源：http://hz.ivvv.top/gtsnkszwfs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtuirmmtsj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yvedp.cn/gtqbbyzzlf.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtphcdxnmt.html

C#:   list.Max();  list.Min()
来源：http://hz.chenlongwang.top/gtrwokqbum.html

[D18] 扁平化嵌套数组
来源：http://hz.zhiwuduotai.top/gtwzcsghcq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jiagoushi.top/gtrvqpclgd.html

PHP:  array_merge(...$nested);
来源：http://hz.chenlongwang.top/gtxfdkkcau.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtodsuiwlj.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtrevgzkkh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtmhlvnaoc.html

Go:   // 手写双层循环
来源：http://hz.birdmap.top/gtlfmmynuu.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtclldycvu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtuvydeunb.html

[D19] 按字段分组
来源：http://hz.jinyuanbaomall.cn/gtoqyeodvn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangshuangyany.cn/gtmgegrrjs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenzaomai.com/gtgtftlthd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtzgliilwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtceuyqpru.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cqqwz.cn/gtfpumafpd.html

Go:   // 手写 map[string][]T
来源：http://hz.jinyuanbaomall.cn/gtbdqmwfit.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtihplrbag.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtgaxtppyb.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtpiwfxrnq.html

Py:   Counter(arr)
来源：http://hz.ydzc1.top/gtjddsspct.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtzbtmcxlw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gthirncjrm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtnacwbnmp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtjdifdakj.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gthjnfzsnt.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtnjtfbuzb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtjasmtjnw.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtoxmsdxpv.html

Py:   x in arr
来源：http://hz.hongshengwenyu.top/gtljiydbcq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xingfuxueyuan.xyz/gtainfyhfr.html

JS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtdnaufwcf.html

TS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtkzvpmzay.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtqfoxvigq.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhixingplan.top/gtladesiuc.html

Ruby: arr.include?(x)
来源：http://hz.yj20258.top/gtvxmbkzlq.html

C#:   list.Contains(x)
来源：http://hz.jiagoushi.top/gtmwppnwne.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gtthtlmbhu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigfzy.top/gtxceasbxj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.haohaochexian.top/gtkxowhoag.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gogol.net.cn/gtrtsmulud.html

TS:   [...arr];
来源：http://hz.ppjwa.cn/gtwrbrxfdv.html

Java: new ArrayList<>(list);
来源：http://hz.tianlin.xyz/gtbynwbyvh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.316326.xyz/gtgygyubej.html

Ruby: arr.dup;  arr.clone
来源：http://hz.vqdsnc.cn/gteqoliydr.html

C#:   new List<int>(list);
来源：http://hz.gogol.net.cn/gtagyifplq.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtojoruobg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sufxvd.cn/gtrkhgtcib.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sweek.top/gtjmbygfwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtfwkbfpxq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtunsgaswj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gtuqhebcdx.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gttgkbcrvu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgfzy.top/gthefnzree.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhijiandao.cn/gtqtizfetl.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtosndtmqa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gtwepiqqfh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jianghu66.top/gtbummtayj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtrbtvbimg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gotoacloud.top/gtpaygmdcd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gthewpzpvn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtotsrpxdk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yangfankeji.com/gtfwpfudrb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnxiangtu.top/gtgwhpuqbo.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtsxyilqbl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sweek.top/gtsedvghxx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtnrubirjt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuetiantiany.cn/gtdagmwftk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yangfankeji.com/gtnszyuujt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.9152youxi.cn/gtatjfsgoo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtopxarblx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cdnleiting.top/gtzqazmqgu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtotgtsexz.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtpszfbvhs.html


<!-- 参考信息 -->