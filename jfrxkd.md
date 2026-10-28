代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtmnetqnyr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guowangkeji.top/gtaahmbwmz.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtgnhpxupl.html

Go:   // 无解构
来源：http://hz.c1oappe.top/gtdyfgcxxc.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtwjquozxd.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtrhfnwslo.html

[C16] 函数 / 方法重载
来源：http://hz.52xcode.cn/gtxkdzyrve.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtvodcwlxm.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtuonwoopx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sxryk.cn/gthrojaivp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.c1oappe.top/gtypphkfvn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gtonivpstm.html

Go:   // 无重载：用不同函数名
来源：http://hz.havefunace.top/gtttrlwggz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydjk.org.cn/gtzeswlgwb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhijiandao.cn/gtsozqpgbo.html

================================================================================
来源：http://hz.52xcode.cn/gtkkztqvxo.html

D. 数组 / 列表 / 集合
来源：http://hz.birdmap.top/gtflhwnjic.html

================================================================================
来源：http://hz.cqqwz.cn/gtlovfsucc.html

[D01] 创建数组 / 列表
来源：http://hz.ydjk.org.cn/gtvxudyapb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.c1oappe.top/gtcydejixb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zdqjudy.top/gtwziiwicn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.feifeiyinyue.top/gtelapujnu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cashguo.top/gtfwgfduta.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258.top/gtmuhtpjbh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yangfankeji.com/gtomhuavgq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtitxorwxl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtvvsmnheh.html

[D02] 追加元素到末尾
来源：http://hz.zhiwuduotai.top/gtgodrnmma.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhengqikj.top/gtvasnplbv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtkudurjkp.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtanfxnpmx.html

TS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtqjayspyc.html

Java: list.add(4);
来源：http://hz.yongpay.top/gtwhknqpcv.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gthitmzhws.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtjagaidoh.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtoboigrpf.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangkeji.top/gtvtnfxnta.html

Py:   arr.insert(0, 0)
来源：http://hz.zhijiandao.cn/gtytvnudlm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhaomingkeji.xyz/gtltyfbexa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gotoacloud.top/gtplpbgobk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.haohaochexian.top/gtrfbrphva.html

Java: list.add(0, 0);
来源：http://hz.bjfxy.top/gttmdvrqtn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gttbfajluk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtjuulibog.html

C#:   list.Insert(0, 0);
来源：http://hz.yongpay.top/gtihvatcem.html

[D04] 删除元素
来源：http://hz.ydjk.org.cn/gtvlejsitd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jyoumei.cn/gtksekneem.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shangyingyoupin.top/gtchgbjvvi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtmuacdmik.html

TS:   arr.splice(0, 1);
来源：http://hz.0kj1m.cn/gtmcgcuhxf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cqqwz.cn/gtruglowch.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtiwszwtvg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtxmqhjtog.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangkeji.top/gtpyngunzo.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gtdsmekwel.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtapbmondw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtxkulwcbu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhoulong.xyz/gtttpdwtoz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtvholticj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangdashe.top/gttatudznr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtxuqzsbke.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtzlomlehj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtidhrflhl.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtymxbpiek.html

Py:   len(arr)
来源：http://hz.yj20258888.top/gtnicjfger.html

PHP:  count($arr);
来源：http://hz.smart0.xyz/gtreztothd.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gtuoslhrfk.html

TS:   arr.length
来源：http://hz.yj20258.top/gtfalblieu.html

Java: list.size();
来源：http://hz.xinyue.icu/gthqxfkksb.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtllrqntmv.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gthwbxdafd.html

C#:   list.Count;
来源：http://hz.cqqwz.cn/gtbewmozpq.html

[D07] 切片 / 取子数组
来源：http://hz.wangdashe.top/gtpbaitetm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258.top/gtdroyagxz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtlvxbavpp.html

JS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtctqpteat.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtowdwjfhl.html

Java: list.subList(1, 4);
来源：http://hz.yonumen.top/gtxjwdrryo.html

Go:   arr[1:4]
来源：http://hz.zycfv.cn/gtxmboiqqb.html

Ruby: arr[1, 3]
来源：http://hz.chenjidiqi.icu/gttzhlyhvr.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhoulong.xyz/gtmcxovywe.html

[D08] 合并两个数组
来源：http://hz.smart0.xyz/gtlvjrswbb.html

Py:   a + b;  a.extend(b)
来源：http://hz.gogol.net.cn/gtbphfuzcq.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtudmuxsrk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xziqi.cn/gturrplsgl.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtpcultsoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gtyhjwccuu.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gtnqpdwssd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yangfankeji.com/gtikzcziuw.html

C#:   a.Concat(b).ToList()
来源：http://hz.ybcxt.top/gtjnjivftk.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtqpsccijw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtlgxizpol.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtlsobsqum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtncgovilb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtzwcgsggo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gtiixjclhb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtsspvbaho.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtryttbyzj.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtxjdeozkt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.meibo888.top/gtvtwvdpni.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tian-w.cn/gteqpnephw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtlbtbdtfj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtwylhjmjw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtygoklklx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gthxjxmiox.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangkeji.top/gtcgjwtmzw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnqzz.top/gtwnqlnosf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gotoacloud.top/gtvsgltwxv.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtuhxakwwy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtwuwnlqmr.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtjnnbgbvf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yangfankeji.com/gtxkdvomwa.html

TS:   [...arr].reverse();
来源：http://hz.jinqigfzy.top/gtpseifgfg.html

Java: Collections.reverse(list);
来源：http://hz.mhx1999.top/gtcdygfbgr.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangkeji.top/gtojnydmrk.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtkdltbmsu.html

C#:   list.Reverse();
来源：http://hz.zhengqikj.top/gtycjwzcmr.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gtvmkyjftp.html

Py:   arr.index(x);  x in arr
来源：http://hz.sysykeji.top/gtqmfdzngi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zycfv.cn/gtnqhxhwag.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtdzwwmczq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtcjnvdfdq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangkeji.top/gthkwsmhtb.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gtxsgivdbf.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtlcxanbuc.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtykjhccqz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenlongwang.top/gtmfrklrkd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xylfe.cn/gttktbzefz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtodnimoqv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtetppritv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtiezqquxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.svipenyu.cn/gtnpzindwn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinghuilouyu.cn/gtosalpxve.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hfpthk.cn/gtsljzvght.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtzhaxtnog.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gogol.net.cn/gtemhdsltz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhixingplan.top/gtcqvhcbbn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtihgkfltp.html

JS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtksqyipek.html

TS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtegsepvty.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.vqdsnc.cn/gtzqkjsvwg.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtzzutldzm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nanxinkj.top/gtyrmsrpjh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cheryme.top/gtmilekyen.html

[D15] 去重
来源：http://hz.wangdashe.top/gtegirvaqz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtnmybzlre.html

PHP:  array_unique($arr);
来源：http://hz.fzhhl.top/gtiqxbpjwp.html

JS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtuiwjqdoa.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtfzkeyqtq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cucudq.cn/gtenzgemae.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtbviimbxr.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtwxveqasj.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtfgjekxpa.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtgligdqul.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtqhstcbsc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ybcxt.top/gtaoqkeoaj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtmujxoqkq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtnesfbjfl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtddpodbeq.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtaadwhayk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tianlin.xyz/gtunpmwlqu.html

C#:   list.Sum();  list.Average()
来源：http://hz.bjfxy.top/gtapahkjks.html

[D17] 最大值与最小值
来源：http://hz.zhongyouzk.top/gtlsovzhre.html

Py:   max(arr);  min(arr)
来源：http://hz.xziqi.cn/gtncroxzyj.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhaomingkeji.xyz/gtdannibzh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhixingplan.top/gtacsdfwew.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtjmfmvuxb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtfjtcwsfo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gtvcotpvnp.html

Ruby: arr.max;  arr.min
来源：http://hz.dashuyun.cn/gthkurcetl.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtegiytkex.html

[D18] 扁平化嵌套数组
来源：http://hz.fzhhl.top/gtdcoubzao.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgufenzy.top/gtizhchqnk.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtjeoysxfq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhiwuduotai.top/gtbjunxhfj.html

TS:   nested.flat();
来源：http://hz.hywenlv.cn/gtxlblfgqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtwkstvqjh.html

Go:   // 手写双层循环
来源：http://hz.iojbl.cn/gtlythhvpf.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtaiumglsd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtptpibryq.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtixnvfusc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtoigtpkfe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtjqnxrfrr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yongpay.top/gtggsehlep.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gteybtktdk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinyuanbaomall.cn/gtslnkypbk.html

Go:   // 手写 map[string][]T
来源：http://hz.cqqwz.cn/gtyfvwdocw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hfpthk.cn/gtnpzixnmn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtgqcjtkjw.html

[D20] 统计每个元素出现次数
来源：http://hz.316326.xyz/gtwwqcmaaw.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gtjmpomcil.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtozfcpxpd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtvdqetapm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtmufobjvi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jianghu66.top/gteiefitql.html

Go:   // 手写 map[T]int
来源：http://hz.daria6918.cn/gtvbchokkb.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtgxticqep.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtqzykskwo.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigfzy.top/gtkkyruwoq.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtwoldzciq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuanzx.com/gtmmmggezg.html

JS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtrikjiwye.html

TS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtnzpaicra.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gtucrpwsfn.html

Go:   slices.Contains(arr, x)
来源：http://hz.yanxiufei.cn/gtcjihefes.html

Ruby: arr.include?(x)
来源：http://hz.aibaodan.cn/gtqagrhzrd.html

C#:   list.Contains(x)
来源：http://hz.aizwys.cn/gtbtqzfpdv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtaekafvat.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.52xcode.cn/gtjahsffti.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gtazxamxtx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtlgtzrkku.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtxfgqajzz.html

Java: new ArrayList<>(list);
来源：http://hz.daxiang520.top/gtnwmedyjc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhoulong.xyz/gtnkavbjhj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtslwapgih.html

C#:   new List<int>(list);
来源：http://hz.ehwqpu.com/gtpyfyazed.html

[D23] reduce 累积计算
来源：http://hz.dianchejie.cn/gtnzojjvxj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ybcxt.top/gtuxfxtiyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtgpwjftue.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtjzrmzskz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtfxrnpllb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yangfankeji.com/gtoxtkktgw.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtjqjyhpxc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yongpay.top/gtvowzqkgy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigfzy.top/gtlplescvd.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtllgihcgz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtmqwkhnve.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.52xcode.cn/gtdrfbfnvm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gtfqwqrggh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtxeshcvcx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigufen.top/gtpfkpfbpi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtyfjtmonc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtpxkzgdgq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtcuwysrka.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtvcupnljw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuxming.cn/gtppqbjvux.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtdbtbnexv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtevfeqfxb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.quarkkingdee.top/gtsbsxyokw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtwoupkphv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shuidangran.top/gtziikimoa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtjehcxaxk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnqzz.top/gtckogofuo.html

[D26] 数组转字符串
来源：http://hz.jianghu66.top/gttxaogtwn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jiagoushi.top/gtniayfxym.html

PHP:  implode(", ", $arr);
来源：http://hz.hongshengwenyu.top/gtlnisiwva.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtpzeauvae.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtpmcxilxz.html

Java: String.join(", ", list)
来源：http://hz.jyoumei.cn/gttmelwhah.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sysykeji.top/gtnqhcvsfr.html

Ruby: arr.join(", ")
来源：http://hz.zhongyouzk.top/gtetfdlmlj.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtjntbtnrs.html

================================================================================
来源：http://hz.jinqigfzy.top/gtzpmpdcgs.html

E. 字符串处理
来源：http://hz.316326.xyz/gtwasokpyy.html

================================================================================
来源：http://hz.sysykeji.top/gtuhahlhvh.html

[E01] 拼接字符串
来源：http://hz.ivvv.top/gtbmuicodw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtzvdebnry.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtlpnapkjy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtpdlurjcy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtimqigilp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yongpay.top/gtxkubezxo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangtech.top/gtuzithwyo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenlongwang.top/gtmhdrmpfv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj202588.top/gtqaprpkjj.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtrcjvekla.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtjsjsqkfh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhijiandao.cn/gtouamcxjy.html

JS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtzjgusmym.html

TS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtqinzesbe.html

Java: "ab".repeat(3)
来源：http://hz.meibo888.top/gtkninypkc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtqgeaslht.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gthgyrepai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.meibo888.top/gtxuhtxvhq.html

[E03] 截取子串
来源：http://hz.gaohongyu789.top/gtykpavrrl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ehwqpu.com/gtxdgcomvt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dianchejie.cn/gtjbcjyiqk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.birdmap.top/gtewxjguxa.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gtvzpqkztk.html

Java: s.substring(1, 4)
来源：http://hz.nanxinkj.top/gtazbjywta.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gttrjrtswe.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtmvffuasw.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgufenzy.top/gtohguipqi.html

[E04] 查找子串位置
来源：http://hz.jlsjyb.cn/gtnuwjpxzt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtqidhkdxe.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtkdaxtntg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtgjienoid.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtxqqaqazv.html

Java: s.indexOf("x")
来源：http://hz.zhoulong.xyz/gttwxsaerb.html

Go:   strings.Index(s, "x")
来源：http://hz.ywan-chungtsiang.top/gtkgravgkx.html

Ruby: s.index("x")
来源：http://hz.cashguo.top/gtprzmhvnf.html

C#:   s.IndexOf("x")
来源：http://hz.jinghuilouyu.cn/gtfltedcka.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ywan-chungtsiang.top/gtgveovfve.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sweek.top/gtpmrtbzdm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtpuvlffdx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtlekwbvak.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.aizwys.cn/gticcdlkbl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtedmhrdfr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtordyzrqn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hfpthk.cn/gtyugxyler.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtpfhprgzd.html


<!-- 参考信息 -->