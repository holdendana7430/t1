代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtjikzanlv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gtgndauddw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtdocaheqt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtwkkauhhh.html

[C10] 变量作用域
来源：http://hz.chenlongwang.top/gtoqgwwgom.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nwbrower.top/gtlzjnmyuo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtdrwmkteq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtajlpgbpw.html

TS:   同 JS
来源：http://hz.cheryme.top/gtqkatvvro.html

Java: 方法内为块级作用域
来源：http://hz.daria6918.cn/gtxgzedxqf.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtlaasmjxx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hywenlv.cn/gtikvshyxg.html

C#:   块级作用域
来源：http://hz.ivvv.top/gtepugqbqq.html

[C11] 模块导入与导出
来源：http://hz.tanke756.top/gtiwfyowvt.html

Py:   from module import func
来源：http://hz.yueranfly.top/gtnxzbvmpb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cdnleiting.top/gtwqkvgxsc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yongpay.top/gtqdhuqntc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gtbswsumtz.html

Java: import java.util.List;
来源：http://hz.hfpthk.cn/gtnmrtnpbe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.iojbl.cn/gtcsyeuhro.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtqhwoomhp.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtkanezbzz.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtcdkmhmvq.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtsrewrepr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj202588.top/gtgxmetizr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtrmrlfmmd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtoxxwdwca.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zycfv.cn/gtdssqowjc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hongshengwenyu.top/gtxxnnudof.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtgkzktxvh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tianlin.xyz/gttjptzrln.html

[C13] 类型声明 / 类型注解
来源：http://hz.yueranfly.top/gtjrpihnxy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj202588.top/gtfifqtpor.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtycceysoj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtxboufjhy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtqajlezus.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtdgvrkmmm.html

Go:   func add(a, b int) int
来源：http://hz.hywenlv.cn/gtefwgnzni.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtkygqgcyw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtuwyelget.html

[C14] 泛型函数
来源：http://hz.yuxming.cn/gttmsllwdy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgfzy.top/gtudcbjslp.html

PHP:  // 无泛型
来源：http://hz.fzhhl.top/gtatlmyoeu.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtorulzdqm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gthpfewxvp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.vqdsnc.cn/gtdzlzjaqa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtexyrnovz.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtcnscqdpk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gteullvkcn.html

[C15] 解构 / 展开参数
来源：http://hz.yueranfly.top/gtrtktxwcw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtwmsnqstt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtllsmmtsl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtnvohlbsq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangkeji.top/gtmizmzgbu.html

Java: // 无解构
来源：http://hz.jinqigfzy.top/gtnbvdysns.html

Go:   // 无解构
来源：http://hz.yvedp.cn/gtahxswofx.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtyidkpsje.html

C#:   var (a, b) = pair;
来源：http://hz.cdnleiting.top/gtihxbdefz.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gthpyrdogc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenlongwang.top/gtftkkkbcd.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtyugtzeig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gtxmosukgu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtqmmabmgr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtbhkmujqg.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtfzfrjpiy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtlaywhgvt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.vqdsnc.cn/gtzxpkfjhy.html

================================================================================
来源：http://hz.316326.xyz/gtxafzcdan.html

D. 数组 / 列表 / 集合
来源：http://hz.zhixingplan.top/gtjycyclqg.html

================================================================================
来源：http://hz.havefunace.top/gtpolfczne.html

[D01] 创建数组 / 列表
来源：http://hz.zhixingplan.top/gtrruwenhu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj202588.top/gtckjjleiu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gzhubu.top/gtegmwcpzt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.andypj.xyz/gteyiugfij.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gtlwzjknlx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtpkgtithh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtlwtotzsx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtakboxigm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigfzy.top/gthhxxsvac.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtwtdghzpc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pycfn.com/gtwctjlden.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtqftntecv.html

JS:   arr.push(4);
来源：http://hz.hnqzz.top/gtljdhubrg.html

TS:   arr.push(4);
来源：http://hz.sysykeji.top/gtebygjkpt.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtbpcvwizd.html

Go:   arr = append(arr, 4)
来源：http://hz.zdqjudy.top/gtroskpviv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hysaishi.cn/gtesrodeyq.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtvwwlbvzf.html

[D03] 在指定位置插入元素
来源：http://hz.bjfxy.top/gthwwdgqag.html

Py:   arr.insert(0, 0)
来源：http://hz.havefunace.top/gtafbrufza.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shangyingyoupin.top/gtvgahfcra.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.svipenyu.cn/gthireipcz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gaohongyu789.top/gtvfrjbaeb.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtfmlbdgre.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtayplenyv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pengpengdd.cyou/gtxwtpkdxc.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangkeji.top/gtbcyggypz.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtdzqxzxip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gtucvnzdui.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuetiantiany.cn/gtafflkvxo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yongpay.top/gtnqdrpnkv.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gteonnkoax.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gtjuhiezes.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtyrzndkxj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guannengcc.top/gtgbswmluv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangshuangyany.cn/gtzewgukwr.html

[D05] 访问与修改元素
来源：http://hz.pengpengdd.cyou/gtgrqskufi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtnqfquskv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gteqfnbuwp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daria6918.cn/gtscxwtwpn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtnajznrda.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.vqdsnc.cn/gtrkpkzslx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtypcobbbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gttwswzlmp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gotoacloud.top/gtjepbdszf.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gtkryggyva.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtdohhaxnw.html

PHP:  count($arr);
来源：http://hz.xingfuxueyuan.xyz/gtlhnmtpze.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtfoldwqal.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtpyxdxeus.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtsmuxayya.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtlhwkdrcf.html

Ruby: arr.length; arr.size
来源：http://hz.yonumen.top/gthbhypbqn.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtmsifafyg.html

[D07] 切片 / 取子数组
来源：http://hz.pengpengdd.cyou/gtifsearwd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.vqdsnc.cn/gttfgxjnfa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtrxciapeu.html

JS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gteaytsvty.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtzdjtkwcn.html

Java: list.subList(1, 4);
来源：http://hz.tianlin.xyz/gtzbsncrgh.html

Go:   arr[1:4]
来源：http://hz.gzhubu.top/gtjrmgxpgt.html

Ruby: arr[1, 3]
来源：http://hz.52xcode.cn/gtwqqdzjmn.html

C#:   list.GetRange(1, 3);
来源：http://hz.cucudq.cn/gtlqhpjnsj.html

[D08] 合并两个数组
来源：http://hz.quarkkingdee.top/gtxsjqpbek.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtwskdqron.html

PHP:  array_merge($a, $b);
来源：http://hz.kuanghao11.cn/gtvyhmdwsq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gotoacloud.top/gtbojifqha.html

TS:   [...a, ...b];
来源：http://hz.smart0.xyz/gtytkjlexx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhaomingkeji.xyz/gtkmwziopp.html

Go:   append(a, b...)
来源：http://hz.ydzc1.top/gtwvidewde.html

Ruby: a + b;  a.concat(b)
来源：http://hz.pycfn.com/gtyxynfvwf.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gthkmuogzp.html

[D09] 排序（升序）
来源：http://hz.shzxlz.cn/gtuunjiipm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtvxpsqmbl.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtfdebsqtn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ivvv.top/gttbtudwpd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtwfzosyoc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtikxavthm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gttwpgcgmz.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtkjvkrssg.html

C#:   list.Sort();
来源：http://hz.chenzaomai.com/gtqnleatrt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.smart0.xyz/gtxbbuwbme.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cqqwz.cn/gtoimgiozs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtvjqfzamm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtnbkglmkk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.52xcode.cn/gteggylvle.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.kuanghao11.cn/gtpgxxmtai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cucudq.cn/gtoexvojyx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtwzptqmnn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gteatansqy.html

[D11] 反转数组
来源：http://hz.gotoacloud.top/gtqsmrsijo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yvedp.cn/gtyzanpdgs.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtojwjvlrs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtmjxfitkw.html

TS:   [...arr].reverse();
来源：http://hz.birdmap.top/gtkpjxwejd.html

Java: Collections.reverse(list);
来源：http://hz.yj202588.top/gteplacdii.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtkxqppyjo.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gtjemdixyo.html

C#:   list.Reverse();
来源：http://hz.smart0.xyz/gtneqnpanc.html

[D12] 查找元素下标
来源：http://hz.yj20258888.top/gtczdrrmyx.html

Py:   arr.index(x);  x in arr
来源：http://hz.zdqjudy.top/gtbpkacjdg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tianlin.xyz/gtcgxrdacc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtuyfsevrm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhiwuduotai.top/gtdbdsmlox.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.havefunace.top/gtubcomoqj.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtrzxfjsls.html

Ruby: arr.index(x)
来源：http://hz.xinyue.icu/gtxprsjtbj.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258888.top/gtanzgsnsf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtphbncxnb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yvedp.cn/gtesoeblkk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ppjwa.cn/gteksathrg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtzjssnwpo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtrzffrkmo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guannengcc.top/gtftjvzgeb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gthqwpixfg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtmczmusyx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258888.top/gtodmtqzbo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtzglmvtik.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258.top/gtlowuniei.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtbtbebqsn.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtnnsubmdn.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtdfnqjyki.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtkpmjvmeo.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtqdypgnqr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nwbrower.top/gtudmtqtjn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtetgcdnhx.html

[D15] 去重
来源：http://hz.guannengcc.top/gtjupxuvch.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gttlyzusrn.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtpzqwoxtd.html

JS:   [...new Set(arr)]
来源：http://hz.9152youxi.cn/gtmaqsgotl.html

TS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtsdrwpihc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtbvroqfof.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangkeji.top/gtbnqeskcg.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtsevrddby.html

C#:   list.Distinct().ToList()
来源：http://hz.zhengqikj.top/gtbgihigql.html

[D16] 求和与平均值
来源：http://hz.ydjk.org.cn/gtixvqhvhf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tanke756.top/gtjhnsvijx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cqqwz.cn/gtpjeaclpi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gtwtjgmgvh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtvrxfhgcz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgufenzy.top/gthxipdleu.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtcuwjicee.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenjidiqi.icu/gtrvrzraji.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtuwiofvwx.html

[D17] 最大值与最小值
来源：http://hz.aibaodan.cn/gtbbobhvcs.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtiyjxwibw.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gtfftkxnsy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtjlydtmkg.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gttdmwsfbx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dianchejie.cn/gtygoexvzx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gtuttdyjjz.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gthgvuwwrj.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtgcghdepc.html

[D18] 扁平化嵌套数组
来源：http://hz.sufxvd.cn/gtkzjerfhz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtprapqpwd.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtjwmkztje.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gthfiykgnb.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtdczufkde.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtfjznyaxm.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtjwpcqdzy.html

Ruby: nested.flatten
来源：http://hz.xingfuxueyuan.xyz/gtzgaajxnx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtpygcuepv.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtwcpxhjng.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gthbcckrqb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gthvynotbh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fengsongda.top/gtvkhprtvo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gtluhvqbkm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtoulbdxih.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtficjnbcr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigufen.top/gtnbmgnsfk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gttfavygkk.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtyfgujewg.html

Py:   Counter(arr)
来源：http://hz.dianchejie.cn/gtiwdjtibx.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtkhkldkic.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shuidangran.top/gtohmuuisb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtqmacfhnl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangkeji.top/gtlgkhvtzx.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtnbcnynfa.html

Ruby: arr.tally
来源：http://hz.gotoacloud.top/gtbcddpbnd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shzxlz.cn/gtfmrancmu.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtdgcofrfc.html

Py:   x in arr
来源：http://hz.ivvv.top/gthveopyvg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shanyushiyangtech.top/gtgisexhnw.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtzfpnwfna.html

TS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtepgurgzb.html

Java: list.contains(x)
来源：http://hz.guannengcc.top/gtukmbqwce.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtzoeckbul.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gthcrchioy.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gtekjdtjlz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenjidiqi.icu/gtgyrxgkba.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gttoxqdlay.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtsbbxxaxu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gtshgpwnmi.html

TS:   [...arr];
来源：http://hz.chenlongwang.top/gthnbtkmgr.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtycwngdti.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtqoupnbic.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gtblwetuuz.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtfgxnqglg.html

[D23] reduce 累积计算
来源：http://hz.iojbl.cn/gtjhyefxzy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtpyctltho.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtoifuryzl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gtxpwrxhdn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtqsvnktqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtyhcelkps.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtmmeesmqd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shuidangran.top/gtbodfalot.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gthwkehhhx.html

[D24] 字典 / Map 基本操作
来源：http://hz.tian-w.cn/gthtuprhjg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gtghebrgnh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hywenlv.cn/gtnajwegyb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xuetiantiany.cn/gtxdhylzef.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ivvv.top/gtvkyukqeo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhongyouzk.top/gtywejegob.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xinyue.icu/gttgolakve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gotoacloud.top/gtojdkwydh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hammf.cn/gtrwdhaagm.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gtnppuyfxu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shuidangran.top/gtlyjcmyhj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtayetnggf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.smart0.xyz/gtqwxecnkw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenzaomai.com/gtktmyftxu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtonnhcidz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangshuangyany.cn/gtbxfwlpuu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtucitvbjp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gtzoknadjs.html

[D26] 数组转字符串
来源：http://hz.jlsjyb.cn/gtttiampva.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yangfankeji.com/gtkazlcvbi.html

PHP:  implode(", ", $arr);
来源：http://hz.zhiwuduotai.top/gtttibrafk.html

JS:   arr.join(", ")
来源：http://hz.sweek.top/gteoohqvue.html

TS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtizrfsmnw.html


<!-- 参考信息 -->