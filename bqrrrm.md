代发 wailian999

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtkcfxdbxp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yueranfly.top/gtczporrwu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhijiandao.cn/gtztoxfucp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnqzz.top/gtpavgsaag.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxuanxn.top/gtisyhnimf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtxwtaoxmn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fzhhl.top/gtmgvqbvuj.html

================================================================================
来源：http://hz.sxryk.cn/gtxpqhymdv.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtzllpacrl.html

================================================================================
来源：http://hz.jinqigufen.top/gtyguqauix.html

[D01] 创建数组 / 列表
来源：http://hz.yuxming.cn/gtgccyxdqh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtrpurwupc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gtzcmjouag.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtydtqbyss.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gtibpwkjcv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhongyouzk.top/gtrluauruw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gtxukldfqh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtocoewdld.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj202588.top/gtaozhgkum.html

[D02] 追加元素到末尾
来源：http://hz.daria6918.cn/gtvkkzkint.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigfzy.top/gthvuepfpp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtakxdobww.html

JS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtonycbdfu.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtrmfusdbj.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtqulkndhc.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gtsxkfoxdw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.52xcode.cn/gtlzgtwqqz.html

C#:   list.Add(4);
来源：http://hz.zdqjudy.top/gtjvslzily.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gttccgmnki.html

Py:   arr.insert(0, 0)
来源：http://hz.jiagoushi.top/gtwyqsxxrb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gtipzsnxqi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tian-w.cn/gtdqrldnwk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhaomingkeji.xyz/gtditanplu.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gthigqgbqq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gthiuvlook.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhoulong.xyz/gtjwrkldvv.html

C#:   list.Insert(0, 0);
来源：http://hz.jiagoushi.top/gtzfpstftx.html

[D04] 删除元素
来源：http://hz.yuxming.cn/gtrenbslty.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtsyforclz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtxpkyspts.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtdobdtjqw.html

TS:   arr.splice(0, 1);
来源：http://hz.daxiang520.top/gtnxwatgqe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tanke756.top/gtawbemyaj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtwmjzbtqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtwapmoajv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtfqtwxqgz.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtfocijcon.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtdyhfkhrq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aizwys.cn/gthhuslclk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtwccdrqja.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj202588.top/gthltenjjs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gtuukgohxc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gtrxtluagy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtuexctizt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtnyhdgkqq.html

[D06] 数组长度
来源：http://hz.yj20258.top/gttowirsds.html

Py:   len(arr)
来源：http://hz.daxiang520.top/gtshliknmj.html

PHP:  count($arr);
来源：http://hz.yuxming.cn/gteevwhbaq.html

JS:   arr.length
来源：http://hz.c1oappe.top/gtmfkqvkgi.html

TS:   arr.length
来源：http://hz.xziqi.cn/gtuwjhyscl.html

Java: list.size();
来源：http://hz.yueranfly.top/gtawojqyxi.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtkpcxokms.html

Ruby: arr.length; arr.size
来源：http://hz.zdqjudy.top/gtyxnavuwr.html

C#:   list.Count;
来源：http://hz.zhengqikj.top/gtllviwsqy.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtmudnivxm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtcnndqqfy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenjidiqi.icu/gtnbglqiig.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtpxqltwkw.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtakjfirwx.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtfgdttiyb.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtcdpiravb.html

Ruby: arr[1, 3]
来源：http://hz.yongpay.top/gtoxowootq.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtfygbyxvi.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtzjoiqfos.html

Py:   a + b;  a.extend(b)
来源：http://hz.c1oappe.top/gtzcjqgvfb.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtbpoprigp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangtech.top/gtyzyaidkp.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtdhfvhgas.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gteldhziyo.html

Go:   append(a, b...)
来源：http://hz.cashguo.top/gtctunwpeq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhongyouzk.top/gtfjrbfiww.html

C#:   a.Concat(b).ToList()
来源：http://hz.cdnleiting.top/gtuqsjypvu.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtlejmkkck.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtxbpmuplh.html

PHP:  sort($arr);
来源：http://hz.meibo888.top/gtezcleyec.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtvxrjralf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtypgyyenv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtdjyqidlz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gthbvzehys.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtflhytmgn.html

C#:   list.Sort();
来源：http://hz.hfpthk.cn/gtuqguflkr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtayokkdyg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtqyjtrrkr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtfhyiruim.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtmbqiieuu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtckbfarxh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gtktfnpxqk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtrsjajebn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fzhhl.top/gtelsftatm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gtmpoixzhs.html

[D11] 反转数组
来源：http://hz.daxiang520.top/gtjttwvpov.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fzhhl.top/gtfwiwswff.html

PHP:  array_reverse($arr);
来源：http://hz.chenlongwang.top/gtfubpfcoe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangtech.top/gtirnnzsug.html

TS:   [...arr].reverse();
来源：http://hz.sufxvd.cn/gtvdbaibjl.html

Java: Collections.reverse(list);
来源：http://hz.yj20258888.top/gtdfffofpj.html

Go:   slices.Reverse(arr)
来源：http://hz.zhixingplan.top/gtfajjljyw.html

Ruby: arr.reverse
来源：http://hz.chenjidiqi.icu/gttutdtmtx.html

C#:   list.Reverse();
来源：http://hz.ybcxt.top/gtluyfrcom.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtmbjsxboo.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuxming.cn/gthsrojccg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tanke756.top/gtruodtkjb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtczifloys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtvgbpjuot.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtvazprdgt.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigfzy.top/gtgkpfsmxm.html

Ruby: arr.index(x)
来源：http://hz.xuetiantiany.cn/gtafhedzta.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gteucdegia.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtxbwnhxcv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shuidangran.top/gtpaijiaks.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aizwys.cn/gtjjihzeti.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtieiiqdik.html

TS:   arr.filter(x => x > 3)
来源：http://hz.havefunace.top/gtcfcscdrz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jianghu66.top/gtzorlmwal.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gtaypjnvwb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.0kj1m.cn/gtctykyncr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gaohongyu789.top/gtyuubrvxl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtutfctpnr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtlvyltifp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnxiangtu.top/gtuuzgkdqy.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtwpuhoqei.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtuoupzjnk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtpkbhlhoq.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtcfhmzhmb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtxbqsdiwu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sysykeji.top/gtpssutuks.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtvtjbphlh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtsludbzbq.html

PHP:  array_unique($arr);
来源：http://hz.meibo888.top/gtfvvftyaw.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gthzpncrtt.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtsjqruibc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtnaoumvtn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jianghu66.top/gtfakaltfo.html

Ruby: arr.uniq
来源：http://hz.gzhubu.top/gtqukqptow.html

C#:   list.Distinct().ToList()
来源：http://hz.ehwqpu.com/gtwqcbajyj.html

[D16] 求和与平均值
来源：http://hz.316326.xyz/gtzohmltdm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gtadcsxfhl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtjzpjhblm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtalpcewhk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gtycosquzz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtshvrqcmb.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtljoodfys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtrfyqxbmo.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gthjporyzd.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtqkdcmekl.html

Py:   max(arr);  min(arr)
来源：http://hz.pengpengdd.cyou/gtwkaqwuxr.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj202588.top/gtfhptkfms.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtaqxfnbab.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gttbahjpim.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daxiang520.top/gtmftczwkx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.birdmap.top/gtilrdakvb.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258888.top/gtmfjszase.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtlskkxcji.html

[D18] 扁平化嵌套数组
来源：http://hz.zycfv.cn/gtjknphcmd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtsvacjdxw.html

PHP:  array_merge(...$nested);
来源：http://hz.gaohongyu789.top/gthbxduxhe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtntsfwucw.html

TS:   nested.flat();
来源：http://hz.hnxiangtu.top/gtkvzbxexx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtppduyonl.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtfenhkpwc.html

Ruby: nested.flatten
来源：http://hz.guowangkeji.top/gtruwmecbo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jyoumei.cn/gtuuvrebmb.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtdbxpjxus.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuanzx.com/gtuydfrhfq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgfzy.top/gtykwsupjc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtmqlsfpfa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtaurqdtrp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtkmmfzcdt.html

Go:   // 手写 map[string][]T
来源：http://hz.feifeiyinyue.top/gtmbckzzhg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangshuangyany.cn/gtimrhtlsa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtufdccqqu.html

[D20] 统计每个元素出现次数
来源：http://hz.aibaodan.cn/gtroegjwqj.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtpkcykihx.html

PHP:  array_count_values($arr);
来源：http://hz.pycfn.com/gtlpnipyqx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gthhtoytjv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gteuetqiya.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guannengcc.top/gtmvjasnqf.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigufen.top/gteumwopar.html

Ruby: arr.tally
来源：http://hz.yonumen.top/gtkycrxbbh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jiagoushi.top/gtacgoxpuj.html

[D21] 判断是否包含某元素
来源：http://hz.yuanzhike.top/gtuzbqluxl.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtlnkeluaq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtmnlehziu.html

JS:   arr.includes(x)
来源：http://hz.316326.xyz/gthhuhkapd.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtdpbhdosr.html

Java: list.contains(x)
来源：http://hz.yuxming.cn/gtqdfydxrv.html

Go:   slices.Contains(arr, x)
来源：http://hz.andypj.xyz/gtomiakkkk.html

Ruby: arr.include?(x)
来源：http://hz.sxryk.cn/gtqwnqfgfp.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtamprlafd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jianghu66.top/gtsiorztpm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gtlylccnef.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtohktzipe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangdashe.top/gtwnhdwtsh.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtkyajaajv.html

Java: new ArrayList<>(list);
来源：http://hz.hfpthk.cn/gtrcavrlbe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuanzhike.top/gtukmxryhq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xziqi.cn/gtkewcultk.html

C#:   new List<int>(list);
来源：http://hz.jqgufenzy.top/gtugxlgwwa.html

[D23] reduce 累积计算
来源：http://hz.sufxvd.cn/gtocrseldb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yanxiufei.cn/gtbbcpyfhv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigufen.top/gtybwqxkgn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtetktqgej.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtcpkpcofj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gtjzbmohpb.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtjbsyavii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hammf.cn/gttnxvseaf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgufenzy.top/gtjkvqumrx.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhaomingkeji.xyz/gtppdddoqb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cqqwz.cn/gtvwhueylv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxuanxn.top/gtkogwtyfv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtnnittsbo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtfsebkqih.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tianlin.xyz/gtkcmrqnsm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhengqikj.top/gtrjpsapal.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gtmidqpwin.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nwbrower.top/gtmgsgzobb.html

[D25] Set 集合去重与交并差
来源：http://hz.pengpengdd.cyou/gtlarzkanc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jyoumei.cn/gtbrhcxatg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tianlin.xyz/gthpnyigwm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gtlzfjcaou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenjidiqi.icu/gthceueylo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydzc1.top/gtmrhnfnnu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtlqfywtkt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuxming.cn/gtxlntszzr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtpfyjlnym.html

[D26] 数组转字符串
来源：http://hz.shzxlz.cn/gtqpymlnfu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhijiandao.cn/gtjsbgjrkr.html

PHP:  implode(", ", $arr);
来源：http://hz.ivvv.top/gtvrnhgmhw.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtozukxamj.html

TS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gttbljpxmx.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtvskkilmb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtszrbjduz.html

Ruby: arr.join(", ")
来源：http://hz.sysykeji.top/gtaqixaecu.html

C#:   string.Join(", ", list)
来源：http://hz.nwbrower.top/gtfhrdthlp.html

================================================================================
来源：http://hz.52xcode.cn/gtfrbffbzf.html

E. 字符串处理
来源：http://hz.jyoumei.cn/gtoilnikiv.html

================================================================================
来源：http://hz.zhixingplan.top/gtojgosgga.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtygxeezcl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtidtxgwct.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.havefunace.top/gtrpqvkzpf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtxydsrrww.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtetrpwhzk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.redwolf501.top/gtmhlhfbuf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gteyxejshr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhengqikj.top/gtkwhnault.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yanxiufei.cn/gtjytuveel.html

[E02] 重复字符串
来源：http://hz.52xcode.cn/gtpeusbjna.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gttldmpdld.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yangfankeji.com/gtbhdodiwe.html

JS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtirsrdlbo.html

TS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gthparokue.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtquekoqbq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sxryk.cn/gtfbkrvasp.html

Ruby: "ab" * 3
来源：http://hz.guannengcc.top/gttozszdvp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ppjwa.cn/gtwlbyckew.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gteqhymjcv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtwtuyqedq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuanzhike.top/gtechuwthf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gthlnunrnm.html

TS:   s.slice(1, 4)
来源：http://hz.redwolf501.top/gtrbcvmcyh.html

Java: s.substring(1, 4)
来源：http://hz.ppjwa.cn/gthzkohxfb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhengqikj.top/gtrmladimr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtexvgxacn.html

C#:   s.Substring(1, 3)
来源：http://hz.52xcode.cn/gtqlpjggdi.html

[E04] 查找子串位置
来源：http://hz.zycfv.cn/gtrncsymen.html

Py:   s.find("x");  s.index("x")
来源：http://hz.iojbl.cn/gtyfssagwg.html

PHP:  strpos($s, "x");
来源：http://hz.xuanzx.com/gtxiuutvnr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gtrelnhnhl.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtlhgdyndb.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtkansbtuy.html

Go:   strings.Index(s, "x")
来源：http://hz.zhijiandao.cn/gtlnvfghxk.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gtyrfjokzz.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtmmbtvmze.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtlgrdtpgg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuanzx.com/gtjznjlbgr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtcjzhuolz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtfgnhhhzp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydzc1.top/gtyprsokgc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.9152youxi.cn/gtyqjatajo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zdqjudy.top/gtlizjshls.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtfuzsozdk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtmzkflnlb.html

[E06] 替换子串
来源：http://hz.andypj.xyz/gtwcvegzyi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hnqzz.top/gtcmcqvxat.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxuanxn.top/gtrnldkxkg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtwxeyuzad.html

TS:   s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtwvzbakop.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtvrwgvnqt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gttmcqutqj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtrbkiomtm.html


<!-- 参考信息 -->