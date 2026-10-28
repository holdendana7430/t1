代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.tianlin.xyz/gtohabxahi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtvthqtgjx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtlewegsle.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.andypj.xyz/gtitekomhq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gtbxaxwlqa.html

Ruby: -> { puts "run" }.call
来源：http://hz.birdmap.top/gtspuymsbx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtgzmweybw.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtollkjnlg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtlgpgvimt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtvyvmefgo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtegeznfce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtqsxqfket.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtdxynefsy.html

Go:   func add(a, b int) int
来源：http://hz.chenzaomai.com/gtjxessmyp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zdqjudy.top/gtzsinzurc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gtanjaeent.html

[C14] 泛型函数
来源：http://hz.316326.xyz/gtngijhhbv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtvcdydcde.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gthcoufvrd.html

JS:   // 无泛型
来源：http://hz.xylfe.cn/gtikxfzata.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtikeddjyi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yvedp.cn/gtoihcblzh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.meibo888.top/gtctolgkwj.html

Ruby: # 无泛型
来源：http://hz.pengpengdd.cyou/gtzlxlmolf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gtqstolpom.html

[C15] 解构 / 展开参数
来源：http://hz.ydzc1.top/gtpyedckvd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aizwys.cn/gtfsjlazdn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guannengcc.top/gtpbwzlmyd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtljbfjvbi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuanzx.com/gtuwbtzugd.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gthasgrbsq.html

Go:   // 无解构
来源：http://hz.yanxiufei.cn/gtyzplasiw.html

Ruby: a, b = pair
来源：http://hz.zhixingplan.top/gtwvxgbwrn.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtgesztxrf.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtozxyjuxm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gterpupqoo.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtplppvxkj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtcftpbjih.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ydjk.org.cn/gtxufyztsa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gtwufdyqml.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtbrprqued.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtqtiwyrom.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fzhhl.top/gtewcstpmu.html

================================================================================
来源：http://hz.ppjwa.cn/gtqlmlztih.html

D. 数组 / 列表 / 集合
来源：http://hz.fengsongda.top/gtyqqzwbts.html

================================================================================
来源：http://hz.hfpthk.cn/gtcqfbdfkn.html

[D01] 创建数组 / 列表
来源：http://hz.sweek.top/gtmtcewonz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.feifeiyinyue.top/gtymlplhmv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtbcpjzssw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.birdmap.top/gthbquaode.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gtlcbgltbr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.mhx1999.top/gtbupvkizo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtrfanecpr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtznxirpfh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtinozcmgp.html

[D02] 追加元素到末尾
来源：http://hz.9152youxi.cn/gtikiefowl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtlkgrntxo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtvnxelgct.html

JS:   arr.push(4);
来源：http://hz.pycfn.com/gteabafvxf.html

TS:   arr.push(4);
来源：http://hz.yuanzhike.top/gtvzkknxfv.html

Java: list.add(4);
来源：http://hz.birdmap.top/gtrcfkkckn.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtxkzpzfsx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigfzy.top/gtilwxowfl.html

C#:   list.Add(4);
来源：http://hz.cqqwz.cn/gtocapscmw.html

[D03] 在指定位置插入元素
来源：http://hz.aibaodan.cn/gtmhzxgfkv.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gthdkfyqkc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gtujeycuzt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guowangkeji.top/gtwldecwks.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ehwqpu.com/gtfgfrmouu.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtiqahpyxx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtpvjkiflr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gtillcmdpd.html

C#:   list.Insert(0, 0);
来源：http://hz.guannengcc.top/gtwysojiay.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtzyjsncuh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cqqwz.cn/gtozkgyznu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gtmyajkvvl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtdvyrzglo.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtowntgfmv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yvedp.cn/gtrbydcrzh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtadnfmjhx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tian-w.cn/gtbzfyykeo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtghecsbed.html

[D05] 访问与修改元素
来源：http://hz.fengsongda.top/gtigijnsdw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtasfbjccr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hywenlv.cn/gtmvudyvav.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtsabpfvoi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtusgcmmfa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ivvv.top/gtsjqrpofo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.c1oappe.top/gtmnaubesn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gttqpdfoce.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tanke756.top/gthlwyepzn.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtqhrfxffa.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtgbskhvbg.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtoibsirdy.html

JS:   arr.length
来源：http://hz.shzxlz.cn/gtktnljkot.html

TS:   arr.length
来源：http://hz.daxiang520.top/gtbcpjsreb.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtvkxojvjh.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gtgkdurgvt.html

Ruby: arr.length; arr.size
来源：http://hz.xuanzx.com/gtlvmqwycf.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtqotraaem.html

[D07] 切片 / 取子数组
来源：http://hz.yonumen.top/gtlwppovqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yongpay.top/gtbvpjzmxb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yanxiufei.cn/gtnriuxbbc.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtmjhunrxp.html

TS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtlsxbjhwp.html

Java: list.subList(1, 4);
来源：http://hz.yanxiufei.cn/gtqngwbzal.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtxuceemck.html

Ruby: arr[1, 3]
来源：http://hz.feifeiyinyue.top/gtjpvnpcqq.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gtfrhlivsx.html

[D08] 合并两个数组
来源：http://hz.redwolf501.top/gtjmdlbala.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtizgqmiod.html

PHP:  array_merge($a, $b);
来源：http://hz.zhixingplan.top/gtgeuqrypa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuanzhike.top/gtshepqnmi.html

TS:   [...a, ...b];
来源：http://hz.tianlin.xyz/gtsutzdyqf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gtgyarbdse.html

Go:   append(a, b...)
来源：http://hz.xziqi.cn/gtgxxzpciw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtdqfwrgsx.html

C#:   a.Concat(b).ToList()
来源：http://hz.redwolf501.top/gttcpsvuie.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtrcejglns.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gttlocstdk.html

PHP:  sort($arr);
来源：http://hz.andypj.xyz/gtykhdzzmi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.svipenyu.cn/gtvayktnbu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.mhx1999.top/gtyqslhndr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtjomarbft.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gthlunpuha.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtuxkjjvcz.html

C#:   list.Sort();
来源：http://hz.kuanghao11.cn/gtagkztgih.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gthbtmwohh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnxiangtu.top/gtjmstonws.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gttuleisfl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtxbadbbeh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtcvxqtddx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gteiehpbmj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtxzjqhhgf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnxiangtu.top/gtosroduay.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sysykeji.top/gtxbrxncqh.html

[D11] 反转数组
来源：http://hz.sxryk.cn/gtwiymbmbl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.birdmap.top/gtyimdvdow.html

PHP:  array_reverse($arr);
来源：http://hz.shzxlz.cn/gtprwkufxk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtwphcjevy.html

TS:   [...arr].reverse();
来源：http://hz.jiagoushi.top/gtvcaybyll.html

Java: Collections.reverse(list);
来源：http://hz.havefunace.top/gtwpjvzbvv.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gttcyjkaqm.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gtarpbiyac.html

C#:   list.Reverse();
来源：http://hz.ywan-chungtsiang.top/gttbafbnfh.html

[D12] 查找元素下标
来源：http://hz.nanxuanxn.top/gtnrrjabnr.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtbclibeub.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.quarkkingdee.top/gtewansuxt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtlkzrqmib.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtlhhbjxmw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtkwzeufmf.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gtflsljxhw.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtuxewcefc.html

C#:   list.IndexOf(x);
来源：http://hz.feifeiyinyue.top/gtrxyxbimn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.redwolf501.top/gtqwsaogtu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fzhhl.top/gtcqxmunok.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuanzx.com/gtnollcjcd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtyhztaqbv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtqgxkclxt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtrsgyapvj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xingfuxueyuan.xyz/gtlzcdekho.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtuwhnepyp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuetiantiany.cn/gtqiilnzxn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hongshengwenyu.top/gtfccfbpqa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtyqlijenp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gtxbkeramh.html

JS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtyouaexey.html

TS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gtdwqdpksc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gtbqgjsroq.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtljygpkhw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sweek.top/gtelsmrezn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gteqzktlxt.html

[D15] 去重
来源：http://hz.xinyue.icu/gtjmmcqrma.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtypikiade.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtplzgrmvh.html

JS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtubwqkpec.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtgdvgzftc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtyyonqmja.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtyocjbacg.html

Ruby: arr.uniq
来源：http://hz.cheryme.top/gtckrqqckw.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gtrnxmmrdk.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtskfajjrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gtkgueqttu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hfpthk.cn/gtwaqixyiv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtweaisumi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtukcoxfnj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtusjwuyml.html

Go:   // 手写循环累加
来源：http://hz.haohaochexian.top/gtyhmcbxpg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.andypj.xyz/gtrcmqsofg.html

C#:   list.Sum();  list.Average()
来源：http://hz.sxryk.cn/gtccjxmnpe.html

[D17] 最大值与最小值
来源：http://hz.cucudq.cn/gtpdyrwkgn.html

Py:   max(arr);  min(arr)
来源：http://hz.jinyuanbaomall.cn/gtmmkbhftw.html

PHP:  max($arr);  min($arr);
来源：http://hz.smart0.xyz/gtxsavtouv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yonumen.top/gtfqkprxaf.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gtzavmtmxc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtofxowjdo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtpbiacsvd.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gthfgqiava.html

C#:   list.Max();  list.Min()
来源：http://hz.zhongyouzk.top/gtjffkdtmx.html

[D18] 扁平化嵌套数组
来源：http://hz.kuanghao11.cn/gtfdwvcrgp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtawghzpfv.html

PHP:  array_merge(...$nested);
来源：http://hz.yueranfly.top/gtqklgvkkv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gtzurpxmeq.html

TS:   nested.flat();
来源：http://hz.zhengqikj.top/gtsgyfbpxx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yueranfly.top/gttgpywugw.html

Go:   // 手写双层循环
来源：http://hz.sufxvd.cn/gtnhonuzsg.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtlynxqnhr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtrbzylpnv.html

[D19] 按字段分组
来源：http://hz.sweek.top/gtfbsusfsl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gtijuoizpj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtjlgvhamk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.0kj1m.cn/gtyhiqzylp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtlsjihcdu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jianghu66.top/gtolcdeobq.html

Go:   // 手写 map[string][]T
来源：http://hz.yanxiufei.cn/gtejbdiohb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fzhhl.top/gtkymgcydu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shzxlz.cn/gtgtwgztyd.html

[D20] 统计每个元素出现次数
来源：http://hz.haohaochexian.top/gtwqmswjpx.html

Py:   Counter(arr)
来源：http://hz.xuetiantiany.cn/gtdipotums.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtcbmenuct.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtepiiqrhe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtogbfpmnp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtkcryzygs.html

Go:   // 手写 map[T]int
来源：http://hz.daria6918.cn/gtgnktawfr.html

Ruby: arr.tally
来源：http://hz.yj20258.top/gtelxjvqsn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shuidangran.top/gtoczwcxpx.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtsbutrxll.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtcmzxoxqw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhengqikj.top/gtobhdcrsu.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtgnmjieql.html

TS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtpfhbrurd.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtulwfscca.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtnaoaknvr.html

Ruby: arr.include?(x)
来源：http://hz.yanxiufei.cn/gtxgekzcub.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtcobuceto.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258888.top/gtufojvgdo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.meibo888.top/gtnlowaitz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zycfv.cn/gtenmwaidd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xinyue.icu/gtgqiezbwa.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtddebgomj.html

Java: new ArrayList<>(list);
来源：http://hz.tanke756.top/gtdamubcje.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtkcxalyjq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xinyue.icu/gtfnkjafxi.html

C#:   new List<int>(list);
来源：http://hz.wangdashe.top/gtghaddxfr.html

[D23] reduce 累积计算
来源：http://hz.pengpengdd.cyou/gtbbfmodua.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtotbwffhe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhongyouzk.top/gtbmeuitqn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtfegwwjyb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtmnnjdlbt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtnghjyeib.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtcsajkbhv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtqbhebvfo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtfscikhps.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhiwuduotai.top/gtwgmmcgms.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xziqi.cn/gtxliwvuvn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtirebbidh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigfzy.top/gtvnzehgrj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxuanxn.top/gtgraczfpz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuetiantiany.cn/gtsqtiwuej.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangkeji.top/gtgkzplovw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtmyxwgprc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.redwolf501.top/gthyqxymic.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gtyptfzbaw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtfgdyokok.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gtsjrezjwa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cucudq.cn/gtbswmlqmw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gthrwnwdfv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pycfn.com/gthmlxoetm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gtaugvamgf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtbxgegtro.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dianchejie.cn/gttclswxqc.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtpjiejpbg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258.top/gtshfjcopd.html

PHP:  implode(", ", $arr);
来源：http://hz.zdqjudy.top/gtpbehmvsl.html

JS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtxhyzehup.html

TS:   arr.join(", ")
来源：http://hz.yj202588.top/gtrxuhadrb.html

Java: String.join(", ", list)
来源：http://hz.yangfankeji.com/gtuzitgswv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtgnjicnrq.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtjmlafsdv.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtoaesuudo.html

================================================================================
来源：http://hz.birdmap.top/gtsoilerly.html

E. 字符串处理
来源：http://hz.guowangkeji.top/gtmwcyimpk.html

================================================================================
来源：http://hz.shuidangran.top/gtrpijjcnt.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtwjmicjve.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gttdbcmzpv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtvnzkkney.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtxidezojo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtmnbkxemi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigufen.top/gtjkdjejpw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigufen.top/gtnmxzpnuc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtnhevytwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jianghu66.top/gtfwlrgirt.html

[E02] 重复字符串
来源：http://hz.vqdsnc.cn/gtjkkhidoa.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtvbmdjexr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtallzxljs.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtyztzhyjx.html

TS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtscblklls.html

Java: "ab".repeat(3)
来源：http://hz.iojbl.cn/gthcyxsqoq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtmnadscbi.html

Ruby: "ab" * 3
来源：http://hz.redwolf501.top/gttclmcini.html


<!-- 参考信息 -->