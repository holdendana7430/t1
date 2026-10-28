代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gthoxkaxoh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gthjfasxaz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtubttfseo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtwvxtlwjh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtwcrpcgsp.html

Go:   func add(a, b int) int
来源：http://hz.ybcxt.top/gtdlrmqatk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.redwolf501.top/gtybwctjft.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtvkjqwdlo.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtdvnftfdr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ehwqpu.com/gtrvxfymik.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtgvsniiyv.html

JS:   // 无泛型
来源：http://hz.hfpthk.cn/gtpmovhral.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydzc1.top/gtyfygxjhv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nwbrower.top/gtblwpkbqr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhijiandao.cn/gtuslujtzd.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtxyrtwjdg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gtjfigyria.html

[C15] 解构 / 展开参数
来源：http://hz.zycfv.cn/gtkervvoih.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xinyue.icu/gtnvbgpxzp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gtqxbdiuah.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtfufjwypf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenzaomai.com/gtbswssqdm.html

Java: // 无解构
来源：http://hz.jqgufenzy.top/gtyekcasom.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtckpexddp.html

Ruby: a, b = pair
来源：http://hz.daria6918.cn/gtizldvaih.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtdtoupisj.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtmfvjyzst.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.kuanghao11.cn/gtqbnzlevb.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtwjfnzzsb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dianchejie.cn/gtokhdagpx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fengsongda.top/gtnnigwrix.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.meibo888.top/gtunagnpte.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangtech.top/gtmeqoleox.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigfzy.top/gttinquoby.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gtdoiamzvu.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtsaxwxjrk.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtoaapgjzs.html

================================================================================
来源：http://hz.hnqzz.top/gtxxjrjmec.html

[D01] 创建数组 / 列表
来源：http://hz.xinyue.icu/gtclyvcbwu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.aibaodan.cn/gtvfuevhlf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhaomingkeji.xyz/gtmepjacpw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangkeji.top/gtbmazjrrw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtjuwttxku.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shangyingyoupin.top/gtyitowxma.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cashguo.top/gtcdlvqcuu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gtozfefbsk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sxryk.cn/gtpjzugapj.html

[D02] 追加元素到末尾
来源：http://hz.sweek.top/gtqabgibbg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sysykeji.top/gtozbhnnbq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtvnsiqcyo.html

JS:   arr.push(4);
来源：http://hz.xuanzx.com/gtjovqszjv.html

TS:   arr.push(4);
来源：http://hz.aizwys.cn/gtovbqrqmh.html

Java: list.add(4);
来源：http://hz.tianlin.xyz/gtiebrgbnm.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtilgttjvb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtwkgxxwvn.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtltfnissc.html

[D03] 在指定位置插入元素
来源：http://hz.chenjidiqi.icu/gtlxzacxrs.html

Py:   arr.insert(0, 0)
来源：http://hz.yanxiufei.cn/gtwqxojirm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yvedp.cn/gtpyipbecy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ybcxt.top/gtmlynmybd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hammf.cn/gtkaglastj.html

Java: list.add(0, 0);
来源：http://hz.chenjidiqi.icu/gtzprqutet.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.iojbl.cn/gtvsavtbqh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtbjuadcpf.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtdkafyikm.html

[D04] 删除元素
来源：http://hz.yj20258.top/gtbietxdti.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtbrwruusd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hongshengwenyu.top/gtahcnjmyy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ehwqpu.com/gtkavrledg.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gtnszxkfvm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtduutsljl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtqnrkynct.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgfzy.top/gtcgutrive.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.52xcode.cn/gtnpkmbmeq.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gteduocygb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtougqegef.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtplggaadf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ybcxt.top/gtzcrhzqxb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gthaybnozk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.kuanghao11.cn/gtpvxpthes.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yonumen.top/gtoxkzgxxz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtyhospyte.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gttejitiyg.html

[D06] 数组长度
来源：http://hz.nanxuanxn.top/gtsgdrcjhk.html

Py:   len(arr)
来源：http://hz.ydjk.org.cn/gtanydwyzv.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gtdqltzmuq.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtayjsqjdq.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gttwpuuydc.html

Java: list.size();
来源：http://hz.shanyushiyangkeji.top/gteqvbzmtb.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gtbrszxxed.html

Ruby: arr.length; arr.size
来源：http://hz.jyoumei.cn/gtalwakmve.html

C#:   list.Count;
来源：http://hz.sweek.top/gtcwvdmute.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangtech.top/gtmevdwzgl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258.top/gtdolknviw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gthkuiwrcu.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtdlobwyeh.html

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtstkmfdxw.html

Java: list.subList(1, 4);
来源：http://hz.52xcode.cn/gtsmvsfrdw.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gtoeaeypdd.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtqoqecfuy.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtuncrkgcp.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtxeelhler.html

Py:   a + b;  a.extend(b)
来源：http://hz.9152youxi.cn/gtaodkcysr.html

PHP:  array_merge($a, $b);
来源：http://hz.havefunace.top/gtwvholsub.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sufxvd.cn/gtgykymeng.html

TS:   [...a, ...b];
来源：http://hz.daria6918.cn/gthhzubaji.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.wangshuangyany.cn/gthhffunpn.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gtyehjqcdr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jlsjyb.cn/gtvyejcztr.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnqzz.top/gtiwwvnqmx.html

[D09] 排序（升序）
来源：http://hz.hongshengwenyu.top/gtkxorjqeb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtuhwkfyza.html

PHP:  sort($arr);
来源：http://hz.haohaochexian.top/gtctutlvmd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daria6918.cn/gtqrwssdjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtcohrdwgv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gthdmfxycz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtcnkxbpcj.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtttbeuyuj.html

C#:   list.Sort();
来源：http://hz.chenzaomai.com/gteytabspv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangdashe.top/gtxzyrupiv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtxduuqhmh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ybcxt.top/gtiovgtqnk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtgudzvnnf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gthuoftjiz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtlgttvezk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydzc1.top/gttgstcnnf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtirjtyxyq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gtssgpvjuc.html

[D11] 反转数组
来源：http://hz.xylfe.cn/gtajezsqbe.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtjpmhbfvj.html

PHP:  array_reverse($arr);
来源：http://hz.bjfxy.top/gtxpmbhwag.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtftbzdblv.html

TS:   [...arr].reverse();
来源：http://hz.bjfxy.top/gthxzedura.html

Java: Collections.reverse(list);
来源：http://hz.jiagoushi.top/gtkbrqgymg.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtshosflvu.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gthiascshv.html

C#:   list.Reverse();
来源：http://hz.chenlongwang.top/gtnatokwsw.html

[D12] 查找元素下标
来源：http://hz.guannengcc.top/gtmggicgys.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtrjfecapz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgfzy.top/gtiwwbdttb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtvelhwlax.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtckbznwij.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zycfv.cn/gtyydqcfrl.html

Go:   slices.Index(arr, x)
来源：http://hz.tian-w.cn/gtziikkvrt.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtpuigxeza.html

C#:   list.IndexOf(x);
来源：http://hz.jlsjyb.cn/gtmgrvawtm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnqzz.top/gtubkjdbvk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.haohaochexian.top/gtcbohjlup.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuxming.cn/gtlrocgxdw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtiiskfbmu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtzipkertc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gtjoelyrbr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtzoxjtlqc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gtjqblmzrw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yanxiufei.cn/gtfauvwkqb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangtech.top/gtpkmtqslm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jyoumei.cn/gtdtjlhytl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtwkqmoaps.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gttfmgtcov.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtvsxglwus.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guannengcc.top/gtrhuwnnvq.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtpkrlsoyn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.haohaochexian.top/gtnmygswww.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtoztgbcbn.html

[D15] 去重
来源：http://hz.tanke756.top/gtkumbauue.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtoqmgvlip.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtvnfelqtb.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtmrojgzig.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtqcdbfafj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cqqwz.cn/gtghrfeues.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sufxvd.cn/gtohmfwasg.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtjrvqfvov.html

C#:   list.Distinct().ToList()
来源：http://hz.shzxlz.cn/gtortwpndb.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtviayprma.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtahaoxmel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gteuidpqsx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtjufjllkw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtgrbucrxd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtdawyrrlx.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gtxkcayzdg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.mhx1999.top/gttnewvccr.html

C#:   list.Sum();  list.Average()
来源：http://hz.hongshengwenyu.top/gtveykadmy.html

[D17] 最大值与最小值
来源：http://hz.zhijiandao.cn/gttptpnqdy.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtumvczbno.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtrswpbsdt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jianghu66.top/gtypofpgpk.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtzzegwwgb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gttoebaprb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gttbmchzob.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtqvthccol.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtjukygbjs.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtyurqwwlr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gthntqbjuk.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gtrtpdglra.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.quarkkingdee.top/gtbqvtbeqg.html

TS:   nested.flat();
来源：http://hz.cashguo.top/gtuitubwvh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnxiangtu.top/gtwdrwmeyh.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtplblkmny.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtmskwlvlp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtxrsledof.html

[D19] 按字段分组
来源：http://hz.xylfe.cn/gtbjrvwuet.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtaudifhxg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydzc1.top/gtxfmhhzww.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtsrwvoikj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sufxvd.cn/gthxtbyfkf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtenwmyyvv.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtmjgbbavk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtpddjlrbm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtgkbvdwnh.html

[D20] 统计每个元素出现次数
来源：http://hz.zhiwuduotai.top/gtaxwqeioj.html

Py:   Counter(arr)
来源：http://hz.hongshengwenyu.top/gtcufeowcm.html

PHP:  array_count_values($arr);
来源：http://hz.guowangkeji.top/gtwlkcmvyt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtmlfewrvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtgtjjukut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtwkqgxfub.html

Go:   // 手写 map[T]int
来源：http://hz.shuidangran.top/gtjshegfvm.html

Ruby: arr.tally
来源：http://hz.shanyushiyangtech.top/gthbehlasi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtdxxqjiou.html

[D21] 判断是否包含某元素
来源：http://hz.xuetiantiany.cn/gtzesotxbp.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtsvgvszii.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtfhniwmgh.html

JS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtfpklinnh.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtilcazlyg.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtzmexumdn.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gteipewyhx.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtzsudabua.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtudawpgvt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gtvrcyupuk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ehwqpu.com/gtxulgqfux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gtsnufgfxx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtzjikcvfj.html

TS:   [...arr];
来源：http://hz.tanke756.top/gtbzpijezk.html

Java: new ArrayList<>(list);
来源：http://hz.havefunace.top/gtaxxabdfu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pengpengdd.cyou/gtxlcvuoej.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtieosqnnj.html

C#:   new List<int>(list);
来源：http://hz.xingfuxueyuan.xyz/gtyuyaocuu.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtkvlqclsh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zdqjudy.top/gtlheoxacb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.mhx1999.top/gtbvzaphoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gtrtpqtgzm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtgyehfnxc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gotoacloud.top/gthgupojnf.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtoyoowayn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xylfe.cn/gtzzqejsfi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtvewmwwvf.html

[D24] 字典 / Map 基本操作
来源：http://hz.c1oappe.top/gtxumugzea.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangdashe.top/gttnoofmas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtapmsaejf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtiweyzfbo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtygsdpmjo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gtldmhxdxy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gogol.net.cn/gtmamrsypb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.52xcode.cn/gtiphmdnxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtaicyziac.html

[D25] Set 集合去重与交并差
来源：http://hz.hammf.cn/gtisiamqug.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtoejixrig.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gtzzbudttp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtinthnotl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtkwbxpzri.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.birdmap.top/gtkioacecj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guannengcc.top/gtgruvskxd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gteilxmnqi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtbtoqrgpi.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtlzxxvpjq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gthwnetmxb.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtwserelqd.html

JS:   arr.join(", ")
来源：http://hz.hywenlv.cn/gtvgommbwl.html

TS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtcfnhbotq.html

Java: String.join(", ", list)
来源：http://hz.haohaochexian.top/gtrfmkngkf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtfmnrbhmg.html

Ruby: arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtxzvzpzxs.html

C#:   string.Join(", ", list)
来源：http://hz.sweek.top/gtonzhfmuk.html

================================================================================
来源：http://hz.zycfv.cn/gtwcvxqjli.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtjqjrozcj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqbdossbg.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtxcrhabpe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtoznvuubh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenjidiqi.icu/gtlawqvrym.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtdkpqeunh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtvtviibly.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ywan-chungtsiang.top/gtujlbiymh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtzacpsgld.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtyyfpphjb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shuidangran.top/gtxmrmxctw.html

[E02] 重复字符串
来源：http://hz.yuanzhike.top/gtlnqdyxta.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtusrinrub.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigufen.top/gtakycyqeg.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtyxbkealw.html

TS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtgrqnvpyy.html

Java: "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtcqlstrls.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gtaausxdjz.html

Ruby: "ab" * 3
来源：http://hz.fengsongda.top/gtxpakuhzb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pycfn.com/gtbkgcncoq.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gtbhdanphc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnxiangtu.top/gtbinkvech.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.mhx1999.top/gtrfnsipok.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtrumjgxdj.html

TS:   s.slice(1, 4)
来源：http://hz.zhiwuduotai.top/gtucshuwaf.html

Java: s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtnykeljdz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.smart0.xyz/gttosdyjkq.html


<!-- 参考信息 -->