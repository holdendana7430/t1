代发 wailian999

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gthcbxxotr.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtecuauclv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtsayeejre.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhaomingkeji.xyz/gthklwhvhq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtiglfywre.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gtvhoefsbb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtxmkkhcrd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xylfe.cn/gtixuwmleb.html

C#:   list.Insert(0, 0);
来源：http://hz.zdqjudy.top/gtzsyojdve.html

[D04] 删除元素
来源：http://hz.shangyingyoupin.top/gtrbbcwiek.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zycfv.cn/gtidenlvbx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtclzrlnsx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigufen.top/gtpbvbfctw.html

TS:   arr.splice(0, 1);
来源：http://hz.chenzaomai.com/gtxpionpmc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtvhzmbgif.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtxsuzkdpf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydjk.org.cn/gtgeeshaxi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gtrpakjlyh.html

[D05] 访问与修改元素
来源：http://hz.gzhubu.top/gtcrvjticj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtaigdbeot.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yangfankeji.com/gthtlrgtdc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtwiyloccd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.redwolf501.top/gthnodiqqj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.0kj1m.cn/gtchjcoobf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.birdmap.top/gtzsrgcjnf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtjdbkqxgu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhoulong.xyz/gtsrokfnik.html

[D06] 数组长度
来源：http://hz.feifeiyinyue.top/gtqxixjzrk.html

Py:   len(arr)
来源：http://hz.316326.xyz/gtvxpxoyoj.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtdnvoqcmm.html

JS:   arr.length
来源：http://hz.yuanzhike.top/gtelaovwel.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gttsjolgld.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtjeyiwhok.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtwjrqvpmk.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtqoccpwnv.html

C#:   list.Count;
来源：http://hz.jinqigfzy.top/gtllbiglix.html

[D07] 切片 / 取子数组
来源：http://hz.daxiang520.top/gtfihotmua.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnxiangtu.top/gtsueydrbw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtoqtnpwom.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtorgnejrt.html

TS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtyxeuscaq.html

Java: list.subList(1, 4);
来源：http://hz.yvedp.cn/gtujsiiypl.html

Go:   arr[1:4]
来源：http://hz.cashguo.top/gtkncxnrkg.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gtrlcyjvph.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhongyouzk.top/gtjtfqriri.html

[D08] 合并两个数组
来源：http://hz.dashuyun.cn/gtvkndofdq.html

Py:   a + b;  a.extend(b)
来源：http://hz.pycfn.com/gtmnrmpwzw.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gtcoecwyrt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtoetqkrcm.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gttdtqgkyl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtgvozhmac.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtlytirtsc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shangyingyoupin.top/gtmvwnajaf.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtbjncgijh.html

[D09] 排序（升序）
来源：http://hz.yj20258888.top/gtvxpwflod.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtsxxwwqbu.html

PHP:  sort($arr);
来源：http://hz.hnqzz.top/gtpawdcggd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtlnqrkrya.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtztjfyrni.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtxvgjtygz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtassgdmpk.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtvatcjuyi.html

C#:   list.Sort();
来源：http://hz.cqqwz.cn/gtihtxshoy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shangyingyoupin.top/gtjceixcaq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtdrhcvlln.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtujvmwyzx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtbuzyxhci.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtcfltrmsq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gthmmukubx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ehwqpu.com/gtjboajjvp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgfzy.top/gtjvwnubqs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtcywiyamz.html

[D11] 反转数组
来源：http://hz.pycfn.com/gtpfjvsbku.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shangyingyoupin.top/gtrjifrikn.html

PHP:  array_reverse($arr);
来源：http://hz.52xcode.cn/gtoxmtmcgl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhiwuduotai.top/gtzrsrcgth.html

TS:   [...arr].reverse();
来源：http://hz.dashuyun.cn/gtwiyybmqh.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gtcllrtirj.html

Go:   slices.Reverse(arr)
来源：http://hz.quarkkingdee.top/gtjzbhsurc.html

Ruby: arr.reverse
来源：http://hz.jqgufenzy.top/gthjpjedhm.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtnylhsuch.html

[D12] 查找元素下标
来源：http://hz.shzxlz.cn/gtmzabxcdv.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhengqikj.top/gtkrajbnqa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gotoacloud.top/gtjseeyzhn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gthonzsfwb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtxkrybwlg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinyuanbaomall.cn/gtwviajwts.html

Go:   slices.Index(arr, x)
来源：http://hz.shangyingyoupin.top/gthnmgpmyy.html

Ruby: arr.index(x)
来源：http://hz.nwbrower.top/gtfodmvxcv.html

C#:   list.IndexOf(x);
来源：http://hz.bjfxy.top/gtahswymtw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtpiarfsih.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhaomingkeji.xyz/gtdgmwgjuv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtzxqieddp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtswgiyutv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtlsedlpuq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gthhsrddbw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgufenzy.top/gthosnnpqc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxuanxn.top/gtkozzecpq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gogol.net.cn/gtvkqvzhyc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hnxiangtu.top/gtrfdfkbhi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtmadobztd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxuanxn.top/gtsaxfptef.html

JS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtvuujrqkj.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtfshqpact.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtxawnvdwh.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtiaxqasqs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xinyue.icu/gtpzpbvqsa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gtuhzoducr.html

[D15] 去重
来源：http://hz.sweek.top/gtrxbgoghr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtwmjdqknk.html

PHP:  array_unique($arr);
来源：http://hz.cdnleiting.top/gtvozuqnyc.html

JS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtomtfstnx.html

TS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gthkggxvhn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.meibo888.top/gtksbithxm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hammf.cn/gtytfrovwc.html

Ruby: arr.uniq
来源：http://hz.hywenlv.cn/gtavlzuuuk.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtwropswhk.html

[D16] 求和与平均值
来源：http://hz.tanke756.top/gtbltrytmh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zycfv.cn/gtzyzfowhy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtgvqkvazx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtaywewovb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtdtxbsjte.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258888.top/gtkesfdhrj.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gtjrbsejqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinghuilouyu.cn/gtnryntaoj.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gtnrwluwbi.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gttmpizyzq.html

Py:   max(arr);  min(arr)
来源：http://hz.smart0.xyz/gtyxlpbzww.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhixingplan.top/gtgdozdapq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtzfkybivj.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtddrhschw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenjidiqi.icu/gtsjocorsh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtkiupgkfx.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtugseuiub.html

C#:   list.Max();  list.Min()
来源：http://hz.zhixingplan.top/gtkkhzmavq.html

[D18] 扁平化嵌套数组
来源：http://hz.pengpengdd.cyou/gtuktwjnsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zycfv.cn/gtfonaiydd.html

PHP:  array_merge(...$nested);
来源：http://hz.gotoacloud.top/gtxtiawdut.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yonumen.top/gtdrdghxdh.html

TS:   nested.flat();
来源：http://hz.daxiang520.top/gtqzpcmmxv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shuidangran.top/gtdaaoxuul.html

Go:   // 手写双层循环
来源：http://hz.daria6918.cn/gtlfvtwuft.html

Ruby: nested.flatten
来源：http://hz.ydjk.org.cn/gteftxbtmv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tian-w.cn/gtksrpdkgs.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtunqohcyr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtlizrpezn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgfzy.top/gtcmkbjgkg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ivvv.top/gtiiajzygj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtycnmnyud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtyphisrfu.html

Go:   // 手写 map[string][]T
来源：http://hz.xinyue.icu/gtptpjqlnv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.52xcode.cn/gtncoreqiy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zdqjudy.top/gtqrvshbir.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtqueibrob.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtzsaplhci.html

PHP:  array_count_values($arr);
来源：http://hz.zhaomingkeji.xyz/gtsuezhzrt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tian-w.cn/gtuxaxejdg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtcrdwxzgs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.bjfxy.top/gtfifozqqr.html

Go:   // 手写 map[T]int
来源：http://hz.xuanzx.com/gtdvdsyyyg.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtaiuunwoi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sysykeji.top/gtsctzjljd.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gtgmbqssty.html

Py:   x in arr
来源：http://hz.yj20258.top/gticirhvxk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gtlowjgtzw.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtewlbffxw.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gtqygvhvxo.html

Java: list.contains(x)
来源：http://hz.9152youxi.cn/gtinfeoutw.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtlmrximnb.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtmdzhrept.html

C#:   list.Contains(x)
来源：http://hz.yvedp.cn/gtlevuhlzr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtxutmwanb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtqdxvekac.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.meibo888.top/gtavrlfvwe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtnuvnetbo.html

TS:   [...arr];
来源：http://hz.gogol.net.cn/gtttfwzmsq.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gtjlqbaiji.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ybcxt.top/gtsudmutdf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xinyue.icu/gtbqfodyhd.html

C#:   new List<int>(list);
来源：http://hz.hnxiangtu.top/gtnpnszbmt.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtxwbdthor.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhixingplan.top/gtdskmtzrj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yongpay.top/gtdgsomkov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtyjxjoaih.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtjdfiwchj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtpaodahag.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtzlrlaohd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigufen.top/gtaaoxffix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtzjtfddoa.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtdzopmyue.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtrevfduqf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtkjgdznty.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtmhhxwcys.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.meibo888.top/gtwtfzhmui.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pengpengdd.cyou/gtrrfousyc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtsnupwhck.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gtyaksdiws.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtgtivjwdh.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtndjpfeue.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jianghu66.top/gtxnlugujr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtbdfjwlpe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtgvfbozvm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtcrqlnrxw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gtujwopivw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtjdwyqupu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hfpthk.cn/gtfzjpxvao.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtxqrsvkhn.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtxbvabanv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtbxwnvctf.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtbtqjazdp.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gtqimhlnpi.html

TS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtndzfdezn.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtniafcwjt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gtgblsiame.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtsbohfgva.html

C#:   string.Join(", ", list)
来源：http://hz.meibo888.top/gtaecujlrl.html

================================================================================
来源：http://hz.yuanzhike.top/gtbvsndnaq.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtjbjqlnmu.html

================================================================================
来源：http://hz.pycfn.com/gtetqmstji.html

[E01] 拼接字符串
来源：http://hz.jianghu66.top/gttfrlsvbn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.316326.xyz/gtaqbdtmft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangkeji.top/gtxfamesxa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtibbfqdau.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtessjrznl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtgdkzljbx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtzwsjlkfw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fengsongda.top/gtyxkgxmes.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtwjylgdcq.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtfqrcjwyq.html

Py:   "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gthsoeseja.html

PHP:  str_repeat("ab", 3);
来源：http://hz.316326.xyz/gtyiktylrp.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtjiybaraa.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtzfisydro.html

Java: "ab".repeat(3)
来源：http://hz.iojbl.cn/gtffvwaqlw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtcjlezjql.html

Ruby: "ab" * 3
来源：http://hz.jqgufenzy.top/gtudwvkmml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtjkawhfox.html

[E03] 截取子串
来源：http://hz.chenzaomai.com/gtqgpaepyy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtecesdwam.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj202588.top/gtjspoyawp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnqzz.top/gtzhbvmfbp.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtrvwbmxky.html

Java: s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtrsxcnzic.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258.top/gtzkrtpphx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jianghu66.top/gthmivtdxl.html

C#:   s.Substring(1, 3)
来源：http://hz.kuanghao11.cn/gthzkyycqq.html

[E04] 查找子串位置
来源：http://hz.52xcode.cn/gtwttisttl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shangyingyoupin.top/gtjpjofsmz.html

PHP:  strpos($s, "x");
来源：http://hz.zhixingplan.top/gtcitxgeln.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.bjfxy.top/gtgvksfgzd.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtdykwykjy.html

Java: s.indexOf("x")
来源：http://hz.yvedp.cn/gtloommxrx.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtlncbbyop.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gtwsontvju.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gtznswuuaz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtkwekerfg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuxming.cn/gtflktugbg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xylfe.cn/gtqqhqgmfu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtoflvyklw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj202588.top/gturwkfowz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtzlkxdipk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sysykeji.top/gtwuopzjif.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhijiandao.cn/gthbhqeews.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.52xcode.cn/gtouwwadgy.html

[E06] 替换子串
来源：http://hz.shanyushiyangtech.top/gthjfjpoli.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gzhubu.top/gtvkpfgtwm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhaomingkeji.xyz/gtyznocvzz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtebocrdpz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtjvjcfkjq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtkbwisrbx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aizwys.cn/gtiurqemrv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtpbstklkp.html

C#:   s.Replace("a", "b")
来源：http://hz.nwbrower.top/gtamidprmc.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtycwdnzqi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cashguo.top/gtxtqbqmii.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtzqxqycid.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtwlvzkadx.html

TS:   s.split(",")
来源：http://hz.sufxvd.cn/gtzimmdasj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenjidiqi.icu/gtvtixivrb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cucudq.cn/gtqbbippdd.html

Ruby: s.split(",");  s.split
来源：http://hz.bjfxy.top/gthnfexaas.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gtwfjqawjd.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtyiuoujcn.html

Py:   ",".join(items)
来源：http://hz.jinqigfzy.top/gtqnpulszt.html

PHP:  implode(",", $items);
来源：http://hz.zhixingplan.top/gtzogfumia.html

JS:   items.join(",")
来源：http://hz.xinyue.icu/gtcofzoacw.html

TS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtbhrublfp.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtrotdnwsa.html

Go:   strings.Join(items, ",")
来源：http://hz.0kj1m.cn/gteemxnqhz.html

Ruby: items.join(",")
来源：http://hz.zycfv.cn/gthfuqqkvf.html

C#:   string.Join(",", items)
来源：http://hz.aizwys.cn/gtdutpxhzg.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtbdikmimr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cqqwz.cn/gtijciebtu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.dianchejie.cn/gtodinteww.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtvuesukbg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtlrwnqpbg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtqdiimnaj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtlsynnypc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuetiantiany.cn/gtdnqdhmzv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gtulnbrppl.html


<!-- 参考信息 -->