代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.birdmap.top/gtkparybtd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gtvhtrkolg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtwsulebfi.html

[C09] 递归
来源：http://hz.gogol.net.cn/gtjhwwiuqo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtoejehbdc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtmgtfitay.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtpegunsub.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtphqafehe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aizwys.cn/gtbdkafksi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.svipenyu.cn/gtnkybsnqq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtalvqpivh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gtvcbswuck.html

[C10] 变量作用域
来源：http://hz.chenzaomai.com/gtobzfsloz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gthblzvbsb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cheryme.top/gtlruoswor.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtevdshyhh.html

TS:   同 JS
来源：http://hz.tian-w.cn/gticmexqcy.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtkughaytn.html

Go:   花括号块级作用域
来源：http://hz.xylfe.cn/gtmbavdlqp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhixingplan.top/gticluhmda.html

C#:   块级作用域
来源：http://hz.gotoacloud.top/gtaubdjnft.html

[C11] 模块导入与导出
来源：http://hz.wangshuangyany.cn/gtxewcylny.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtkknelnoc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtkawmfogx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtofjoyftc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtleugkhjx.html

Java: import java.util.List;
来源：http://hz.ywan-chungtsiang.top/gtcbtpiqly.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhixingplan.top/gtmfjtqntc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtcuwgvslo.html

C#:   using System.Text;
来源：http://hz.jqgfzy.top/gtjbgqecqy.html

[C12] 立即执行函数 IIFE
来源：http://hz.iojbl.cn/gtreucibvu.html

Py:   (lambda: print("run"))()
来源：http://hz.quarkkingdee.top/gtzamhvmes.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenzaomai.com/gtjvwqzpvn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gttfxfvfez.html

TS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gtyabdwslw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtfqqlljhe.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenjidiqi.icu/gtwwmynlhy.html

Ruby: -> { puts "run" }.call
来源：http://hz.sweek.top/gtyiwbxhqg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuanzx.com/gtacldzmwp.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gtbgtfczid.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgufenzy.top/gtcintrwxi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtdhbiufud.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gtnzlftokv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtzrhgdgwb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtcrehfmlv.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gtslatvxwl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtqrziaeqf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hfpthk.cn/gtfeukglbm.html

[C14] 泛型函数
来源：http://hz.chenzaomai.com/gtiwvipwts.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtbociocyc.html

PHP:  // 无泛型
来源：http://hz.smart0.xyz/gtdzugpzfm.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gttuxipapo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shzxlz.cn/gtouuernwm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gtcvjxovjx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gtluapqjmc.html

Ruby: # 无泛型
来源：http://hz.zycfv.cn/gtckxqthez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtouxvbfws.html

[C15] 解构 / 展开参数
来源：http://hz.chenzaomai.com/gtscquaokk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.dashuyun.cn/gtegmoracd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtoxmvviim.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtnummirzy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xingfuxueyuan.xyz/gtumnccugm.html

Java: // 无解构
来源：http://hz.gzhubu.top/gtopvfscie.html

Go:   // 无解构
来源：http://hz.zdqjudy.top/gtsqzsfvnj.html

Ruby: a, b = pair
来源：http://hz.zhijiandao.cn/gtrdcmrybz.html

C#:   var (a, b) = pair;
来源：http://hz.hnqzz.top/gtyjwiwjue.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtutjzhxcv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gtfzoecqls.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gthjutzcrl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gttakdggnk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtytetvehp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gthchsdoae.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gthrulhjgo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuxming.cn/gtguxjjpcs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj202588.top/gttkmjjvma.html

================================================================================
来源：http://hz.zhoulong.xyz/gthnhswsen.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtfqixmyic.html

================================================================================
来源：http://hz.sxryk.cn/gtwfmugjeb.html

[D01] 创建数组 / 列表
来源：http://hz.yvedp.cn/gtfczaxemb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cucudq.cn/gtocgqwmfw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nwbrower.top/gtssqfswlq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydjk.org.cn/gtryekroni.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ywan-chungtsiang.top/gtxqqidysu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.birdmap.top/gtfdhqlmeo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuanzhike.top/gtolyzhper.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xinyue.icu/gtdkgtqcxn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigfzy.top/gtuaotxzso.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gtjgdoxdey.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigufen.top/gtuhvonxev.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xziqi.cn/gtvvfytriy.html

JS:   arr.push(4);
来源：http://hz.redwolf501.top/gthfuqzupx.html

TS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtxpkqnkeg.html

Java: list.add(4);
来源：http://hz.smart0.xyz/gtnjfwyhyb.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gtpnjgsqsy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sysykeji.top/gtznrlcvvo.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gtosfeipwo.html

[D03] 在指定位置插入元素
来源：http://hz.zycfv.cn/gtszngyamz.html

Py:   arr.insert(0, 0)
来源：http://hz.zhijiandao.cn/gtrdaaabpo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.birdmap.top/gtjqmwnedu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gogol.net.cn/gtgywmivgu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cqqwz.cn/gtvxwwscrd.html

Java: list.add(0, 0);
来源：http://hz.c1oappe.top/gteczgqbkb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtopjjgnpd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ivvv.top/gtmjefhudj.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtgqwrrmur.html

[D04] 删除元素
来源：http://hz.ywan-chungtsiang.top/gtdhwlxebj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.vqdsnc.cn/gtxqgwguqq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pengpengdd.cyou/gtugvugioa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dianchejie.cn/gtxuulvhze.html

TS:   arr.splice(0, 1);
来源：http://hz.0kj1m.cn/gthanzpqtw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigufen.top/gtnroohmlg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuetiantiany.cn/gtxhziwopm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zycfv.cn/gteaktayau.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtfinpbtuz.html

[D05] 访问与修改元素
来源：http://hz.zhijiandao.cn/gtnxzeptxj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtdjcdzkin.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aizwys.cn/gtkjjvoarc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtffzfqkqd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pycfn.com/gtgztjrpwf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.52xcode.cn/gtmfweucgv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gtrxaykbtk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtjdbmyfyg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtinbpifxc.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtbhevpsyn.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtbawyikgp.html

PHP:  count($arr);
来源：http://hz.chenzaomai.com/gtkrqggpxb.html

JS:   arr.length
来源：http://hz.ivvv.top/gtziyfpine.html

TS:   arr.length
来源：http://hz.xingfuxueyuan.xyz/gttcjutybf.html

Java: list.size();
来源：http://hz.sysykeji.top/gtrybywuvu.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtlcxglfsp.html

Ruby: arr.length; arr.size
来源：http://hz.yj202588.top/gtrehjkjmh.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gtegbjjlwc.html

[D07] 切片 / 取子数组
来源：http://hz.xinyue.icu/gtppqdeing.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.pycfn.com/gtilpgenxr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtfwrratuk.html

JS:   arr.slice(1, 4);
来源：http://hz.zhoulong.xyz/gtbkotftds.html

TS:   arr.slice(1, 4);
来源：http://hz.vqdsnc.cn/gtekmegfou.html

Java: list.subList(1, 4);
来源：http://hz.c1oappe.top/gtphsurrzf.html

Go:   arr[1:4]
来源：http://hz.jlsjyb.cn/gtslvlsdee.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtoptmwccr.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtpumvkytc.html

[D08] 合并两个数组
来源：http://hz.xylfe.cn/gtgsikhloi.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuetiantiany.cn/gtpqifwbfu.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtzbxmfdzj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtavwhbswz.html

TS:   [...a, ...b];
来源：http://hz.fzhhl.top/gtjduzztld.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtkbkonmok.html

Go:   append(a, b...)
来源：http://hz.jianghu66.top/gtdmjmdozi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aizwys.cn/gtsqmkuvdb.html

C#:   a.Concat(b).ToList()
来源：http://hz.kuanghao11.cn/gtlcmktabi.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtqzkqylfg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gticsrmtof.html

PHP:  sort($arr);
来源：http://hz.xingfuxueyuan.xyz/gtzqedzswr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtmdowgpyf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gtuxfzkdla.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zycfv.cn/gtwcrjtnlm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtnnayoxas.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtprigddtg.html

C#:   list.Sort();
来源：http://hz.yj20258.top/gtmzcuaqsd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shzxlz.cn/gtsfjeswov.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sweek.top/gtutvluoyz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtvncxxvro.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtkgynmgpd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtirpxpadm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydjk.org.cn/gtufniiimg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtuusefrzw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinghuilouyu.cn/gtgguqjldn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gtzusnkaqr.html

[D11] 反转数组
来源：http://hz.pycfn.com/gtmazhrpzz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shangyingyoupin.top/gtscsmzgkr.html

PHP:  array_reverse($arr);
来源：http://hz.chenzaomai.com/gtnftwpkrq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtvbdltrvp.html

TS:   [...arr].reverse();
来源：http://hz.meibo888.top/gtzbqcrffa.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtwvbulwjd.html

Go:   slices.Reverse(arr)
来源：http://hz.guowangkeji.top/gtscolyasd.html

Ruby: arr.reverse
来源：http://hz.zhixingplan.top/gtfarlqrmg.html

C#:   list.Reverse();
来源：http://hz.mhx1999.top/gtcpifxgke.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtysmqfnhs.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gtxphrmgvr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnxiangtu.top/gtcfqhsxqh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtpfahrisu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtxjsoghzg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtnslglnyn.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtahgcumbi.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtenunrdqs.html

C#:   list.IndexOf(x);
来源：http://hz.havefunace.top/gtcreooakd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fzhhl.top/gtqjojbubt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangtech.top/gtkahykykk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnqzz.top/gtfwabcigk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gtdjjrtebx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtaigujtjn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenlongwang.top/gtykwamldd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tian-w.cn/gttdyljsri.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtuuwkuccd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenjidiqi.icu/gtgcstlluy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hnqzz.top/gtgmiiiecc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gtcfaifxhl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dianchejie.cn/gtdrjbxpfi.html

JS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gtnhdtbwdu.html

TS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtqhuaxrps.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtfzbvwoeb.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtpdkfybot.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gtrqjuazvm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhijiandao.cn/gtiozmxast.html

[D15] 去重
来源：http://hz.zhiwuduotai.top/gtcsmistbh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtfscyehoz.html

PHP:  array_unique($arr);
来源：http://hz.xuetiantiany.cn/gtsnvaokbe.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtwnjjlhhv.html

TS:   [...new Set(arr)]
来源：http://hz.hysaishi.cn/gtyyvbebxc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ybcxt.top/gtwrnarnuq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuanzx.com/gtwtjdjmuf.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtyyazlxzt.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtpxmtixah.html

[D16] 求和与平均值
来源：http://hz.zhiwuduotai.top/gtnpyiejgp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.quarkkingdee.top/gtzyenecqj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtntycuyic.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtbltnzjro.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtceqlpmvu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtxbyihbvo.html

Go:   // 手写循环累加
来源：http://hz.gogol.net.cn/gtrvxrhvrw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtdmdimksv.html

C#:   list.Sum();  list.Average()
来源：http://hz.xingfuxueyuan.xyz/gttqzzxolv.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtygurwikv.html

Py:   max(arr);  min(arr)
来源：http://hz.hywenlv.cn/gtbqjsmdyo.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtvxrthnzh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenjidiqi.icu/gttwqaivak.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gtvnektlve.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zycfv.cn/gtymixdmvv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtghyuyczi.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gthedhcbdt.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtkxnwmgaz.html

[D18] 扁平化嵌套数组
来源：http://hz.zhaomingkeji.xyz/gtznxouqjy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinqigfzy.top/gtwmicvffv.html

PHP:  array_merge(...$nested);
来源：http://hz.ydjk.org.cn/gtiycvjrgw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtnusodtjl.html

TS:   nested.flat();
来源：http://hz.kuanghao11.cn/gtvggqjhze.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtycbucpce.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtarxiswlk.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtjuprdhzy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtrysjkwia.html

[D19] 按字段分组
来源：http://hz.wangdashe.top/gtqpcnpplw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnqzz.top/gttpmjojfs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.quarkkingdee.top/gtlqpypymj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tanke756.top/gtfcyyhahw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtvuptszuw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtwifbudxp.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtwpftimxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangshuangyany.cn/gtdbajsmas.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gtldzmlhcy.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtkyyrxabo.html

Py:   Counter(arr)
来源：http://hz.jqgufenzy.top/gtsdlagfli.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtbbyuarho.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gthdydcfep.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtobffackq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gaohongyu789.top/gtyxonpssn.html

Go:   // 手写 map[T]int
来源：http://hz.zhiwuduotai.top/gtlonvgvmb.html

Ruby: arr.tally
来源：http://hz.zhijiandao.cn/gtbwwqokoj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.mhx1999.top/gtcwdmtask.html

[D21] 判断是否包含某元素
来源：http://hz.guowangkeji.top/gtbgwnptyz.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtpxlpsjpy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtupymwycy.html

JS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtziovoozk.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtcqkfmksx.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtrnitupvg.html

Go:   slices.Contains(arr, x)
来源：http://hz.fengsongda.top/gtgpfnakgu.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtwclgeayf.html

C#:   list.Contains(x)
来源：http://hz.nanxuanxn.top/gtftbwdery.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtmplwcvnq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yvedp.cn/gtmwadcpxv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydzc1.top/gtvxpdoitj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gtbgaaejan.html

TS:   [...arr];
来源：http://hz.tanke756.top/gtavqqutpf.html

Java: new ArrayList<>(list);
来源：http://hz.zycfv.cn/gtrqynpura.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zdqjudy.top/gtlipjecnb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hywenlv.cn/gtyckbxnhm.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtmqbpzzys.html

[D23] reduce 累积计算
来源：http://hz.shangyingyoupin.top/gtevbfjjww.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.0kj1m.cn/gtygrrejsr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yueranfly.top/gtzobvkajr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtkduuulqb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtysgneyuh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.fzhhl.top/gttvoeevbp.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtwntedwxy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zdqjudy.top/gtebcazquu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtwhwlbhsr.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gtzpaevdtf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtjfavaedh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigfzy.top/gtnbyjmpah.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gthxycrbmp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aibaodan.cn/gtbmdfjbvj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuetiantiany.cn/gtnzruanzd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtcmzacltl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangtech.top/gtdgfxequq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.quarkkingdee.top/gtpnrcunyi.html

[D25] Set 集合去重与交并差
来源：http://hz.zycfv.cn/gtrqiwfaii.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxuanxn.top/gtysmmymqr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xinyue.icu/gtzjdpccia.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangshuangyany.cn/gtpmjnyqwt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.daria6918.cn/gttdxafqad.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigufen.top/gtwusznokj.html


<!-- 参考信息 -->