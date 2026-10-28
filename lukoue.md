代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gtbmlxbrps.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydjk.org.cn/gtmbaqjolb.html

[D09] 排序（升序）
来源：http://hz.xuanzx.com/gthnhcfcxs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtdoyxubou.html

PHP:  sort($arr);
来源：http://hz.tian-w.cn/gtcedhfdhu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pycfn.com/gtvjscluwm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aibaodan.cn/gtirkfjtsw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cqqwz.cn/gtygarfcwf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtneuyvszb.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gttiwzdtjv.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtjlqvgrrv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtcbwaoaab.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.c1oappe.top/gtzviguppc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtupknzkhb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtaobcicia.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtiheesfvi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhijiandao.cn/gtgjzxoecp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtscmciaxk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nwbrower.top/gtpcxodfch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenlongwang.top/gtqlapynpm.html

[D11] 反转数组
来源：http://hz.pycfn.com/gtscnqsudk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydzc1.top/gtylartogo.html

PHP:  array_reverse($arr);
来源：http://hz.snrcjt.cn/gtmbqpqsrk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhijiandao.cn/gtcfhrvlny.html

TS:   [...arr].reverse();
来源：http://hz.bjfxy.top/gtoazqmmbw.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtcdvamhdl.html

Go:   slices.Reverse(arr)
来源：http://hz.zhijiandao.cn/gtmxyqdzku.html

Ruby: arr.reverse
来源：http://hz.fzhhl.top/gtsetziqul.html

C#:   list.Reverse();
来源：http://hz.gzhubu.top/gtrocnyfdj.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gthcbknhpp.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gtwfsfntvx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.9152youxi.cn/gtowghmbqw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtsivgelwp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gteeeefhzo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhongyouzk.top/gtkdcgywls.html

Go:   slices.Index(arr, x)
来源：http://hz.bjfxy.top/gtjyttsalm.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtawdhpwub.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtkigadpaq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtskvuyyle.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.0kj1m.cn/gtucnmzjcg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgfzy.top/gtprhonopr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtzjncufpj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtnbejxuva.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gtpslrqxmw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgfzy.top/gthjqgeueb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hfpthk.cn/gtiixltmxk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gtahstvdws.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hammf.cn/gtjqcrnfcy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xinyue.icu/gtxywmzfwg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gogol.net.cn/gtcbxamdox.html

JS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gttprgtrgg.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxinkj.top/gtyffyticl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtepsznuof.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtnatwvgxx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sxryk.cn/gtuftyrvzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtowmfodtf.html

[D15] 去重
来源：http://hz.jlsjyb.cn/gtelojvmlu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtosjzzzfz.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtjccomnld.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gttygbcjgt.html

TS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtyuyuyumh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtavttehlh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yongpay.top/gtpvppoyts.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gterxdgmat.html

C#:   list.Distinct().ToList()
来源：http://hz.dashuyun.cn/gtivsccidu.html

[D16] 求和与平均值
来源：http://hz.daxiang520.top/gtdgoxaqcb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gaohongyu789.top/gthkpuevui.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtehmiuvnx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtkldoiyeb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtxonbeiox.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pycfn.com/gtdfbxgsdj.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtqqaubriy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gtgoebbkvx.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangdashe.top/gtndgpmerz.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtbzevsziq.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigfzy.top/gtsyzijzhn.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gteszsgfgy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ivvv.top/gtcyponrvu.html

TS:   Math.max(...arr);
来源：http://hz.xuetiantiany.cn/gtbaiqzzxv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhaomingkeji.xyz/gtmmonvpgq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtobutvvzn.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gttqpdhkur.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtklbqnzmd.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtdubodapx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtnxmpzgzi.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtqmzzwpry.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtkktsqytu.html

TS:   nested.flat();
来源：http://hz.havefunace.top/gtwvpxaneh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtgtukbusb.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtiufsneex.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtvqnzuagh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gogol.net.cn/gtizsduewd.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtifvloyus.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gtbrxcjglz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ehwqpu.com/gtekpcbsdw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtkjbmozag.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtgnldplwd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtwknmdkjq.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtweecdvrc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtjawzibmc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dianchejie.cn/gtzsycapbb.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gtccoucekt.html

Py:   Counter(arr)
来源：http://hz.hongshengwenyu.top/gtvnbinsyu.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtcgzmfnpb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtkkphfjze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtddcqqado.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yangfankeji.com/gttqheuxbm.html

Go:   // 手写 map[T]int
来源：http://hz.zhoulong.xyz/gtlwfdtsly.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtbdfmzuxt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.meibo888.top/gtlzupdszh.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtpydansgw.html

Py:   x in arr
来源：http://hz.hammf.cn/gtzzdsfchf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhiwuduotai.top/gtnhgbneky.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtbbbbuzvk.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtjiwnxabf.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtqeyagake.html

Go:   slices.Contains(arr, x)
来源：http://hz.jlsjyb.cn/gtarlvxsgd.html

Ruby: arr.include?(x)
来源：http://hz.chenlongwang.top/gtxbubrcxj.html

C#:   list.Contains(x)
来源：http://hz.ehwqpu.com/gtjaqallrd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yanxiufei.cn/gtfzvhqvue.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.fengsongda.top/gtjyitunfk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtnnzmcabn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.snrcjt.cn/gtvfedzdba.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtzoliagmx.html

Java: new ArrayList<>(list);
来源：http://hz.gotoacloud.top/gtxiurhpan.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sxryk.cn/gtozsjlkrf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtjyzsrjfq.html

C#:   new List<int>(list);
来源：http://hz.hywenlv.cn/gtasoorgfr.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gtjbjwucwx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtrnxasavf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ehwqpu.com/gtvweqzkbw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtuinxiuke.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtcocqbave.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtsdvewrnz.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtigomlofw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtpgjcgord.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sxryk.cn/gtrwhnoqjy.html

[D24] 字典 / Map 基本操作
来源：http://hz.zdqjudy.top/gtvyssngfv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtszvzndrr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gteerxiwot.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gtvfoufhst.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ppjwa.cn/gtdqdrxuvp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cucudq.cn/gtiarkvzho.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtinjbmdgh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtsfrvpulc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtbsoyajdy.html

[D25] Set 集合去重与交并差
来源：http://hz.andypj.xyz/gtyqgeuiwk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtiurfynat.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinyuanbaomall.cn/gtmycbapic.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtblhhsdwe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtfydzsfwz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinyuanbaomall.cn/gtoeisgdht.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sxryk.cn/gtbykxumdm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtyouqnvqx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtnyuvwura.html

[D26] 数组转字符串
来源：http://hz.hnxiangtu.top/gtlyoravgq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jiagoushi.top/gtzjahuzwp.html

PHP:  implode(", ", $arr);
来源：http://hz.sweek.top/gtpvdwwnja.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtkpvewrgp.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtpgsnpazj.html

Java: String.join(", ", list)
来源：http://hz.yuxming.cn/gtwnhylbbj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtooqekjfe.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtqcwwzfex.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtwnsbxyzb.html

================================================================================
来源：http://hz.wangdashe.top/gtfnbwxbhg.html

E. 字符串处理
来源：http://hz.yj20258.top/gtuzokkvim.html

================================================================================
来源：http://hz.cashguo.top/gtyarapwtg.html

[E01] 拼接字符串
来源：http://hz.snrcjt.cn/gthwbobzpu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gotoacloud.top/gtqymxjojy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtczlshqqh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtuncnlpne.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gthygilbcj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cheryme.top/gtqhonntaz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hysaishi.cn/gtlymecqlb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hfpthk.cn/gtdbiryflm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.meibo888.top/gtqwwjoknk.html

[E02] 重复字符串
来源：http://hz.redwolf501.top/gtwxfqemnq.html

Py:   "ab" * 3
来源：http://hz.daxiang520.top/gtcoxvwbsr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtcvwmfkoa.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtempolbxa.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtbedbpwhh.html

Java: "ab".repeat(3)
来源：http://hz.yj20258888.top/gtqmqzflzo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnxiangtu.top/gtswprmkby.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gtqytmajoq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.birdmap.top/gtffkifbqp.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gttmkriucl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.c1oappe.top/gtbblqtyxw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gtfjopzhlq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cqqwz.cn/gtkndkzcrz.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtytpskztj.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtfhosbxmm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnxiangtu.top/gtbbmcdfgr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yonumen.top/gtuknfluzx.html

C#:   s.Substring(1, 3)
来源：http://hz.tian-w.cn/gtuhpnhobh.html

[E04] 查找子串位置
来源：http://hz.sxryk.cn/gtqlehsikl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtcjiapjvj.html

PHP:  strpos($s, "x");
来源：http://hz.jqgfzy.top/gtwdwpamys.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guannengcc.top/gtrobiqqxh.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtkihfnbzf.html

Java: s.indexOf("x")
来源：http://hz.xziqi.cn/gtwjxadjwu.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtrjlbcwwc.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtjsyqeitv.html

C#:   s.IndexOf("x")
来源：http://hz.hfpthk.cn/gtnftgdpfj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258888.top/gtqhuqendb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jiagoushi.top/gtgcykohng.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sxryk.cn/gtgmegaeet.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtqenewssg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.316326.xyz/gtzpgxayqa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtelwuothf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dashuyun.cn/gtpzdxjunh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gogol.net.cn/gtfhapmxrf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.meibo888.top/gtkfytjqmk.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtvtdzsnoj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.smart0.xyz/gtlefijfvb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ehwqpu.com/gtztitpccl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtqvduivtz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtzasrclyk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtaszbyrof.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenlongwang.top/gtcgyazuxt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtswhimvll.html

C#:   s.Replace("a", "b")
来源：http://hz.shangyingyoupin.top/gtocabvfts.html

[E07] 按分隔符拆分
来源：http://hz.fzhhl.top/gtvnfwdfdt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.havefunace.top/gtmfefkqnp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gtukokpouy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtpdkgwjge.html

TS:   s.split(",")
来源：http://hz.yanxiufei.cn/gtlxjhktyo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yonumen.top/gtfetlhbkk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.havefunace.top/gtqxomjqfc.html

Ruby: s.split(",");  s.split
来源：http://hz.jyoumei.cn/gtbyuturkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gtsvxqoeve.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gtfbzjhjnh.html

Py:   ",".join(items)
来源：http://hz.52xcode.cn/gtzmvyylau.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtjpnybdnt.html

JS:   items.join(",")
来源：http://hz.yvedp.cn/gtzpkwqnbu.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtfjmczdyx.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gttketwvzp.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtpryahtob.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gtzgueigfn.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtejyrjeam.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gtcjugsllq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cqqwz.cn/gtubzkgjzd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daria6918.cn/gtnwjmjjlj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtvqnqtiar.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtiofkocst.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gthluhmkip.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhaomingkeji.xyz/gtsoztzhvl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.kuanghao11.cn/gtlprnmykf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtlixqihwr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gtmystdxxy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.meibo888.top/gtxpajpcfs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.smart0.xyz/gtztqirxxe.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtwqnygrgq.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtspxgtzgh.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtcixbpblf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.kuanghao11.cn/gtprdwqqrp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenlongwang.top/gtkeufvzbf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xingfuxueyuan.xyz/gtqutdatvh.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gtopxpljmh.html

Py:   s[::-1]
来源：http://hz.snrcjt.cn/gtncdoavym.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtaaxsxjms.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtvnjnttwk.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtjncskckd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhaomingkeji.xyz/gtylvwkfwx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jlsjyb.cn/gtrlyzawpq.html

Ruby: s.reverse
来源：http://hz.smart0.xyz/gtwqgjghtk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtrynchhlz.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtmaohorbd.html

Py:   s.count("a")
来源：http://hz.chenzaomai.com/gtqhzlmjyk.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtvlcmiwew.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtzxjghhhj.html

TS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtjyyczmwd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtwyszcqlk.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtbokrhztx.html

Ruby: s.count("a")
来源：http://hz.gogol.net.cn/gtypmwlkia.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gttysszysl.html

[E13] 逐字符遍历
来源：http://hz.dashuyun.cn/gtuemeqdlr.html

Py:   for ch in s: print(ch)
来源：http://hz.pycfn.com/gtmuvyilms.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtsivnkqdd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtfgalvrlp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtsbuqycns.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gtmgdzoedk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cucudq.cn/gtbhrseypa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dashuyun.cn/gtgvotuwsx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangshuangyany.cn/gtcjfuactk.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtglquiwzy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtabupablt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gtnylkyyto.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hongshengwenyu.top/gtwkipxwmb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtkolcqagb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gtpqprrdbv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtdkqgabch.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtemmsgfyy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtcdftqqwm.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtovgeklnm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenzaomai.com/gtadpvzhlj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zdqjudy.top/gtwsubpusg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxinkj.top/gtrhdiqxbu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.iojbl.cn/gtehdudzdo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtgmmemfxq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhengqikj.top/gtuyubxzlr.html


<!-- 参考信息 -->