代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cucudq.cn/gteaihzyqv.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gthsoksdvv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtuqherqjx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtotxnsnid.html

Ruby: arr.map(&:upcase)
来源：http://hz.kuanghao11.cn/gtaeyfiqzu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtcjekghfd.html

[C08] 闭包
来源：http://hz.feifeiyinyue.top/gtywwiqgmg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydzc1.top/gtntafbzgq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fzhhl.top/gtvtrrafga.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtkmqkcxem.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gttkeftdfl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtxakhxnkb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtnkkwtixo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zdqjudy.top/gtglkcjwxf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gthjtucres.html

[C09] 递归
来源：http://hz.cheryme.top/gtwvsawucm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.bjfxy.top/gtbiomqduh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtvsgdxpsa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtvlhahbgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daria6918.cn/gtacogyswa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gtslhniveh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pycfn.com/gtdtbydmqo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tian-w.cn/gtxhrslflw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtsrvjkpxb.html

[C10] 变量作用域
来源：http://hz.hfpthk.cn/gtjbejclxt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtdonjloqh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.fzhhl.top/gtdneiowvd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gteesvmgzj.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtsiqyonpp.html

Java: 方法内为块级作用域
来源：http://hz.kuanghao11.cn/gtkejwwjhc.html

Go:   花括号块级作用域
来源：http://hz.hysaishi.cn/gttffghzsf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zycfv.cn/gtpmxairml.html

C#:   块级作用域
来源：http://hz.9152youxi.cn/gtvocvendc.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gteabvhnwg.html

Py:   from module import func
来源：http://hz.ywan-chungtsiang.top/gtrnqkgiza.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhixingplan.top/gtvxhacxvx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yongpay.top/gtrxtnffjx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xingfuxueyuan.xyz/gtrbldnqat.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gthwojxfky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gaohongyu789.top/gtffteockq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hfpthk.cn/gtyncobirr.html

C#:   using System.Text;
来源：http://hz.zhengqikj.top/gttadbzbdh.html

[C12] 立即执行函数 IIFE
来源：http://hz.fengsongda.top/gtjqqmzzla.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtsukiuzpf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gttyrdhkef.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nanxuanxn.top/gteywddwmv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gttjmkxmis.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtkmqbfyau.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.9152youxi.cn/gtjhckcxqr.html

Ruby: -> { puts "run" }.call
来源：http://hz.jlsjyb.cn/gtsieliezp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtgvyvavxs.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtnucoggvf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cqqwz.cn/gtygkxxven.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtmonmmaiy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pycfn.com/gtzhyoikny.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtaesexlpp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtnlazcmnd.html

Go:   func add(a, b int) int
来源：http://hz.wangdashe.top/gtmxvuznly.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigufen.top/gtqweiynql.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtzgafkshe.html

[C14] 泛型函数
来源：http://hz.birdmap.top/gtebcsnwlg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj202588.top/gtciyzlbud.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtybkzcenf.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gthnxpufoa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtghhyzwqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hywenlv.cn/gtdvifkgzo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtjlsiwgrf.html

Ruby: # 无泛型
来源：http://hz.dashuyun.cn/gtorigcvmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenlongwang.top/gtxaimuage.html

[C15] 解构 / 展开参数
来源：http://hz.dashuyun.cn/gtityndxwe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtykfmarme.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangdashe.top/gtvxgewdde.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtmxbrstmu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtgahfvdyx.html

Java: // 无解构
来源：http://hz.sxryk.cn/gtywdodojm.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtnxgntgrl.html

Ruby: a, b = pair
来源：http://hz.gotoacloud.top/gtmffgonqa.html

C#:   var (a, b) = pair;
来源：http://hz.xziqi.cn/gtrrzmggdh.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtqcepqfay.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.snrcjt.cn/gtozualapv.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtwbvaostg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.svipenyu.cn/gtwyilddyi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gtbbitlmrg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.snrcjt.cn/gtixpduugg.html

Go:   // 无重载：用不同函数名
来源：http://hz.birdmap.top/gtibphmytw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.iojbl.cn/gtlnksxfdw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtlofbhbre.html

================================================================================
来源：http://hz.pycfn.com/gtafwwmvzt.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangtech.top/gtqrenenfi.html

================================================================================
来源：http://hz.quarkkingdee.top/gthahqbcbb.html

[D01] 创建数组 / 列表
来源：http://hz.ydjk.org.cn/gtaabhyism.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydjk.org.cn/gtvzkmgkeo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenzaomai.com/gtzhrlsmig.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangdashe.top/gtevuwrxse.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yangfankeji.com/gtjlhxkxjj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sufxvd.cn/gtymbghiop.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aizwys.cn/gtpbfxoqkv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtjknpnqvo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.kuanghao11.cn/gtedcsiiew.html

[D02] 追加元素到末尾
来源：http://hz.sweek.top/gtwcbaffvt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnxiangtu.top/gtyzbyzgji.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.iojbl.cn/gtfhfzyznv.html

JS:   arr.push(4);
来源：http://hz.jyoumei.cn/gttbqmkkox.html

TS:   arr.push(4);
来源：http://hz.52xcode.cn/gtgdwpbund.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtywjegmzb.html

Go:   arr = append(arr, 4)
来源：http://hz.yonumen.top/gtebnvvshd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.meibo888.top/gtbpxxdliw.html

C#:   list.Add(4);
来源：http://hz.smart0.xyz/gtobpqhonr.html

[D03] 在指定位置插入元素
来源：http://hz.hfpthk.cn/gtlsqqkbxt.html

Py:   arr.insert(0, 0)
来源：http://hz.pengpengdd.cyou/gtxcomeclg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aizwys.cn/gtmdboyydl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tian-w.cn/gtcolzhdqo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtfldahtry.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtqwxscoap.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.feifeiyinyue.top/gteymogkbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xingfuxueyuan.xyz/gtfbhtowvn.html

C#:   list.Insert(0, 0);
来源：http://hz.zycfv.cn/gtwbgohnjn.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtxlvwsbsj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtlwscrgot.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtkxayvsfp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cucudq.cn/gtbbpwtuwn.html

TS:   arr.splice(0, 1);
来源：http://hz.vqdsnc.cn/gtkzgxhavq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtiwjneniq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hywenlv.cn/gtrzbmkloh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtbsajwois.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.316326.xyz/gtpaojebsp.html

[D05] 访问与修改元素
来源：http://hz.xylfe.cn/gtjpfwsbku.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtdhgddwtp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gttaewglxc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtavgrzxjs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.redwolf501.top/gtwrepiedx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hammf.cn/gtqmlytytf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtewvfixvs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtfsdspwhe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydzc1.top/gtxrdqxrhq.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtzymgtqey.html

Py:   len(arr)
来源：http://hz.jinqigufen.top/gtzravppta.html

PHP:  count($arr);
来源：http://hz.xuetiantiany.cn/gtsldkykhr.html

JS:   arr.length
来源：http://hz.xinyue.icu/gtnpmvyzsc.html

TS:   arr.length
来源：http://hz.sweek.top/gteiqokgii.html

Java: list.size();
来源：http://hz.nwbrower.top/gtapiuizqh.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtjczernmm.html

Ruby: arr.length; arr.size
来源：http://hz.gotoacloud.top/gtifpxcwir.html

C#:   list.Count;
来源：http://hz.sysykeji.top/gttiiqzexu.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258.top/gtphqlftuq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtpazukeun.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtbalzancf.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtrjfxufsz.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtgobrokur.html

Java: list.subList(1, 4);
来源：http://hz.zhiwuduotai.top/gtyhgfnxio.html

Go:   arr[1:4]
来源：http://hz.jlsjyb.cn/gtxqkciffc.html

Ruby: arr[1, 3]
来源：http://hz.yj20258888.top/gtydqopbip.html

C#:   list.GetRange(1, 3);
来源：http://hz.fzhhl.top/gturbxhprx.html

[D08] 合并两个数组
来源：http://hz.zhaomingkeji.xyz/gtiftcyoop.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtsbttqgme.html

PHP:  array_merge($a, $b);
来源：http://hz.daxiang520.top/gtkgevjxwn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtglcjvmei.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtxtsdxkos.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtlsgmldja.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtseqgvaly.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuanzx.com/gtejhvenxh.html

C#:   a.Concat(b).ToList()
来源：http://hz.jianghu66.top/gtwzhnlnwf.html

[D09] 排序（升序）
来源：http://hz.fengsongda.top/gtewxxnrzk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtekdyrnrk.html

PHP:  sort($arr);
来源：http://hz.tianlin.xyz/gtnzjaowvm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtorlaeoep.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnqzz.top/gtevazosxu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtmpjemmid.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.andypj.xyz/gtryzdezby.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtmrxqosyh.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtiixtsghx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtbdeohwxa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtqxnlybde.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtveuzecya.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gttarfnbsd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.mhx1999.top/gtznxbvsvd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigfzy.top/gtjvhvjqpv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhijiandao.cn/gtypsngvwk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.redwolf501.top/gtlynvnzah.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ppjwa.cn/gtoelyinwy.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtjkyvztzn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtgevldpvs.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtfsscbojo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtcbjpflds.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtwedcplgt.html

Java: Collections.reverse(list);
来源：http://hz.chenlongwang.top/gticvnxmtg.html

Go:   slices.Reverse(arr)
来源：http://hz.hammf.cn/gtnxsylree.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtyxjwcdic.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gtqkpbmlii.html

[D12] 查找元素下标
来源：http://hz.chenjidiqi.icu/gtmzahxzuz.html

Py:   arr.index(x);  x in arr
来源：http://hz.ywan-chungtsiang.top/gtowbsbzii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.haohaochexian.top/gtbpvpvimb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xingfuxueyuan.xyz/gtxgvunkig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtvkeefzrl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtncjnyqyb.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtewrnrnes.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtlsydxoum.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtronymehw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydzc1.top/gtbplesnbp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtvkhmbsuw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.316326.xyz/gtsovynuzs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtvomljsbh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtutktvdhf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtimrkmfvt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgfzy.top/gtpscautpm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yonumen.top/gtoapkepse.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtjmbpzlpq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtvihdbaof.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtxgirphpc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtjeqapcne.html

JS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtfmjcdxif.html

TS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtwbeafshz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gtcvejmxfh.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gthabgynqq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtvobbijpg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtmcslvmmd.html

[D15] 去重
来源：http://hz.svipenyu.cn/gtqvjocqll.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtubsshldm.html

PHP:  array_unique($arr);
来源：http://hz.shuidangran.top/gtcrjrgbbf.html

JS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtvbwaeton.html

TS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtrmhbagbf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aibaodan.cn/gtwnzswunl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtwrjflvxw.html

Ruby: arr.uniq
来源：http://hz.zhixingplan.top/gtewoastkz.html

C#:   list.Distinct().ToList()
来源：http://hz.meibo888.top/gtewahpqrv.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtscwxmqzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gtcgotwlfm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinghuilouyu.cn/gtbfahsmdj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtrnyzcbys.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtdpungdns.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtvhndooyp.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtburjyojj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gthlkimzgz.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnxiangtu.top/gtsxcxtxzt.html

[D17] 最大值与最小值
来源：http://hz.zhixingplan.top/gtqtcavkxm.html

Py:   max(arr);  min(arr)
来源：http://hz.sweek.top/gtymjeyrso.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gttfhpouhi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtvoathnyx.html

TS:   Math.max(...arr);
来源：http://hz.guowangkeji.top/gtjagirzrj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.0kj1m.cn/gtzmjhntzb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gttxycodtq.html

Ruby: arr.max;  arr.min
来源：http://hz.ivvv.top/gtazmwunai.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtdsgwxagn.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gtcczgdnjm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dianchejie.cn/gtjexlytid.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gttyusvyip.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jlsjyb.cn/gtkpkljylv.html

TS:   nested.flat();
来源：http://hz.cdnleiting.top/gtoeoichbp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtnovabfjy.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gthkkmrjvd.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtyjpbywgm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangdashe.top/gtiqskxeso.html

[D19] 按字段分组
来源：http://hz.shanyushiyangtech.top/gtutzgqvgs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cheryme.top/gtsbsdhepe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtqaqvtreu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtqtfbesmd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtzctrnawo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtiedwwihx.html

Go:   // 手写 map[string][]T
来源：http://hz.zhiwuduotai.top/gtqlivxsjl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtpidrreea.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtuimplkiy.html

[D20] 统计每个元素出现次数
来源：http://hz.cheryme.top/gtwcctnrra.html

Py:   Counter(arr)
来源：http://hz.ehwqpu.com/gtrdglfawv.html

PHP:  array_count_values($arr);
来源：http://hz.sweek.top/gtqdzfjeiv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gttocumawo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtfvipghmr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yonumen.top/gtxknrfryg.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtcnqovyek.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtysqvfyls.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtbvupqlqy.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtqmqwtjuf.html

Py:   x in arr
来源：http://hz.ehwqpu.com/gtzoqlohnx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gttpicujsk.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtroikcyly.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtaghbflvk.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtwracjjsf.html

Go:   slices.Contains(arr, x)
来源：http://hz.snrcjt.cn/gtwgwdinfh.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtcrpoqnab.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gthftsukkn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jqgufenzy.top/gtrkjbqogh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtmvyjlrdw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtucpyzupk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigufen.top/gtfyjmucvt.html

TS:   [...arr];
来源：http://hz.pycfn.com/gtuujzxeti.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtihhrivdz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gotoacloud.top/gtlgfnykyf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jiagoushi.top/gtvbxtjdbh.html

C#:   new List<int>(list);
来源：http://hz.pycfn.com/gtzwhprpbl.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtclscaimi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yongpay.top/gtqycjkozz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangtech.top/gtooaszjch.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtwroqynjp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtmlhlisuo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gtlzuoxpql.html

Go:   // 手写循环
来源：http://hz.shuidangran.top/gtmbegagrr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtyrsndket.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.meibo888.top/gtyutswdpo.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuxming.cn/gtspgadnul.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydzc1.top/gtpwuiqzjw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gteqsyxbfe.html


<!-- 参考信息 -->