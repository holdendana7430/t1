代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.shzxlz.cn/gttqttynme.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.nanxinkj.top/gtkxlzutno.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gaohongyu789.top/gtqbhnbleo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydjk.org.cn/gtzdbewrzx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.smart0.xyz/gtzbxpaglt.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtdcogouop.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hammf.cn/gtxxbumzxj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ydjk.org.cn/gtyccvirax.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuetiantiany.cn/gtgdltetbt.html

TS:   arr.map(String)
来源：http://hz.kuanghao11.cn/gtfyshguqk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fzhhl.top/gtovgmhmmr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shuidangran.top/gtbkmsrima.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtgspmfgbi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guowangkeji.top/gtqsjoewnv.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtbzicahtm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xuetiantiany.cn/gttqzyfzfz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sufxvd.cn/gtswqgodop.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtcohmsfgd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtfegepzpf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangdashe.top/gtnpbaskxg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhixingplan.top/gtlmxtktmq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fzhhl.top/gtpwbyyrri.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtktalbgrs.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtkessvwoq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cheryme.top/gtyqaokcfa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtwqbangkr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtnecbgyfy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtdzbyjamc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydjk.org.cn/gtxzyfucyx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gttmloxwkx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtzktawxct.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtzbvwqhos.html

[C10] 变量作用域
来源：http://hz.9152youxi.cn/gtxzdbrrco.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtszacsnes.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dianchejie.cn/gtgclgocmy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhoulong.xyz/gtcjzsfqog.html

TS:   同 JS
来源：http://hz.ybcxt.top/gtrqtrhxvy.html

Java: 方法内为块级作用域
来源：http://hz.jlsjyb.cn/gtzhdnkzsp.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtkpsnehgr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenjidiqi.icu/gtargxumdt.html

C#:   块级作用域
来源：http://hz.yvedp.cn/gtbejkjocc.html

[C11] 模块导入与导出
来源：http://hz.52xcode.cn/gtxyntjake.html

Py:   from module import func
来源：http://hz.bjfxy.top/gtwutblzoc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.kuanghao11.cn/gtdckgsfga.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gtxxjahyna.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtlzldkglr.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gthezfqjhe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sysykeji.top/gtdexvyica.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sysykeji.top/gtznwbunfs.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtryiqphky.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuanzx.com/gtogfiorqx.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtgljznpfz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gtaprtsxjd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtphrkaoqo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtsaawbhei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtsktnnrdz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gotoacloud.top/gtjfpvlmes.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtkefjxkcf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jqgfzy.top/gtfzpeakkq.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtoewlwlzs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shanyushiyangtech.top/gtrnzllmqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtmjaqlskh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtqekmzmox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtluhxeusj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gthryozclg.html

Go:   func add(a, b int) int
来源：http://hz.nanxuanxn.top/gtmbitbxxr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtffxqetrw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtdzlnoaei.html

[C14] 泛型函数
来源：http://hz.chenzaomai.com/gtfpzcmqoj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtxmewbxnk.html

PHP:  // 无泛型
来源：http://hz.ydjk.org.cn/gttyeuhuxo.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtzqawnzrg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daxiang520.top/gtwyhntrbt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fzhhl.top/gtqeedfvff.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtkhcpiuin.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtovchngmq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtyqebeoxx.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangtech.top/gtsquafmwq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtvnikohsk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtqioezcai.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtmdoxwtdl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtwxbmndkn.html

Java: // 无解构
来源：http://hz.havefunace.top/gtlzwjofjs.html

Go:   // 无解构
来源：http://hz.dashuyun.cn/gtaoihvkbm.html

Ruby: a, b = pair
来源：http://hz.jinqigfzy.top/gtwvdgkztc.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtirgtfcix.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtyiesdwbp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gtvyzefshd.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtxxlxwfpq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zdqjudy.top/gtabpdtghp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gtojquonkf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.52xcode.cn/gtsdggubyu.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangshuangyany.cn/gtyopixsau.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtvonzizqd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gtsjgscczk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gttrdioxui.html

D. 数组 / 列表 / 集合
来源：http://hz.feifeiyinyue.top/gtrwrmacxk.html

================================================================================
来源：http://hz.sufxvd.cn/gtzbgesdny.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtunjswnhh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yongpay.top/gtstmktqer.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtxejhhyqh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtarbuzhkz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nwbrower.top/gtjalbcayg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hfpthk.cn/gtqfcxlcdr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtzhgjlogq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pycfn.com/gtgvhiqvhh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnqzz.top/gtmmzdmvos.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gtpafbcahe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gtximtkmem.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtybrtmvlx.html

JS:   arr.push(4);
来源：http://hz.guannengcc.top/gtwxsrhwdr.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtzrshnmgl.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtfncgqbtj.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtfmsmtdgp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cucudq.cn/gtltpnxqor.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtdwbratje.html

[D03] 在指定位置插入元素
来源：http://hz.cdnleiting.top/gtesiovpcm.html

Py:   arr.insert(0, 0)
来源：http://hz.yuanzhike.top/gttmwwqgyk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gzhubu.top/gtnclchlno.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtpwucllbt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtwhrkokrl.html

Java: list.add(0, 0);
来源：http://hz.nanxinkj.top/gthkilhlmu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtpuhcphlc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtllqbddsg.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtkwcbqhgy.html

[D04] 删除元素
来源：http://hz.tian-w.cn/gthxygusbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuanzhike.top/gtbpslzpqj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sxryk.cn/gtnsktbqgx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fengsongda.top/gtlnoaqvop.html

TS:   arr.splice(0, 1);
来源：http://hz.yuanzhike.top/gtntykfgzh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnqzz.top/gtntzsvogv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtzyrdlsmd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yangfankeji.com/gtnzgbbdai.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gtkhpovfar.html

[D05] 访问与修改元素
来源：http://hz.ywan-chungtsiang.top/gtwmxjpgna.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtqboaaasp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.redwolf501.top/gtjctvosgb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtphobsrhv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gttjoxobwl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgufenzy.top/gtujbkdbvu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtyzgwatfz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtvvyjjtah.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtymxcfkou.html

[D06] 数组长度
来源：http://hz.zhixingplan.top/gtklnyioof.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gtnzipfjli.html

PHP:  count($arr);
来源：http://hz.aibaodan.cn/gtvcnkgzjh.html

JS:   arr.length
来源：http://hz.jinqigufen.top/gtolqaokwm.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtluprybox.html

Java: list.size();
来源：http://hz.xziqi.cn/gtqouqgadz.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtokxcxvdf.html

Ruby: arr.length; arr.size
来源：http://hz.jiagoushi.top/gtpvphinvu.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtsapvwcdh.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtfyrhqinx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cqqwz.cn/gtesrtcnsa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gotoacloud.top/gtdjdgehhm.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtfaeacdxt.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtwkkzpuxu.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtzplmfynt.html

Go:   arr[1:4]
来源：http://hz.gaohongyu789.top/gtmcmmvvyq.html

Ruby: arr[1, 3]
来源：http://hz.redwolf501.top/gtzuuypjws.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtfnhoudax.html

[D08] 合并两个数组
来源：http://hz.zycfv.cn/gtsipthqnz.html

Py:   a + b;  a.extend(b)
来源：http://hz.dianchejie.cn/gtiuhodroq.html

PHP:  array_merge($a, $b);
来源：http://hz.zhengqikj.top/gtlwxlkvmo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnxiangtu.top/gtthirxyxi.html

TS:   [...a, ...b];
来源：http://hz.mhx1999.top/gtncebeeyb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hywenlv.cn/gtjczxthad.html

Go:   append(a, b...)
来源：http://hz.aibaodan.cn/gtbnfuutex.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gtuhrcyjqs.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtcxkajotd.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtsjbxdufh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtbxekkbbz.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtugjmpnwg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gogol.net.cn/gtmqhzedwx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gtpnpdmcng.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gthvsrxohw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtryyocfdy.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtwnsfdlab.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtxlektoag.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhongyouzk.top/gtmezprmrj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.c1oappe.top/gtnlkhmbiq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhixingplan.top/gtocuonrpm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtzyybvcrp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtwluwsjsb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtvwpnleav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtzlxuaqcm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ppjwa.cn/gtbdrwpbem.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtdfcnrjyo.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtsalsiswk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtahddoyww.html

PHP:  array_reverse($arr);
来源：http://hz.vqdsnc.cn/gtatbsmyuz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtsohdsgoh.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtettgvudt.html

Java: Collections.reverse(list);
来源：http://hz.xuetiantiany.cn/gtvovchcwu.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gttzxgputj.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtfprrqepa.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtwirgtoyp.html

[D12] 查找元素下标
来源：http://hz.zhiwuduotai.top/gtsslkygar.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtdyavoati.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gotoacloud.top/gtmdtrumsa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtydapyqeq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtzhnpacui.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sufxvd.cn/gtzggbcbhp.html

Go:   slices.Index(arr, x)
来源：http://hz.snrcjt.cn/gtihqoqjsl.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangtech.top/gtgytljixq.html

C#:   list.IndexOf(x);
来源：http://hz.feifeiyinyue.top/gtcndvuidm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jyoumei.cn/gtvrgemmgi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zdqjudy.top/gtyymfpiut.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.snrcjt.cn/gtjvwfyeyu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtbtxwehuy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtbkrtrzbs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.birdmap.top/gtuvdpsyeu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtshxjjmoo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydjk.org.cn/gtyxwqglco.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.vqdsnc.cn/gtdtobcjbd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yanxiufei.cn/gtwukuqnaf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gthotwxskq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gthrnufhxi.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtgqeascju.html

TS:   arr.map(x => x * 2)
来源：http://hz.cqqwz.cn/gtnidfwabw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gtrgvhqgge.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gthmstxwld.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtpiymqfkz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtffuuxuvr.html

[D15] 去重
来源：http://hz.smart0.xyz/gtmcljxfpb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtqglhnhoi.html

PHP:  array_unique($arr);
来源：http://hz.yonumen.top/gtemdvfzsr.html

JS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtkftfnuan.html

TS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtimwdefik.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtxuufpvia.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtzqnckabv.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtakxrpsyn.html

C#:   list.Distinct().ToList()
来源：http://hz.jyoumei.cn/gtghmrdnco.html

[D16] 求和与平均值
来源：http://hz.yvedp.cn/gtehaszkyq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gtnsmgbggo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtqtirhgkr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gttloarksx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gteecxxphy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtptiwqdiy.html

Go:   // 手写循环累加
来源：http://hz.yangfankeji.com/gtsxobtrab.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtqfdahopk.html

C#:   list.Sum();  list.Average()
来源：http://hz.xingfuxueyuan.xyz/gttnnryjzs.html

[D17] 最大值与最小值
来源：http://hz.9152youxi.cn/gtslvjszot.html

Py:   max(arr);  min(arr)
来源：http://hz.nwbrower.top/gtdddkkgbf.html

PHP:  max($arr);  min($arr);
来源：http://hz.jianghu66.top/gtcjqbxrbp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtyxghlwke.html

TS:   Math.max(...arr);
来源：http://hz.cqqwz.cn/gtbuctocet.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hywenlv.cn/gtydwwakts.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gotoacloud.top/gtyafpceja.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtkvqprdmv.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtcwcigvwk.html

[D18] 扁平化嵌套数组
来源：http://hz.wangshuangyany.cn/gtbzcseiaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.haohaochexian.top/gtsnntztpu.html

PHP:  array_merge(...$nested);
来源：http://hz.quarkkingdee.top/gtoyeibvqs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gtcnyjzdov.html

TS:   nested.flat();
来源：http://hz.yongpay.top/gtftoablom.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinghuilouyu.cn/gtzhkzjntu.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtchcrdpyj.html

Ruby: nested.flatten
来源：http://hz.daria6918.cn/gtdnifgsgm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtldxceynp.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtdllvjfwi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtxstujxpe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hammf.cn/gtirotgjhu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtuaiaidkw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtjmjmpnjx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtfgqemlep.html

Go:   // 手写 map[string][]T
来源：http://hz.ivvv.top/gtikcxneux.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtdkpbduut.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gtlsrbxdlq.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtxplenthd.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtvnfamdae.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gtubzzprtq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtypwowjqh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnxiangtu.top/gtqqbozazb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtuvxntsar.html

Go:   // 手写 map[T]int
来源：http://hz.xuetiantiany.cn/gtegtqstfq.html

Ruby: arr.tally
来源：http://hz.cdnleiting.top/gtzidtbify.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtzeikvgoa.html

[D21] 判断是否包含某元素
来源：http://hz.xylfe.cn/gtzrrsohsc.html

Py:   x in arr
来源：http://hz.fengsongda.top/gtiylgcqcl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtyoqaatmm.html

JS:   arr.includes(x)
来源：http://hz.redwolf501.top/gtwwbqjlly.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtjvuxgtio.html

Java: list.contains(x)
来源：http://hz.shanyushiyangtech.top/gtjsoguyha.html

Go:   slices.Contains(arr, x)
来源：http://hz.yonumen.top/gtvspajmvt.html

Ruby: arr.include?(x)
来源：http://hz.chenzaomai.com/gtciiyerhc.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gtajzxudth.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtldrqpxrj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gthvnqrkkw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtxcyrhkql.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xinyue.icu/gtvnehbuvq.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtnlxtxiqx.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtpzwtgkdd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tianlin.xyz/gtoukwzmgo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gtkutsxjab.html

C#:   new List<int>(list);
来源：http://hz.gaohongyu789.top/gtqckmfknz.html

[D23] reduce 累积计算
来源：http://hz.chenzaomai.com/gtghmdmody.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtlprafhyh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gogol.net.cn/gtdkgumaar.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtoqekkylw.html


<!-- 参考信息 -->