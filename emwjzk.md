代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtkjchrguc.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gtthzokcbg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtzpqeghzx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gaohongyu789.top/gtmebjiabv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgfzy.top/gtasiawqga.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gteldcvdqr.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtgyvzaocu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.birdmap.top/gtwcbzbifw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtlvnomxts.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtlqypcmuu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fzhhl.top/gtmvvhiuvg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtyothaing.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ybcxt.top/gthnwwnfph.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtyllknmrw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yonumen.top/gtppcdebpf.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtuwdismow.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtkovdoirb.html

PHP:  count($arr);
来源：http://hz.ivvv.top/gtuwgnjokd.html

JS:   arr.length
来源：http://hz.guannengcc.top/gtjnfprbbx.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gtlwsxbyer.html

Java: list.size();
来源：http://hz.daxiang520.top/gtoyqaynpr.html

Go:   len(arr)
来源：http://hz.nwbrower.top/gtmcxzanac.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtewjbrqsf.html

C#:   list.Count;
来源：http://hz.zhaomingkeji.xyz/gtvpblbnck.html

[D07] 切片 / 取子数组
来源：http://hz.yueranfly.top/gthgrujdtp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hywenlv.cn/gtzsndzxor.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yanxiufei.cn/gtypugkhzu.html

JS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtrdtjuvde.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtwxbebkwu.html

Java: list.subList(1, 4);
来源：http://hz.chenjidiqi.icu/gtitchddjw.html

Go:   arr[1:4]
来源：http://hz.c1oappe.top/gteeckegmv.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtsmzqjbiu.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhaomingkeji.xyz/gtmerzhgdu.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gtrlccyule.html

Py:   a + b;  a.extend(b)
来源：http://hz.hfpthk.cn/gtyuyddunz.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtvkynpmkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtwmwqmmxd.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtyjzbuvyg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtakymxwee.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtwdfuaqtw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenjidiqi.icu/gtfroaujbr.html

C#:   a.Concat(b).ToList()
来源：http://hz.ehwqpu.com/gtdrfrmvpv.html

[D09] 排序（升序）
来源：http://hz.yj20258.top/gtxvktbfox.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtjoqqjofv.html

PHP:  sort($arr);
来源：http://hz.52xcode.cn/gtrlwiuhnn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.vqdsnc.cn/gtnlopnaky.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yongpay.top/gtkboqvawn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sweek.top/gttketmdlw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.smart0.xyz/gtptfnuyzq.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtelqjlrwx.html

C#:   list.Sort();
来源：http://hz.xylfe.cn/gtbsyotjar.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtlolbuxbo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shanyushiyangkeji.top/gtnciousaf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtqknsysxz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtqrvktqka.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtvahxgcrk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.mhx1999.top/gtejgrnwet.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtwccdqsjh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtugjtvbzd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtpzvrhlnr.html

[D11] 反转数组
来源：http://hz.yueranfly.top/gtiazfzmkp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gthfxplfvb.html

PHP:  array_reverse($arr);
来源：http://hz.quarkkingdee.top/gtifxolqpt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hongshengwenyu.top/gtdyaleekz.html

TS:   [...arr].reverse();
来源：http://hz.pengpengdd.cyou/gtuepjwfqf.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtjmlhstwn.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gthsfwbifb.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtboijtxcj.html

C#:   list.Reverse();
来源：http://hz.jinqigfzy.top/gtjiyuswel.html

[D12] 查找元素下标
来源：http://hz.hnxiangtu.top/gtljqwkoyc.html

Py:   arr.index(x);  x in arr
来源：http://hz.jyoumei.cn/gtzaiczxru.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtsppmzgmt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtvbbritlj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtrsnpmxha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtswnxcxnd.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtbxuteqql.html

Ruby: arr.index(x)
来源：http://hz.cucudq.cn/gtskvfpqva.html

C#:   list.IndexOf(x);
来源：http://hz.cdnleiting.top/gtsgcnubkf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtocefvnfz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.dianchejie.cn/gtfnveekyo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gtrdwsuhjl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtcflnyytl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtlirvmflb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtteluavjz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.kuanghao11.cn/gtsvzqwthr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtclmuyarp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ivvv.top/gtaszmtkll.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cdnleiting.top/gtlcobbvft.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hnqzz.top/gtcbsdeset.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gtjqfzefez.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gthwxodcoi.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtfnftrirp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtnjcorvfd.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtsgbfqplr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hongshengwenyu.top/gtvmyckvwr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gtivdjjzfa.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtozheuuzu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gthzuibomj.html

PHP:  array_unique($arr);
来源：http://hz.xuanzx.com/gtelslpvbv.html

JS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gtvprngvtq.html

TS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtlktkddyw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtiwtotmlg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenzaomai.com/gtcjycmfyi.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gtebfilval.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtovzbzdaz.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtfcpkabdz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gtkgbhfvxk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtkzorxxnb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtjftxrtfg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtjligwmuz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtcnzvitmm.html

Go:   // 手写循环累加
来源：http://hz.hnxiangtu.top/gtnfcypnmm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigfzy.top/gtsrhioswx.html

C#:   list.Sum();  list.Average()
来源：http://hz.meibo888.top/gtnstterzd.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtxcqkldkm.html

Py:   max(arr);  min(arr)
来源：http://hz.svipenyu.cn/gtezlvkarv.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangshuangyany.cn/gtbyqfkyqz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtxxvdpenm.html

TS:   Math.max(...arr);
来源：http://hz.yongpay.top/gtxcbhovsq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtxragvxvv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gtnfahpfze.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtecbuvvwr.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gtxsvnxwel.html

[D18] 扁平化嵌套数组
来源：http://hz.shuidangran.top/gttxnfywdi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.52xcode.cn/gtjyujexgf.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gtrbfhoyro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gteughdgje.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtebflkopk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhixingplan.top/gtslkoveax.html

Go:   // 手写双层循环
来源：http://hz.sxryk.cn/gtnavcvznr.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtscnpbzbs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtrwgiuqvn.html

[D19] 按字段分组
来源：http://hz.sweek.top/gtleyrgwzc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnqzz.top/gtjcitcbzy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgufenzy.top/gtmphidhad.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jiagoushi.top/gtaownfuey.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtlnlvchvi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydzc1.top/gtquhhuqlx.html

Go:   // 手写 map[string][]T
来源：http://hz.cucudq.cn/gttzackhys.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sweek.top/gtcrvychjy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtjdwbnsbs.html

[D20] 统计每个元素出现次数
来源：http://hz.havefunace.top/gtmtixplvt.html

Py:   Counter(arr)
来源：http://hz.iojbl.cn/gtzhtqvmoz.html

PHP:  array_count_values($arr);
来源：http://hz.jlsjyb.cn/gtfxqdgdox.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtqpqpeztw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtsijnxyfo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guannengcc.top/gtpwkimfku.html

Go:   // 手写 map[T]int
来源：http://hz.ehwqpu.com/gthxkgfykf.html

Ruby: arr.tally
来源：http://hz.dashuyun.cn/gtedoxswmk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenjidiqi.icu/gtveeynogr.html

[D21] 判断是否包含某元素
来源：http://hz.xinyue.icu/gtebmaldel.html

Py:   x in arr
来源：http://hz.xylfe.cn/gttmckgqjo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gtcefitlje.html

JS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtuzppfaod.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtkcdkqpya.html

Java: list.contains(x)
来源：http://hz.yueranfly.top/gtfpgzcipe.html

Go:   slices.Contains(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gttaxbrhsm.html

Ruby: arr.include?(x)
来源：http://hz.yuanzhike.top/gtmpyjrxrt.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtzocxkcud.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shuidangran.top/gtnizbrydd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtadmfgwpy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydjk.org.cn/gtwiejpgsl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fengsongda.top/gthrtabnun.html

TS:   [...arr];
来源：http://hz.sysykeji.top/gtumeeodfu.html

Java: new ArrayList<>(list);
来源：http://hz.zdqjudy.top/gttgifcnqs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtnrnxuaws.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gttboepass.html

C#:   new List<int>(list);
来源：http://hz.jiagoushi.top/gtobwmzhhe.html

[D23] reduce 累积计算
来源：http://hz.pengpengdd.cyou/gtkliytbpc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtrcugkgts.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtusxatote.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gticmffnzj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtsjrikdpp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenjidiqi.icu/gtkszzhzrp.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtprrfceax.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtsmjfovrd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtigpmqovl.html

[D24] 字典 / Map 基本操作
来源：http://hz.zycfv.cn/gtlysafrkb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jianghu66.top/gttwbuazkk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jiagoushi.top/gtfhxrcyys.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtqhboejio.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydjk.org.cn/gtcbwrmnxc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gtqpehvlti.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtiejoqkla.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hywenlv.cn/gtzoxdkscb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtqzmuyzfx.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtjkwobekf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtpzeplqka.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtmibwqyif.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydjk.org.cn/gtgmjjorqd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydzc1.top/gtcisyxytx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgufenzy.top/gtcbeswebr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtjctzqkfw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenzaomai.com/gtiobcnano.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gtkroykyme.html

[D26] 数组转字符串
来源：http://hz.ydjk.org.cn/gtlnmjoedm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.316326.xyz/gtajmawjcr.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gttgvmtdsv.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtxunthfhj.html

TS:   arr.join(", ")
来源：http://hz.316326.xyz/gtcdsnbjcg.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtdnxuvptq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigufen.top/gtqxlyoibl.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtimolcjke.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtoxkviatf.html

================================================================================
来源：http://hz.nanxinkj.top/gtzfzepggr.html

E. 字符串处理
来源：http://hz.xylfe.cn/gtmruotrbf.html

================================================================================
来源：http://hz.316326.xyz/gtlwnjlqhd.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtzotrzfwv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.c1oappe.top/gtimzlumgk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gthjytzfoi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtuafvvvdv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtxnstnqni.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.svipenyu.cn/gtyyjkpwvy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangtech.top/gtczykadoz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhixingplan.top/gttvtjosvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hongshengwenyu.top/gttgefwpqr.html

[E02] 重复字符串
来源：http://hz.wangdashe.top/gtoiwqfquu.html

Py:   "ab" * 3
来源：http://hz.daria6918.cn/gtvgpcuaiu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dashuyun.cn/gtwfkmnowe.html

JS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtcdoghoel.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtauscvwvu.html

Java: "ab".repeat(3)
来源：http://hz.gotoacloud.top/gteumfmffh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gtjthyuapx.html

Ruby: "ab" * 3
来源：http://hz.snrcjt.cn/gtcstidawo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenjidiqi.icu/gtjejsmkcm.html

[E03] 截取子串
来源：http://hz.redwolf501.top/gtyrthqxxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gtwnwnileh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gtioejifhb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtjsjwknxt.html

TS:   s.slice(1, 4)
来源：http://hz.tanke756.top/gtkkcknlrx.html

Java: s.substring(1, 4)
来源：http://hz.cucudq.cn/gtffgzpqsw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gogol.net.cn/gtikhshnin.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gtclcpdaeb.html

C#:   s.Substring(1, 3)
来源：http://hz.hywenlv.cn/gtskmzvxhg.html

[E04] 查找子串位置
来源：http://hz.andypj.xyz/gtvwddvdts.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuxming.cn/gtdopcfhul.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtpprpqvxt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gthzhsnyhd.html

TS:   s.indexOf("x")
来源：http://hz.zdqjudy.top/gtyqxgfqdp.html

Java: s.indexOf("x")
来源：http://hz.yvedp.cn/gtzyxbndue.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtgsircxei.html

Ruby: s.index("x")
来源：http://hz.pycfn.com/gtjilwslnz.html

C#:   s.IndexOf("x")
来源：http://hz.hongshengwenyu.top/gtbhyeizzm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tianlin.xyz/gtuzvazlhu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guannengcc.top/gtdetilmon.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yonumen.top/gtusmdzfwz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aizwys.cn/gtpzjbybzw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtcylwqocc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtxkvjbemv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258.top/gtdxpxntus.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangkeji.top/gtnjekheeq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxuanxn.top/gtuoiqduth.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtlhzaxfcr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xinyue.icu/gtepirfxsu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtclnqsraq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtepyantup.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtrkkcirfu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtjvnqolag.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gtlbxekcgj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sufxvd.cn/gtrbalwzsp.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtkgyycmay.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtlpwqjblj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtshdcxsbb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jyoumei.cn/gtqtxbktxt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhengqikj.top/gtztasrdry.html

TS:   s.split(",")
来源：http://hz.hysaishi.cn/gttdzcngrg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtunwvbjtw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtrwhlodge.html

Ruby: s.split(",");  s.split
来源：http://hz.sxryk.cn/gtwfvzikrx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnxiangtu.top/gtgeohhcfw.html

[E08] 数组按分隔符合并
来源：http://hz.hnxiangtu.top/gtlzheoayc.html

Py:   ",".join(items)
来源：http://hz.feifeiyinyue.top/gthnarztwo.html

PHP:  implode(",", $items);
来源：http://hz.svipenyu.cn/gtwtiqtovc.html

JS:   items.join(",")
来源：http://hz.jiagoushi.top/gtftpoqkrs.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtevzrvkyc.html

Java: String.join(",", items)
来源：http://hz.nwbrower.top/gtmcpjllwf.html

Go:   strings.Join(items, ",")
来源：http://hz.zhengqikj.top/gtvpqbmudp.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtvgyhepsj.html

C#:   string.Join(",", items)
来源：http://hz.jiagoushi.top/gtdnbtpksy.html

[E09] 去除所有空白字符
来源：http://hz.vqdsnc.cn/gtrpjzxpsb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxinkj.top/gtfempkkti.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtssvnxsou.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtbjqughjx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtukixnwzt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ehwqpu.com/gtoqzhgvkm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtofyfbdrf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.haohaochexian.top/gtgqlxiaio.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtkwtaytzz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtdcehplhu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangtech.top/gtjdqyhpdz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtuyyhdqnp.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtequortif.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtcndtnkfn.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtdufkcwrh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydjk.org.cn/gtbjrmfvod.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtupahoqdm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtsblgqgpr.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtegnxnwft.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gtjirjptwf.html

PHP:  strrev($s);
来源：http://hz.yj20258.top/gtcdclakiq.html


<!-- 参考信息 -->