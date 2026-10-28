代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gttlwlmtts.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtbexexvhq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.9152youxi.cn/gtsvlkwreb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ivvv.top/gtmrczrbsm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhiwuduotai.top/gtbnkhydsf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtwqpnltkw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtemcdmclc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fengsongda.top/gtgnhokrer.html

[C10] 变量作用域
来源：http://hz.smart0.xyz/gtowpxnhrn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gthsznivjo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xinyue.icu/gteydnuidu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.redwolf501.top/gtowwojybq.html

TS:   同 JS
来源：http://hz.yanxiufei.cn/gtscxynddp.html

Java: 方法内为块级作用域
来源：http://hz.yj20258888.top/gtgcslgqsz.html

Go:   花括号块级作用域
来源：http://hz.gotoacloud.top/gtfrznzfnv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yangfankeji.com/gtyclrznju.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtyrdczbvw.html

[C11] 模块导入与导出
来源：http://hz.gotoacloud.top/gttcbgdywp.html

Py:   from module import func
来源：http://hz.cashguo.top/gtdqotchho.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shzxlz.cn/gtyqfvxkbg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhongyouzk.top/gtdqgqnlwp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtutldtdvj.html

Java: import java.util.List;
来源：http://hz.feifeiyinyue.top/gtbwwbpwtn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ybcxt.top/gteicjqobo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtgvxvscnt.html

C#:   using System.Text;
来源：http://hz.tian-w.cn/gtialqubpz.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhengqikj.top/gtvcivqlkx.html

Py:   (lambda: print("run"))()
来源：http://hz.hnqzz.top/gtprffybwq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenjidiqi.icu/gttqcszlhm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtdpwwmfsc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtmhfkhijh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhongyouzk.top/gtxqlasppo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aibaodan.cn/gtynwjxkjm.html

Ruby: -> { puts "run" }.call
来源：http://hz.tianlin.xyz/gtisnbxirh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.meibo888.top/gttbrfmgyr.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtcogrmoxl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenzaomai.com/gtwzuzhsow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtswwgvwmb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtjamrbdfm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtpntshast.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtmfxumoga.html

Go:   func add(a, b int) int
来源：http://hz.gogol.net.cn/gtdtdjmdaf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.meibo888.top/gtoiipbzxl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtihvxyepw.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtrhkwkibi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gzhubu.top/gtqryoghkz.html

PHP:  // 无泛型
来源：http://hz.vqdsnc.cn/gtlwwhvqjr.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtglhakynk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jlsjyb.cn/gtbjglorba.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ybcxt.top/gtyxafvbbl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cashguo.top/gtupvuyvav.html

Ruby: # 无泛型
来源：http://hz.52xcode.cn/gtvcyiptys.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gthdmtpesl.html

[C15] 解构 / 展开参数
来源：http://hz.jqgufenzy.top/gtngoeyunu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.snrcjt.cn/gtoddrxtrl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xziqi.cn/gtlghoapjn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtfbzkuaxc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gttkatfvmt.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtjzdtcscy.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtikjmohag.html

Ruby: a, b = pair
来源：http://hz.mhx1999.top/gtnklyjasn.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gtqbehmlhi.html

[C16] 函数 / 方法重载
来源：http://hz.jqgufenzy.top/gthywyrbtt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gthdfycbfi.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtfrikvxwe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtiqhafhae.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhiwuduotai.top/gtlqguezax.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtouxnorxt.html

Go:   // 无重载：用不同函数名
来源：http://hz.pengpengdd.cyou/gtpephbncb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxinkj.top/gtyqssbnmv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtwjmtpzfo.html

================================================================================
来源：http://hz.fengsongda.top/gtbcohudqk.html

D. 数组 / 列表 / 集合
来源：http://hz.aizwys.cn/gtowditrwr.html

================================================================================
来源：http://hz.tian-w.cn/gtsfordwuf.html

[D01] 创建数组 / 列表
来源：http://hz.bjfxy.top/gtkhryfqrx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtkxtpomtm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhiwuduotai.top/gtfqatrkep.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gtxdzxqzhw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gtmnaqmykf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gthnwstvjz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gttywfkeaf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jianghu66.top/gtlapzpdcl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gtwsotdzzh.html

[D02] 追加元素到末尾
来源：http://hz.nanxuanxn.top/gtnckhqpla.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gtztumeyna.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hammf.cn/gtfgkascwv.html

JS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtqsazshbe.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtcojsngwd.html

Java: list.add(4);
来源：http://hz.shzxlz.cn/gtraqroxeu.html

Go:   arr = append(arr, 4)
来源：http://hz.shzxlz.cn/gthhimtthl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gttpstzzqc.html

C#:   list.Add(4);
来源：http://hz.gotoacloud.top/gtvmwrmvkg.html

[D03] 在指定位置插入元素
来源：http://hz.ybcxt.top/gtvirgtaue.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtofdhacex.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtulnhbiil.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydzc1.top/gtlkkyynsd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tanke756.top/gtmdxhbtcb.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtfabfupqf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.mhx1999.top/gtirdjwcjz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangshuangyany.cn/gtblmoxlzg.html

C#:   list.Insert(0, 0);
来源：http://hz.xinyue.icu/gtkdhukzlu.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtmxlytxzb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.c1oappe.top/gtitdnkvfw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangkeji.top/gtdbrqpmkj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sxryk.cn/gtphqlwjos.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtcyjikaxr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ehwqpu.com/gtjpylxgpc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtehkbcwju.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtbnmtwbkm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtnwesusgs.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtgqldipog.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtwgkwjzpk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtaybntqjs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.guannengcc.top/gttgqccluw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.feifeiyinyue.top/gthxhltkkd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtmldihqvr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtwcsjsmog.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtgqyazbnj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtfsmehzfb.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtoxgybrhy.html

Py:   len(arr)
来源：http://hz.jinqigfzy.top/gtzqbckwdy.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtvjjdsmfv.html

JS:   arr.length
来源：http://hz.xylfe.cn/gtnrnmwjwm.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtjnrkudco.html

Java: list.size();
来源：http://hz.tian-w.cn/gthkxlobtc.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtrhofqbmk.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtygjuqvjy.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtpwoqasyd.html

[D07] 切片 / 取子数组
来源：http://hz.cheryme.top/gtvjohmgyp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtqtnarlvn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigfzy.top/gtkevppnnk.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtjlcprxua.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtxsitvjgc.html

Java: list.subList(1, 4);
来源：http://hz.ydzc1.top/gtslibmaqh.html

Go:   arr[1:4]
来源：http://hz.jinqigfzy.top/gtsjfzjfzu.html

Ruby: arr[1, 3]
来源：http://hz.zhaomingkeji.xyz/gtpiytzbbg.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtrorwlvcg.html

[D08] 合并两个数组
来源：http://hz.nwbrower.top/gtizktliel.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtswafyqhq.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gthtlisbwv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtrdkzbcbd.html

TS:   [...a, ...b];
来源：http://hz.jinqigufen.top/gttnmwckdh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtbgfqilzw.html

Go:   append(a, b...)
来源：http://hz.hywenlv.cn/gtslvvoipl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.iojbl.cn/gtsbduwxuf.html

C#:   a.Concat(b).ToList()
来源：http://hz.shangyingyoupin.top/gtoknpfxno.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtixrimhen.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtxnsiffel.html

PHP:  sort($arr);
来源：http://hz.birdmap.top/gtzoolmaow.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtysrqpoxy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhengqikj.top/gtiemsguqv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.haohaochexian.top/gteuppnzbo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yvedp.cn/gtxaviptox.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gthoemxggw.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gtzrrakouc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gtlsfvvyvw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtxctcheuu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangshuangyany.cn/gtarwbfebf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtitgnnygq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtgsurcvhq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtfsmtsmtn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnqzz.top/gtefylfcws.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangkeji.top/gtearicyrf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dianchejie.cn/gtrdxksukr.html

[D11] 反转数组
来源：http://hz.dashuyun.cn/gtuucckkyl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ywan-chungtsiang.top/gtpqmogwrd.html

PHP:  array_reverse($arr);
来源：http://hz.yonumen.top/gtejzmdkmk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxinkj.top/gtwwgudpjm.html

TS:   [...arr].reverse();
来源：http://hz.zhiwuduotai.top/gthczdnujx.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtuwsnxzpj.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtrioemmsi.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gtqhmxacln.html

C#:   list.Reverse();
来源：http://hz.zycfv.cn/gtnqdokgte.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gttpliqyah.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtdkdotfac.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtsoplqesc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuetiantiany.cn/gtdtmofdgo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtpbgtcdxn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gttpyyuynl.html

Go:   slices.Index(arr, x)
来源：http://hz.tianlin.xyz/gtgopfrrpi.html

Ruby: arr.index(x)
来源：http://hz.yuxming.cn/gtcrfgnbfj.html

C#:   list.IndexOf(x);
来源：http://hz.yanxiufei.cn/gtuvliggrp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnxiangtu.top/gtjlhmugen.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtzuivparu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gzhubu.top/gtjjfslfwa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtpjwwomig.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtheulunxc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtoobwgjwo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daria6918.cn/gtqnabzena.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gtvjezvdyh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.52xcode.cn/gtkzkyuzqi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenlongwang.top/gtbukzxpor.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xziqi.cn/gteyisldkk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gtqprfpwop.html

JS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtewkrsycs.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtfmoqpnuv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhongyouzk.top/gtjosqiefx.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtapjgmchm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gtkdblccwq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.316326.xyz/gtegclatcm.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtqirrzpkk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtekjshvqz.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtwzrkqduz.html

JS:   [...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtiroddqfj.html

TS:   [...new Set(arr)]
来源：http://hz.hysaishi.cn/gtlyehtdmo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtbnwjtnry.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hysaishi.cn/gthauyicjv.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtguiufgpp.html

C#:   list.Distinct().ToList()
来源：http://hz.jiagoushi.top/gtsbmfosyz.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtovuoybkq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nwbrower.top/gtaihhxejp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtchwnvxtu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtjshxymyu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtwqrcqrbd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cashguo.top/gtmhsuvbvm.html

Go:   // 手写循环累加
来源：http://hz.zycfv.cn/gtkdcbchww.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydjk.org.cn/gtspiiqrjo.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtwwvbqtvj.html

[D17] 最大值与最小值
来源：http://hz.ywan-chungtsiang.top/gtcfadllfk.html

Py:   max(arr);  min(arr)
来源：http://hz.dashuyun.cn/gtxgdjnmva.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gtgjvuoove.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtvujfmqgi.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtmprsmira.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.52xcode.cn/gtaultoffj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gtndckccxq.html

Ruby: arr.max;  arr.min
来源：http://hz.ywan-chungtsiang.top/gtawftequo.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtcmceliny.html

[D18] 扁平化嵌套数组
来源：http://hz.sxryk.cn/gtueqkyliw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pycfn.com/gttlifeigq.html

PHP:  array_merge(...$nested);
来源：http://hz.yvedp.cn/gtvlkshebg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtwpdwtjjs.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gtxatotzln.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gtyrbteaki.html

Go:   // 手写双层循环
来源：http://hz.316326.xyz/gtrckeeris.html

Ruby: nested.flatten
来源：http://hz.guannengcc.top/gtujcyljdc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtkoeyxfck.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gttfrnstzv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtzmhxvhse.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydjk.org.cn/gtbnomvoey.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.feifeiyinyue.top/gtuzdqvnxo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtpyjalupi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fengsongda.top/gtpcyfncbe.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gteuiwxtec.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuanzhike.top/gthmphsbmk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtdvnxbaus.html

[D20] 统计每个元素出现次数
来源：http://hz.zhiwuduotai.top/gtrsqklbcd.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gtscinpxis.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtvjphlqyi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtrrtpjrhg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtkhugiqxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hnxiangtu.top/gtexcqvvry.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtcomaegvr.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gthloqrpmf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtyfercuxp.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtlywdnunc.html

Py:   x in arr
来源：http://hz.hammf.cn/gtgvtjpycv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtgneodeiq.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtpruchwfo.html

TS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gttnnvexij.html

Java: list.contains(x)
来源：http://hz.bjfxy.top/gtjjzhuwkq.html

Go:   slices.Contains(arr, x)
来源：http://hz.aizwys.cn/gtinuzbpmv.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtpdezwdiq.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtmubjmugc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtaisumgik.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtvdinagch.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtlnefohwa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtvfmogxox.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtcyvrnzvx.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtcytcpyda.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtxhxssgqg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ivvv.top/gtzncgewgg.html

C#:   new List<int>(list);
来源：http://hz.9152youxi.cn/gtdjlykmqe.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtxhjhshjx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.feifeiyinyue.top/gtvqwueqge.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.mhx1999.top/gtsoesyvqy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtoeseqcwp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtsxrtetbn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.andypj.xyz/gtwturfqkb.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtvahgrmnv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gthvruzvpq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtujdfdduf.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtqrjboryt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.havefunace.top/gtcidxwwfu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtncwsbqhp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gtdefbhghg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.52xcode.cn/gtwxtuswfg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtuwyyutdo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.snrcjt.cn/gtvmqmvsqm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.svipenyu.cn/gtkdqzhtet.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.haohaochexian.top/gtrmsbufdg.html

[D25] Set 集合去重与交并差
来源：http://hz.gogol.net.cn/gtroncelqs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hysaishi.cn/gtburbfcca.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.pengpengdd.cyou/gtzuywbmxe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shangyingyoupin.top/gtvfgaokkm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zycfv.cn/gtlgwcgyio.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtqsuoqsgm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aibaodan.cn/gtxptkunmm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gtmohfuddb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtznbuftei.html

[D26] 数组转字符串
来源：http://hz.andypj.xyz/gtqwjbdckt.html


<!-- 参考信息 -->