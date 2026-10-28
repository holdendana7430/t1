代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtraopkncj.html

Go:   func add(a, b int) int
来源：http://hz.jqgufenzy.top/gtgqpqqmob.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.redwolf501.top/gtbfjejxii.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xziqi.cn/gtlxoyixkb.html

[C14] 泛型函数
来源：http://hz.shanyushiyangkeji.top/gtwxshbpel.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhixingplan.top/gtktzhsiel.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtifrxyyxz.html

JS:   // 无泛型
来源：http://hz.yueranfly.top/gtzluorfvi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenlongwang.top/gtayfwfgyf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtxfmzptkq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gteawbsikw.html

Ruby: # 无泛型
来源：http://hz.zhengqikj.top/gtxglezqfd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuetiantiany.cn/gthmfbxxog.html

[C15] 解构 / 展开参数
来源：http://hz.kuanghao11.cn/gtsmfxdukn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sysykeji.top/gtibxenecr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtqwmznfjp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtstjiufyp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuanzhike.top/gtymljuedm.html

Java: // 无解构
来源：http://hz.jyoumei.cn/gtiucqnntm.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtvuunltrq.html

Ruby: a, b = pair
来源：http://hz.hfpthk.cn/gtohmmiytj.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtitqtebrc.html

[C16] 函数 / 方法重载
来源：http://hz.dianchejie.cn/gtuaxdvwek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtsdaswuau.html

PHP:  // 无重载
来源：http://hz.yj20258.top/gtcuyfpbxu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuanzhike.top/gtueqjufgk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aizwys.cn/gtsdrzavtw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.kuanghao11.cn/gtiiwzducw.html

Go:   // 无重载：用不同函数名
来源：http://hz.daria6918.cn/gtxaxpqsak.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtumbehbcp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangdashe.top/gtselsazfh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtecwswigr.html

D. 数组 / 列表 / 集合
来源：http://hz.tanke756.top/gtvrglsuha.html

================================================================================
来源：http://hz.9152youxi.cn/gtndgwoiyi.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtxigejqkq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydjk.org.cn/gtwebfaoby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.9152youxi.cn/gtjtbbndto.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sysykeji.top/gtovmyevya.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtrcjdvhtd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtsrtbpiqn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tanke756.top/gtvrkyzlfg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jiagoushi.top/gtehbvmoyi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtwemaespi.html

[D02] 追加元素到末尾
来源：http://hz.smart0.xyz/gtlovjyxid.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtwimapvdp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtakywcqug.html

JS:   arr.push(4);
来源：http://hz.daxiang520.top/gtwrenhyji.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtqkstpdcy.html

Java: list.add(4);
来源：http://hz.gotoacloud.top/gtjuglxfjv.html

Go:   arr = append(arr, 4)
来源：http://hz.ivvv.top/gtmgmjgxhs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtqgvgwmen.html

C#:   list.Add(4);
来源：http://hz.316326.xyz/gthplcsels.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtrvzyyfyq.html

Py:   arr.insert(0, 0)
来源：http://hz.hfpthk.cn/gtasocioqk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cdnleiting.top/gtylfudiww.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtesejazmq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gtkotxjhye.html

Java: list.add(0, 0);
来源：http://hz.gogol.net.cn/gtcfwrsyqq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cqqwz.cn/gtkjsbytvw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258888.top/gtjnpkoczv.html

C#:   list.Insert(0, 0);
来源：http://hz.sysykeji.top/gtmspaglox.html

[D04] 删除元素
来源：http://hz.redwolf501.top/gtetneiqlh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtfbjzzfcu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hongshengwenyu.top/gtajzqpeif.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhixingplan.top/gtsauetnti.html

TS:   arr.splice(0, 1);
来源：http://hz.vqdsnc.cn/gtfxujxstd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yanxiufei.cn/gtminriebm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.meibo888.top/gtiejfludp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tian-w.cn/gtpgsygzbb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.havefunace.top/gtispfvkmq.html

[D05] 访问与修改元素
来源：http://hz.cqqwz.cn/gtnfordzvv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtctcopfxl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtwiiznjrq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cqqwz.cn/gtowikyoit.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtedrxyfdi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cucudq.cn/gtmczyclui.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtyuhdzvup.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtzuqchdno.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtpxvfapxi.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtvmqubnev.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtfucovasd.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtxbrijnzo.html

JS:   arr.length
来源：http://hz.gotoacloud.top/gtnutsjxrh.html

TS:   arr.length
来源：http://hz.ybcxt.top/gtcwskwuma.html

Java: list.size();
来源：http://hz.shanyushiyangkeji.top/gtczlqqrcr.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gtigijcwsq.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtpomkluni.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtyvsmrzmi.html

[D07] 切片 / 取子数组
来源：http://hz.zhaomingkeji.xyz/gtgwicdzeq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ybcxt.top/gtdiqtdciu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daxiang520.top/gtrdrghaqk.html

JS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtalnnmyxm.html

TS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gtbyjdrcdx.html

Java: list.subList(1, 4);
来源：http://hz.xinyue.icu/gtrduxzkhg.html

Go:   arr[1:4]
来源：http://hz.jinqigfzy.top/gtkzuebjdn.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtaconjxoc.html

C#:   list.GetRange(1, 3);
来源：http://hz.52xcode.cn/gtkwjymthd.html

[D08] 合并两个数组
来源：http://hz.yangfankeji.com/gtvqgngzrc.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtfifgrryt.html

PHP:  array_merge($a, $b);
来源：http://hz.c1oappe.top/gtbidmgomq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxinkj.top/gtrwmmsplb.html

TS:   [...a, ...b];
来源：http://hz.ivvv.top/gtmcsddgsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtrijhtmiq.html

Go:   append(a, b...)
来源：http://hz.jinqigfzy.top/gtrcjpviob.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtrtkurvvt.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtbkdbucuq.html

[D09] 排序（升序）
来源：http://hz.vqdsnc.cn/gtmzyfnbeg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtzfhgcbuy.html

PHP:  sort($arr);
来源：http://hz.hywenlv.cn/gtwsybtocl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.c1oappe.top/gteepqxait.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtubjsslcm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gotoacloud.top/gtblquxsvx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cqqwz.cn/gthpxxmrcz.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtilpipcok.html

C#:   list.Sort();
来源：http://hz.shuidangran.top/gtyitnmxsi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuetiantiany.cn/gtcohhuqdc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtorbwhwdg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhijiandao.cn/gtbblamtah.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtuvbkoipx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtiajdenup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuanzhike.top/gtuwgyfvqs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.svipenyu.cn/gtpmziibhn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.52xcode.cn/gtdvamjtwj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangtech.top/gtmyvmbiba.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtdysnhnzf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.0kj1m.cn/gtetyrfxee.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gtrdyuhvkq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gtvpjpkyfu.html

TS:   [...arr].reverse();
来源：http://hz.zhoulong.xyz/gtbhhusrds.html

Java: Collections.reverse(list);
来源：http://hz.chenjidiqi.icu/gtsjxxubhz.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gtxptajkog.html

Ruby: arr.reverse
来源：http://hz.yuanzhike.top/gtuwglyxjr.html

C#:   list.Reverse();
来源：http://hz.yj202588.top/gtonyvfosn.html

[D12] 查找元素下标
来源：http://hz.zhaomingkeji.xyz/gtklisyrpc.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtxlytkfqg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aibaodan.cn/gtxisolnrz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtviwwbhbi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtuwrzvqaz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ywan-chungtsiang.top/gtezjmcgtc.html

Go:   slices.Index(arr, x)
来源：http://hz.dashuyun.cn/gtlqxaveup.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gtrgtkmurh.html

C#:   list.IndexOf(x);
来源：http://hz.wangshuangyany.cn/gtyhuzrtuo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.haohaochexian.top/gtoyiurwml.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenjidiqi.icu/gtzxvietfd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhoulong.xyz/gtysxudsoj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtewqpnvwa.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gttjrwcvrf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtefavgoxk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gtjahobczi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gtqgxsmxtx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtwtcmamgd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuanzhike.top/gtfuegjzbv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtjwaczkjn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydzc1.top/gtzijylbrn.html

JS:   arr.map(x => x * 2)
来源：http://hz.cqqwz.cn/gtvzutqnnb.html

TS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtpashumtv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj202588.top/gttaxbqihq.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtgaqacmoy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtknhcoavb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jlsjyb.cn/gtofewrohd.html

[D15] 去重
来源：http://hz.yj20258888.top/gtzqexlswv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtyrozxdji.html

PHP:  array_unique($arr);
来源：http://hz.shangyingyoupin.top/gtqowpwhbm.html

JS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtrjsmiwhv.html

TS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gttzwrmvnf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxinkj.top/gtjgsmyxiy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gttbdnwlye.html

Ruby: arr.uniq
来源：http://hz.daria6918.cn/gtamkejpzu.html

C#:   list.Distinct().ToList()
来源：http://hz.xziqi.cn/gtjiuyzjiu.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtagytupob.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gthnouvnfy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtyjvzifoi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangtech.top/gtcnbxlbjx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtrkqfkvgq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shuidangran.top/gteniymeli.html

Go:   // 手写循环累加
来源：http://hz.zhoulong.xyz/gtwusqzsop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtvtfgxncu.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnxiangtu.top/gtjyoijvtt.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtctfgjsjz.html

Py:   max(arr);  min(arr)
来源：http://hz.birdmap.top/gtveveqgrc.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtoorsmpkn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nwbrower.top/gtfushzzyc.html

TS:   Math.max(...arr);
来源：http://hz.zdqjudy.top/gtagdvrcuj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtkggtgflt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gtwahxtadt.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangkeji.top/gtxqkjnoor.html

C#:   list.Max();  list.Min()
来源：http://hz.iojbl.cn/gtishvcdax.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtmjkzjxum.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtngulwcwe.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtomiaigwx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ywan-chungtsiang.top/gthobblvxt.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtjufiopal.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gtelqrsmdu.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtepxvvqos.html

Ruby: nested.flatten
来源：http://hz.ybcxt.top/gtiwguxkbb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtiulorxsj.html

[D19] 按字段分组
来源：http://hz.snrcjt.cn/gtznuucylx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.svipenyu.cn/gtjqmtrxyx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtirkxzyql.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtmzxidjdc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtoneyjapj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtenazqhjz.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtsgrcixxk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aizwys.cn/gtpzsxejrm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtzougghyz.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxinkj.top/gthfpnisas.html

Py:   Counter(arr)
来源：http://hz.chenzaomai.com/gtxmzibroj.html

PHP:  array_count_values($arr);
来源：http://hz.pycfn.com/gtheengono.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtwfpjmnca.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtjkohfifx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtahfsorms.html

Go:   // 手写 map[T]int
来源：http://hz.ehwqpu.com/gtjikhjuuz.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtbecbfvgq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtplgxjjud.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtkezawxik.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtkzkhbtzj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtxfjnmtfc.html

JS:   arr.includes(x)
来源：http://hz.cheryme.top/gtfljigbsx.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gterrgwdnz.html

Java: list.contains(x)
来源：http://hz.jyoumei.cn/gteiazsgut.html

Go:   slices.Contains(arr, x)
来源：http://hz.jianghu66.top/gthfbfehpo.html

Ruby: arr.include?(x)
来源：http://hz.jianghu66.top/gtczacseji.html

C#:   list.Contains(x)
来源：http://hz.pycfn.com/gtqchzvkml.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxinkj.top/gtxhmwkyne.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haohaochexian.top/gtslogpiou.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtwvfdoffy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shangyingyoupin.top/gtlczhceyn.html

TS:   [...arr];
来源：http://hz.zhixingplan.top/gthfdpwkxt.html

Java: new ArrayList<>(list);
来源：http://hz.ydzc1.top/gtpikovtsm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhongyouzk.top/gtmedzdszm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtyfytqyqm.html

C#:   new List<int>(list);
来源：http://hz.daxiang520.top/gtfruwwwtw.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gttyvrcghk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtsuiqqssg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtpuzkehsm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtnbzyuyjw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtkhyxoyob.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgufenzy.top/gtcfyuujrz.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtrzudqagf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gthtzwfokn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuxming.cn/gtkgugvmwc.html

[D24] 字典 / Map 基本操作
来源：http://hz.yanxiufei.cn/gtijycngql.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtciatpgbf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhoulong.xyz/gtnwjrqssn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shangyingyoupin.top/gtmstobmtz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtoqxanteq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yueranfly.top/gtdrasrjff.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hfpthk.cn/gtiugwlufw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtnrmwagji.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtqdqbbxgi.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtzyjhpnnh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtrqvkgcxt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuetiantiany.cn/gteteshqtc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aibaodan.cn/gtkeceewbk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtgjpnfrmp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gtccrckgkm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhaomingkeji.xyz/gttifltygc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydzc1.top/gtdoqppjay.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtzhlhwitj.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtklnbsftn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gthfsfkuvo.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtwpwthcfa.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtxrozzobb.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtyodipnha.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtdtpeebkn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gaohongyu789.top/gtlfdopioa.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtydsuhksh.html

C#:   string.Join(", ", list)
来源：http://hz.jqgufenzy.top/gtomptdaro.html

================================================================================
来源：http://hz.fzhhl.top/gtdxishjsu.html

E. 字符串处理
来源：http://hz.tianlin.xyz/gtsordfjxc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtulmretxg.html

[E01] 拼接字符串
来源：http://hz.ydzc1.top/gtdxxmtyvu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tanke756.top/gtviraccft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtyfhvjsnt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtghbmmihx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.svipenyu.cn/gtixgskbju.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gogol.net.cn/gtyvljncdc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxinkj.top/gttjktfshp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.birdmap.top/gtgwewbpfu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.kuanghao11.cn/gtpofrqdar.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gttcfieusr.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gtjsmsckut.html

PHP:  str_repeat("ab", 3);
来源：http://hz.kuanghao11.cn/gtnrvemnyz.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtnsbpdfjf.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtlsnhqlbm.html

Java: "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtnnorzzzf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.quarkkingdee.top/gtshpiyijk.html

Ruby: "ab" * 3
来源：http://hz.cqqwz.cn/gtigsgixjc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sweek.top/gtwsrlsyav.html

[E03] 截取子串
来源：http://hz.jinqigfzy.top/gtigbtekkk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtvqnvnmwr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gthdaiymtv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gthkzpvcvl.html

TS:   s.slice(1, 4)
来源：http://hz.sweek.top/gtnihwvvbh.html

Java: s.substring(1, 4)
来源：http://hz.tanke756.top/gtmuhlnnpe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gaohongyu789.top/gtbmxinhtj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fzhhl.top/gtcoacqpou.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258.top/gtsltpapol.html

[E04] 查找子串位置
来源：http://hz.zhiwuduotai.top/gtpkpgnhom.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gteevnfvxc.html


<!-- 参考信息 -->