代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtdxnwzmxf.html

C#:   using System.Text;
来源：http://hz.aizwys.cn/gtyegfjyjq.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtupvjkrpc.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtmyzxvlmp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dashuyun.cn/gtmzxdfoif.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtistcukmq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtxekafgir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hammf.cn/gtqfvgrmnq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtphmesguu.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtbshhygrs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtoiskitso.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuanzx.com/gtgtahvyxn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtfqhnkhaz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gttvgryecn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxinkj.top/gtfkakkknb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtsjsupxtu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtclbcbjgk.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gtuajadccn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yongpay.top/gtliosuvlj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtexgikggz.html

[C14] 泛型函数
来源：http://hz.jinqigufen.top/gtpldjovrp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtufwqrvkl.html

PHP:  // 无泛型
来源：http://hz.feifeiyinyue.top/gtspyhbrqf.html

JS:   // 无泛型
来源：http://hz.chenzaomai.com/gthqtwlmkd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigfzy.top/gtzwhuidwn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtekkgrufm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gtzccparec.html

Ruby: # 无泛型
来源：http://hz.svipenyu.cn/gtxcqxwqjb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tianlin.xyz/gtgwqqjxwl.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtiryveppr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ybcxt.top/gtfwqenpgs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtauzicvtf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtmoupikfd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtsdmejatu.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtpxkabnzj.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtemraaiym.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gtllsyelgn.html

C#:   var (a, b) = pair;
来源：http://hz.xingfuxueyuan.xyz/gtqvgdglrj.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtdvuqinxj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sufxvd.cn/gtjpagbimi.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtbtfluyqo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtuawordtm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtfakvmlme.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.meibo888.top/gtlkrdtyek.html

Go:   // 无重载：用不同函数名
来源：http://hz.yangfankeji.com/gtaznhdjbo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cdnleiting.top/gtvnspcdyg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gttuzsjpzh.html

================================================================================
来源：http://hz.zhengqikj.top/gtsplccjmh.html

D. 数组 / 列表 / 集合
来源：http://hz.gotoacloud.top/gtlxrqzfqx.html

================================================================================
来源：http://hz.aibaodan.cn/gtsneqqvbc.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtguzjnbdx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gtplvlixin.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtxkgdstyi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sufxvd.cn/gtznxgpdbf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nwbrower.top/gtzicfanby.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenjidiqi.icu/gtnpcgydlv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtqrnkyumv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gthlgxzrbg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gtzrxyjtas.html

[D02] 追加元素到末尾
来源：http://hz.andypj.xyz/gtblrzmkev.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cheryme.top/gtadzuemij.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtpahkrvcu.html

JS:   arr.push(4);
来源：http://hz.ydzc1.top/gtpjksfhyu.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtnemhqfou.html

Java: list.add(4);
来源：http://hz.zhijiandao.cn/gtifrbimai.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtefrgvtqj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.iojbl.cn/gtffnpaqfn.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtnlczjvla.html

[D03] 在指定位置插入元素
来源：http://hz.feifeiyinyue.top/gtayhzxdjo.html

Py:   arr.insert(0, 0)
来源：http://hz.yongpay.top/gtmojcksbs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.bjfxy.top/gtotfqonxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gaohongyu789.top/gtqenkggcv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhengqikj.top/gtzjggdsvv.html

Java: list.add(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtcvlsqtiu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtcwhdoczy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenzaomai.com/gtbmeyurbz.html

C#:   list.Insert(0, 0);
来源：http://hz.pengpengdd.cyou/gtasmituyj.html

[D04] 删除元素
来源：http://hz.jinyuanbaomall.cn/gtkiksmxel.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.316326.xyz/gtmjhqhqqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuanzx.com/gtwdcoyqpx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtcspkfoym.html

TS:   arr.splice(0, 1);
来源：http://hz.cqqwz.cn/gtmirquhme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hfpthk.cn/gtyfiihkzy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shuidangran.top/gtqhekhccl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gtfxucusfw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gtmuqzhodc.html

[D05] 访问与修改元素
来源：http://hz.shangyingyoupin.top/gtibpqqvod.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtpedhevpz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtnnexxktp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtrmvzgizo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.bjfxy.top/gtqqjjktjm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtuegmdzwj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtrvhkcjrf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtnazdcsxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtzkxktgej.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtzqoridsr.html

Py:   len(arr)
来源：http://hz.jinqigfzy.top/gtgqcvmubl.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtvjmkdsit.html

JS:   arr.length
来源：http://hz.hfpthk.cn/gttwlzqrps.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtqshxuupe.html

Java: list.size();
来源：http://hz.mhx1999.top/gtsxlkuica.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtuturbnmj.html

Ruby: arr.length; arr.size
来源：http://hz.gaohongyu789.top/gtpcqvwcki.html

C#:   list.Count;
来源：http://hz.yongpay.top/gtgxlwyfst.html

[D07] 切片 / 取子数组
来源：http://hz.ivvv.top/gtbkwlyslz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtujgjadeo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtokqgfsek.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtkfonibot.html

TS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtbuqewtai.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gtsdtnamio.html

Go:   arr[1:4]
来源：http://hz.snrcjt.cn/gtiqicpiur.html

Ruby: arr[1, 3]
来源：http://hz.aizwys.cn/gtezgdsxwk.html

C#:   list.GetRange(1, 3);
来源：http://hz.guowangkeji.top/gthlqgqifl.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtbftmzmth.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gtdfabcnbp.html

PHP:  array_merge($a, $b);
来源：http://hz.xuetiantiany.cn/gtwsrgyemv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtexsvjykh.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtteshmkbw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgufenzy.top/gtizsdxima.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtruzgucgs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gtvcnpuwhg.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangtech.top/gtlshiqhmo.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtsqfptfbh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtcfsttblv.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtytbvsslx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhaomingkeji.xyz/gtfbnzvjqy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtnuaqusac.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtratlxqyn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtlooohzsi.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtpuovymgx.html

C#:   list.Sort();
来源：http://hz.zhoulong.xyz/gtubrbhawe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gaohongyu789.top/gtypieuina.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtlfofztct.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtfegvnbmo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtqvjcayyl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtrfhskpvp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.kuanghao11.cn/gtsbcwwlcn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shangyingyoupin.top/gtxfozhpbm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtzcljmcvh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ppjwa.cn/gtlxajyszt.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gtygshlkol.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.316326.xyz/gtscowqgsp.html

PHP:  array_reverse($arr);
来源：http://hz.yj202588.top/gtujejdldr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shuidangran.top/gtjtcqsjew.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtacrzaaxz.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtewomgauw.html

Go:   slices.Reverse(arr)
来源：http://hz.cdnleiting.top/gtyctagqfb.html

Ruby: arr.reverse
来源：http://hz.yanxiufei.cn/gtojckszku.html

C#:   list.Reverse();
来源：http://hz.wangdashe.top/gtannltowx.html

[D12] 查找元素下标
来源：http://hz.fengsongda.top/gtobnxsdej.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtxtmwyynd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tian-w.cn/gtuqsuxkbw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtthdzgjgz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtfdbnfmma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gzhubu.top/gtzklrfnat.html

Go:   slices.Index(arr, x)
来源：http://hz.cashguo.top/gtnaahpndx.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtbyniaeku.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtifwrpnec.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xylfe.cn/gtmzspooxk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtepyabvya.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gzhubu.top/gtageuabet.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtwmwyivns.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtlezapdgx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtzfigutem.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sxryk.cn/gtmslmdqxr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shzxlz.cn/gtmfphiifg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtwpkjcjxo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtuljulnkf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhaomingkeji.xyz/gtxgejqrbc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sysykeji.top/gtfexkozlr.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtwddftehs.html

TS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtingznezu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigfzy.top/gtybhwyjpn.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtoxefvbso.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.redwolf501.top/gtcleemfpp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jyoumei.cn/gtxmwmtsib.html

[D15] 去重
来源：http://hz.chenlongwang.top/gtbgilcqrk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtkcmuqikr.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtpecrranw.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtlegjtwwv.html

TS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtltdmsfty.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sweek.top/gtrgdjynbq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtrobcunha.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtwxccwpaq.html

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gtyewdbiet.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtifmaikoz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xuanzx.com/gtgqieatqo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtjdefbfib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gticefrzoz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtljbpljdj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gtycqweztf.html

Go:   // 手写循环累加
来源：http://hz.mhx1999.top/gtctjfijvx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtahbtwefl.html

C#:   list.Sum();  list.Average()
来源：http://hz.nwbrower.top/gtdzlslnpk.html

[D17] 最大值与最小值
来源：http://hz.guowangkeji.top/gtdtfuvbjf.html

Py:   max(arr);  min(arr)
来源：http://hz.svipenyu.cn/gtuyiwynvw.html

PHP:  max($arr);  min($arr);
来源：http://hz.yongpay.top/gtpeeyncdp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtmzdvhndu.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtzmfiohqc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtilhicwmh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtweyybnic.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtbqlznqdg.html

C#:   list.Max();  list.Min()
来源：http://hz.iojbl.cn/gtxyonffdj.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtdclmdyzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.meibo888.top/gtxqhzdthr.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtcmqobiql.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gthxptmorb.html

TS:   nested.flat();
来源：http://hz.nanxinkj.top/gtvrsxjiuy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtrwibcvad.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtgvgtvnnk.html

Ruby: nested.flatten
来源：http://hz.hnxiangtu.top/gtcnydapyp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtgqyygmos.html

[D19] 按字段分组
来源：http://hz.tanke756.top/gtvirvsuqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ywan-chungtsiang.top/gtoagmxssy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtrolroehn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gtaaetxpgw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtdzidbueu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cashguo.top/gtafssmjtq.html

Go:   // 手写 map[string][]T
来源：http://hz.zhengqikj.top/gtojxadkwj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtnfwewdwk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgufenzy.top/gteercohtc.html

[D20] 统计每个元素出现次数
来源：http://hz.jianghu66.top/gtzgzrdcey.html

Py:   Counter(arr)
来源：http://hz.hammf.cn/gtufayrzse.html

PHP:  array_count_values($arr);
来源：http://hz.zhengqikj.top/gttcdbjrrd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtysihxbmc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gttubwggej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xylfe.cn/gtwoijlttu.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtxbnsllzj.html

Ruby: arr.tally
来源：http://hz.tianlin.xyz/gtpsaddzhr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gtcuvflrtr.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtulgyhohf.html

Py:   x in arr
来源：http://hz.jianghu66.top/gtzpgfrmek.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258888.top/gtcyevbdmo.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtfmoaamgg.html

TS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtaavlgakt.html

Java: list.contains(x)
来源：http://hz.jyoumei.cn/gtyxzdpaoq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yonumen.top/gtizkvmjfi.html

Ruby: arr.include?(x)
来源：http://hz.jiagoushi.top/gteihixuhh.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtfwnoatpq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtbxizyjjc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shangyingyoupin.top/gtpacrhybb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zdqjudy.top/gttothaakj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cashguo.top/gtquannrjk.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtvgzujivo.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gttipyizen.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sysykeji.top/gthbzuwdyg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gtaekvqqhw.html

C#:   new List<int>(list);
来源：http://hz.chenjidiqi.icu/gtkuuscidi.html

[D23] reduce 累积计算
来源：http://hz.sufxvd.cn/gtnrfqfzyc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cucudq.cn/gtiuzeuyum.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gaohongyu789.top/gtkswlxlsh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtpyhykgql.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtpxndajxk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtneaizvec.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtuwuemkvo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.52xcode.cn/gtvvkqpxkg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sxryk.cn/gtoidkwfue.html

[D24] 字典 / Map 基本操作
来源：http://hz.snrcjt.cn/gtmpwtfyvi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydjk.org.cn/gtsjlbornh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gtebwugtap.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gtigywflig.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtzorotyau.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gtahqvjxdg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.svipenyu.cn/gtstvtonmt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cucudq.cn/gtnmdlzqov.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinyuanbaomall.cn/gttozhpvec.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtqvoyivzq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zycfv.cn/gteflesphe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cheryme.top/gtxxuxgcax.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtvodqgibf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gtzdolxcmp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hongshengwenyu.top/gtgkgxktcg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.mhx1999.top/gtxhlnuezt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydzc1.top/gtpjrmgeeq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtgzbzbeov.html

[D26] 数组转字符串
来源：http://hz.yangfankeji.com/gtqujebosd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gtxadzlono.html

PHP:  implode(", ", $arr);
来源：http://hz.hongshengwenyu.top/gtqergzsiv.html

JS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtwzkfvgbf.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtgenklmdi.html

Java: String.join(", ", list)
来源：http://hz.wangshuangyany.cn/gtxypusjfa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtsmlvdipk.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtgbvjeugv.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtrlqerbhv.html

================================================================================
来源：http://hz.hfpthk.cn/gtdscmfwjx.html

E. 字符串处理
来源：http://hz.jlsjyb.cn/gtqbpfsbkg.html

================================================================================
来源：http://hz.andypj.xyz/gtkuihasoa.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gtgndndirz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sweek.top/gtsojsjbox.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtcuictzir.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtkgoohyqk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtznojwjbs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhengqikj.top/gtudbjqkdi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cashguo.top/gtrkocxylx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gogol.net.cn/gtluraaurr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cdnleiting.top/gtnjqiieen.html

[E02] 重复字符串
来源：http://hz.wangshuangyany.cn/gtgxqnnczb.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtrgnrirqq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtrxvbgsep.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtcbprvzko.html


<!-- 参考信息 -->