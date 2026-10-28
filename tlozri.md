代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtuxbtxluo.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtuciwdgcq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xuanzx.com/gtunpmygqs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gteirnppio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cdnleiting.top/gtlczjovyu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtpuvgyoop.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtiuxvomug.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtwmxuvbpi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtidibsxrs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xziqi.cn/gtzfyifxju.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxuanxn.top/gthktyjsmt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtlbbergdz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtvupeaxsh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtqozlgeap.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.feifeiyinyue.top/gteqxchppl.html

[D06] 数组长度
来源：http://hz.jlsjyb.cn/gthcylxpyg.html

Py:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtktdivfcl.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtzywucezl.html

JS:   arr.length
来源：http://hz.haohaochexian.top/gtyqcguhgk.html

TS:   arr.length
来源：http://hz.feifeiyinyue.top/gtplufuwwy.html

Java: list.size();
来源：http://hz.fzhhl.top/gtinyihzmz.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gthtupdfin.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtomuwogjd.html

C#:   list.Count;
来源：http://hz.wangshuangyany.cn/gtkghswqeb.html

[D07] 切片 / 取子数组
来源：http://hz.cqqwz.cn/gtngotfujj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtcqiqnusg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gotoacloud.top/gtnjalznxw.html

JS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtmbllezwz.html

TS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtxupyzjeq.html

Java: list.subList(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtwzbugchb.html

Go:   arr[1:4]
来源：http://hz.zdqjudy.top/gtioqaozaa.html

Ruby: arr[1, 3]
来源：http://hz.gzhubu.top/gtndcilydm.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtpvyghovq.html

[D08] 合并两个数组
来源：http://hz.jyoumei.cn/gtxpfitnuq.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtlplyeeef.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtbxynicdw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zdqjudy.top/gtkvuwibmx.html

TS:   [...a, ...b];
来源：http://hz.jqgufenzy.top/gtujiwqzun.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtytyugvjs.html

Go:   append(a, b...)
来源：http://hz.zhoulong.xyz/gtwwfgqvmd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gtegbajkft.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtqenxmggn.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtveewkalf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtvwcnykdi.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtmkateite.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yvedp.cn/gtggqkwzqv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nanxuanxn.top/gtbvfubqnx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gotoacloud.top/gtboofbqkm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtropwwvac.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtdqpxyntz.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtxaitxaou.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gtjlutsisf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgfzy.top/gtpgkxbspe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtlsxjmjus.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtsnfdqklw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtdhawjzre.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tianlin.xyz/gtaotbfbiq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fengsongda.top/gtdqqwjgcw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258888.top/gtuoauiqpi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtlurjireo.html

[D11] 反转数组
来源：http://hz.9152youxi.cn/gtzeyezxsp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtyxqspvse.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtjqvrttpg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtormorkuj.html

TS:   [...arr].reverse();
来源：http://hz.zhengqikj.top/gtblhumskf.html

Java: Collections.reverse(list);
来源：http://hz.316326.xyz/gtydvrtptt.html

Go:   slices.Reverse(arr)
来源：http://hz.hnqzz.top/gtpfyxyqiz.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtfqfpcbad.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gteenwieji.html

[D12] 查找元素下标
来源：http://hz.andypj.xyz/gtedhtkavj.html

Py:   arr.index(x);  x in arr
来源：http://hz.yongpay.top/gthfunxiqp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ivvv.top/gtwoqwenuq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtvujbyqeb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xingfuxueyuan.xyz/gtzfsgdkim.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cdnleiting.top/gtpispozyz.html

Go:   slices.Index(arr, x)
来源：http://hz.tianlin.xyz/gtfifmouoa.html

Ruby: arr.index(x)
来源：http://hz.0kj1m.cn/gtogdgdixj.html

C#:   list.IndexOf(x);
来源：http://hz.ywan-chungtsiang.top/gtardajzjd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cashguo.top/gtusplktyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhoulong.xyz/gtdiaqfpzy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hongshengwenyu.top/gtxwppzlac.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gtgdyovflj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtuzsupkiv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtobrtslng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtnpoxrgki.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.quarkkingdee.top/gtvpafpwzj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.9152youxi.cn/gtgkubnyen.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtupkwvfpf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtwggtgzxj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnqzz.top/gtfsrlngxx.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtffflfwkt.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtvhojlxmu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtctgkfqgh.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtrobrrxry.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuanzhike.top/gtdftsfqgl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ppjwa.cn/gtrntrznmi.html

[D15] 去重
来源：http://hz.sxryk.cn/gttmnthwsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtltomjbpn.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtgpbhgrmw.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gttrqircyd.html

TS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtnxpalidn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtqdudbiht.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtqdwlmffn.html

Ruby: arr.uniq
来源：http://hz.nwbrower.top/gtilrrfrry.html

C#:   list.Distinct().ToList()
来源：http://hz.9152youxi.cn/gtvorxzxpf.html

[D16] 求和与平均值
来源：http://hz.zhengqikj.top/gtsqssorra.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtqhszbyfp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gtldhlongs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtjbyhumyl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gtzwcvxmtb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtxkvhfjbm.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gttsuolueb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yuxming.cn/gtkabbisfo.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gtdzytmvoj.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtomdnzdko.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgfzy.top/gthionjutw.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtrtyisefk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtpfwachte.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtgqekhkrm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zycfv.cn/gtrywhvize.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtjsscuetu.html

Ruby: arr.max;  arr.min
来源：http://hz.cqqwz.cn/gtooyildwm.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtnfgropqz.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtylyzybrk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtbsvqflkz.html

PHP:  array_merge(...$nested);
来源：http://hz.gogol.net.cn/gtjjdhzltn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daria6918.cn/gtnrocylqx.html

TS:   nested.flat();
来源：http://hz.jlsjyb.cn/gtuiiwgjsc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xziqi.cn/gtmenoteqr.html

Go:   // 手写双层循环
来源：http://hz.ybcxt.top/gtetsbvjrx.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtyjrlhvja.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ybcxt.top/gtzigbkbmt.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtiihvhkzv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtmwpjeqfx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gzhubu.top/gtijnkghyw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtbaydpgmk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtdsetpfbj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtipsiyssa.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtlqcwgmlf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj202588.top/gtkhkvqzsk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtmbkjpqkc.html

[D20] 统计每个元素出现次数
来源：http://hz.yangfankeji.com/gtbggaqvgl.html

Py:   Counter(arr)
来源：http://hz.guowangkeji.top/gtjtepccac.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtvgmzlwsk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gteopjralh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtawrlpylq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.52xcode.cn/gtiugxbxrc.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gttelwckkt.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gthqkkqkvm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtscrrdqmq.html

[D21] 判断是否包含某元素
来源：http://hz.9152youxi.cn/gtdqcfzhiy.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtxekcsmnp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtxukykimc.html

JS:   arr.includes(x)
来源：http://hz.yonumen.top/gtthsdkmpl.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtxsmhzeec.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtygywsbiz.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtxqndkyct.html

Ruby: arr.include?(x)
来源：http://hz.zhiwuduotai.top/gtdsjyydwa.html

C#:   list.Contains(x)
来源：http://hz.guannengcc.top/gtvtxcnqsb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xinyue.icu/gtwafqbzxz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.meibo888.top/gtyioloaak.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxinkj.top/gtwwkdzuas.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtdcgyymxx.html

TS:   [...arr];
来源：http://hz.hywenlv.cn/gtmbcasivj.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtamwmhmva.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shuidangran.top/gtunyqgjpp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cqqwz.cn/gtvaujytzo.html

C#:   new List<int>(list);
来源：http://hz.hywenlv.cn/gtyownlsgl.html

[D23] reduce 累积计算
来源：http://hz.cucudq.cn/gtjhosskit.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtbzhfrirj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigufen.top/gtxuocjqap.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtdortyehx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtzsflswqh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtsyqvwawr.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtblgqavuu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydzc1.top/gtiaabsquy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gtdiadtxba.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtwfpsdase.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gotoacloud.top/gtbbrpjasz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xziqi.cn/gtnedpkxcs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtugrezmpx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinghuilouyu.cn/gtisyyfnyl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pycfn.com/gtllhfabnl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtkxkgmquv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dashuyun.cn/gtbdweuplv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xziqi.cn/gtovfgithx.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtaaddysvm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtmbyeexcw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtleihqzri.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtolvmdoyn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtnslodrkc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shangyingyoupin.top/gtuyqkkqjt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258.top/gtbsdpfjgn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.fengsongda.top/gtizxhncee.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shzxlz.cn/gtcnicjwbv.html

[D26] 数组转字符串
来源：http://hz.feifeiyinyue.top/gtjsffknhq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gteakqayaq.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gtxfmwpakm.html

JS:   arr.join(", ")
来源：http://hz.cheryme.top/gtvffmoyve.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtbgpskstj.html

Java: String.join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtvljyuzxy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tianlin.xyz/gtgransfsk.html

Ruby: arr.join(", ")
来源：http://hz.jiagoushi.top/gtbbklbiwx.html

C#:   string.Join(", ", list)
来源：http://hz.shzxlz.cn/gtshabecgv.html

================================================================================
来源：http://hz.316326.xyz/gthlyswekl.html

E. 字符串处理
来源：http://hz.cashguo.top/gtlevjnled.html

================================================================================
来源：http://hz.chenlongwang.top/gtffiyymwv.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtloyqqygp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.quarkkingdee.top/gtljsmuwik.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtvlsfemhz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtrrpgxwkp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtegdpfwcm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xinyue.icu/gtebgthkuv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtbzwubflo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtdbhncupj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gtnkgggvyb.html

[E02] 重复字符串
来源：http://hz.tianlin.xyz/gtrwkmtiho.html

Py:   "ab" * 3
来源：http://hz.yj20258888.top/gtadgmcotj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gtlktnuatq.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtkgrpubot.html

TS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtynpqzltj.html

Java: "ab".repeat(3)
来源：http://hz.c1oappe.top/gtwyclxlxx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangkeji.top/gtkparldhj.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gtsrzsxsty.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gthvfpusvg.html

[E03] 截取子串
来源：http://hz.pycfn.com/gtqxvzylkg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.kuanghao11.cn/gtcujponah.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnqzz.top/gtclkfiyxo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.havefunace.top/gtrqbihviq.html

TS:   s.slice(1, 4)
来源：http://hz.sufxvd.cn/gtnvdqttpl.html

Java: s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtzitopfhf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ywan-chungtsiang.top/gtnokflmti.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nwbrower.top/gtxtcoecea.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gthyhiwhwv.html

[E04] 查找子串位置
来源：http://hz.nwbrower.top/gtvhxfdqhl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yanxiufei.cn/gtidunjkwz.html

PHP:  strpos($s, "x");
来源：http://hz.guowangkeji.top/gteixhibvc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ybcxt.top/gtzkiystqg.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtesqdgsmd.html

Java: s.indexOf("x")
来源：http://hz.yuxming.cn/gtfqjcnobo.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtxhlnigeh.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtdiknonvn.html

C#:   s.IndexOf("x")
来源：http://hz.gotoacloud.top/gtasbwqdmn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtcjegpzjw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuxming.cn/gtkhftbdye.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xylfe.cn/gtdcnapdna.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtwpzqwykb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ybcxt.top/gtdkaotswd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtebnonmfa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dianchejie.cn/gtogwwprbc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgufenzy.top/gtkxmcnmdy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.9152youxi.cn/gtyhveuucb.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gtiuokwrbc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtvvazfsow.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.bjfxy.top/gtuyrcyeao.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtzmjxvhet.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtcbbjqjnh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtbopdyzrm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydzc1.top/gtdninifpm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sweek.top/gtlwipajws.html

C#:   s.Replace("a", "b")
来源：http://hz.fzhhl.top/gtutqaqdpq.html

[E07] 按分隔符拆分
来源：http://hz.xylfe.cn/gtzhzssxwb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hongshengwenyu.top/gtvxkccnwz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gtkgsdkwcs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fzhhl.top/gtcvmnqfzg.html

TS:   s.split(",")
来源：http://hz.ywan-chungtsiang.top/gtsjmaqrhr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.snrcjt.cn/gtndtwjqdt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hysaishi.cn/gtjxzkdctn.html

Ruby: s.split(",");  s.split
来源：http://hz.yuxming.cn/gtpsjnpgzf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtmgiocjzs.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtprawawrb.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gtepbrmzfm.html

PHP:  implode(",", $items);
来源：http://hz.shuidangran.top/gttnrzvzyr.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtplwtfagk.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtesidahoc.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gtocryducc.html

Go:   strings.Join(items, ",")
来源：http://hz.yanxiufei.cn/gtqgaqesfg.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtcninzxij.html

C#:   string.Join(",", items)
来源：http://hz.shangyingyoupin.top/gtvfthgbyz.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtkmwticnc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtzvbbcyhr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yanxiufei.cn/gtcjktnpsz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtelhdnvbh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtahjkjbur.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gttajamsmf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hysaishi.cn/gtzjodfnhc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gtzwfkdacp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.bjfxy.top/gtazshbdus.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhijiandao.cn/gtzyianwhy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zdqjudy.top/gtbrmprttu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258.top/gtkzojafre.html

JS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtwiuexwgt.html

TS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gttdbhfkpw.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtnoywyvbm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zdqjudy.top/gtvgoketlr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.c1oappe.top/gtohnmflnp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtnusycgvt.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gtigghqtpl.html

Py:   s[::-1]
来源：http://hz.iojbl.cn/gtuwodbecl.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtpkizrwml.html


<!-- 参考信息 -->