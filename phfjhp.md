代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xziqi.cn/gtoxinoxya.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gtbganuuic.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtzzynmowk.html

[C09] 递归
来源：http://hz.ywan-chungtsiang.top/gtjazktjpg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtngtgkcyt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenjidiqi.icu/gtsiwwtkys.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtnngjxjtn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtvwsipfuh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shangyingyoupin.top/gttdhxpdtg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtfcqocldf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nwbrower.top/gtjtrjbbpb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gaohongyu789.top/gtgbhynwly.html

[C10] 变量作用域
来源：http://hz.jinghuilouyu.cn/gtxhyxeeab.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtmyicnghf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtxaorbtdr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xinyue.icu/gtzkmqygev.html

TS:   同 JS
来源：http://hz.gzhubu.top/gtqqunnmof.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gthelqekiz.html

Go:   花括号块级作用域
来源：http://hz.cheryme.top/gtykvtuyjt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtrnhzhdjy.html

C#:   块级作用域
来源：http://hz.shanyushiyangkeji.top/gtyieqeknj.html

[C11] 模块导入与导出
来源：http://hz.52xcode.cn/gtfruycmdg.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gtdmfhbxwu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sysykeji.top/gtvjaahspf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guowangkeji.top/gttrhvhxeo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ppjwa.cn/gtpitdswnl.html

Java: import java.util.List;
来源：http://hz.gzhubu.top/gtdzrskcdq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jlsjyb.cn/gtcehqratj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtvoupnmxn.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtwjmuthfj.html

[C12] 立即执行函数 IIFE
来源：http://hz.52xcode.cn/gtorydfqbx.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtomjdskhz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtxchdanwe.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gthflympqh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hongshengwenyu.top/gtoflxzizn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhixingplan.top/gtpgjbhtom.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xylfe.cn/gtivwiyusi.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtseuiuiyr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sysykeji.top/gtofbiczuj.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtyvlaqtit.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sxryk.cn/gtcmfbmksf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtdywdbfks.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.c1oappe.top/gthxtvmmot.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtydxupywy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtbiwjbayp.html

Go:   func add(a, b int) int
来源：http://hz.hnqzz.top/gtudnrwgoh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fengsongda.top/gttdfnnmap.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gtokpaqifm.html

[C14] 泛型函数
来源：http://hz.ydjk.org.cn/gtryexudri.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.snrcjt.cn/gtiscpyhga.html

PHP:  // 无泛型
来源：http://hz.jinqigufen.top/gtdlctglqx.html

JS:   // 无泛型
来源：http://hz.gogol.net.cn/gtzzortmoi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gtotwgecsp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.andypj.xyz/gtpsrnsslf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yangfankeji.com/gtdrrpwguh.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gtpdkvqujs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hnxiangtu.top/gtazbhahvf.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtpbxzrwqe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.meibo888.top/gtzniffoyg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daria6918.cn/gtlowwvbol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtjcwwobts.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtkykwblaa.html

Java: // 无解构
来源：http://hz.iojbl.cn/gtvnudrfpp.html

Go:   // 无解构
来源：http://hz.yvedp.cn/gtqkedissl.html

Ruby: a, b = pair
来源：http://hz.andypj.xyz/gtojweqnuq.html

C#:   var (a, b) = pair;
来源：http://hz.jinghuilouyu.cn/gtxmlxqyrb.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtbqlfmfib.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.havefunace.top/gtoghsnymg.html

PHP:  // 无重载
来源：http://hz.ivvv.top/gtgwqeaczy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtfcwoujmz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gtmintbomh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenzaomai.com/gtyhlrlcbp.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtucdmfodd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xylfe.cn/gtuamylxai.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sysykeji.top/gtlxyxldhj.html

================================================================================
来源：http://hz.xuanzx.com/gteetgxwwv.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtasnybwno.html

================================================================================
来源：http://hz.guowangkeji.top/gthbkfpcuz.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtiigbywls.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guannengcc.top/gtldhpxvrp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigufen.top/gtyudmnmpk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtmdpmcjxq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.redwolf501.top/gtoqiycxhk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sufxvd.cn/gtadueheun.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yueranfly.top/gtbnzsxcpx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.mhx1999.top/gtflzzxuew.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gthlwtdody.html

[D02] 追加元素到末尾
来源：http://hz.hongshengwenyu.top/gtunetlyko.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtioizdmdd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.9152youxi.cn/gtvfnvuhvf.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtkkivgqrl.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gthohhizfl.html

Java: list.add(4);
来源：http://hz.dashuyun.cn/gtgopdnjed.html

Go:   arr = append(arr, 4)
来源：http://hz.tanke756.top/gtnokxywtr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.52xcode.cn/gtvjankmsz.html

C#:   list.Add(4);
来源：http://hz.xylfe.cn/gtrucjiyqc.html

[D03] 在指定位置插入元素
来源：http://hz.kuanghao11.cn/gtdfqzzlag.html

Py:   arr.insert(0, 0)
来源：http://hz.daxiang520.top/gtlfqrtalo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gttvztcqwh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtcknlhbyt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jlsjyb.cn/gthvfcnydq.html

Java: list.add(0, 0);
来源：http://hz.yongpay.top/gtwlwqlbct.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nwbrower.top/gtgrxpzdyi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.dianchejie.cn/gtabzkxsgn.html

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gthnyzjrks.html

[D04] 删除元素
来源：http://hz.daria6918.cn/gtmkavtqhd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangshuangyany.cn/gtslutkoir.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fengsongda.top/gtuoaxgyxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.snrcjt.cn/gtkifqlvam.html

TS:   arr.splice(0, 1);
来源：http://hz.redwolf501.top/gtvqxljuvl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gtscdsvwbv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gtlythdymg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yanxiufei.cn/gthwkjfclg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tian-w.cn/gtsadpubco.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gtdpguceok.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtqwtkxpci.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtonwfqsuc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtxitforez.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtdjslttbg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtvhdzmoba.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtylvbiosm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtcjepplbw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.snrcjt.cn/gtznfkotag.html

[D06] 数组长度
来源：http://hz.aibaodan.cn/gtyyogujxw.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtwgoepirb.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gtgusndzmo.html

JS:   arr.length
来源：http://hz.ppjwa.cn/gtfyidqqye.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gtwapvckhi.html

Java: list.size();
来源：http://hz.jinqigufen.top/gtbatckakd.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtmlskpziy.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtlbfgtikq.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtfseqolsk.html

[D07] 切片 / 取子数组
来源：http://hz.hfpthk.cn/gtgdwvuaxx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtrvqzjgec.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fzhhl.top/gtemuohwfz.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtucfuxjir.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gthmmkzqry.html

Java: list.subList(1, 4);
来源：http://hz.nanxinkj.top/gtsxephtvs.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtpqfuchfv.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gtlndzogni.html

C#:   list.GetRange(1, 3);
来源：http://hz.c1oappe.top/gtzfiiiszo.html

[D08] 合并两个数组
来源：http://hz.dashuyun.cn/gtnsepjdmp.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtrtiiinhr.html

PHP:  array_merge($a, $b);
来源：http://hz.sweek.top/gtalmsmndc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gthhfhdmlu.html

TS:   [...a, ...b];
来源：http://hz.nanxuanxn.top/gtzefdxtqt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.meibo888.top/gtscouzwnu.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtfbornvxu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhixingplan.top/gtmqenraxl.html

C#:   a.Concat(b).ToList()
来源：http://hz.dashuyun.cn/gtinogzlaz.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtsxqagyng.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtvmvioiob.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtknkgkfbx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258888.top/gtnqmgukkk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.vqdsnc.cn/gtneyzvkoi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xingfuxueyuan.xyz/gtxvffwjai.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtogdawdkm.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtyegcsjfe.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtsutxygxs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigfzy.top/gtgyoxlqbe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daria6918.cn/gtkzvfyhnc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gtivvpowpg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtvowkrveu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtaioizzkj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtuiegfwcd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.52xcode.cn/gtzfbbhbws.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zycfv.cn/gtuhzuwudi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtoasyefjl.html

[D11] 反转数组
来源：http://hz.vqdsnc.cn/gtrbtraxrz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtrnfjivcq.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gtjzfxqrko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.vqdsnc.cn/gtiiuugyyr.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtweoyuuzm.html

Java: Collections.reverse(list);
来源：http://hz.smart0.xyz/gtwopwnhfi.html

Go:   slices.Reverse(arr)
来源：http://hz.quarkkingdee.top/gtujmjpdlm.html

Ruby: arr.reverse
来源：http://hz.iojbl.cn/gtnzfrtqen.html

C#:   list.Reverse();
来源：http://hz.ppjwa.cn/gtvlobtxyp.html

[D12] 查找元素下标
来源：http://hz.xuetiantiany.cn/gtdlnrpyxg.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtktesjpox.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sxryk.cn/gtyupvqrlk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtsdxrtubk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtselfawlj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtfgzrsuke.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gtyguimykv.html

Ruby: arr.index(x)
来源：http://hz.tian-w.cn/gtucuiplsx.html

C#:   list.IndexOf(x);
来源：http://hz.jyoumei.cn/gtgnpxmziu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xziqi.cn/gthiyrpesl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtdsmmilpy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yonumen.top/gtooviomxx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gttlqxfedr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtcgbfuuad.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtxjdyvomi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gttmbtqyag.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fzhhl.top/gtlmictnfw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gtjujkbpsp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zycfv.cn/gtbnswkvwo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xziqi.cn/gtbbalslxm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gtgwyzcvce.html

JS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtnzearawm.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gthbcqtwds.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtaocrxobr.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gttobndjbs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj202588.top/gtqdlcbtma.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtarxlbgtu.html

[D15] 去重
来源：http://hz.daxiang520.top/gtqiwbymzv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtrlcvvism.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtqihhdfmt.html

JS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtaxnjxzqu.html

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtggmsekjl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hongshengwenyu.top/gtsvwjkmcz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtuasdppoc.html

Ruby: arr.uniq
来源：http://hz.iojbl.cn/gttgduskpt.html

C#:   list.Distinct().ToList()
来源：http://hz.yj202588.top/gtsyqagsql.html

[D16] 求和与平均值
来源：http://hz.quarkkingdee.top/gtcbhtbbsq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hywenlv.cn/gtszllmcwi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aizwys.cn/gtvzlpwiit.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtoyhkqrnr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtltykgwsx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtpprbluyr.html

Go:   // 手写循环累加
来源：http://hz.chenzaomai.com/gtvvvydkrp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zdqjudy.top/gtwulllntk.html

C#:   list.Sum();  list.Average()
来源：http://hz.bjfxy.top/gtaxpkaowc.html

[D17] 最大值与最小值
来源：http://hz.9152youxi.cn/gtzrqugerv.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtjrrfjbvj.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigfzy.top/gtmpbtwxzw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yongpay.top/gtrdoyxxhy.html

TS:   Math.max(...arr);
来源：http://hz.jlsjyb.cn/gtecthmjkv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenjidiqi.icu/gtertknwhq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtjqmunpik.html

Ruby: arr.max;  arr.min
来源：http://hz.havefunace.top/gtqoqvrybm.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gthzudboah.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtqbvhpspv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daria6918.cn/gtokontelw.html

PHP:  array_merge(...$nested);
来源：http://hz.feifeiyinyue.top/gtqqlajmhs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtcfpwdnjj.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtowotlamu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinghuilouyu.cn/gthokdeilp.html

Go:   // 手写双层循环
来源：http://hz.zhiwuduotai.top/gtceofndcb.html

Ruby: nested.flatten
来源：http://hz.andypj.xyz/gtrrkrptjo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhiwuduotai.top/gtqahyhyvs.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtsltvdkvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtkexvmdmm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.0kj1m.cn/gtosykymph.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.meibo888.top/gtotmzmjfm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gtafdwvemb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yangfankeji.com/gtaztfryvj.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtjlpzuvxc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yangfankeji.com/gtrhjerukz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuanzx.com/gtecmwjakd.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtcyecvvpd.html

Py:   Counter(arr)
来源：http://hz.meibo888.top/gtytnjkpqg.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtmtwmkzqs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gthlczvmna.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtpojudoie.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gthzvikjat.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtpfbxxuxk.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtsykdqbfp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtrhvyfpve.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtxobcuede.html

Py:   x in arr
来源：http://hz.iojbl.cn/gtgashufrg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtyeriqpts.html

JS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gttqbkfsqo.html

TS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtotkagcjv.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtawgimbqr.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtihhvgpwi.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtvhwbngnr.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtlqsnaphy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.vqdsnc.cn/gtmihngkmf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgufenzy.top/gtxxjmcdme.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtfukmlrpt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtrvvyhfqx.html

TS:   [...arr];
来源：http://hz.daria6918.cn/gtvnirdtnk.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gttcmwkqsa.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtotzgglsp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guowangkeji.top/gtzpnqtozz.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gtghzyxxyx.html

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gtdmodfqwd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gtbcdsshyu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gtvcteltme.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtvomtjkno.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtfvhvhzuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhiwuduotai.top/gtuciddfoj.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtyyazwnll.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.iojbl.cn/gtsvindkbg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yvedp.cn/gtjoqdvrdz.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtgkpywred.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtihumpkmn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gtrimakhiz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtwgrzlknb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gtgozfpucs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.0kj1m.cn/gtsyvmdgua.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtgwxgsmdj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zycfv.cn/gtghoazfzl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhongyouzk.top/gtdtrxrjyx.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gtulqtjtro.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gttethgvkz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtfixoxgqt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtpomwzwyy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtypazvbvs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtyqtdikhp.html


<!-- 参考信息 -->