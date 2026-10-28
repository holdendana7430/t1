代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ehwqpu.com/gtkyvhfpcd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtnsderffl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtuxrdcdck.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yongpay.top/gtxblqbeah.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jlsjyb.cn/gthjwrvede.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hongshengwenyu.top/gtvqoayoyl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtggfedllu.html

[C09] 递归
来源：http://hz.shzxlz.cn/gteggdkyyy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxuanxn.top/gtmwehpokz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sysykeji.top/gtkqdaxvpx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.svipenyu.cn/gtehpquvjk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cqqwz.cn/gtxbcdfakm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gogol.net.cn/gtnpyaqjbi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhoulong.xyz/gtkkuxxyae.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtakzonxhg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ywan-chungtsiang.top/gtzsjxycku.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtmlhrdgku.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenlongwang.top/gthcyvdikg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tianlin.xyz/gtzjeaoheg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtusttqkwh.html

TS:   同 JS
来源：http://hz.svipenyu.cn/gtlsltzgbg.html

Java: 方法内为块级作用域
来源：http://hz.svipenyu.cn/gtfpbnoqbi.html

Go:   花括号块级作用域
来源：http://hz.sysykeji.top/gtfzahhdyi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tianlin.xyz/gtretbrwlz.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gttihdpolx.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtxfricobu.html

Py:   from module import func
来源：http://hz.shangyingyoupin.top/gtgztdpniu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.svipenyu.cn/gtztfbxtry.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cqqwz.cn/gtkhzdwxfw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhoulong.xyz/gtlybmwcau.html

Java: import java.util.List;
来源：http://hz.yangfankeji.com/gtkztrattk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.iojbl.cn/gtgxugfuhr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shzxlz.cn/gtfkadjlcb.html

C#:   using System.Text;
来源：http://hz.pycfn.com/gtpafvprtn.html

[C12] 立即执行函数 IIFE
来源：http://hz.kuanghao11.cn/gtplqxtmtj.html

Py:   (lambda: print("run"))()
来源：http://hz.cdnleiting.top/gtkhcjyiyw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtnfkmtupt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gtkqvtusck.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtwpxlagou.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtbnzcjivd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gthpatotnc.html

Ruby: -> { puts "run" }.call
来源：http://hz.sweek.top/gttyamussd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtfakkkqze.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gthrihhmyx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yanxiufei.cn/gtnkvkrsdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtsvwkldng.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtlskcytvq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtdnjcmjnr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtkkhietcz.html

Go:   func add(a, b int) int
来源：http://hz.fzhhl.top/gtqwqzjvid.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dashuyun.cn/gtwpmjlawe.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ivvv.top/gtbelaamcr.html

[C14] 泛型函数
来源：http://hz.yonumen.top/gticwevrmt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnxiangtu.top/gtfzfseqdz.html

PHP:  // 无泛型
来源：http://hz.nanxinkj.top/gtrhwpjedo.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtmpvinlsw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtmznrjwrq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangtech.top/gtiofvtapz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gtvfafpcly.html

Ruby: # 无泛型
来源：http://hz.daxiang520.top/gtumlvpndh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cqqwz.cn/gtukkffbvh.html

[C15] 解构 / 展开参数
来源：http://hz.pengpengdd.cyou/gtzuqkomvn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhixingplan.top/gtrsydgvti.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ivvv.top/gtykcqlulh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtlmconyiz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sweek.top/gtwdwljkfo.html

Java: // 无解构
来源：http://hz.c1oappe.top/gtstibggad.html

Go:   // 无解构
来源：http://hz.yj20258.top/gtsgjbuoyi.html

Ruby: a, b = pair
来源：http://hz.yueranfly.top/gtqjtzacjw.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gtlkdiqbuu.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtgljsbrrh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sysykeji.top/gtxxswvdya.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtbbizqlhq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xylfe.cn/gtvopmpkxr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtzeyapwat.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtqrfgmnsp.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinyuanbaomall.cn/gtgukixyrg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.meibo888.top/gttjaxrktc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gtihmygruf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsptusfyh.html

D. 数组 / 列表 / 集合
来源：http://hz.dianchejie.cn/gtsqzhtjal.html

================================================================================
来源：http://hz.iojbl.cn/gtltadeujd.html

[D01] 创建数组 / 列表
来源：http://hz.zhongyouzk.top/gtimvvdiab.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gtvjqfdeav.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhoulong.xyz/gtjsfamrmv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangtech.top/gtzkatxitg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtihmycanl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258.top/gtvzzwuovs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj202588.top/gtbkzncfph.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gthbszaryy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtukmymznd.html

[D02] 追加元素到末尾
来源：http://hz.jlsjyb.cn/gtltuvccki.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxuanxn.top/gtufjqbzvr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gzhubu.top/gtaaauoseu.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtmcjqggav.html

TS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtuwdmhfed.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gtriivmzcj.html

Go:   arr = append(arr, 4)
来源：http://hz.cashguo.top/gtzltpydzh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.haohaochexian.top/gtuurcjiib.html

C#:   list.Add(4);
来源：http://hz.yj20258.top/gtyxzbttlc.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigufen.top/gtulheoabu.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtytkxkwma.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtkrsudmem.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtueqdwxvp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtezgcfqdo.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtvjavsrlc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtqltzzcry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtihsfuilk.html

C#:   list.Insert(0, 0);
来源：http://hz.sysykeji.top/gthyeaomao.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtuqlstcww.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nwbrower.top/gthldpidkr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhijiandao.cn/gtfuddpkgw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gtogjroufs.html

TS:   arr.splice(0, 1);
来源：http://hz.jiagoushi.top/gtaxjgyrmi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sufxvd.cn/gtglxfogog.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangdashe.top/gtpcfburbn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.kuanghao11.cn/gtkvjcpztu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj20258888.top/gtuvyeteih.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gtangwfajx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtvezcdcjt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shzxlz.cn/gtqdwbtjua.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtzstvynbc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuanzx.com/gtpqkzjakw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtrmmduhrs.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtkzqwnusr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtgddwrtjn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gthxgmdzlb.html

[D06] 数组长度
来源：http://hz.zhongyouzk.top/gtkxgadvzj.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtsnatwabo.html

PHP:  count($arr);
来源：http://hz.zhijiandao.cn/gtjjskypel.html

JS:   arr.length
来源：http://hz.gotoacloud.top/gtvpibojbe.html

TS:   arr.length
来源：http://hz.guannengcc.top/gtujxsuxom.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtxanrswyx.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtfdsxtgih.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtcwlvpujd.html

C#:   list.Count;
来源：http://hz.sweek.top/gtdcngwuyv.html

[D07] 切片 / 取子数组
来源：http://hz.xylfe.cn/gttauhjkrn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gtzpfgcwhl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gthekrocvc.html

JS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtahpklzxt.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtjrzdzttj.html

Java: list.subList(1, 4);
来源：http://hz.gogol.net.cn/gtxvzocjml.html

Go:   arr[1:4]
来源：http://hz.jqgufenzy.top/gtrutpahxe.html

Ruby: arr[1, 3]
来源：http://hz.birdmap.top/gtahfbfjln.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtrpbvmwqv.html

[D08] 合并两个数组
来源：http://hz.zhongyouzk.top/gtbwrefbrb.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtwralfzer.html

PHP:  array_merge($a, $b);
来源：http://hz.pengpengdd.cyou/gttztypjqz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hammf.cn/gtccidpgog.html

TS:   [...a, ...b];
来源：http://hz.quarkkingdee.top/gtdxqozifw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yanxiufei.cn/gtofxkkuxb.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtgtwziavj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgufenzy.top/gtuzznqslr.html

C#:   a.Concat(b).ToList()
来源：http://hz.meibo888.top/gtniyvpvie.html

[D09] 排序（升序）
来源：http://hz.redwolf501.top/gteiunsbte.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zycfv.cn/gtnhrdvovy.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtnjjwbwhd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtbhpqhtcr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtjfmxgdyb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtsdrchrgy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtrlkokvke.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gturiaasyz.html

C#:   list.Sort();
来源：http://hz.yj202588.top/gtslzhjzld.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jianghu66.top/gtvbxfnbsr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gtsbxtbgeb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtwejjdvdn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtniybdjig.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtwytajgdo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtjfclrqxk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtzusolcbw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtmbslksnz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gtiissmbqg.html

[D11] 反转数组
来源：http://hz.yvedp.cn/gtearkbbrt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.quarkkingdee.top/gtkqnmtvcs.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gttvlsngfo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtydguvcoq.html

TS:   [...arr].reverse();
来源：http://hz.fzhhl.top/gtqjassdla.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtpcmwngui.html

Go:   slices.Reverse(arr)
来源：http://hz.jyoumei.cn/gtuqyycawd.html

Ruby: arr.reverse
来源：http://hz.mhx1999.top/gteozjfajm.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtpyfuczak.html

[D12] 查找元素下标
来源：http://hz.ybcxt.top/gtlncztuzh.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtqsolvuvy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtgejbwycf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gttsartmwf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtxesceaxy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhongyouzk.top/gtxkadmfpz.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtuctyotky.html

Ruby: arr.index(x)
来源：http://hz.gogol.net.cn/gtmvuzkqrq.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtmjcnrdez.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cqqwz.cn/gtpsukbjad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinqigfzy.top/gtiuhbkyhz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtxqjkbejz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtunqzaozn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtmxbypquh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigfzy.top/gtsytkgfjb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jyoumei.cn/gtubzpksdh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gtofybidbj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhongyouzk.top/gtrtbdjmxq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtyozckibf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cqqwz.cn/gtufzhruoz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tianlin.xyz/gtrbeqcfza.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtuwjnyrbe.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtptmsxcjp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gtvxefskvr.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtgmfeirsw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydjk.org.cn/gtbgtnloqm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gthhryokdm.html

[D15] 去重
来源：http://hz.fengsongda.top/gtzjzquhwp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtcjowjuiv.html

PHP:  array_unique($arr);
来源：http://hz.haohaochexian.top/gtyxrbpbog.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtxiywxevl.html

TS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtpluyjdnr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtpoztifyb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtssfpjutu.html

Ruby: arr.uniq
来源：http://hz.svipenyu.cn/gtfwwgnjgi.html

C#:   list.Distinct().ToList()
来源：http://hz.ehwqpu.com/gtvqwcnnrh.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtypubjfoo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.andypj.xyz/gtuurjdsme.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.haohaochexian.top/gtkwovdloa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtkhdmxluy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtkkuciehp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gthixcerve.html

Go:   // 手写循环累加
来源：http://hz.xuanzx.com/gtudubzppw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtboetfogv.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtzgidvzbw.html

[D17] 最大值与最小值
来源：http://hz.gotoacloud.top/gtzreigqyj.html

Py:   max(arr);  min(arr)
来源：http://hz.guowangkeji.top/gtdgnklqis.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtkfekpteu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gtgatpffso.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gttxvyyrcv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tian-w.cn/gtzuniypsj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.quarkkingdee.top/gtracwbycc.html

Ruby: arr.max;  arr.min
来源：http://hz.yonumen.top/gtjafraowf.html

C#:   list.Max();  list.Min()
来源：http://hz.zdqjudy.top/gtvmgzmhar.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gtkgnijkri.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dianchejie.cn/gteyzrvxsb.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtklwordlj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.havefunace.top/gtohankryl.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gtporxzwzd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cqqwz.cn/gttoxrdkwu.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtyjcmpeau.html

Ruby: nested.flatten
来源：http://hz.zdqjudy.top/gthlenxalz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zycfv.cn/gtxpetvipf.html

[D19] 按字段分组
来源：http://hz.cucudq.cn/gtmbfauorm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ehwqpu.com/gttxdxdwpf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtjuzkkggn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xziqi.cn/gtumkvdjqw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtshulcsww.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gtujbwitxm.html

Go:   // 手写 map[string][]T
来源：http://hz.nwbrower.top/gthpbjgrfe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtgtrrflua.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgfzy.top/gtnohqvwin.html

[D20] 统计每个元素出现次数
来源：http://hz.gzhubu.top/gtxkrdnkse.html

Py:   Counter(arr)
来源：http://hz.hnqzz.top/gtmaerxpzv.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gtgwhvrmmf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtconaksfx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtxonzcmvu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtvpprkzau.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtnbznbizu.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gtibcgaujv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinghuilouyu.cn/gtihmeiegc.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gtrzljouyq.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtigyfrbnr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtcofseuth.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtxfqgamdy.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtpdbjucoi.html

Java: list.contains(x)
来源：http://hz.kuanghao11.cn/gtylblnpfz.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtpvvpljsf.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gthrpqjthk.html

C#:   list.Contains(x)
来源：http://hz.cucudq.cn/gtaympiqka.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtepunvsyv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zdqjudy.top/gtjqpvmrai.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinghuilouyu.cn/gtnprtwozd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fzhhl.top/gtvajkamps.html

TS:   [...arr];
来源：http://hz.ivvv.top/gteerckmrj.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258888.top/gtifhgqrec.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zdqjudy.top/gtgeeenqby.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtyptgpddi.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtqkatlaga.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtxtjgspwm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cashguo.top/gtmpadnnah.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shuidangran.top/gtlqozjqif.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtultavfiy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtwpdkbodd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtvkatlqsu.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtcintovem.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hammf.cn/gtoeruxcac.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sufxvd.cn/gtmmfcbzxt.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtvccsgtkd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtvhuxlcqs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtosvemoii.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtgfejnoxi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtzxyknwwb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258.top/gtmzwqiqlq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtqyiqfrsn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guowangkeji.top/gtlyngyjzf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.vqdsnc.cn/gtznxwrfbc.html

[D25] Set 集合去重与交并差
来源：http://hz.yuanzhike.top/gtnnpzifmk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtkelpqcvi.html


<!-- 参考信息 -->