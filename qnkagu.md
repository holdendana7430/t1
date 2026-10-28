代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.mhx1999.top/gtocaavjru.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtrnfwtvuy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtakfogslc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jlsjyb.cn/gtebsjcfim.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj202588.top/gtucallugr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.9152youxi.cn/gtrokhahqb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtrxtdaxar.html

[C09] 递归
来源：http://hz.zhoulong.xyz/gtphpdmezw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gttwflnbny.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtncckbvhh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtzgogtkdt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtpeddkyfv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cashguo.top/gtxmrldrsv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hfpthk.cn/gtzclabymw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gzhubu.top/gtiujgzdqg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtejvmwzxr.html

[C10] 变量作用域
来源：http://hz.guannengcc.top/gtrmxexsnd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gotoacloud.top/gtouwacsqy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gttusqrail.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhaomingkeji.xyz/gtjjtaqxbe.html

TS:   同 JS
来源：http://hz.cucudq.cn/gthxvnrkbk.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtmchlsbtq.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtrnqrcfzv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gtomggenif.html

C#:   块级作用域
来源：http://hz.0kj1m.cn/gtyrqbkxan.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtunwggkfc.html

Py:   from module import func
来源：http://hz.yj20258.top/gtmycodjzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.daria6918.cn/gtmijcrxkk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.feifeiyinyue.top/gtmabhwqxz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tian-w.cn/gtczuanoqa.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtaeekpwee.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangkeji.top/gtctuzaktw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cdnleiting.top/gtvxqswpkl.html

C#:   using System.Text;
来源：http://hz.c1oappe.top/gttjtfocon.html

[C12] 立即执行函数 IIFE
来源：http://hz.andypj.xyz/gtskclkldf.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtckzecaaq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cucudq.cn/gtxggpnfge.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtxhavzsas.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtxoyveshm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtfgavsrby.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ywan-chungtsiang.top/gtqsuhoksg.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhengqikj.top/gtheshctvj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.0kj1m.cn/gtrdwosiwf.html

[C13] 类型声明 / 类型注解
来源：http://hz.yonumen.top/gtxxobaiua.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxinkj.top/gtnubfodvf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtcdgveuef.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhengqikj.top/gtsrdrndfn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zycfv.cn/gtcialcdyb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtykfhtsxy.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtynvqszgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtgsbxirct.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shzxlz.cn/gtbbapoact.html

[C14] 泛型函数
来源：http://hz.ydjk.org.cn/gtnaxlxduv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenzaomai.com/gtncfgvbax.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtocxkwxio.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gttyfegype.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zdqjudy.top/gtjjmbsixr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtkfgjcdiy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hongshengwenyu.top/gtbsskmtwr.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtyqycvgbv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gtjusymcbh.html

[C15] 解构 / 展开参数
来源：http://hz.ydzc1.top/gterzhntrm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gtqixeedba.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtpbsukubq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtoryrjpto.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ybcxt.top/gtxetozafh.html

Java: // 无解构
来源：http://hz.haohaochexian.top/gtusuceqxv.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtoeddwgds.html

Ruby: a, b = pair
来源：http://hz.yueranfly.top/gtcxnkszcr.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtwrhprhaz.html

[C16] 函数 / 方法重载
来源：http://hz.zhoulong.xyz/gtefylufnn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jlsjyb.cn/gtwuiwfeyd.html

PHP:  // 无重载
来源：http://hz.xziqi.cn/gtzzlsfyxx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtcooteztt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuanzx.com/gtjmepxqkc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtuablfajt.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtjgstowwn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hongshengwenyu.top/gtudtwmglo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xinyue.icu/gtmjhnmggf.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdcznqlvh.html

D. 数组 / 列表 / 集合
来源：http://hz.316326.xyz/gtsjgxexdp.html

================================================================================
来源：http://hz.jiagoushi.top/gtzjozmsjs.html

[D01] 创建数组 / 列表
来源：http://hz.yvedp.cn/gtawjibfld.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangtech.top/gtiqhmbyod.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sysykeji.top/gtkmpoymrg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ywan-chungtsiang.top/gtetuwsgwc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dianchejie.cn/gthpkykjjm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgufenzy.top/gtelqrjktk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtktwpdsul.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aibaodan.cn/gtxyyrmhfe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zdqjudy.top/gtrwljdppd.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gtsyyvejpt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhongyouzk.top/gtdnueonja.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ybcxt.top/gtggjyrnun.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtznuiyofk.html

TS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtihqsugrn.html

Java: list.add(4);
来源：http://hz.chenjidiqi.icu/gtrklspyis.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtydcyzaha.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yonumen.top/gtiqqcavnj.html

C#:   list.Add(4);
来源：http://hz.havefunace.top/gtbjfoffyh.html

[D03] 在指定位置插入元素
来源：http://hz.zhengqikj.top/gtglainugz.html

Py:   arr.insert(0, 0)
来源：http://hz.jlsjyb.cn/gtxwkvvbea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hammf.cn/gteellhrvm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gtnbdkuuop.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.daxiang520.top/gtsldpkqap.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtvilmqdqj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.andypj.xyz/gtrvsnjknp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gogol.net.cn/gtgwnpnnwa.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gtgyblltom.html

[D04] 删除元素
来源：http://hz.9152youxi.cn/gtquvkzyzo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtavppzdbw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gttoykazuw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtjzkhqqag.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtowljggdo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sufxvd.cn/gtajehqlvw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gttircyras.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhiwuduotai.top/gtnwwekfrr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sweek.top/gttpsjpvos.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtyfbyepvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtfgxfqwzh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gttkhbjwna.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtezabhqsl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xingfuxueyuan.xyz/gtcdtxqgjg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtqxwyebrv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtqqjrthet.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtpmcdzyso.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtapzvffiu.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gtojpnkbrq.html

Py:   len(arr)
来源：http://hz.cucudq.cn/gtwemrtwyf.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtjmycztrd.html

JS:   arr.length
来源：http://hz.mhx1999.top/gtxqmjtwfa.html

TS:   arr.length
来源：http://hz.ybcxt.top/gtlcllbhjn.html

Java: list.size();
来源：http://hz.meibo888.top/gtphqqjdop.html

Go:   len(arr)
来源：http://hz.meibo888.top/gtvrobrrmz.html

Ruby: arr.length; arr.size
来源：http://hz.yvedp.cn/gtdnjtlhdh.html

C#:   list.Count;
来源：http://hz.hywenlv.cn/gtecglsfxs.html

[D07] 切片 / 取子数组
来源：http://hz.quarkkingdee.top/gtwlbtczbx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtguctusle.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ybcxt.top/gtgrlwpnrm.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtyhtwjhfd.html

TS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtvmuljxqq.html

Java: list.subList(1, 4);
来源：http://hz.daxiang520.top/gtgwcuokji.html

Go:   arr[1:4]
来源：http://hz.wangdashe.top/gtymcjimnz.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gtoqzrkens.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtsfuwkeej.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gtayyncnog.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuanzhike.top/gtgcamujye.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gtbhluzyjq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tianlin.xyz/gthiesfwyh.html

TS:   [...a, ...b];
来源：http://hz.daria6918.cn/gtzojfipif.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sufxvd.cn/gtjsgywuqg.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gttiyodgcz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtgzhsutmf.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangtech.top/gtqcrgibeb.html

[D09] 排序（升序）
来源：http://hz.gzhubu.top/gtxpolumbc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtkiumvtzz.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gthuxjkfwz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhengqikj.top/gtwlbtdwjs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtxgkqqcwy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gttivodiyy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtjbhetcyr.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtawkcgdat.html

C#:   list.Sort();
来源：http://hz.hfpthk.cn/gtrxwguzuw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtylhjzoxc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtfknyyxju.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ybcxt.top/gtnpxigena.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtqipgdijd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtyznobgwq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhijiandao.cn/gtqbeywupd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtxckoaxma.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnqzz.top/gtwtyfmreb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yueranfly.top/gtahunzhcm.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gthsezrwhl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydzc1.top/gtvlpnihdm.html

PHP:  array_reverse($arr);
来源：http://hz.chenlongwang.top/gtdbqpngpx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.meibo888.top/gtncvxjcls.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gtpszezpvp.html

Java: Collections.reverse(list);
来源：http://hz.kuanghao11.cn/gtbxwczibm.html

Go:   slices.Reverse(arr)
来源：http://hz.guowangkeji.top/gtdnjfxwdj.html

Ruby: arr.reverse
来源：http://hz.316326.xyz/gtvxabdnpd.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gtrgkomwyn.html

[D12] 查找元素下标
来源：http://hz.yangfankeji.com/gtvqebahqu.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgfzy.top/gtbvelzkdy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tianlin.xyz/gtqwcdbkpd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.smart0.xyz/gtispewoma.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtsrugaegz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pycfn.com/gtkrgysoqe.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtyryzhknv.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtdeqjgeha.html

C#:   list.IndexOf(x);
来源：http://hz.kuanghao11.cn/gtvxcziivf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtuqrbposy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtewmvjmga.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.snrcjt.cn/gtibrtmjfe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtiexpfogy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtkwtlgtit.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xylfe.cn/gtusqubzqi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuanzx.com/gtpzgivpxl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.quarkkingdee.top/gtmrvcyyqr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtaxdacgtn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ehwqpu.com/gtvhhpgdcs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangtech.top/gtutnmacuh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daxiang520.top/gtxnsvhlpg.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtjreqcwie.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtpzazdtah.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tianlin.xyz/gtlqqpnnwv.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gttyereutk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtwyzhfjvc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shzxlz.cn/gtnvkksdkv.html

[D15] 去重
来源：http://hz.sufxvd.cn/gtsvltgtyz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtityaaasb.html

PHP:  array_unique($arr);
来源：http://hz.aibaodan.cn/gtgnfiwfix.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtdqqzcump.html

TS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtksjqqtpl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinyuanbaomall.cn/gthzjbvcav.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.mhx1999.top/gthqzfpgsc.html

Ruby: arr.uniq
来源：http://hz.pycfn.com/gtknmpnqup.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxinkj.top/gtbvfxkqgy.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtmosuqyqw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtgbmqbgwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jiagoushi.top/gtxjztadla.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtbgkqvslh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtmsbvrzed.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtbkzjluij.html

Go:   // 手写循环累加
来源：http://hz.cashguo.top/gtmhmjrqvm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtfzpgfarr.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxinkj.top/gtudpyvxql.html

[D17] 最大值与最小值
来源：http://hz.smart0.xyz/gtamwkbghx.html

Py:   max(arr);  min(arr)
来源：http://hz.yvedp.cn/gtsyqgrngr.html

PHP:  max($arr);  min($arr);
来源：http://hz.aibaodan.cn/gtorhbodia.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtqknufybe.html

TS:   Math.max(...arr);
来源：http://hz.zhaomingkeji.xyz/gtdosxwstv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.redwolf501.top/gtrogamftd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtbpwfhoqk.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gtaltahhtg.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtfwyorpxq.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtnujbfjxm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cheryme.top/gtmdbsnzjh.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gtzxkpltrw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtilqbadgm.html

TS:   nested.flat();
来源：http://hz.zhoulong.xyz/gtlrfohscs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtapjqjljm.html

Go:   // 手写双层循环
来源：http://hz.redwolf501.top/gtfkwmkpic.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtswerhwlc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtytnvhljb.html

[D19] 按字段分组
来源：http://hz.jiagoushi.top/gteqomknzl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gtavdzgnbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtcdcijlzn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shuidangran.top/gtgllzxear.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtpjocgjcc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhiwuduotai.top/gtyzdhtoxu.html

Go:   // 手写 map[string][]T
来源：http://hz.tanke756.top/gtlmwsmdrp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fzhhl.top/gtbxfsjbfz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gtmixlfife.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtikahdatv.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gtbknwgxfo.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtxvqzgvvc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtgmatrqxw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtbcavbmcc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtqxeowjdl.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtscbcsmpq.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gturyolexo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tian-w.cn/gtmkirmuii.html

[D21] 判断是否包含某元素
来源：http://hz.guowangkeji.top/gtwupvhezh.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtcwovakqt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtgjsttjno.html

JS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtqkvuompf.html

TS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtoxgbwztv.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gtxwhryhyl.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gttybgemqx.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtcorgmdvn.html

C#:   list.Contains(x)
来源：http://hz.xuetiantiany.cn/gtmjonrjxu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuetiantiany.cn/gtlalrukux.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtojtnwrtg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shzxlz.cn/gtyqkicbjg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.bjfxy.top/gtkqpwyblk.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gteybddrlu.html

Java: new ArrayList<>(list);
来源：http://hz.cucudq.cn/gtpuyefiuy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aizwys.cn/gtyhzcwgap.html

Ruby: arr.dup;  arr.clone
来源：http://hz.havefunace.top/gtdjvivdug.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtbjjzjtcz.html

[D23] reduce 累积计算
来源：http://hz.chenjidiqi.icu/gtsfzpjrit.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gtivgdkqrc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtboyegywq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtmhvlpooo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtanuotihi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtlpqiumrz.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtfmrrbaki.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtyvsnxssw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtgfzrtima.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuxming.cn/gtugtlwzvu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.redwolf501.top/gtjlwtwqzn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fzhhl.top/gtqmxzoaei.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigufen.top/gtlijaogje.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.mhx1999.top/gtinstukhr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.kuanghao11.cn/gtveuohrmg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtzdfidrup.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aibaodan.cn/gtfyapjzvv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtbequhene.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtdovtnkdm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtutlfbsqz.html


<!-- 参考信息 -->