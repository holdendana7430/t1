代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.cucudq.cn/gtccggiqcc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtzkdsqivl.html

[C08] 闭包
来源：http://hz.jqgfzy.top/gtbbhcxjze.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pengpengdd.cyou/gtlgsodrmm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.c1oappe.top/gtfnoepfzd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gteopxuelm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtvwtdzicf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gtfhcambii.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shangyingyoupin.top/gtnbukqhbl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gtlniqznmr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtjnyvvocr.html

[C09] 递归
来源：http://hz.shzxlz.cn/gtbdcvpnrm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hongshengwenyu.top/gtbbwkyjpw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hongshengwenyu.top/gtawustmjh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangdashe.top/gtepwnmxvx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtcdioyvpg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xinyue.icu/gtskygatky.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtnrorwvpd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtkpiwslxi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gtuifmaonb.html

[C10] 变量作用域
来源：http://hz.feifeiyinyue.top/gtubxiurqh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shuidangran.top/gtjmdxqzgh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nwbrower.top/gtlhzsjywq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxuanxn.top/gttvhguejd.html

TS:   同 JS
来源：http://hz.ivvv.top/gtwpsbglol.html

Java: 方法内为块级作用域
来源：http://hz.guowangkeji.top/gtktloclqd.html

Go:   花括号块级作用域
来源：http://hz.kuanghao11.cn/gtpzzcfuuo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuxming.cn/gtykjqgfmj.html

C#:   块级作用域
来源：http://hz.yj20258888.top/gtgdmjqpix.html

[C11] 模块导入与导出
来源：http://hz.aibaodan.cn/gtamdnjbdv.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtygwqgjto.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtheatbcfx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ivvv.top/gtyguzeooa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.snrcjt.cn/gtqxluvimk.html

Java: import java.util.List;
来源：http://hz.yj202588.top/gtvprkvwxw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhongyouzk.top/gtwjftiheb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hnxiangtu.top/gtpoexutbc.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtfiffqegh.html

[C12] 立即执行函数 IIFE
来源：http://hz.guannengcc.top/gtrxvbzqnz.html

Py:   (lambda: print("run"))()
来源：http://hz.zhijiandao.cn/gtceawbzej.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cheryme.top/gtmewnbzmq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtaklbyrlu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gthrqghrsw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.andypj.xyz/gtxwlcyskl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtjwahdugd.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtgcwvhwcw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.quarkkingdee.top/gtkepmwscu.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhengqikj.top/gtfvyeqzvl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtozlhcvpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gthigleymd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fengsongda.top/gtfucyjeov.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtcfcdbhit.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtvvdwtcgn.html

Go:   func add(a, b int) int
来源：http://hz.gzhubu.top/gtmmxopsmx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtifzjpacs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhijiandao.cn/gttyuhxipb.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtqhhmhshx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtwyfeonxd.html

PHP:  // 无泛型
来源：http://hz.smart0.xyz/gtasdbcljp.html

JS:   // 无泛型
来源：http://hz.cdnleiting.top/gtbiuffpuy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtqpuzfxpq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.quarkkingdee.top/gtjfiwmfme.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daxiang520.top/gtmeuwubjp.html

Ruby: # 无泛型
来源：http://hz.ivvv.top/gtcrqeqmcw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.bjfxy.top/gtwnsklkci.html

[C15] 解构 / 展开参数
来源：http://hz.tanke756.top/gtnhszijvp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtqduyhxof.html

PHP:  [$a, $b] = $pair;
来源：http://hz.quarkkingdee.top/gtjkkcclwn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtfmwrkdjc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtxgxzyjjh.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtkuvlaikn.html

Go:   // 无解构
来源：http://hz.ydzc1.top/gtuexnsfur.html

Ruby: a, b = pair
来源：http://hz.iojbl.cn/gtdiolzjvc.html

C#:   var (a, b) = pair;
来源：http://hz.jlsjyb.cn/gtmlaemthj.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangtech.top/gtunbpdxyq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtilyznoyb.html

PHP:  // 无重载
来源：http://hz.jqgufenzy.top/gtfsqdqlps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtpbilkowl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ppjwa.cn/gtoxujqaoh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aibaodan.cn/gtapqhjyzg.html

Go:   // 无重载：用不同函数名
来源：http://hz.316326.xyz/gttvssszcb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dashuyun.cn/gtudmavnpw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xingfuxueyuan.xyz/gtkdlztktv.html

================================================================================
来源：http://hz.zhixingplan.top/gtditabmlg.html

D. 数组 / 列表 / 集合
来源：http://hz.pycfn.com/gtueyxnrew.html

================================================================================
来源：http://hz.yuanzhike.top/gtuexdoczb.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtvqhwngea.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.andypj.xyz/gtmxbmgttg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtqfjimkpq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.andypj.xyz/gtkoxcurbf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cdnleiting.top/gttnsqqzco.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daxiang520.top/gtoholmokj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnxiangtu.top/gtesxvhmez.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtzicuguoz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangtech.top/gtxczmguak.html

[D02] 追加元素到末尾
来源：http://hz.hnqzz.top/gtgzpxeffx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.vqdsnc.cn/gtcocbkocg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuanzhike.top/gtdexehdmz.html

JS:   arr.push(4);
来源：http://hz.nwbrower.top/gthieyszsq.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtevhzpttb.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtmzgdfujn.html

Go:   arr = append(arr, 4)
来源：http://hz.yueranfly.top/gtoxvseqkd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nwbrower.top/gtvgbmewmh.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtgcetopxs.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtvokwnmev.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtgifqgmlx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.smart0.xyz/gtuxcmhkmr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sufxvd.cn/gtdjpjdoyy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtizsxnsbl.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtugqoslrv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtlfukxgta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hongshengwenyu.top/gtxmisqswy.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtfrwlncmw.html

[D04] 删除元素
来源：http://hz.quarkkingdee.top/gtxmkhtyml.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.c1oappe.top/gtlsjpvvon.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.0kj1m.cn/gtkvoxxmff.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ehwqpu.com/gteuiebxhd.html

TS:   arr.splice(0, 1);
来源：http://hz.jiagoushi.top/gtsqkkpsiy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgfzy.top/gtwuxmazoq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fzhhl.top/gtdlftopdw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtbhzojepy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hysaishi.cn/gtgwqczrfb.html

[D05] 访问与修改元素
来源：http://hz.ywan-chungtsiang.top/gtsoqntchu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtgrtwcjea.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hammf.cn/gtdefqhibb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gthelsxwbd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtidgzaahy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xziqi.cn/gtiogxtpef.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtaojlspaj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtpizypvcv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuanzhike.top/gtdilontkw.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtnmvuaces.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtgchcmawv.html

PHP:  count($arr);
来源：http://hz.chenjidiqi.icu/gtussmktcc.html

JS:   arr.length
来源：http://hz.jqgufenzy.top/gttcwiaelp.html

TS:   arr.length
来源：http://hz.cdnleiting.top/gthjrgawkb.html

Java: list.size();
来源：http://hz.jinghuilouyu.cn/gtmmuffteu.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtxbgoimnw.html

Ruby: arr.length; arr.size
来源：http://hz.zycfv.cn/gtipsaeqfl.html

C#:   list.Count;
来源：http://hz.ybcxt.top/gtludnwypn.html

[D07] 切片 / 取子数组
来源：http://hz.daria6918.cn/gtvxndliws.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtmnfhaheb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtljvarczk.html

JS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtmqtcmdqo.html

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtcudqzpyc.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtooawiuhv.html

Go:   arr[1:4]
来源：http://hz.aizwys.cn/gtbobixfsj.html

Ruby: arr[1, 3]
来源：http://hz.aibaodan.cn/gtmbasshhf.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhengqikj.top/gtgtvjqqus.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtsgpbootr.html

Py:   a + b;  a.extend(b)
来源：http://hz.yangfankeji.com/gtmaqthrzy.html

PHP:  array_merge($a, $b);
来源：http://hz.havefunace.top/gtqrfojfmq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtqamknshq.html

TS:   [...a, ...b];
来源：http://hz.aibaodan.cn/gttrbgpvht.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtxjjkvrda.html

Go:   append(a, b...)
来源：http://hz.jiagoushi.top/gtvwtlcztp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuanzhike.top/gtmbididzj.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhengqikj.top/gtzqpvqqzx.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtibmuhdwj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtigchzfye.html

PHP:  sort($arr);
来源：http://hz.andypj.xyz/gtednokbgt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtvoqqnpju.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258888.top/gtwwddsiqx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yangfankeji.com/gtfhnpmzbm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.0kj1m.cn/gtldpcqjpx.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtxqguwpsv.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtgacsuwqk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtuolkhkor.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zycfv.cn/gtdrtutjbj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtsobazckq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jlsjyb.cn/gtekejniyh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtoofwjoxt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtjfydwrrz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gthgfuyims.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtaskggepb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gteakzcqsv.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtsdztfusq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnqzz.top/gtoegzkjbl.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gtlzwqlmtv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtacgpbqym.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gteksmajnd.html

Java: Collections.reverse(list);
来源：http://hz.dianchejie.cn/gtdzgogpsa.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtgqkcjuuh.html

Ruby: arr.reverse
来源：http://hz.tian-w.cn/gtnldpylre.html

C#:   list.Reverse();
来源：http://hz.gaohongyu789.top/gteuqcylhj.html

[D12] 查找元素下标
来源：http://hz.andypj.xyz/gtjudmnfrf.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gtkujmlnjx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtrycihtet.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtpyyodcbg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtzfdwqons.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.feifeiyinyue.top/gtesztokpy.html

Go:   slices.Index(arr, x)
来源：http://hz.cucudq.cn/gtlwddbyln.html

Ruby: arr.index(x)
来源：http://hz.guowangkeji.top/gtyarkoygl.html

C#:   list.IndexOf(x);
来源：http://hz.cheryme.top/gtqflfjnjj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxinkj.top/gtlgthspss.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenlongwang.top/gtcjiumjyt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gtovmzoemh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtwcmihwuy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtdqnggaau.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zdqjudy.top/gtnmxoiuol.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtulzsjtnt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jlsjyb.cn/gtdqbtfzjj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yongpay.top/gtcfjmyldf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.52xcode.cn/gtfjdyxdgt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtkijklsda.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinyuanbaomall.cn/gtkhyyhgiu.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtmipfvfdz.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtdovhvdll.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zdqjudy.top/gtxbncnjoi.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtmkqpkity.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pengpengdd.cyou/gtxhqsetql.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxuanxn.top/gtubbrehip.html

[D15] 去重
来源：http://hz.xingfuxueyuan.xyz/gtqgyltvpd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtdfxtazev.html

PHP:  array_unique($arr);
来源：http://hz.zdqjudy.top/gtndwpxhgd.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtbcydnwvk.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtfpfrognq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtwpbyodsn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtsrytncoa.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtteldpcco.html

C#:   list.Distinct().ToList()
来源：http://hz.sxryk.cn/gtjbypcraw.html

[D16] 求和与平均值
来源：http://hz.yvedp.cn/gthyiufrbi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gtaqfeafia.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guowangkeji.top/gtqhayfqmk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtckniimsw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtxyafkxie.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtdfftlhtg.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gtooghtljk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtwagbrveq.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtaitrzpbm.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtflwfjejq.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gtanxjsiib.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gtwmzrchda.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gtnzqlquhw.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtasjsvosq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtzcbgzvig.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gttammkfcu.html

Ruby: arr.max;  arr.min
来源：http://hz.hnqzz.top/gtpupkzltz.html

C#:   list.Max();  list.Min()
来源：http://hz.fzhhl.top/gtcilbguiz.html

[D18] 扁平化嵌套数组
来源：http://hz.snrcjt.cn/gtrwyftynu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jlsjyb.cn/gtchuorxsk.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtzvyqaemp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yanxiufei.cn/gtwtpejmlt.html

TS:   nested.flat();
来源：http://hz.zhoulong.xyz/gtrotnelub.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gtqspzfcip.html

Go:   // 手写双层循环
来源：http://hz.aizwys.cn/gtznolaxzc.html

Ruby: nested.flatten
来源：http://hz.hnqzz.top/gtmppfcjlp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zycfv.cn/gtgdtxrfzs.html

[D19] 按字段分组
来源：http://hz.chenjidiqi.icu/gtouhqdtrz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gtiqvvvrjk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cashguo.top/gtytupqogt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhaomingkeji.xyz/gtyvsmghev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtjwgekjga.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ywan-chungtsiang.top/gtrjbhalqx.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtmqeejsri.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtjovldjin.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtuqdpfqpo.html

[D20] 统计每个元素出现次数
来源：http://hz.zhoulong.xyz/gtzauvgyrk.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtvilcdpfk.html

PHP:  array_count_values($arr);
来源：http://hz.316326.xyz/gtrmpoifdp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtflzadoii.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtrgiqfhdd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daxiang520.top/gtdbzjaxvw.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtvanuzpzz.html

Ruby: arr.tally
来源：http://hz.zhongyouzk.top/gtfxlupnwd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yonumen.top/gtlcquqqzj.html

[D21] 判断是否包含某元素
来源：http://hz.cdnleiting.top/gtvexwtkaz.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtyzfgexfc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daxiang520.top/gtmkdlsxut.html

JS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtelznbcex.html

TS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtbkmydhmp.html

Java: list.contains(x)
来源：http://hz.chenlongwang.top/gtibhovnoq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yanxiufei.cn/gtzryxehwo.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtwpyiapxd.html

C#:   list.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gteshgkzpp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.c1oappe.top/gtsczykpwb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtzipcqddh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gtlupvevhc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gthswxpcyv.html

TS:   [...arr];
来源：http://hz.redwolf501.top/gtxnkthivy.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtrdjrhblg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tianlin.xyz/gtjwdpoijh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.feifeiyinyue.top/gtptrtuxui.html

C#:   new List<int>(list);
来源：http://hz.dashuyun.cn/gtfcpzsjkb.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gtronfnncw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtxteqaokk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhoulong.xyz/gtdsjukevu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtyazddoci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtktdnckti.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtlmqbknoq.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtzrrkfslo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtprtidnxd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dashuyun.cn/gthmnwambz.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtsajqjcea.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtiejtfabv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtrnffeeqq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gttqfnhnjt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgfzy.top/gtoplrhogz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtbdtggqzv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sysykeji.top/gtocghmmcf.html


<!-- 参考信息 -->