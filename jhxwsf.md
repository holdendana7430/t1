代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtlofkausw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtcryweszn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gogol.net.cn/gthfjvviwm.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtfahcizqg.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtgkvmdinv.html

PHP:  count($arr);
来源：http://hz.redwolf501.top/gtsnntgxek.html

JS:   arr.length
来源：http://hz.xuetiantiany.cn/gthrdqtpzg.html

TS:   arr.length
来源：http://hz.zycfv.cn/gttluhpsmz.html

Java: list.size();
来源：http://hz.yuanzhike.top/gtghwlenof.html

Go:   len(arr)
来源：http://hz.zhoulong.xyz/gtcqafdhci.html

Ruby: arr.length; arr.size
来源：http://hz.ybcxt.top/gtpclwycjz.html

C#:   list.Count;
来源：http://hz.haohaochexian.top/gtbnypqrdq.html

[D07] 切片 / 取子数组
来源：http://hz.zhixingplan.top/gthtcieksl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxuanxn.top/gtnojfkqih.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuanzx.com/gtysunsjpg.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtotsbsvwp.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtvwlwqfdj.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtpeoeflop.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtccghwbnw.html

Ruby: arr[1, 3]
来源：http://hz.mhx1999.top/gtfubxyphu.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtkgphrlux.html

[D08] 合并两个数组
来源：http://hz.hfpthk.cn/gtzyjklhjn.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtcfjusfac.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtkbybsawv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yanxiufei.cn/gtlswmczal.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtslwyzjtt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gtxmyxojds.html

Go:   append(a, b...)
来源：http://hz.hnxiangtu.top/gtzwuvktlz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tianlin.xyz/gtwngsfplb.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtxiyvrkds.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtcwpnemmp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtdxpyymdq.html

PHP:  sort($arr);
来源：http://hz.tianlin.xyz/gtbehisyrz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.svipenyu.cn/gtaxxkrbqd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jqgufenzy.top/gtsyarlako.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtffixgbqt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gtzeexqgxr.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtppbtlxgr.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtckkssgkk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jlsjyb.cn/gtswmhgmps.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gaohongyu789.top/gtxbhbnpdc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtjzpcheki.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtlgykmirz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gthlypizai.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.316326.xyz/gtdtyyyxgf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sysykeji.top/gtrulziuqq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.haohaochexian.top/gtipeudblg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jyoumei.cn/gtniwxmyok.html

[D11] 反转数组
来源：http://hz.dashuyun.cn/gtjatcclfg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtrgqzpkkn.html

PHP:  array_reverse($arr);
来源：http://hz.tianlin.xyz/gtuznixptb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.mhx1999.top/gtztgovroe.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtriicaynz.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtsufgudhd.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gtjfmxgllr.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gtcctiyzmt.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gtuetjmmhs.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtbqypmaxl.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtptfuczfx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.birdmap.top/gtfpyoocvy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gteyiojjap.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtwpqljllv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zycfv.cn/gtxsyikted.html

Go:   slices.Index(arr, x)
来源：http://hz.iojbl.cn/gtjmxjqqbq.html

Ruby: arr.index(x)
来源：http://hz.svipenyu.cn/gtautimwsd.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtzkcqukhv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtsrduxqwe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj202588.top/gtiymojpag.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtkfwosusy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtvnxnwclq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtecofuwrp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.redwolf501.top/gtklkxolsc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fengsongda.top/gtsgayjtom.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtbudeovze.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gzhubu.top/gtuodabkva.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtkhewunhl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtwsnoqpim.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hywenlv.cn/gtdhivsptp.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtimhygvre.html

TS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gthuwkimxi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtpqewyhbp.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtfideqxmr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtlqkorohl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtbjbehntw.html

[D15] 去重
来源：http://hz.yvedp.cn/gtqzkgrymh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtbnzqrtbp.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtrtlgxntk.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtygdajmcd.html

TS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtvbopqzzv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gthgprdmmw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtlcnuioyp.html

Ruby: arr.uniq
来源：http://hz.tianlin.xyz/gtbnzqmmni.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gtqmnndktz.html

[D16] 求和与平均值
来源：http://hz.snrcjt.cn/gtsmowpesk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daxiang520.top/gtwznrxojd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtgtxbaauh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gttnutakov.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gthjqjbsij.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shangyingyoupin.top/gtyerybgbl.html

Go:   // 手写循环累加
来源：http://hz.aizwys.cn/gtsrdrmlqt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gteyktvoqy.html

C#:   list.Sum();  list.Average()
来源：http://hz.redwolf501.top/gtkcpcgaso.html

[D17] 最大值与最小值
来源：http://hz.andypj.xyz/gtymcnplxv.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtmjzpgswy.html

PHP:  max($arr);  min($arr);
来源：http://hz.cashguo.top/gtaosfgspg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtdtovmlof.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gtrlhnbxpr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtajrahzqo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.snrcjt.cn/gtpkjvvnxi.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gtojjqtamz.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtqqbqpkbv.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtesmeqeun.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtpvowalsm.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtxgdxkcop.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.9152youxi.cn/gtgcgfuvjc.html

TS:   nested.flat();
来源：http://hz.fengsongda.top/gtvfhutpvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shuidangran.top/gtmrymaugh.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtgtpiukjq.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtleatlzie.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gogol.net.cn/gtxwfcurbi.html

[D19] 按字段分组
来源：http://hz.shanyushiyangtech.top/gtgzytlzdx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ppjwa.cn/gtlvxnfdtx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gtbhgensyh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sysykeji.top/gtfjllycts.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258888.top/gtaeihyjgt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jianghu66.top/gtnvskzcwx.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gteyhlbtbi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhijiandao.cn/gtsfnzgkew.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sysykeji.top/gtnbrqxbmc.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtjsivnhbq.html

Py:   Counter(arr)
来源：http://hz.havefunace.top/gtqkprvefa.html

PHP:  array_count_values($arr);
来源：http://hz.52xcode.cn/gtqutlvjpc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtdkbjfgvv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtlxintjwh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gtufjwtoze.html

Go:   // 手写 map[T]int
来源：http://hz.pengpengdd.cyou/gtgrqrpqkn.html

Ruby: arr.tally
来源：http://hz.zhaomingkeji.xyz/gtbzsxjhfx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yangfankeji.com/gtprnripiq.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtynifawvf.html

Py:   x in arr
来源：http://hz.redwolf501.top/gtheyoeiuu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jianghu66.top/gtxnqdmwhl.html

JS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtjstptpxc.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtzziszzqu.html

Java: list.contains(x)
来源：http://hz.jiagoushi.top/gtgrjhecvz.html

Go:   slices.Contains(arr, x)
来源：http://hz.zdqjudy.top/gtvnqrbitp.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtpvorobyf.html

C#:   list.Contains(x)
来源：http://hz.sweek.top/gtltitnagd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.0kj1m.cn/gtxuggcuah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yongpay.top/gtukkeiatg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jyoumei.cn/gthxziudut.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtxubjwyge.html

TS:   [...arr];
来源：http://hz.0kj1m.cn/gtbxewyvxv.html

Java: new ArrayList<>(list);
来源：http://hz.dianchejie.cn/gtmixrmqny.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jiagoushi.top/gtqzflmjhu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtbcjqovjw.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtrdizyvkc.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtmfiocpoz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gteawtdgpa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ehwqpu.com/gtlamfnfwa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtgexqcezu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtvvjliaah.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtoogksjsk.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtvyucetye.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.mhx1999.top/gtsbvzxhjf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtsotifxoz.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtfzkvtqdy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtezqigbzj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.mhx1999.top/gtojbmxrnk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtzpjvmgkr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.haohaochexian.top/gtxgflsmeo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtcastbvbi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtuiajppke.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.smart0.xyz/gttfiqfnrt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangkeji.top/gtxdeuqhxw.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtuuhpfvza.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtlzflkuaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shuidangran.top/gtngzzhstf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shuidangran.top/gthddzhpos.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtcatsskca.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dianchejie.cn/gtuptcjyos.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gtmjmdtcgk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtoigfwjge.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sweek.top/gtppmrqxkc.html

[D26] 数组转字符串
来源：http://hz.bjfxy.top/gtmjqrwufz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenlongwang.top/gtsiwmqenu.html

PHP:  implode(", ", $arr);
来源：http://hz.chenlongwang.top/gthtuhosvp.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtahvgfxnx.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gtwunskayl.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtbinamxag.html

Go:   strings.Join(strs, ", ")
来源：http://hz.birdmap.top/gtpkijddkt.html

Ruby: arr.join(", ")
来源：http://hz.nanxuanxn.top/gtkynepkcx.html

C#:   string.Join(", ", list)
来源：http://hz.guowangkeji.top/gtxqhrfani.html

================================================================================
来源：http://hz.yueranfly.top/gtgdnwhhwc.html

E. 字符串处理
来源：http://hz.dianchejie.cn/gtsdwhtifu.html

================================================================================
来源：http://hz.xinyue.icu/gtjdgswgyz.html

[E01] 拼接字符串
来源：http://hz.9152youxi.cn/gtetaegkfs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zdqjudy.top/gtdciyzjyy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtzpzwyryi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtvjzgpaix.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtwycoawxh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.52xcode.cn/gtlceesdjo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gtirhajxqw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtfqwvfmib.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuxming.cn/gtnldvextn.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gtjlujbnuv.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtypxxqydw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuanzhike.top/gtrbfmmyqu.html

JS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtvhcmsopd.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtwsogilnv.html

Java: "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtxgcderry.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gtwctaqdhp.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtfexcbjsh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtlusvzajr.html

[E03] 截取子串
来源：http://hz.gaohongyu789.top/gtqclabrst.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pengpengdd.cyou/gtrdlcczji.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtwabuqxee.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtdhltreaw.html

TS:   s.slice(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtmjdwxvbf.html

Java: s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtffjrbtwa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuxming.cn/gtarknmoci.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtbhgabaon.html

C#:   s.Substring(1, 3)
来源：http://hz.cucudq.cn/gtwosvlgnt.html

[E04] 查找子串位置
来源：http://hz.fengsongda.top/gtjjzlxmyo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.haohaochexian.top/gtuuuqbycd.html

PHP:  strpos($s, "x");
来源：http://hz.cashguo.top/gteofywfmv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtyrayvijh.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtwvgetvzq.html

Java: s.indexOf("x")
来源：http://hz.52xcode.cn/gtikatbtfo.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtoxpvbhpq.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtdpcurvcb.html

C#:   s.IndexOf("x")
来源：http://hz.dashuyun.cn/gtabezmklf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtuvmdvnwz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtelwfuoqf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangtech.top/gtmdfkjott.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtqwtqxnah.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yuanzhike.top/gtqsbjdmst.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtdcfxyhtk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hywenlv.cn/gtmiiyojbb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtyqsexvvo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gtlfpgwmkz.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtzzsspcel.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.kuanghao11.cn/gtwenzwdoe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtzwrsitsx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtlcrhvxpu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtxwrhotel.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtxpllyzff.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtumxxnjxd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yangfankeji.com/gtdrsivbii.html

C#:   s.Replace("a", "b")
来源：http://hz.jiagoushi.top/gtcwuxhslc.html

[E07] 按分隔符拆分
来源：http://hz.zhixingplan.top/gtggmcoeik.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.svipenyu.cn/gtiwfliovr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtskhdwywd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhoulong.xyz/gtdbpomznp.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtnzdazvxn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hammf.cn/gtlworyvdl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtygbcalvb.html

Ruby: s.split(",");  s.split
来源：http://hz.daxiang520.top/gtuobxmhrj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xziqi.cn/gtsbgcairw.html

[E08] 数组按分隔符合并
来源：http://hz.zdqjudy.top/gtmsqnpyrm.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtsfrgqxse.html

PHP:  implode(",", $items);
来源：http://hz.shangyingyoupin.top/gtfiaaguij.html

JS:   items.join(",")
来源：http://hz.hammf.cn/gtraafdufe.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtusawvxvo.html

Java: String.join(",", items)
来源：http://hz.jiagoushi.top/gtsviqfmoa.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gtowtrkbcr.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtjdfqvqei.html

C#:   string.Join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtmmaoainc.html

[E09] 去除所有空白字符
来源：http://hz.tanke756.top/gtrgxgyhgi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgfzy.top/gtryaxjbbs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtfkaaekqy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtblfyyire.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtesyxzggw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daria6918.cn/gtetwmgzxp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gtmyxxscee.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangshuangyany.cn/gtsphztvoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258888.top/gtavrgwbqj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtmvccjmpu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtqinbicls.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtwukntrkp.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gthyhsnhhv.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtzgwzuend.html

Java: String.format("%03d", 7)
来源：http://hz.xziqi.cn/gttxpzqhqy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtutqxikda.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yangfankeji.com/gtjwgaeusl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtmoauojnd.html

[E11] 反转字符串
来源：http://hz.gogol.net.cn/gtefdshxhd.html

Py:   s[::-1]
来源：http://hz.birdmap.top/gtmyxohrhe.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtfreghxhf.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtcvortzxh.html

TS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtnrcnogsa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gtpulmmodh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtkocrygyz.html

Ruby: s.reverse
来源：http://hz.bjfxy.top/gteozpxkkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtsleirnka.html

[E12] 统计某字符出现次数
来源：http://hz.sufxvd.cn/gtprpmslat.html

Py:   s.count("a")
来源：http://hz.zhongyouzk.top/gtsrfcpufy.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gtjamzhtxx.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtnurivblj.html

TS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gtchcslthh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtxfkwxrxe.html


<!-- 参考信息 -->