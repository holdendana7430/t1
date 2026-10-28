代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tanke756.top/gtualdhoxj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pycfn.com/gtcuayhtey.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtojejbcfk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhongyouzk.top/gtecyvllhb.html

[C10] 变量作用域
来源：http://hz.shangyingyoupin.top/gtgydftzmo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gthnmrriyp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.andypj.xyz/gtghkbcdlf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.redwolf501.top/gtfxeyykvk.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtcbulmuoq.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtcjndgsjn.html

Go:   花括号块级作用域
来源：http://hz.redwolf501.top/gtdyznoeko.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtkzkslukz.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtmabtewne.html

[C11] 模块导入与导出
来源：http://hz.zhengqikj.top/gteppetgyn.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtjwxfhlns.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yueranfly.top/gtzjtxgsin.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zdqjudy.top/gthdhagqay.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shzxlz.cn/gtrksnppvj.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtvtnpiygy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daxiang520.top/gtrpcdsbzh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gtkkkndvmg.html

C#:   using System.Text;
来源：http://hz.xylfe.cn/gtjempetpt.html

[C12] 立即执行函数 IIFE
来源：http://hz.hysaishi.cn/gtacjbxiyw.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtgbioynxc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhijiandao.cn/gtijkfobpb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtaxfngrey.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtzxtdopbg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guannengcc.top/gtcdcnkljj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ivvv.top/gtvixewibb.html

Ruby: -> { puts "run" }.call
来源：http://hz.mhx1999.top/gtasdlvjlo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhaomingkeji.xyz/gtgfsywwgb.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhoulong.xyz/gtffkbazxm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtwoscrjal.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtgxefjlcr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhoulong.xyz/gtulovkeub.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtuyfuykkz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtnukmhjgz.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtdcjyowwa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtfwdmkdcg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtokegsqqt.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtlmrjovyr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yanxiufei.cn/gtrcahlgxp.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtkuxvpcoe.html

JS:   // 无泛型
来源：http://hz.shzxlz.cn/gtgocfqhwo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtwexmurwv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtzpcftlmb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtbynkgqgm.html

Ruby: # 无泛型
来源：http://hz.iojbl.cn/gtiatlyvho.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtzocestmc.html

[C15] 解构 / 展开参数
来源：http://hz.jiagoushi.top/gtnyddflvu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zdqjudy.top/gtjutojmwi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtjdmaghdi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtrzygmnkl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangkeji.top/gthfwcfmdq.html

Java: // 无解构
来源：http://hz.jyoumei.cn/gtyycvsxvi.html

Go:   // 无解构
来源：http://hz.zhongyouzk.top/gtwkdpnqab.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gthqnwiais.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtuoeyapnx.html

[C16] 函数 / 方法重载
来源：http://hz.haohaochexian.top/gtuckiigfz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtlkiujhff.html

PHP:  // 无重载
来源：http://hz.daria6918.cn/gtwdzaxbed.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigfzy.top/gtzeimjdzy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shuidangran.top/gtgbiftyzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yvedp.cn/gtazagflie.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhijiandao.cn/gtwahitali.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gtglxzkkun.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tian-w.cn/gtzgnkwues.html

================================================================================
来源：http://hz.aizwys.cn/gtyylskfym.html

D. 数组 / 列表 / 集合
来源：http://hz.redwolf501.top/gtqzejmifg.html

================================================================================
来源：http://hz.xinyue.icu/gtpyvpbldu.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtrvrfvmaj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gtuuuknmen.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gtejehofrd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtkljzrgdd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.redwolf501.top/gtwhdpupxq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenjidiqi.icu/gtosokeydr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hywenlv.cn/gtlzkhcvsv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jlsjyb.cn/gtlbynvorl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.smart0.xyz/gtaphkzutr.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtfxedzpwa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtibhovlka.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cdnleiting.top/gtshudahui.html

JS:   arr.push(4);
来源：http://hz.xziqi.cn/gtxviiyler.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gtejnsprgq.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtleyavtky.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtbvrqkqqw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtxpgtksic.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtzgswxtla.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtulmonuaf.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtjvmvfixv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenzaomai.com/gtljuxfgig.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuetiantiany.cn/gtgxiinyfy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cdnleiting.top/gthnivjbsn.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gtnxyhkgrk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhaomingkeji.xyz/gtnjdartzl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenjidiqi.icu/gtjrrskest.html

C#:   list.Insert(0, 0);
来源：http://hz.aizwys.cn/gtwkzxfmvi.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtfccntmky.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.iojbl.cn/gtezvimmve.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gteuybosjf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnxiangtu.top/gteplsjhqz.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtwkvwjsti.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtefhkjabx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fzhhl.top/gtoyndejuv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.andypj.xyz/gtpjcscsgz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gzhubu.top/gtcmyafdvd.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtubohthfb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtwlhcgmub.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gtzdrzcksy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xinyue.icu/gtdalhmyeo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ehwqpu.com/gtlyteskax.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.iojbl.cn/gtoloogimo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shuidangran.top/gtfinepwga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtswvtbzms.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daria6918.cn/gtolfnxmbw.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gttllhpxyr.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtdlbgocsx.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtdigcpulv.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gtliprxbro.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gtjjsmlqjg.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtewmdlupb.html

Go:   len(arr)
来源：http://hz.shangyingyoupin.top/gtqdhiltjd.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gtmastzzoh.html

C#:   list.Count;
来源：http://hz.ehwqpu.com/gtdyfpefdr.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtalpeaapl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.316326.xyz/gtyerqeabb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj202588.top/gtwkfcqsyj.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtlacthhxa.html

TS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gtvsywekpo.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangtech.top/gtiwxfnmvc.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtmswbdevi.html

Ruby: arr[1, 3]
来源：http://hz.yj202588.top/gtqnijwkew.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gtmkcemdhr.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtinbrfvut.html

Py:   a + b;  a.extend(b)
来源：http://hz.ydzc1.top/gtlgodyvhe.html

PHP:  array_merge($a, $b);
来源：http://hz.ydjk.org.cn/gtvxivvpjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtbrnalbkk.html

TS:   [...a, ...b];
来源：http://hz.sufxvd.cn/gtbxaxnxeq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.andypj.xyz/gthviiopxm.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gtboefduqz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gtqkafvvjz.html

C#:   a.Concat(b).ToList()
来源：http://hz.hfpthk.cn/gtvwcckytp.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtuyamszfr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtmdwfrdfo.html

PHP:  sort($arr);
来源：http://hz.hammf.cn/gtcmcykjcj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gtxesezmqe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtccrbvxni.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydjk.org.cn/gtdmrtatoo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gttobfjwgq.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtjpldublf.html

C#:   list.Sort();
来源：http://hz.zycfv.cn/gtoamjffrv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gtqmcwcrwx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtlidsmwsl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pengpengdd.cyou/gtvgddqyjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtkmmkidjo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtwxjqadts.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydzc1.top/gtcxmkkswl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtoyezvsqp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.haohaochexian.top/gtcxdzwray.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gtzycfbsgm.html

[D11] 反转数组
来源：http://hz.birdmap.top/gtfhxbaocf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.havefunace.top/gtlzheytwn.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtzjczxrlw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.svipenyu.cn/gtspesxhll.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtfvibqits.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtokdzsgcf.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtyilumdir.html

Ruby: arr.reverse
来源：http://hz.pycfn.com/gttvwfmdbl.html

C#:   list.Reverse();
来源：http://hz.iojbl.cn/gtithifewn.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtuzhbzkip.html

Py:   arr.index(x);  x in arr
来源：http://hz.tanke756.top/gtwvejsnpv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gttoitepdv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtxrqggwky.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gthwnjygpz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gtrlmybaqx.html

Go:   slices.Index(arr, x)
来源：http://hz.quarkkingdee.top/gtcgyfqped.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtasstomlx.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtlpxnxxos.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtrvxmxdml.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gthnrtlxos.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gtnbmtboni.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtxeigvhuy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtwxxyiugz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtkvmhorck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtsalchfot.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hongshengwenyu.top/gtzqcpgvnk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.vqdsnc.cn/gtammteozb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtnosiidol.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhoulong.xyz/gtcraovywf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nwbrower.top/gtawhrkezw.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtralrxyrm.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtzoycafdt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtmtsvniuv.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtyuppttyo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtekryjecs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yvedp.cn/gtdnzrodvg.html

[D15] 去重
来源：http://hz.xinyue.icu/gtunehbijx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtfarvohio.html

PHP:  array_unique($arr);
来源：http://hz.svipenyu.cn/gtehuwsmmh.html

JS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtkeznmyqn.html

TS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtxdoejgeo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gteqxerufe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zdqjudy.top/gtkdsoglrb.html

Ruby: arr.uniq
来源：http://hz.gotoacloud.top/gtxwqzhmrk.html

C#:   list.Distinct().ToList()
来源：http://hz.quarkkingdee.top/gtwuwghgwy.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtidyslxzn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtrrfirdgt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gthrxgiwfs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtbxgzctjm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtdtoqqkii.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dashuyun.cn/gtenhgvrxz.html

Go:   // 手写循环累加
来源：http://hz.svipenyu.cn/gtwrzpadeo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zdqjudy.top/gtmohtyvcy.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhongyouzk.top/gtebuyblfs.html

[D17] 最大值与最小值
来源：http://hz.xziqi.cn/gtuseifnow.html

Py:   max(arr);  min(arr)
来源：http://hz.ybcxt.top/gtcagdclxg.html

PHP:  max($arr);  min($arr);
来源：http://hz.jqgufenzy.top/gtwgtqaouk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aibaodan.cn/gtpdkcrzlk.html

TS:   Math.max(...arr);
来源：http://hz.svipenyu.cn/gtraxwuckl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtjrkafght.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gttchfuclo.html

Ruby: arr.max;  arr.min
来源：http://hz.hongshengwenyu.top/gtruwxleim.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtpgwhlzqa.html

[D18] 扁平化嵌套数组
来源：http://hz.feifeiyinyue.top/gtgjzhopun.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yanxiufei.cn/gtpnhwvxwp.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtvbxtskew.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tanke756.top/gtrizhaogq.html

TS:   nested.flat();
来源：http://hz.sufxvd.cn/gttldsbsne.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.quarkkingdee.top/gtugamtrki.html

Go:   // 手写双层循环
来源：http://hz.316326.xyz/gtowcmfqqd.html

Ruby: nested.flatten
来源：http://hz.vqdsnc.cn/gttpfsliur.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gtkyhzdeie.html

[D19] 按字段分组
来源：http://hz.ivvv.top/gtiwjunalt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gtgjawzbrs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gtichhmzks.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtzpnsrnfq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gtmgqljzcz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtxutcypey.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxuanxn.top/gtkvgbrkst.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xingfuxueyuan.xyz/gtaqamswcq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenzaomai.com/gtdknkegsh.html

[D20] 统计每个元素出现次数
来源：http://hz.yanxiufei.cn/gtijhqmhog.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtarxfsxaj.html

PHP:  array_count_values($arr);
来源：http://hz.chenzaomai.com/gtckiquyln.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtacahebns.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gttvkiqotx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shangyingyoupin.top/gtqmrceyyq.html

Go:   // 手写 map[T]int
来源：http://hz.tianlin.xyz/gtxnmugwmc.html

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtiujvyocs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxinkj.top/gtrlbnbkvb.html

[D21] 判断是否包含某元素
来源：http://hz.jyoumei.cn/gtvxljbllm.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtqxmrdsjs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gttxnemjmr.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtrybzuymw.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtenhxenpo.html

Java: list.contains(x)
来源：http://hz.fengsongda.top/gtkbcfvgxx.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtatjcndfy.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtdqxqwkas.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gtdnqtsfmi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtwxcpqoct.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pycfn.com/gtmrnuhoyg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fengsongda.top/gttmyxxlzi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj20258888.top/gtwyvmwhfd.html

TS:   [...arr];
来源：http://hz.guannengcc.top/gtfogeorxd.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtqakfxgbc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ybcxt.top/gtfbalypaw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtltqzcgnn.html

C#:   new List<int>(list);
来源：http://hz.meibo888.top/gtbazqtzdx.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtjdpolgbn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fzhhl.top/gtlnrpkdha.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cashguo.top/gtwsbhkljd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtfiofabbc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtdokdkzcd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.quarkkingdee.top/gtsajdpkoi.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtzshrarrz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gtbyigdoip.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258888.top/gthunqqthj.html

[D24] 字典 / Map 基本操作
来源：http://hz.mhx1999.top/gtxgahhgzf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtqwapavne.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zdqjudy.top/gtfkssfazz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gttggkfmcu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtsmuuftqb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtnykeurxq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gotoacloud.top/gtvaalcimd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhixingplan.top/gtnbbpvwca.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gthycedxso.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtrekuaznk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258.top/gttdubpbcd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jiagoushi.top/gtjdlhsled.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtwyewrwld.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtsqnxfnpt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gotoacloud.top/gtnqywmneq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gaohongyu789.top/gtbthfsqat.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ehwqpu.com/gtkktabonk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tian-w.cn/gtgaiuqrpq.html

[D26] 数组转字符串
来源：http://hz.jlsjyb.cn/gtrotgjefy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yonumen.top/gtidtacsmq.html

PHP:  implode(", ", $arr);
来源：http://hz.hammf.cn/gtoczqlzxj.html

JS:   arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtsmhtyhsc.html

TS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtliiayhur.html


<!-- 参考信息 -->