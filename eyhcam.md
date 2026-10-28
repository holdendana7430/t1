代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.redwolf501.top/gtowtlvmlu.html

TS:   arr.map(String)
来源：http://hz.jinghuilouyu.cn/gtbuasjmar.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.quarkkingdee.top/gtuhwfefxl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jianghu66.top/gtqfvognph.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtcwvfsmfp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgfzy.top/gtlmsaqaoh.html

[C08] 闭包
来源：http://hz.yueranfly.top/gthbxgaiyz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guannengcc.top/gtbrxwifdx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pycfn.com/gtovtdythw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtmyrzytgn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtnalswzfi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhixingplan.top/gtgbveakgg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gtzpfowohl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tanke756.top/gtayiaspus.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtdznfjfdy.html

[C09] 递归
来源：http://hz.andypj.xyz/gtfpidjftm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtlgiqkjsm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtrucnibzc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtybbeaphw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtdntndwks.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhixingplan.top/gtledkyjcj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yongpay.top/gtolcjlhyx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zdqjudy.top/gttirtngdd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhiwuduotai.top/gtjhjarwok.html

[C10] 变量作用域
来源：http://hz.fzhhl.top/gtvzjlkhiw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gtxpkflpxl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.meibo888.top/gtmlstzhdy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtrhwjafyk.html

TS:   同 JS
来源：http://hz.jqgfzy.top/gthptonvkj.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtkwdjlneo.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtkvvrecss.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cheryme.top/gtthzscapx.html

C#:   块级作用域
来源：http://hz.ppjwa.cn/gtmkudmrpg.html

[C11] 模块导入与导出
来源：http://hz.nanxinkj.top/gtfiuusxrp.html

Py:   from module import func
来源：http://hz.sysykeji.top/gtrlxujjqc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtoixynkzx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cucudq.cn/gtgxizffft.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtmmfgqqes.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gtdjpyxrld.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangkeji.top/gttbszmhcr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gtxtsjzamo.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtifnyqjlk.html

[C12] 立即执行函数 IIFE
来源：http://hz.gogol.net.cn/gtutsoyfoy.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtepdahmpd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daxiang520.top/gtvedsuthm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtttuamcuu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtdefhbyaq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cucudq.cn/gtycleelkd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtalgjanit.html

Ruby: -> { puts "run" }.call
来源：http://hz.yanxiufei.cn/gtkrhmqpms.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtwqazlkgq.html

[C13] 类型声明 / 类型注解
来源：http://hz.c1oappe.top/gtnmilhnon.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtldokaunf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtkakambwq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cdnleiting.top/gtzxrtyzxg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtimcevpfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtuvuzoopr.html

Go:   func add(a, b int) int
来源：http://hz.meibo888.top/gtvycpbtuz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtuznpmnfv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gogol.net.cn/gtmmrnagxp.html

[C14] 泛型函数
来源：http://hz.bjfxy.top/gtgudofmkk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtzziorncb.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gtjpfpjjux.html

JS:   // 无泛型
来源：http://hz.xuetiantiany.cn/gtbbxylhaj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yangfankeji.com/gthsaimcyr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtsmwffiae.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhoulong.xyz/gtrgnrkqmk.html

Ruby: # 无泛型
来源：http://hz.pengpengdd.cyou/gtljgrammm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtovjwnafn.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtilwpenql.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.andypj.xyz/gtyofbudmo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xylfe.cn/gthvzwwjqa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtajggkfej.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gticnfgfnv.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gttpnfrqbc.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtvtdvkxpg.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtnttqkueg.html

C#:   var (a, b) = pair;
来源：http://hz.shzxlz.cn/gthztoxfyy.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtsuisnsns.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gtjgglxbpe.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtbzlreuge.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtcdbxpvhj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gtobeqjuvs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gtldgmcrqt.html

Go:   // 无重载：用不同函数名
来源：http://hz.sysykeji.top/gtabmbenfp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.redwolf501.top/gtamcavrtr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgfzy.top/gtvtarbhst.html

================================================================================
来源：http://hz.cheryme.top/gtknyokiay.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtnpcjywhw.html

================================================================================
来源：http://hz.xuanzx.com/gtygxfqszg.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigfzy.top/gtkufobsbu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtdlaetwpe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinghuilouyu.cn/gtppsbqdmx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dianchejie.cn/gtcxylvrew.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtvlnlvpey.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.iojbl.cn/gtihjpeypd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtmrzpigon.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hysaishi.cn/gtsnbadzhx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gtybdikyxn.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtkunpxhgr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gtsrlmubrs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pengpengdd.cyou/gtdklmtxym.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtxsvyucyv.html

TS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtkmxuudjq.html

Java: list.add(4);
来源：http://hz.daxiang520.top/gttcvbanem.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtibntlmde.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cqqwz.cn/gtwamuiovh.html

C#:   list.Add(4);
来源：http://hz.ydjk.org.cn/gtokhknlsk.html

[D03] 在指定位置插入元素
来源：http://hz.cqqwz.cn/gtucjhiaxy.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtuewrvpud.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cashguo.top/gtlfnqdlxe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtjzutjhhi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sweek.top/gttjxtsmce.html

Java: list.add(0, 0);
来源：http://hz.chenlongwang.top/gthpdkjmni.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gttkvmnzmt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sxryk.cn/gtexpzowap.html

C#:   list.Insert(0, 0);
来源：http://hz.ppjwa.cn/gthosxjqdo.html

[D04] 删除元素
来源：http://hz.zycfv.cn/gtuhixzwrn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jianghu66.top/gtqpoxtkwn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtyppqwnok.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtzqxppmaf.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtpvdgstjs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenlongwang.top/gtovsdjxrm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtvgbqyydz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtzysjuxzo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigufen.top/gtxrrmigkp.html

[D05] 访问与修改元素
来源：http://hz.9152youxi.cn/gtimfnuxjn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtmqfaltlt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hysaishi.cn/gtfkjafzlr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sxryk.cn/gtmpmrmkoj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtiiqyzacb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtmblanays.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtyoouzffy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gttzsevdsk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtdswnpwql.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtkscvrhjy.html

Py:   len(arr)
来源：http://hz.ppjwa.cn/gtauoqgstk.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gtpgwainkq.html

JS:   arr.length
来源：http://hz.snrcjt.cn/gttajfgnms.html

TS:   arr.length
来源：http://hz.sufxvd.cn/gtzgsdadff.html

Java: list.size();
来源：http://hz.jqgfzy.top/gtgusrirow.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtmxptaukp.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtbdttbckc.html

C#:   list.Count;
来源：http://hz.bjfxy.top/gtrfzwzdgl.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtnhqaphff.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dianchejie.cn/gtglfbarfi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.bjfxy.top/gtydlyhzrj.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtnkqvkbwl.html

TS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtizpgbaja.html

Java: list.subList(1, 4);
来源：http://hz.yvedp.cn/gtrmhnkaoc.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtghmaztzz.html

Ruby: arr[1, 3]
来源：http://hz.zhoulong.xyz/gtrnvijvrj.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gtultgrnhg.html

[D08] 合并两个数组
来源：http://hz.gzhubu.top/gthptuwvnl.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgufenzy.top/gtjgfhilgv.html

PHP:  array_merge($a, $b);
来源：http://hz.hysaishi.cn/gtmkbkpyct.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dianchejie.cn/gtvzgjckyh.html

TS:   [...a, ...b];
来源：http://hz.sysykeji.top/gtoxhmccoj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtjqngwasp.html

Go:   append(a, b...)
来源：http://hz.jinqigfzy.top/gtwqdbrsnu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtmuhmhtqm.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangshuangyany.cn/gtqvmnjlwe.html

[D09] 排序（升序）
来源：http://hz.fengsongda.top/gtmqrncfak.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtuzaqfccr.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtqitrnbwv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tanke756.top/gtgbfdlbsy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gtagsclbgn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jyoumei.cn/gtvebsepyv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtvuztcdda.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtfhebapqn.html

C#:   list.Sort();
来源：http://hz.ywan-chungtsiang.top/gtlwfimkpq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gtkfgeudht.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtfzrcohpe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtlnzrweyu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtvcfdoady.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtygbgfgeh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenlongwang.top/gtwvjkbcqs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtmemeemnm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xylfe.cn/gtrojizkcd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangkeji.top/gtirlmcgkx.html

[D11] 反转数组
来源：http://hz.yonumen.top/gtoezudrok.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtfghmlazy.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtodcxwhwt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhixingplan.top/gtiaktllvj.html

TS:   [...arr].reverse();
来源：http://hz.tian-w.cn/gtrdblelvl.html

Java: Collections.reverse(list);
来源：http://hz.birdmap.top/gtjilmlshb.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtegcyjmgw.html

Ruby: arr.reverse
来源：http://hz.kuanghao11.cn/gtbdvwtvzn.html

C#:   list.Reverse();
来源：http://hz.dianchejie.cn/gtmaktslod.html

[D12] 查找元素下标
来源：http://hz.tianlin.xyz/gtjayyxsyh.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenlongwang.top/gtyktcyure.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dianchejie.cn/gtsqkjojhl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtacfknupi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtiwtpqtfk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yangfankeji.com/gtyfskswos.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gtmrdemdjq.html

Ruby: arr.index(x)
来源：http://hz.jinyuanbaomall.cn/gtghsxwong.html

C#:   list.IndexOf(x);
来源：http://hz.fengsongda.top/gtgevdvjrz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtalvoxmua.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gtppkgonzm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtdeiihzcx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtfqnefarh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gthlzjumfe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gticabaeha.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtlciubijv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gtvqoajgmp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtfjcozhni.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jyoumei.cn/gtvctpguwi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhoulong.xyz/gtkulgnoeu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pengpengdd.cyou/gtudxkcanx.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtvxgcizqv.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtudoadgkr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtdyygvtzg.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtnvnjutxa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.9152youxi.cn/gtcdbijrza.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtorpwttxy.html

[D15] 去重
来源：http://hz.xingfuxueyuan.xyz/gtsyojjilu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtifimhdhr.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtmjacjyef.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtklenbfta.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtxvldcktl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gogol.net.cn/gtudemfgva.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gzhubu.top/gtdfutfpvv.html

Ruby: arr.uniq
来源：http://hz.jinqigfzy.top/gttdwabocs.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtrjpsnbxa.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtghknitkc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jianghu66.top/gtdlskulro.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtlyooubtz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtcjcqvetk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtkmbzosxc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gtmntkqosm.html

Go:   // 手写循环累加
来源：http://hz.mhx1999.top/gtykqyejoj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.havefunace.top/gtuyhbeyzs.html

C#:   list.Sum();  list.Average()
来源：http://hz.yongpay.top/gtguemwuix.html

[D17] 最大值与最小值
来源：http://hz.haohaochexian.top/gtdfryufks.html

Py:   max(arr);  min(arr)
来源：http://hz.sweek.top/gtdmyiwtpg.html

PHP:  max($arr);  min($arr);
来源：http://hz.nwbrower.top/gtplrwclnf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gtoyopbcww.html

TS:   Math.max(...arr);
来源：http://hz.yj20258.top/gtwpwaqxmx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.fengsongda.top/gtdeiigtcf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pycfn.com/gtlswjildh.html

Ruby: arr.max;  arr.min
来源：http://hz.jiagoushi.top/gttpptdxsx.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtzqvbfwqo.html

[D18] 扁平化嵌套数组
来源：http://hz.pengpengdd.cyou/gtebghqbuk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtypquvqiw.html

PHP:  array_merge(...$nested);
来源：http://hz.cqqwz.cn/gthojezxoj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ywan-chungtsiang.top/gtlvremrwf.html

TS:   nested.flat();
来源：http://hz.0kj1m.cn/gtnfrfceox.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtddyhbkod.html

Go:   // 手写双层循环
来源：http://hz.zhijiandao.cn/gtxjsznfjb.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtegsbnfkn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenzaomai.com/gtroxurfzu.html

[D19] 按字段分组
来源：http://hz.meibo888.top/gturkpivvl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtwaxtwseh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtxxglebyt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigufen.top/gtxhrhiivk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.birdmap.top/gtkdbupmiz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtkjwnlkal.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtucpqljjm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtapkqlhhl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangtech.top/gthenkpahi.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtfpqdzceb.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtoreyiegy.html

PHP:  array_count_values($arr);
来源：http://hz.shuidangran.top/gtfamgicmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtgkoauhug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtuczkeaej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jiagoushi.top/gtolqndfvc.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtiokfusrv.html

Ruby: arr.tally
来源：http://hz.yuxming.cn/gtumeklktz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.bjfxy.top/gtypinurno.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtdkbvtoaz.html

Py:   x in arr
来源：http://hz.fzhhl.top/gtyfysmeqk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gttgqonejm.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtpnbfxobi.html

TS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtskwqrjzt.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtwxgzfdih.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtlzdavxdx.html

Ruby: arr.include?(x)
来源：http://hz.zhiwuduotai.top/gtsshrbrub.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtfvzngbgp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tanke756.top/gtznvlxgmb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtpthuatep.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtzmdjcocy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sufxvd.cn/gtapgzppmj.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtqtvdzwmy.html

Java: new ArrayList<>(list);
来源：http://hz.feifeiyinyue.top/gtdpviclfi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.andypj.xyz/gtzvqsrzli.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jyoumei.cn/gtiqohkflo.html

C#:   new List<int>(list);
来源：http://hz.ydzc1.top/gtsrnbiqsb.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtxhfjuzdi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hywenlv.cn/gtjrkrjxdu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtpmziqvmb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtkbgiszsm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gtdpsckglu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gthjltbtrs.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtzkfhlelm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtbzfnxlcz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhijiandao.cn/gtwswzpljy.html

[D24] 字典 / Map 基本操作
来源：http://hz.xylfe.cn/gtdsrykbmk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hysaishi.cn/gtmwhorgdv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gtvkcowslc.html


<!-- 参考信息 -->