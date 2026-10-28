代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jiagoushi.top/gtnqwejwnx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtrckfyzpn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gttlqysyhn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gtrevrngch.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtbmgsihay.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258.top/gtzibhsxfl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtedkbrxrz.html

[C09] 递归
来源：http://hz.yuxming.cn/gttjqjejrc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gthbvheaec.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtrbjrnrul.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtpljhuotx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtdhlefgcg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dianchejie.cn/gtlwwuyokr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnxiangtu.top/gtagzdykje.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258888.top/gtbmmyzvfy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.tian-w.cn/gtryqrlysc.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtmiylkibe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hnxiangtu.top/gtmpbcnfbk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yangfankeji.com/gtqbozztls.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtaksorayy.html

TS:   同 JS
来源：http://hz.yuanzhike.top/gtszokdmdz.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtgbvffouz.html

Go:   花括号块级作用域
来源：http://hz.gaohongyu789.top/gtchqyjykq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtnmwmzuvw.html

C#:   块级作用域
来源：http://hz.jinyuanbaomall.cn/gtvyiqsmts.html

[C11] 模块导入与导出
来源：http://hz.aibaodan.cn/gtcibkdipn.html

Py:   from module import func
来源：http://hz.c1oappe.top/gtwcitwbrk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jiagoushi.top/gtnfbrtwiq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtbszngixt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtqpbwmxyn.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtnwoloycx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxinkj.top/gtokvabypy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gttkrtvtac.html

C#:   using System.Text;
来源：http://hz.dashuyun.cn/gtirztkhge.html

[C12] 立即执行函数 IIFE
来源：http://hz.aizwys.cn/gtszspajtr.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtlmrfbwxw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aizwys.cn/gtdkcvysqq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhoulong.xyz/gtfywjdlfs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtcedggzfh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.havefunace.top/gtmiuadsqs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.316326.xyz/gtylbgfppf.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gtjuptippz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gtjiskixyq.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxinkj.top/gtjkxqkhdg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cqqwz.cn/gtxexxdgee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtnpqohyaj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtzfyjusao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sysykeji.top/gtfcngxkvv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtknncweln.html

Go:   func add(a, b int) int
来源：http://hz.nanxuanxn.top/gtoohjejzs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtqfvqzebe.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sysykeji.top/gtpfudvksd.html

[C14] 泛型函数
来源：http://hz.ydjk.org.cn/gtpjftoqau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hongshengwenyu.top/gtukwergtg.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtsjgzlbsw.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gtiplxdzqz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtqmevqkiy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtipckvere.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gthicvyfqp.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gtbiwtltww.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.52xcode.cn/gtfmaydvns.html

[C15] 解构 / 展开参数
来源：http://hz.daria6918.cn/gtyqysovfx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtpcsjuakg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gtxrublpiv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gtebrvjsap.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ybcxt.top/gtcbqsyehm.html

Java: // 无解构
来源：http://hz.cheryme.top/gtzfkaqsvh.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gtreggullv.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gttovefxsy.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtxmcnhten.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtjlftlhdu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.iojbl.cn/gtetpcwmlf.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtpahmbwni.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yonumen.top/gtnlwljkeq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgfzy.top/gtigweloxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guowangkeji.top/gtqdzirule.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtwzueeqxa.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cdnleiting.top/gtrjhbpdug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtnwnrreit.html

================================================================================
来源：http://hz.redwolf501.top/gturqufpel.html

D. 数组 / 列表 / 集合
来源：http://hz.smart0.xyz/gtheaubyxv.html

================================================================================
来源：http://hz.ppjwa.cn/gtdjvetrma.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtiraeiyuo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gtzkoiglle.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xylfe.cn/gtykpeudjm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtwhlhhmuj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tianlin.xyz/gtmzqtfuik.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtplbigedh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fengsongda.top/gtmsaopofm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.mhx1999.top/gtkqwpmgsj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.52xcode.cn/gtfyfthfxl.html

[D02] 追加元素到末尾
来源：http://hz.birdmap.top/gtrhtepenu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtrkykmnex.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtmmodwfwt.html

JS:   arr.push(4);
来源：http://hz.hysaishi.cn/gtwejdoqhx.html

TS:   arr.push(4);
来源：http://hz.ivvv.top/gtnnpwzjkn.html

Java: list.add(4);
来源：http://hz.zhaomingkeji.xyz/gtyvuslzom.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gtltbamegu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gttfuosfxy.html

C#:   list.Add(4);
来源：http://hz.feifeiyinyue.top/gtelguhrdy.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigfzy.top/gtoiocppze.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gtlsadxlwk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtrudxrvkk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangshuangyany.cn/gtwesjxpbj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtdqhasndu.html

Java: list.add(0, 0);
来源：http://hz.gogol.net.cn/gtubdnbrcs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jlsjyb.cn/gtjeklgrek.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zycfv.cn/gtnrrxzuqj.html

C#:   list.Insert(0, 0);
来源：http://hz.shuidangran.top/gtbiiauhyy.html

[D04] 删除元素
来源：http://hz.52xcode.cn/gtvyocqdad.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daria6918.cn/gtofbtdfwp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ybcxt.top/gtkfvsnbtq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aizwys.cn/gtwhbcgcse.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtcbvotheh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gttpvgsqih.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtazbwneso.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtvuzkfevi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtgmravnic.html

[D05] 访问与修改元素
来源：http://hz.cqqwz.cn/gtspazvnhg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtiyhifboh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.redwolf501.top/gtrcvkkssf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtadsohadx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gtyisusmhd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shuidangran.top/gtalkooayp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.iojbl.cn/gtdkakhuug.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtafuenkbv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhoulong.xyz/gtalcebtxu.html

[D06] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtsigaxrbx.html

Py:   len(arr)
来源：http://hz.cucudq.cn/gtkqvagfzg.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtionexrhd.html

JS:   arr.length
来源：http://hz.nanxuanxn.top/gtdmtxonar.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtggnleyyo.html

Java: list.size();
来源：http://hz.c1oappe.top/gttvgolrjl.html

Go:   len(arr)
来源：http://hz.chenjidiqi.icu/gtswrxtaik.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gtswnojeds.html

C#:   list.Count;
来源：http://hz.zhongyouzk.top/gtvfyuwihn.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gtbhcffsji.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yangfankeji.com/gtpxkpqqia.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gtpjjbuhqd.html

JS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gtryrzfzer.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtpuuvkwwt.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gtziqytgnj.html

Go:   arr[1:4]
来源：http://hz.gogol.net.cn/gthimgiopl.html

Ruby: arr[1, 3]
来源：http://hz.cheryme.top/gtqxryzggu.html

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtcmkifhal.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtfilopacv.html

Py:   a + b;  a.extend(b)
来源：http://hz.sweek.top/gtntrwmfjf.html

PHP:  array_merge($a, $b);
来源：http://hz.cqqwz.cn/gtlgtjukaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtqmgwvvhh.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gtzpcgkkoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnxiangtu.top/gtuspheinn.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gtcqqirkql.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydjk.org.cn/gtlclszdyu.html

C#:   a.Concat(b).ToList()
来源：http://hz.redwolf501.top/gttsxkruxk.html

[D09] 排序（升序）
来源：http://hz.haohaochexian.top/gtqwmsewyd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtndcrkdsy.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtsjpxkcgm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangkeji.top/gtuflmlfuv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinghuilouyu.cn/gtdhfkwcpj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtgcyvwnwl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yonumen.top/gtxnhxqcbo.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtnxjpkzwa.html

C#:   list.Sort();
来源：http://hz.jqgufenzy.top/gtuqyxokxk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtlkdlyzoz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dashuyun.cn/gtstrbvnxi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtkwurhxak.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gtqgsfvxgu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtopozvkqe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hysaishi.cn/gtmrtmwwqu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtezyxxbxg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangdashe.top/gteneicurs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aibaodan.cn/gtsisuvvxm.html

[D11] 反转数组
来源：http://hz.yj202588.top/gtaxobuqlz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gtdvkjjecy.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtfkhtjlxb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtdpaoxjan.html

TS:   [...arr].reverse();
来源：http://hz.zhoulong.xyz/gtmoieaems.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtgcnyuhed.html

Go:   slices.Reverse(arr)
来源：http://hz.cashguo.top/gtudmfegby.html

Ruby: arr.reverse
来源：http://hz.jqgfzy.top/gtupzzetzy.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtwhoqpckw.html

[D12] 查找元素下标
来源：http://hz.yuanzhike.top/gtjxpmvvny.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtqczujhoa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aizwys.cn/gtyqurlhlz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtykpztjaj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.316326.xyz/gtectmekfv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtggvsuwtf.html

Go:   slices.Index(arr, x)
来源：http://hz.9152youxi.cn/gtzlskymyw.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtoitqshfz.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtzauknycg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sxryk.cn/gtftlvxfca.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtdcdlwexe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtymticbay.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtukftyict.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtpdjhnykt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.c1oappe.top/gtgjuljjvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gthqpilycp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhongyouzk.top/gtincfhedj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.316326.xyz/gtwutknmjj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhoulong.xyz/gtdzvpaxwo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtltbqphrd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtjojnenwn.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtjtjbfeiw.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtagohqbry.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fengsongda.top/gtxbilijkc.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtnetthtxq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tanke756.top/gtqmoouxic.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtunnsdjnv.html

[D15] 去重
来源：http://hz.sxryk.cn/gtprixqish.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtjcgmaaud.html

PHP:  array_unique($arr);
来源：http://hz.yueranfly.top/gtbgbnenwh.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtssjtomnf.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtwyyumsji.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtltzaxauo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shuidangran.top/gtcvtwsuww.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtyndhsion.html

C#:   list.Distinct().ToList()
来源：http://hz.xziqi.cn/gtuvxqzsps.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtisbyzcbg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jlsjyb.cn/gtziaiqahz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhijiandao.cn/gtmftxxbxa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtpuzyihoe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtchlpplgz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtitnnnhiv.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtjvfedbmi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtzfkriesi.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtiprxctmp.html

[D17] 最大值与最小值
来源：http://hz.zhengqikj.top/gtiwefbvmk.html

Py:   max(arr);  min(arr)
来源：http://hz.hammf.cn/gtjpifvfhv.html

PHP:  max($arr);  min($arr);
来源：http://hz.yueranfly.top/gtmncfkwdv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtpgbvauaa.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gteeqjgpyv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtkaqeiyky.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigufen.top/gtexrvrogc.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtsxkpxqbk.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gtocznmxes.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gtqywmftxl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtrwfcxmex.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtpyqawwwu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zdqjudy.top/gtprjsnjbh.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gtazxodtaw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gtqxqeeexc.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangkeji.top/gtdpymymvu.html

Ruby: nested.flatten
来源：http://hz.wangshuangyany.cn/gtqabltxed.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daria6918.cn/gtoejchfir.html

[D19] 按字段分组
来源：http://hz.nanxuanxn.top/gtrruymkxo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ywan-chungtsiang.top/gthmmclhfq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gtekhylmoi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtzbouylpz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gtrbyhgjxq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fengsongda.top/gtcjhxekri.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtobcufhlp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhixingplan.top/gtlxendhir.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ivvv.top/gtiqydelpx.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtfhihlcdc.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtivxwmemv.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtoamwlnfi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shuidangran.top/gtmaftlvnn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtdeclcanf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtctchsbhy.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtiowymfju.html

Ruby: arr.tally
来源：http://hz.nwbrower.top/gtbwaacfrj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtgrxmdxdc.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtroogrtnv.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtfvhsxgxq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtmalhczew.html

JS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtxgirdpth.html

TS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtgwcwvwjb.html

Java: list.contains(x)
来源：http://hz.chenjidiqi.icu/gtgyltlvpn.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gtwhludqrr.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtlpxpaodo.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtfevoqapk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtrillmwrx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtvcjqinfz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtlpcywddv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenzaomai.com/gtvkipytkn.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtmfkycznm.html

Java: new ArrayList<>(list);
来源：http://hz.daria6918.cn/gtwtnmqyza.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenjidiqi.icu/gtnkwwgiax.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhaomingkeji.xyz/gtkceinlde.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtuyafrwau.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtsjmtyyxn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zycfv.cn/gtncjrnpsy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtxknuujaq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtwgoauyji.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gteauzrlta.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtzugqxtbi.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtujjyqyhn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.0kj1m.cn/gtnoifcfvu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gthzonknwl.html

[D24] 字典 / Map 基本操作
来源：http://hz.meibo888.top/gtwgafcekw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtfycrtwrq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtmtzbuojs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shangyingyoupin.top/gtbnxemxhg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.bjfxy.top/gtmmnkpvnl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtjjwqekvj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtipavxxeu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ivvv.top/gtseyjpyst.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hywenlv.cn/gtqtehfciq.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtxmjnijhr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daria6918.cn/gtxbhemrun.html


<!-- 参考信息 -->