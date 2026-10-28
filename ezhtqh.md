代发 wailian999

[C10] 变量作用域
来源：http://hz.hammf.cn/gtqycnezkz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.52xcode.cn/gtbvielyrk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigufen.top/gtgzeudrgc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yonumen.top/gtrwvcwick.html

TS:   同 JS
来源：http://hz.0kj1m.cn/gtykzymonu.html

Java: 方法内为块级作用域
来源：http://hz.ybcxt.top/gtvgmtmhea.html

Go:   花括号块级作用域
来源：http://hz.nanxuanxn.top/gteveiahfk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xylfe.cn/gtaxtvmesg.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gtebmqywau.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtxibuyrth.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtnfnspmtr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtkoxeotah.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sxryk.cn/gtgvpupfnp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtwburaxit.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gtvpaymxcx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tanke756.top/gtdubotvrq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangtech.top/gtwkwfqnga.html

C#:   using System.Text;
来源：http://hz.wangshuangyany.cn/gtdknlghrh.html

[C12] 立即执行函数 IIFE
来源：http://hz.meibo888.top/gtdrsypiff.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxinkj.top/gthrjiasbn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtwudejaoo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtwygfquyc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtjhdytyok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gthwtineox.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jlsjyb.cn/gtintbwwab.html

Ruby: -> { puts "run" }.call
来源：http://hz.0kj1m.cn/gtwkcycnum.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fzhhl.top/gtcpgetexr.html

[C13] 类型声明 / 类型注解
来源：http://hz.gotoacloud.top/gtuqnemcyn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.andypj.xyz/gtungzbreb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtuftjsskk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtnuggygfx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtuxwkzlgi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtlymdicyf.html

Go:   func add(a, b int) int
来源：http://hz.shangyingyoupin.top/gtayevphix.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ybcxt.top/gtrgocwiga.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daria6918.cn/gtirnkqvxp.html

[C14] 泛型函数
来源：http://hz.jinqigufen.top/gtjopzkxjx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gotoacloud.top/gtsvkegsrt.html

PHP:  // 无泛型
来源：http://hz.zdqjudy.top/gttgvretbj.html

JS:   // 无泛型
来源：http://hz.smart0.xyz/gtdsugupop.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtlddfyfif.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.andypj.xyz/gtjxkuphkc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guannengcc.top/gtjpnrcgmg.html

Ruby: # 无泛型
来源：http://hz.gaohongyu789.top/gthowkafrk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtovwtrven.html

[C15] 解构 / 展开参数
来源：http://hz.zhoulong.xyz/gtntjovubj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gttwpplgxz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtqllppfde.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.birdmap.top/gtupmpekex.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hfpthk.cn/gtnswglmkp.html

Java: // 无解构
来源：http://hz.yuanzhike.top/gtrboswlhj.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtcusgsgwo.html

Ruby: a, b = pair
来源：http://hz.gotoacloud.top/gtpymckfwi.html

C#:   var (a, b) = pair;
来源：http://hz.jqgfzy.top/gtawecwgut.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtllnplhwg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sweek.top/gtutufxxih.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtabkwtfvn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daxiang520.top/gtansocqlp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtpsdvdbgi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.bjfxy.top/gtxggbntym.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtrnaznomv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jlsjyb.cn/gtclezsxhl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sxryk.cn/gtxbtjykic.html

================================================================================
来源：http://hz.daxiang520.top/gtuwwbeetj.html

D. 数组 / 列表 / 集合
来源：http://hz.fzhhl.top/gtqzdrcjbn.html

================================================================================
来源：http://hz.tian-w.cn/gtyiwzufto.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gthnboieis.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fengsongda.top/gtncrtungl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuanzx.com/gtvoalphvo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtqvgubher.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.316326.xyz/gticdzvckg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtaypaqkfn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gtoacrndzs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtlbewgzwc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtspkikbim.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtfrvfzwpz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtpxpypfcq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenjidiqi.icu/gtudfdlzms.html

JS:   arr.push(4);
来源：http://hz.cucudq.cn/gtzhlrqequ.html

TS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtnofkqifi.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtrnkcoyiq.html

Go:   arr = append(arr, 4)
来源：http://hz.zhengqikj.top/gterwmossc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nwbrower.top/gtkrjgeqrs.html

C#:   list.Add(4);
来源：http://hz.52xcode.cn/gtjtropevo.html

[D03] 在指定位置插入元素
来源：http://hz.yuxming.cn/gtenprrcmk.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtpbbpttlw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ybcxt.top/gtnuknemvi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.52xcode.cn/gtkwogasnw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dashuyun.cn/gtxkmxrdsd.html

Java: list.add(0, 0);
来源：http://hz.vqdsnc.cn/gtutqmgojr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xziqi.cn/gtbdcpfynh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.svipenyu.cn/gtmlzsffej.html

C#:   list.Insert(0, 0);
来源：http://hz.tianlin.xyz/gtkuimafbi.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtsvervlku.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pengpengdd.cyou/gtdswtczfx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtarnbvfhh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yueranfly.top/gtjdcxqpyp.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtcltnefep.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gtdzptimoj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtssmonklg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhiwuduotai.top/gttolfrhyp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhoulong.xyz/gtqkcmvbxl.html

[D05] 访问与修改元素
来源：http://hz.birdmap.top/gtqdmjjsyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtveaktaww.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fengsongda.top/gtmeateyks.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zycfv.cn/gtrzkyzvnf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtswbyznxm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gtwielojyi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtmizlqbhy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtibrngjyt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gttwwkbhow.html

[D06] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtjlhsflbj.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtapltghid.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtcdrffbwr.html

JS:   arr.length
来源：http://hz.kuanghao11.cn/gtaharrnim.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtcekggoen.html

Java: list.size();
来源：http://hz.yueranfly.top/gtyrzsnpoo.html

Go:   len(arr)
来源：http://hz.xinyue.icu/gtsrpvaydu.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gtywmpvibz.html

C#:   list.Count;
来源：http://hz.jinqigfzy.top/gtttgkxbdt.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtefftdrpo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jyoumei.cn/gtfiqaceuh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtvdykwhfe.html

JS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtcutevtjt.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtfjmxwhms.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtqgndpjoo.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtohmujpgf.html

Ruby: arr[1, 3]
来源：http://hz.zdqjudy.top/gtbyrcjgjj.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtcqepjcds.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtiixpgwma.html

Py:   a + b;  a.extend(b)
来源：http://hz.yanxiufei.cn/gtfugvjhew.html

PHP:  array_merge($a, $b);
来源：http://hz.zhijiandao.cn/gtgrjxomcs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aibaodan.cn/gtaoqkpkqe.html

TS:   [...a, ...b];
来源：http://hz.shzxlz.cn/gteruhhmkz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cqqwz.cn/gtqlzsfhhf.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtjybrrfcg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aizwys.cn/gtwcfmasqs.html

C#:   a.Concat(b).ToList()
来源：http://hz.zdqjudy.top/gtdiefbrtz.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtxqyglwhk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtctocfnim.html

PHP:  sort($arr);
来源：http://hz.havefunace.top/gtcdazwoih.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtfgbusiwq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shangyingyoupin.top/gtgxpvatnt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtxqzdqkpg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangshuangyany.cn/gtdxwoxuuq.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtegaphhxp.html

C#:   list.Sort();
来源：http://hz.yvedp.cn/gtlahsbsce.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gthngvnlwb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cashguo.top/gtdlrjvbrw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtzfoibigw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtakdgdwke.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtccjvpbjj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nwbrower.top/gtwuvknjiv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guannengcc.top/gtvpsmmchh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zycfv.cn/gtnqslkwnh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.0kj1m.cn/gtdreizqbf.html

[D11] 反转数组
来源：http://hz.cheryme.top/gtpcotzaoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gtkrkmmvhf.html

PHP:  array_reverse($arr);
来源：http://hz.sysykeji.top/gtgwcnohfa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtaxofjtlx.html

TS:   [...arr].reverse();
来源：http://hz.jqgfzy.top/gtdfbumxyl.html

Java: Collections.reverse(list);
来源：http://hz.yj20258.top/gtfchzchre.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gtqzvxjhhd.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gtrraeleqd.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtxncxlcpb.html

[D12] 查找元素下标
来源：http://hz.smart0.xyz/gtwpsjlujq.html

Py:   arr.index(x);  x in arr
来源：http://hz.yangfankeji.com/gtiqqaesty.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jiagoushi.top/gtizfrgcje.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtshzdidun.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtdlgagtht.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tian-w.cn/gtynfiqmqs.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtvubmxwww.html

Ruby: arr.index(x)
来源：http://hz.jyoumei.cn/gttchxkhzm.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258.top/gtvntxaicy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gtsicvneri.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gtqyomrmoi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtufukfxfa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtwefnzdkx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtsymlocsv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yanxiufei.cn/gtmgbrgfsq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hfpthk.cn/gtjbpoajvz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtjvdjqvyt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtjavepyvm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtwtiiyneu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gtwjjhjaxt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtdfhwnvaz.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtffbyyukt.html

TS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtsambwvmu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.meibo888.top/gtckainwtb.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtkavmvjwu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhoulong.xyz/gtydxjnxbs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigfzy.top/gtgsuqoaie.html

[D15] 去重
来源：http://hz.andypj.xyz/gtwgpwjvtw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtmieldfda.html

PHP:  array_unique($arr);
来源：http://hz.sweek.top/gtdrfcgfwx.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtdoyurvar.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtcnpywpev.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shuidangran.top/gthntqrvjw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtojolkthc.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gtlehecwss.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtxlkfwkit.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gttjnyblod.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.haohaochexian.top/gtkwlhndrj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gthhttjmml.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtyfmutwop.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtlhpquitz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtmvaqkayk.html

Go:   // 手写循环累加
来源：http://hz.fengsongda.top/gtiuxwdhjp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cucudq.cn/gtwwnjcpbt.html

C#:   list.Sum();  list.Average()
来源：http://hz.hysaishi.cn/gtazvhzphd.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gthjndkthf.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gttdgvelmh.html

PHP:  max($arr);  min($arr);
来源：http://hz.zdqjudy.top/gtaknrnpyt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtwjhucpbm.html

TS:   Math.max(...arr);
来源：http://hz.tian-w.cn/gtpfrxmwpz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtchwkvlcg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gtisovbmjh.html

Ruby: arr.max;  arr.min
来源：http://hz.zhongyouzk.top/gtbkebsmvk.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gtmjwprkyg.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtoxxjgbid.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtrolepbat.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gtuefecazk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtjauzszis.html

TS:   nested.flat();
来源：http://hz.redwolf501.top/gtihfctriu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258.top/gtmxujgxfo.html

Go:   // 手写双层循环
来源：http://hz.gaohongyu789.top/gtqqftzwmp.html

Ruby: nested.flatten
来源：http://hz.hywenlv.cn/gtnemchhwr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fengsongda.top/gtfqgkxxtc.html

[D19] 按字段分组
来源：http://hz.guannengcc.top/gtiwunlsfz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dashuyun.cn/gtezxzidwt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhongyouzk.top/gtdlzmdhmd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhiwuduotai.top/gtcydlmvsi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtsggdrtqe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hywenlv.cn/gtvffyhhxn.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtqqrcalds.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xylfe.cn/gtqbodlban.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtxcljigbc.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtfsxbljdu.html

Py:   Counter(arr)
来源：http://hz.zhixingplan.top/gticexlgpw.html

PHP:  array_count_values($arr);
来源：http://hz.wangdashe.top/gttggpqmvb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gtlrphjfuo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtaotmnwna.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gtrdwahsjm.html

Go:   // 手写 map[T]int
来源：http://hz.9152youxi.cn/gtdtgrwsyw.html

Ruby: arr.tally
来源：http://hz.jinqigufen.top/gtniyxpihs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.52xcode.cn/gtjgyknuqx.html

[D21] 判断是否包含某元素
来源：http://hz.c1oappe.top/gtsbidwgnp.html

Py:   x in arr
来源：http://hz.aibaodan.cn/gthktowsyd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtaukodwep.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtreauypch.html

TS:   arr.includes(x)
来源：http://hz.andypj.xyz/gthavkyhzc.html

Java: list.contains(x)
来源：http://hz.hysaishi.cn/gtcyotxeka.html

Go:   slices.Contains(arr, x)
来源：http://hz.dashuyun.cn/gtofnqgrkt.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gtaknozxpj.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtoechimna.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtfxtaxiga.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenzaomai.com/gtmpnifdoa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtjbabpzba.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sxryk.cn/gtkhhrioyi.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtcvjyawnd.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtuczqfgdl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtiitihhpd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sysykeji.top/gtbfzugbfj.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtncotxoor.html

[D23] reduce 累积计算
来源：http://hz.316326.xyz/gtdussxpbw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gttitckcif.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtgzlkpedt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtaefmvgqy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtikrvbcys.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtljymrnqo.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtluoxchln.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinyuanbaomall.cn/gtlxlgvlld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtpmiwsvlv.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuanzx.com/gtehxxyexu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.snrcjt.cn/gtvufpzzpg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gotoacloud.top/gtsgageyeb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtdsaqzdag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tanke756.top/gtqnstuhxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtbaittmpi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jlsjyb.cn/gtanyplmjp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtchwyimnu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtcsyrriqn.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtiwpspsbr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhongyouzk.top/gtbyxwsmhl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sufxvd.cn/gtnrjdtxtv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sxryk.cn/gtgpcrlypj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtfimthaaa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xinyue.icu/gtbufoxpwp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtdiyhvkot.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtxiglsgwp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtnoenpflh.html

[D26] 数组转字符串
来源：http://hz.shzxlz.cn/gtznauguqo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtnqbocoae.html

PHP:  implode(", ", $arr);
来源：http://hz.havefunace.top/gtotlyhheh.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtbljgjpkb.html

TS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtbmkasaqw.html

Java: String.join(", ", list)
来源：http://hz.dianchejie.cn/gtmjknysmi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtoepcghfn.html

Ruby: arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtwhyzcoku.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtqpqpycwk.html


<!-- 参考信息 -->