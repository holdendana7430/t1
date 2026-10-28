代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.iojbl.cn/gtgeupyjel.html

TS:   arr.map(String)
来源：http://hz.jinqigufen.top/gtcayainqy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.svipenyu.cn/gtsogfgimy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuanzhike.top/gtcfkfwjyo.html

Ruby: arr.map(&:upcase)
来源：http://hz.snrcjt.cn/gtphxnbwxq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.quarkkingdee.top/gtilysdcln.html

[C08] 闭包
来源：http://hz.yongpay.top/gtmabpqbeq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhoulong.xyz/gtyaczogon.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.kuanghao11.cn/gtplmrliut.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtssgfpigk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtmemyunvj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhijiandao.cn/gtxqecxrns.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pengpengdd.cyou/gtcmwdgrmu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtcvgbbusm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtgfglcaja.html

[C09] 递归
来源：http://hz.daria6918.cn/gthnktktpk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtfayyggne.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtojwtleho.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtuphxogbc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gthekvlwxg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gttnbljexp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydzc1.top/gtwlgngrqp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangshuangyany.cn/gtjyeikzly.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenjidiqi.icu/gturlavsmp.html

[C10] 变量作用域
来源：http://hz.ppjwa.cn/gtstmluvdi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yongpay.top/gtlpjdarlx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtyjajzqyv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtbtuvzktq.html

TS:   同 JS
来源：http://hz.hnqzz.top/gtuayyvyft.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtblczhbzz.html

Go:   花括号块级作用域
来源：http://hz.redwolf501.top/gtrefjkezc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinyuanbaomall.cn/gtdresogox.html

C#:   块级作用域
来源：http://hz.guowangkeji.top/gtaozbgusb.html

[C11] 模块导入与导出
来源：http://hz.9152youxi.cn/gtrhlpdmsr.html

Py:   from module import func
来源：http://hz.mhx1999.top/gtqbcnxnml.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guannengcc.top/gtwrnvuerr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.mhx1999.top/gtzavrubit.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigufen.top/gtqrtixcls.html

Java: import java.util.List;
来源：http://hz.chenlongwang.top/gtllrbtixb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tianlin.xyz/gtmgquudoe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cdnleiting.top/gtiodzxyvv.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtfyngdowt.html

[C12] 立即执行函数 IIFE
来源：http://hz.dashuyun.cn/gtyqalqejp.html

Py:   (lambda: print("run"))()
来源：http://hz.yueranfly.top/gtajcxlqcq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cashguo.top/gtxchvvyyu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtrsvvpsqz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.snrcjt.cn/gtgynkenwi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.0kj1m.cn/gtbtaxjlsk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtsuussuzd.html

Ruby: -> { puts "run" }.call
来源：http://hz.xinyue.icu/gtugbviqco.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.meibo888.top/gtxqftewqv.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtmxcugfeg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtbjklbtip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gturccnlhl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jlsjyb.cn/gtjbuayrfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtfufioyty.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtmiwzobei.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gtqgmtllqq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuanzx.com/gtzmmyyuef.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenjidiqi.icu/gtzixcoutd.html

[C14] 泛型函数
来源：http://hz.xuanzx.com/gtnqolqmsl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daxiang520.top/gtiezgwlbk.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtierojkag.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtchijrjem.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtsihfazqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xingfuxueyuan.xyz/gtngybjdvr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhaomingkeji.xyz/gtsvknqtkr.html

Ruby: # 无泛型
来源：http://hz.jqgfzy.top/gtihiuabem.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtaiaxqjtm.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gteichktul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.dianchejie.cn/gtxxytmeir.html

PHP:  [$a, $b] = $pair;
来源：http://hz.feifeiyinyue.top/gtpeowotvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtgfydrnvv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.snrcjt.cn/gtytkmqtgw.html

Java: // 无解构
来源：http://hz.gogol.net.cn/gtkstqjbgy.html

Go:   // 无解构
来源：http://hz.havefunace.top/gtyjkignpb.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gtlndrbevl.html

C#:   var (a, b) = pair;
来源：http://hz.52xcode.cn/gtoncjuatq.html

[C16] 函数 / 方法重载
来源：http://hz.chenlongwang.top/gtugqvfand.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtwnmenpfz.html

PHP:  // 无重载
来源：http://hz.wangdashe.top/gtvknobihy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtaksnknpp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinghuilouyu.cn/gtwursbspb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sysykeji.top/gtumoclpkg.html

Go:   // 无重载：用不同函数名
来源：http://hz.316326.xyz/gtjqiuauoq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cucudq.cn/gttawmgsae.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.mhx1999.top/gtrvzhvhtw.html

================================================================================
来源：http://hz.jianghu66.top/gtnuuqmuow.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtpvidawgm.html

================================================================================
来源：http://hz.yvedp.cn/gttwqdgkzm.html

[D01] 创建数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtgqsbwqqj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangtech.top/gtyuayaajl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.bjfxy.top/gtacdbmxiy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xinyue.icu/gtsdqgdhax.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigufen.top/gtobziocsy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jlsjyb.cn/gtpgaeuxgy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtllinsrwt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtmlpqizga.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtmlmdfjsu.html

[D02] 追加元素到末尾
来源：http://hz.cqqwz.cn/gtkcfoalhv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtqlikcpda.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gttoghrsdq.html

JS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtytcxsoaj.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtdfezdrrv.html

Java: list.add(4);
来源：http://hz.sweek.top/gtifpvyfmr.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtleprrrrb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gotoacloud.top/gtzcyaresw.html

C#:   list.Add(4);
来源：http://hz.yonumen.top/gtowverjex.html

[D03] 在指定位置插入元素
来源：http://hz.ydjk.org.cn/gtodlqatho.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgfzy.top/gtemiamvfz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtbwbmwaef.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj202588.top/gtmofuypuy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhengqikj.top/gtafcvjihs.html

Java: list.add(0, 0);
来源：http://hz.yuanzhike.top/gtkurethbj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangtech.top/gtefsohvrv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gtghfzcsbg.html

C#:   list.Insert(0, 0);
来源：http://hz.aibaodan.cn/gtggpanius.html

[D04] 删除元素
来源：http://hz.zhixingplan.top/gthcmkpkph.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtyrohwarv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cashguo.top/gtkknhnaxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yueranfly.top/gtoifnrspk.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtafdyouva.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtrumzucqf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtnyqjwwrf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guannengcc.top/gtwioayqkb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtrozfzdnk.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangtech.top/gttximiedk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtqszddrvc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jianghu66.top/gtdnmswmrr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtyqtojwzu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jianghu66.top/gtnibronea.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnqzz.top/gtelhhktlh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gtlgfmphsd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtrslxfyko.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gogol.net.cn/gtbsxeqqzb.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtjvckmgtc.html

Py:   len(arr)
来源：http://hz.pengpengdd.cyou/gtupijsvgz.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtdglnqzfm.html

JS:   arr.length
来源：http://hz.9152youxi.cn/gtlzinypza.html

TS:   arr.length
来源：http://hz.yj202588.top/gtmgnjurty.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtayjijknk.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtcgkfxjqf.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtifwdtsem.html

C#:   list.Count;
来源：http://hz.gaohongyu789.top/gtzfxxkuzu.html

[D07] 切片 / 取子数组
来源：http://hz.ehwqpu.com/gtoyqvclab.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuxming.cn/gtwrzehhtn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtkhxnelie.html

JS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gthibgkfdv.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gttykcrywb.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtbwrewnbh.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtsbrscmcv.html

Ruby: arr[1, 3]
来源：http://hz.shangyingyoupin.top/gtsiloxexn.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxinkj.top/gtuptgqieu.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtfeykgipv.html

Py:   a + b;  a.extend(b)
来源：http://hz.yonumen.top/gtgkndnurs.html

PHP:  array_merge($a, $b);
来源：http://hz.xingfuxueyuan.xyz/gtlmqzzxpz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zycfv.cn/gtwvocjfsq.html

TS:   [...a, ...b];
来源：http://hz.vqdsnc.cn/gtiwdrroky.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtgmrjtgeb.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gtypmoniog.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jlsjyb.cn/gtjqhhvvib.html

C#:   a.Concat(b).ToList()
来源：http://hz.bjfxy.top/gtbcgakvoz.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtrziioyjk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtwmvfauqx.html

PHP:  sort($arr);
来源：http://hz.ivvv.top/gthxjsdmvl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zdqjudy.top/gtjkzevahm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hongshengwenyu.top/gtuantmtuh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtgqlzasfz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtzwfazxci.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtpfinydxz.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtuklgilag.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtzniceghe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gtxwgmitjn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtgfcfoqmg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtrbvogith.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtwabbgrui.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtdyzhncmv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gthyrctvxv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cucudq.cn/gtcccteqwk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hywenlv.cn/gtamauirym.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gtouvukbdk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtsullexse.html

PHP:  array_reverse($arr);
来源：http://hz.0kj1m.cn/gtxsflygic.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtibgwljpt.html

TS:   [...arr].reverse();
来源：http://hz.zhengqikj.top/gttrtqbouj.html

Java: Collections.reverse(list);
来源：http://hz.ehwqpu.com/gtogzaigrj.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gtvzqvivtp.html

Ruby: arr.reverse
来源：http://hz.gzhubu.top/gtwbeyejle.html

C#:   list.Reverse();
来源：http://hz.zycfv.cn/gtnsqyrufd.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtnnwcvhvb.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gthhymbfvx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shuidangran.top/gtqindrwaj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtglcmbjkz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtnbvsihag.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sufxvd.cn/gtkxvegrlq.html

Go:   slices.Index(arr, x)
来源：http://hz.cucudq.cn/gtlgkvhlmx.html

Ruby: arr.index(x)
来源：http://hz.cqqwz.cn/gthkpbcaal.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtypzxddyd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.haohaochexian.top/gttajaqkbd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtntkhrtiq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gtwwxtfgmx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtqojymgfo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtmwduntoy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhengqikj.top/gtokzcblaa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtmuhzoxby.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gttwhoqzal.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuanzx.com/gthfajaope.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gtiaxkhhkj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtxxeykpjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yongpay.top/gtzquwwsve.html

JS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtdqflpilp.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtmsoffilp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtbtosymtf.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtpjrfhltf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sxryk.cn/gtxizgcamd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtapkrejnh.html

[D15] 去重
来源：http://hz.shanyushiyangtech.top/gttsxdywyz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtyxttwypx.html

PHP:  array_unique($arr);
来源：http://hz.shuidangran.top/gtjfgzfeta.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtwbhporfi.html

TS:   [...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtznpqdywo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.vqdsnc.cn/gtvjxwlbug.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnxiangtu.top/gtbrdomntk.html

Ruby: arr.uniq
来源：http://hz.zhixingplan.top/gtckgskpmu.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtskqxrill.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtvimmkcph.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtiiemjirl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gtsmuywhxc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtrtdbgufc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtdkjhrreq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gttijyjseb.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtqyohowfq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtqlxsmnfv.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhongyouzk.top/gtmwfgljtn.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtjbktqfjk.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gthfsblmre.html

PHP:  max($arr);  min($arr);
来源：http://hz.0kj1m.cn/gthgesvrry.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtesmupfmz.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gttuclhvba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtpssprsxv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yangfankeji.com/gtdstrxpbb.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtcgdvlrqv.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtoxsdopgo.html

[D18] 扁平化嵌套数组
来源：http://hz.yangfankeji.com/gtilveqluf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hysaishi.cn/gtnmdtelmn.html

PHP:  array_merge(...$nested);
来源：http://hz.shuidangran.top/gtffveuvnj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.haohaochexian.top/gtveavumwb.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtazflgpbc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gtotqeieby.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtbtrkompd.html

Ruby: nested.flatten
来源：http://hz.nwbrower.top/gtlqgnfhyr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tianlin.xyz/gtxjlnkkca.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gtigfbnisu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtrjzmamdn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtpremhjrq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtzrohydwc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sysykeji.top/gtlblasqry.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hysaishi.cn/gtxbefrrzx.html

Go:   // 手写 map[string][]T
来源：http://hz.jinyuanbaomall.cn/gtkxdnfhae.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigfzy.top/gtxyvoatsp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gthxcitxmx.html

[D20] 统计每个元素出现次数
来源：http://hz.zhongyouzk.top/gteeckrdyl.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtjuimorqk.html

PHP:  array_count_values($arr);
来源：http://hz.zhaomingkeji.xyz/gtnwpgpyhk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtbflchbiu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtvdpjzahf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hongshengwenyu.top/gtsgtbctgb.html

Go:   // 手写 map[T]int
来源：http://hz.hnxiangtu.top/gtiqvhdklh.html

Ruby: arr.tally
来源：http://hz.tian-w.cn/gtngjixkar.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtkkjvrkvg.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gtgeirnukj.html

Py:   x in arr
来源：http://hz.yonumen.top/gttbxrosvc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtzxvswdqp.html

JS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtcmlppwzx.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtkvkrusfv.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtikxrkolo.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gtmuojfetm.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtembnmzgw.html

C#:   list.Contains(x)
来源：http://hz.cucudq.cn/gtbrakariu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gthnyixtqj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.316326.xyz/gtlszyeytj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.bjfxy.top/gtzympqrau.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.quarkkingdee.top/gtqstkdswl.html

TS:   [...arr];
来源：http://hz.zhaomingkeji.xyz/gtegiyljpm.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtcretslvl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtdbkwbqvi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gtvbaelllw.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtmplkddts.html

[D23] reduce 累积计算
来源：http://hz.yongpay.top/gtdmbmyslk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtzpxkzvda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xingfuxueyuan.xyz/gttelmybxn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gttxezsbme.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtplkwfktb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gthlifmljn.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtcqhiozkp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guannengcc.top/gtbdxkoazx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nwbrower.top/gtkeerlsbi.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gtszdbxyhe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtsqfwaxna.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtrndhnaul.html


<!-- 参考信息 -->