代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydzc1.top/gtyftuiudo.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gtqwkubfdi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenlongwang.top/gtjfjhponz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dashuyun.cn/gtvjotnfru.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gtzgadizoc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.vqdsnc.cn/gtbjakrigr.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtkhqfypzl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xingfuxueyuan.xyz/gtenwdriju.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.wangdashe.top/gtbznkjefc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gteoekdzio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtuxuhsmds.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xingfuxueyuan.xyz/gtlclckbpb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinyuanbaomall.cn/gtmupvocss.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xylfe.cn/gtdffahrdv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtpmqwyfnz.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gtmtbhtavc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtjuabicqc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtccvmdttq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.svipenyu.cn/gtyzogeqve.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtnzaghghv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtsxnvjlji.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtrkbzczvb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtihrcecix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gttvqnenjt.html

[C10] 变量作用域
来源：http://hz.ywan-chungtsiang.top/gtahxlxyjt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.9152youxi.cn/gtdfjycjka.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zycfv.cn/gtfcdpckrk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtuwxnhnyv.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtzknxmalo.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtdhezzerk.html

Go:   花括号块级作用域
来源：http://hz.hammf.cn/gtxowadcmc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenjidiqi.icu/gtvpoasfyi.html

C#:   块级作用域
来源：http://hz.52xcode.cn/gtyogijkxs.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gttrigrueg.html

Py:   from module import func
来源：http://hz.hongshengwenyu.top/gtsgschxmx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.0kj1m.cn/gtkzbczrce.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.vqdsnc.cn/gtntkmiezo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shzxlz.cn/gtwxmcwuxa.html

Java: import java.util.List;
来源：http://hz.tianlin.xyz/gthmxktmdf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gttifeeeov.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtgpzbmexp.html

C#:   using System.Text;
来源：http://hz.gzhubu.top/gtddfurdgy.html

[C12] 立即执行函数 IIFE
来源：http://hz.sweek.top/gtobdrdowq.html

Py:   (lambda: print("run"))()
来源：http://hz.aibaodan.cn/gthrxivjlg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtbqkkrxaw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtckfmaisx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtiftwmqbd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gaohongyu789.top/gteyihfyks.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenlongwang.top/gtvzvgyuhq.html

Ruby: -> { puts "run" }.call
来源：http://hz.aizwys.cn/gtvxelihrf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.havefunace.top/gttecrqhnx.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj202588.top/gttrvhlmpk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yvedp.cn/gtwhbcyctn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtsxtgcnkf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtqiaxotim.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtcddorjyc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtgmnwdnzi.html

Go:   func add(a, b int) int
来源：http://hz.hywenlv.cn/gtlrityxrs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangkeji.top/gthtfpvmrt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuanzhike.top/gtmyqinxlk.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtowencghg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tianlin.xyz/gtaiaenejj.html

PHP:  // 无泛型
来源：http://hz.svipenyu.cn/gtztubyknv.html

JS:   // 无泛型
来源：http://hz.gogol.net.cn/gtorsmokln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhijiandao.cn/gtjavgdbqn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ppjwa.cn/gtogadcbuo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yangfankeji.com/gtwnwfodoo.html

Ruby: # 无泛型
来源：http://hz.yanxiufei.cn/gthnvzcyjh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gthoicfasf.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtqofsicpz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sufxvd.cn/gtzkaxekbr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhengqikj.top/gtkqkydfxn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtxtslxzed.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fengsongda.top/gtdufxoqyd.html

Java: // 无解构
来源：http://hz.vqdsnc.cn/gtkhufdkvi.html

Go:   // 无解构
来源：http://hz.bjfxy.top/gtuzorjtca.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtsvpacatb.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtwnrruhah.html

[C16] 函数 / 方法重载
来源：http://hz.hongshengwenyu.top/gtzcoogfrn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxinkj.top/gterzbowln.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtuntmxuzr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtlpckqxjj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ywan-chungtsiang.top/gtoagolhxh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xingfuxueyuan.xyz/gtvvqpjaoe.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtmdhoxepb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sufxvd.cn/gtkzzgrwhg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangdashe.top/gtmegvoead.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxzzkkqwd.html

D. 数组 / 列表 / 集合
来源：http://hz.jiagoushi.top/gtmfypgows.html

================================================================================
来源：http://hz.ybcxt.top/gtisnevxpa.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtifbayxtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtrgldoqox.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangkeji.top/gtulplhnaw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shzxlz.cn/gttrvpxxbh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.0kj1m.cn/gtppvszeqi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hysaishi.cn/gttijcljaq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dianchejie.cn/gtgrqzqfmy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gtxnmysgkl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cqqwz.cn/gtdobjpynw.html

[D02] 追加元素到末尾
来源：http://hz.zhijiandao.cn/gtrlvzzdzf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtzbnmkiea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtkhsocjap.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtoxufvcsv.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtvkvlffhz.html

Java: list.add(4);
来源：http://hz.ydzc1.top/gtwvwpcwnn.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gtawzpikhi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xingfuxueyuan.xyz/gtabcnyuxq.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtziohfxqa.html

[D03] 在指定位置插入元素
来源：http://hz.andypj.xyz/gtgmjhtbpz.html

Py:   arr.insert(0, 0)
来源：http://hz.feifeiyinyue.top/gtjvqaopoe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.52xcode.cn/gtnrfretig.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gtzqxlkrem.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.smart0.xyz/gtakfzuneh.html

Java: list.add(0, 0);
来源：http://hz.haohaochexian.top/gtwcdnvwhe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtzisqsbbz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtpawgfzah.html

C#:   list.Insert(0, 0);
来源：http://hz.jlsjyb.cn/gtqnpixqeb.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtzeexpdkd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtfbzolwbv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jlsjyb.cn/gtpxmodvhb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fengsongda.top/gtaiuozpze.html

TS:   arr.splice(0, 1);
来源：http://hz.dashuyun.cn/gtsmqfzame.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gthzyjgtxq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.quarkkingdee.top/gtllvvzwyp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinghuilouyu.cn/gthkartkkv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtriaooohd.html

[D05] 访问与修改元素
来源：http://hz.smart0.xyz/gtpocctgtj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gttqiuyozk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtixqlxdjs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtaugtqrhf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tianlin.xyz/gtwgagrbxk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hammf.cn/gtytauahrp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtnccxkouf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtjnxmmfaz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hysaishi.cn/gtpcenhkbk.html

[D06] 数组长度
来源：http://hz.gaohongyu789.top/gtryksbxqd.html

Py:   len(arr)
来源：http://hz.cashguo.top/gtizcursso.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtsbzhziox.html

JS:   arr.length
来源：http://hz.nanxinkj.top/gtwsjnqtnj.html

TS:   arr.length
来源：http://hz.jinqigufen.top/gtrsavclnx.html

Java: list.size();
来源：http://hz.cashguo.top/gtedldntcu.html

Go:   len(arr)
来源：http://hz.jinqigufen.top/gtkinclzlz.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtjexnwdrl.html

C#:   list.Count;
来源：http://hz.smart0.xyz/gtjtbzvyld.html

[D07] 切片 / 取子数组
来源：http://hz.zhijiandao.cn/gtilwxchkk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtiopyxrqg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guowangkeji.top/gtsqaqpxpe.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gteckuzftp.html

TS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtvwekoavr.html

Java: list.subList(1, 4);
来源：http://hz.yonumen.top/gtbwkitmfj.html

Go:   arr[1:4]
来源：http://hz.guowangkeji.top/gtmerovzfd.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtesbbqfsa.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gtdavoadyz.html

[D08] 合并两个数组
来源：http://hz.haohaochexian.top/gtxyxshcvs.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenlongwang.top/gthrqkfosp.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtttvblirt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtgfeedgav.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtyqruwmwu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cdnleiting.top/gtbsjdlowr.html

Go:   append(a, b...)
来源：http://hz.svipenyu.cn/gtofhpcage.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hfpthk.cn/gtmwqiveiu.html

C#:   a.Concat(b).ToList()
来源：http://hz.c1oappe.top/gtzzbdxklu.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtmiogzcdl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtyvjawznd.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gtnzizaddi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtyutofwpj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gtuqervzuu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.havefunace.top/gtijcdrmkh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtnzurwgmy.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtjhhsdrnl.html

C#:   list.Sort();
来源：http://hz.xuetiantiany.cn/gtnwhcpcyr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtxjiijwka.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnqzz.top/gtfxborlms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtkvhqebus.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtpvuhatqq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.quarkkingdee.top/gtajurvuup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aibaodan.cn/gthdvexxsf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.meibo888.top/gtjidenfcd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuxming.cn/gtswkgljsy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gaohongyu789.top/gtiuccygjt.html

[D11] 反转数组
来源：http://hz.sxryk.cn/gtnnzcgiwg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yuanzhike.top/gtgeemtzke.html

PHP:  array_reverse($arr);
来源：http://hz.guowangkeji.top/gtxfwfjwvq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ywan-chungtsiang.top/gtlkskjksp.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtqebiuazb.html

Java: Collections.reverse(list);
来源：http://hz.pengpengdd.cyou/gtjwrpyxep.html

Go:   slices.Reverse(arr)
来源：http://hz.feifeiyinyue.top/gtspjwkhop.html

Ruby: arr.reverse
来源：http://hz.meibo888.top/gtwekvdtcu.html

C#:   list.Reverse();
来源：http://hz.ybcxt.top/gtdbskgrsa.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtihcjxlsu.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gttocebqjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gaohongyu789.top/gtjerronvu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtdescctvd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtkviwtvqx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gttnlkvwmz.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtwdrdsqgz.html

Ruby: arr.index(x)
来源：http://hz.mhx1999.top/gtwromhxos.html

C#:   list.IndexOf(x);
来源：http://hz.c1oappe.top/gtgoyvjjpr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtmgnjqfyf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtfrtdqplq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zycfv.cn/gtknqrwtgd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtynclecwh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtxrzqioyi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yvedp.cn/gtuyptmgxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zdqjudy.top/gticsysfpe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ppjwa.cn/gtbubozpzq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.guowangkeji.top/gtoqtncobg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gtfqmxhwjy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtduusaxqy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtjyzzawcv.html

JS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtibkruaer.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtxsehckhu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydjk.org.cn/gtjqgiavbe.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtampfesyy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigfzy.top/gtvmgvadyh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangtech.top/gtofgatmva.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtsvojkabn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yvedp.cn/gtplvyflko.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtpkilmbjs.html

JS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtybfkxwlo.html

TS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtxqoxuiiy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhixingplan.top/gtowgncmhs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtzgwzqvsc.html

Ruby: arr.uniq
来源：http://hz.0kj1m.cn/gtarobfkgc.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtdhwziamu.html

[D16] 求和与平均值
来源：http://hz.hnqzz.top/gtfftoemhm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtqfashsmz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtlqztzpkz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtfhntspxa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtyrgzbucf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtprykwjsi.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtlrqgvmba.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtkiatagrh.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258888.top/gtkpfbniqy.html

[D17] 最大值与最小值
来源：http://hz.fengsongda.top/gtcdxxsmml.html

Py:   max(arr);  min(arr)
来源：http://hz.ydzc1.top/gtddoycrpz.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtgieftxfl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtkcnwkdrm.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtpoedolka.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xinyue.icu/gtahhonbxg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yangfankeji.com/gtdzbzmpuz.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gtbnyzypej.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtgdrknvdb.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gteejputma.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtadofokkt.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtdjqgolka.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgufenzy.top/gtruuywwvk.html

TS:   nested.flat();
来源：http://hz.zhengqikj.top/gtgtfgtosw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtbwsypjrm.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtwmkhisgg.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gtgisuwdsn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nwbrower.top/gtpnbcasiw.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gtfywksirm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dianchejie.cn/gtbhhajlyh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangshuangyany.cn/gtvkzjzoqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258888.top/gtiruscgjj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtwsmhnqqg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gthvjvvqdv.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtfzlpmaww.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj202588.top/gtjoqemuzl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nwbrower.top/gtryfqfbie.html

[D20] 统计每个元素出现次数
来源：http://hz.hongshengwenyu.top/gtwnyritly.html

Py:   Counter(arr)
来源：http://hz.kuanghao11.cn/gtmrtdhxfq.html

PHP:  array_count_values($arr);
来源：http://hz.yanxiufei.cn/gtetojzaxr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtsvepuaek.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtnborntch.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yanxiufei.cn/gtadzufamc.html

Go:   // 手写 map[T]int
来源：http://hz.gaohongyu789.top/gtmdbhpnyg.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtmscedldf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xylfe.cn/gtzmaqoadn.html

[D21] 判断是否包含某元素
来源：http://hz.tanke756.top/gteyhdwdqv.html

Py:   x in arr
来源：http://hz.yangfankeji.com/gtzptircjh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.havefunace.top/gtvygciufw.html

JS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtpemnoqbh.html

TS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtmikfiarw.html

Java: list.contains(x)
来源：http://hz.jinyuanbaomall.cn/gteuvkdbwi.html

Go:   slices.Contains(arr, x)
来源：http://hz.fzhhl.top/gtmyoqcomo.html

Ruby: arr.include?(x)
来源：http://hz.bjfxy.top/gtphfbjftf.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtiajjccot.html

[D22] 复制数组（避免共享引用）
来源：http://hz.havefunace.top/gthbmcvgnk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gaohongyu789.top/gthlvyljtv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxuanxn.top/gterbbkgdy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuxming.cn/gtcktyqkxs.html

TS:   [...arr];
来源：http://hz.sxryk.cn/gtphfupkcb.html

Java: new ArrayList<>(list);
来源：http://hz.gaohongyu789.top/gttueihmdo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dianchejie.cn/gtgplgzchb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gogol.net.cn/gtwrvskkfg.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gtroprakxj.html

[D23] reduce 累积计算
来源：http://hz.zdqjudy.top/gtufvewocv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dashuyun.cn/gthkuksxjj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhixingplan.top/gtsguzjatz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtfsrcadbx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtmahjdews.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gttmydxdes.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtvtpgwhug.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnxiangtu.top/gtbkiilqmn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.bjfxy.top/gtqeyyactl.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gtaznapult.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gaohongyu789.top/gtqgfkpqdb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tian-w.cn/gtljmcqqsp.html


<!-- 参考信息 -->