代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.xuetiantiany.cn/gtqbynwknn.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangkeji.top/gtpuetjass.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtyavqifhf.html

JS:   const square = x => x * x;
来源：http://hz.nanxinkj.top/gtubfsebhw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zycfv.cn/gtjuafwkgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aibaodan.cn/gtaitziqas.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cheryme.top/gtggzdgzai.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtxqvlnxih.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtflptcnyw.html

[C07] 把函数作为参数传入
来源：http://hz.svipenyu.cn/gtacudawze.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jyoumei.cn/gtqgmoacny.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuanzhike.top/gtnfjhvoex.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xingfuxueyuan.xyz/gtjpepnrpx.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtrrjqucdr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cheryme.top/gtdccrkfqz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.havefunace.top/gtqtrkuqlc.html

Ruby: arr.map(&:upcase)
来源：http://hz.guannengcc.top/gtmckkrskz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.kuanghao11.cn/gtfiutgfap.html

[C08] 闭包
来源：http://hz.xuanzx.com/gtphfpsohw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.haohaochexian.top/gtzquconok.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ppjwa.cn/gtaeroulec.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtacaovtos.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtcsqbaxgp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydzc1.top/gtllsaxcwq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuanzx.com/gtyltsvtjk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yueranfly.top/gtqmqknfsw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtmlgbxovk.html

[C09] 递归
来源：http://hz.kuanghao11.cn/gtqiaquepr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gttzhpmiql.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xinyue.icu/gtqhowavts.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtpxmhterg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtssavrjuq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtrtdyrtdr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtxswleyso.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gtxuvlywwi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtullkbflm.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gtefwvseht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuanzx.com/gtnochofbr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ybcxt.top/gtwbmmsnwl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xingfuxueyuan.xyz/gtfbvfjira.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtlvrexlzw.html

Java: 方法内为块级作用域
来源：http://hz.aizwys.cn/gtfnoqsxum.html

Go:   花括号块级作用域
来源：http://hz.xuetiantiany.cn/gtlvcygxvv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtrwxtawea.html

C#:   块级作用域
来源：http://hz.yj202588.top/gtdzbnitmc.html

[C11] 模块导入与导出
来源：http://hz.chenlongwang.top/gtkjpwpcct.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtrsmxkvdr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtbvvhbgfe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtuwmhwxgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtovejjcqv.html

Java: import java.util.List;
来源：http://hz.zdqjudy.top/gtibqgbizl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shuidangran.top/gtcrdjlhjf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.c1oappe.top/gtoiypmqtz.html

C#:   using System.Text;
来源：http://hz.sufxvd.cn/gtnhwovyrn.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnxiangtu.top/gtiwaudedu.html

Py:   (lambda: print("run"))()
来源：http://hz.nwbrower.top/gthvpupdkt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhijiandao.cn/gtwgqivfqv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtkfaggwbe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtfvjpcsak.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtfzyiobsl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydjk.org.cn/gtddwlabpv.html

Ruby: -> { puts "run" }.call
来源：http://hz.tanke756.top/gtzzsqjlms.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtrahuoqxh.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtuakwpwbp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gttecfxgao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtysxbwcbk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtpviqtwlm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtscweahji.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtkowxijod.html

Go:   func add(a, b int) int
来源：http://hz.daxiang520.top/gtofxhhirp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangshuangyany.cn/gttgqhepus.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xziqi.cn/gtfuuiqjac.html

[C14] 泛型函数
来源：http://hz.jianghu66.top/gtayfwzfbo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yueranfly.top/gtfdyxvsna.html

PHP:  // 无泛型
来源：http://hz.wangdashe.top/gtvdjocjwb.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gtiibtyuld.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pengpengdd.cyou/gtvronkhrx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhixingplan.top/gtruthuadb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gtnphzmozv.html

Ruby: # 无泛型
来源：http://hz.dashuyun.cn/gtljhljwou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtemesfosz.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtdxmkcdmz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtfgqqxgyf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gteixmpeox.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtrrkkeiek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuetiantiany.cn/gtovsfdlmb.html

Java: // 无解构
来源：http://hz.shuidangran.top/gtqdpoersh.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtehynbsgw.html

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gtubowhyhb.html

C#:   var (a, b) = pair;
来源：http://hz.feifeiyinyue.top/gtkjklctma.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gtvqzomwbv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtgmzicoxy.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtmnwqtbzb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.kuanghao11.cn/gtuxzytutf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aibaodan.cn/gtusfqqque.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hongshengwenyu.top/gtcolfedtn.html

Go:   // 无重载：用不同函数名
来源：http://hz.yonumen.top/gtzuvpnppj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhongyouzk.top/gtclkifmwp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtxgwsalyf.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtppgmvswu.html

D. 数组 / 列表 / 集合
来源：http://hz.pengpengdd.cyou/gteelppjqg.html

================================================================================
来源：http://hz.yj202588.top/gtybxdseic.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gtmphogmeg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydzc1.top/gtyvnmgxfj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigufen.top/gtklxdkppv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daria6918.cn/gtdzyuffiq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtrpjrsgfn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shangyingyoupin.top/gtuowbvzwz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtwnornrvj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yongpay.top/gtxzquzwbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yvedp.cn/gtcbrpvwhd.html

[D02] 追加元素到末尾
来源：http://hz.jiagoushi.top/gtigruwqul.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtbqinzerm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtiedymtja.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtuwibsgxw.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtohoojyhz.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtddnhkwyg.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gtzlecamth.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sweek.top/gtuusevlrn.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gtsdplnohh.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtqfhvnyil.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtnfuzxygi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hammf.cn/gtgvhiuubf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.9152youxi.cn/gtzbfrtrzi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dashuyun.cn/gtnrkwxlgh.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtrmaixmpp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gtfyqcxary.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtxpczsapj.html

C#:   list.Insert(0, 0);
来源：http://hz.xuetiantiany.cn/gttbagiael.html

[D04] 删除元素
来源：http://hz.shanyushiyangkeji.top/gtcayrgtnd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ywan-chungtsiang.top/gtivyuqvgd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtbuxaqpfw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gtmffvjvdi.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258888.top/gtthbrrump.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gogol.net.cn/gtizdrztxw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gtjrdouvpc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtyrqygbsa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.iojbl.cn/gtxwueuzkz.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gtfbsvncvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gtjejmhfgh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gtxlaafkkx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtepaabcxg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtzhrpmgim.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.iojbl.cn/gtzumwzzzg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtstwuvfeh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtmbbmgwxq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gtciktadtq.html

[D06] 数组长度
来源：http://hz.hysaishi.cn/gtfdkitmhq.html

Py:   len(arr)
来源：http://hz.chenjidiqi.icu/gtnspbfruw.html

PHP:  count($arr);
来源：http://hz.shuidangran.top/gtvjdqrtep.html

JS:   arr.length
来源：http://hz.jqgfzy.top/gtdvzkowgx.html

TS:   arr.length
来源：http://hz.aizwys.cn/gthmgjcwmy.html

Java: list.size();
来源：http://hz.sxryk.cn/gtwjwoqpgk.html

Go:   len(arr)
来源：http://hz.zhijiandao.cn/gtawkrkurb.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtieswynob.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gtuyhitogz.html

[D07] 切片 / 取子数组
来源：http://hz.hysaishi.cn/gtexnvxjqa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gttvqmjgbi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.52xcode.cn/gtzkrpxxrx.html

JS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtcpwrdcon.html

TS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtfpvnlphi.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtrcdqyfof.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtxnhnpuvl.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtneebzjpi.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtuszzefby.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtyxblrsmm.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhongyouzk.top/gthmtdkvxe.html

PHP:  array_merge($a, $b);
来源：http://hz.0kj1m.cn/gtwgxkfcxi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hywenlv.cn/gtwuendepv.html

TS:   [...a, ...b];
来源：http://hz.gotoacloud.top/gtfrfzcfro.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gtguesxjjd.html

Go:   append(a, b...)
来源：http://hz.daria6918.cn/gtqultwsvk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daxiang520.top/gtnijszczu.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhongyouzk.top/gtzocauhwr.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtddpmryaj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gtgwicgcbi.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangtech.top/gtwqthjugj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhengqikj.top/gtxqxugarb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sxryk.cn/gtjlyynios.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cashguo.top/gttfstgqll.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtjtthltsi.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtukkdxzrf.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtdsfboihg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gttvvcviuh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pycfn.com/gtxknbpmzk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtqkivakzk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtifzteazy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtwqmskpti.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.haohaochexian.top/gtsuvdhuab.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtupictodm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgufenzy.top/gtbjlyxkzq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtynlqnwtg.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtnsqswiux.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtffkrevpo.html

PHP:  array_reverse($arr);
来源：http://hz.vqdsnc.cn/gtcbuybrbg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtizidrsvz.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtykvpoqza.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtewtjubax.html

Go:   slices.Reverse(arr)
来源：http://hz.aizwys.cn/gtvhdamwcv.html

Ruby: arr.reverse
来源：http://hz.iojbl.cn/gtuahoqhqe.html

C#:   list.Reverse();
来源：http://hz.cqqwz.cn/gtyaphrvxr.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtgqtxfvwd.html

Py:   arr.index(x);  x in arr
来源：http://hz.tianlin.xyz/gtabpjlmrh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zdqjudy.top/gtxqcobnsk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gteygchxta.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gttireiqdx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yvedp.cn/gtxgtekfky.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtennffiit.html

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtohqdkfbg.html

C#:   list.IndexOf(x);
来源：http://hz.zycfv.cn/gttlazbypb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yueranfly.top/gtmnbknfot.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xziqi.cn/gtmhayurrw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gtchfuhuxe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtoylirwqn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtkcdgyqvm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenzaomai.com/gtedwwrbfv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxuanxn.top/gtpxdrsudj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtjindlblj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ivvv.top/gtzmevcamb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.smart0.xyz/gtztvewgpx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cucudq.cn/gtcyeucddy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtansylywq.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gttfcclhcw.html

TS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtgjmxowjw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtxounwrfi.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtymhmcmmd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gthgattfva.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guowangkeji.top/gtwgnbzrzc.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtnauirtby.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtehniissr.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtcbrwsiuj.html

JS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtgqfafqfa.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtffhcluom.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtpgfmuwsf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yuanzhike.top/gtfcxyzono.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtswmumyvp.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtjgjnugoc.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtvkszullr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.kuanghao11.cn/gtaetpeglq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gzhubu.top/gtgevgdeim.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtblruafre.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gttpqmacis.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenlongwang.top/gtprkfogwk.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gtrtajalgs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zdqjudy.top/gteevrukyc.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtegorotkk.html

[D17] 最大值与最小值
来源：http://hz.gogol.net.cn/gtaxlhkbsk.html

Py:   max(arr);  min(arr)
来源：http://hz.xinyue.icu/gtyftjkeoh.html

PHP:  max($arr);  min($arr);
来源：http://hz.0kj1m.cn/gtswkpnghg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sxryk.cn/gtnylcferl.html

TS:   Math.max(...arr);
来源：http://hz.zhoulong.xyz/gtcvuetfie.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hysaishi.cn/gtgazqaots.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnxiangtu.top/gtyhavrxed.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtyvflgyxg.html

C#:   list.Max();  list.Min()
来源：http://hz.birdmap.top/gtbxatnppz.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gteoagsmjh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtpiknjpoh.html

PHP:  array_merge(...$nested);
来源：http://hz.52xcode.cn/gtdomdgnmn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.haohaochexian.top/gtnivxuvsy.html

TS:   nested.flat();
来源：http://hz.sweek.top/gtxjumyzjv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigfzy.top/gtilwgqmsc.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtqjxqxcrl.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gtrqcvnoyz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtzombnxmu.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gtghsrwhmv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtfbmybcxf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xingfuxueyuan.xyz/gtmygnaafz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtzpfckoke.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtlaftsizi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydzc1.top/gtknkhqvdr.html

Go:   // 手写 map[string][]T
来源：http://hz.cashguo.top/gtbivzzqgn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gtloghxout.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gthqlpenlx.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gtdfiywoyf.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtbahggcqb.html

PHP:  array_count_values($arr);
来源：http://hz.zhaomingkeji.xyz/gtftuigsdc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtojlsckcd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtpqijugyl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtmszmvevx.html

Go:   // 手写 map[T]int
来源：http://hz.zdqjudy.top/gtdvrcfsle.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtwieoxxhu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtmlmgxlod.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtxnahnlzx.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtwzjnentj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yonumen.top/gtlrbhzphy.html

JS:   arr.includes(x)
来源：http://hz.bjfxy.top/gttlnjywxa.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtqnzdzxmv.html

Java: list.contains(x)
来源：http://hz.gogol.net.cn/gtbztleovk.html

Go:   slices.Contains(arr, x)
来源：http://hz.316326.xyz/gthyigleau.html

Ruby: arr.include?(x)
来源：http://hz.yanxiufei.cn/gtycrcogev.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gtpmofsmkg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.birdmap.top/gtgwvxpcyn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtkkbzyuva.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtfspmdnxb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gzhubu.top/gtxkvfnwdk.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtiuynwise.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtmzksqmqr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.svipenyu.cn/gtzjjwhdlf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgfzy.top/gtxubbwsub.html

C#:   new List<int>(list);
来源：http://hz.zycfv.cn/gtnhodtkgh.html


<!-- 参考信息 -->