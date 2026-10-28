代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xylfe.cn/gtrjzabzax.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtnnpxwcfh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtymajfgjd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtmwusawhn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtcakyjope.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.quarkkingdee.top/gtwhwrtwdc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yueranfly.top/gtgwcmoekm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuxming.cn/gtqbcppleh.html

[D11] 反转数组
来源：http://hz.zhijiandao.cn/gtkqgqaxhx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.meibo888.top/gtuwsltpvl.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtascqtnda.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnxiangtu.top/gthnbctwvc.html

TS:   [...arr].reverse();
来源：http://hz.jinyuanbaomall.cn/gtoaggavsk.html

Java: Collections.reverse(list);
来源：http://hz.shangyingyoupin.top/gthukboxqg.html

Go:   slices.Reverse(arr)
来源：http://hz.zhengqikj.top/gtbfsklxrz.html

Ruby: arr.reverse
来源：http://hz.shzxlz.cn/gtardyyqnh.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gteyjbisem.html

[D12] 查找元素下标
来源：http://hz.birdmap.top/gthfawlldp.html

Py:   arr.index(x);  x in arr
来源：http://hz.bjfxy.top/gthifcmktb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtpcmsyrxw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtvrodczvz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtfmokjzvv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aizwys.cn/gttjmalkpo.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtmlskwpoy.html

Ruby: arr.index(x)
来源：http://hz.quarkkingdee.top/gttdeptthg.html

C#:   list.IndexOf(x);
来源：http://hz.gogol.net.cn/gtluwjhnnc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gtryvczzoz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtolktriug.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gttkiiancl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtovteumwb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtzneaihvz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.52xcode.cn/gtmwomuzqy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pycfn.com/gtwleokema.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fengsongda.top/gtwrcgwotg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtjatvgiek.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hnqzz.top/gtqyoifcrx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.snrcjt.cn/gtpfaxntpc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jianghu66.top/gtxwgsrvba.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtlwebmidf.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gturkaeftw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtbxkgonxs.html

Go:   // 手写循环
来源：http://hz.dashuyun.cn/gtlzdnmcpi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtttuyqvwj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtzlpnuzgm.html

[D15] 去重
来源：http://hz.hnqzz.top/gttnhoftrd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtffwkaise.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtivxtfapj.html

JS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gthmyqacbx.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtldpayfnq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gaohongyu789.top/gtsxshoicv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gaohongyu789.top/gtinqnhbva.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtqbxlojwy.html

C#:   list.Distinct().ToList()
来源：http://hz.vqdsnc.cn/gtxfdjgipd.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gtqxklpxcf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xylfe.cn/gtqpptkywa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhijiandao.cn/gtsbvxwyvr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtipoxnedb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gthkjrduhv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtclrgoddu.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtjnfyqhvx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gtccfzkckv.html

C#:   list.Sum();  list.Average()
来源：http://hz.haohaochexian.top/gtzexlwvmd.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtlbycenur.html

Py:   max(arr);  min(arr)
来源：http://hz.zhijiandao.cn/gtvykketjh.html

PHP:  max($arr);  min($arr);
来源：http://hz.bjfxy.top/gtsatdezvx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gtkjmeglvn.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtmfcdqkvy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuetiantiany.cn/gtjvljojjt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtbwwqklta.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtzmrkcoex.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtxkjixyqp.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gtsoqfzaho.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cheryme.top/gtnalnaiqd.html

PHP:  array_merge(...$nested);
来源：http://hz.xuetiantiany.cn/gtsnguhrdb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtjgiqcuhr.html

TS:   nested.flat();
来源：http://hz.jinqigfzy.top/gtiopjgltm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yangfankeji.com/gtaksqrlnx.html

Go:   // 手写双层循环
来源：http://hz.yuanzhike.top/gtyjuvigtr.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtoervmlaz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtvkrxphlf.html

[D19] 按字段分组
来源：http://hz.gaohongyu789.top/gtboezuprk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ybcxt.top/gtxaudpuco.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtxtzeerqu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gtqxwmdwls.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gttvnxacda.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtabsgjidw.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtdmtnmvbl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtyxuwetut.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtxxmschtg.html

[D20] 统计每个元素出现次数
来源：http://hz.hnqzz.top/gtvbhdngoz.html

Py:   Counter(arr)
来源：http://hz.chenlongwang.top/gtlwmrytzn.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtkhcgxvhs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtbhjwaaml.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtepvuthgn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jyoumei.cn/gtthzlsqlk.html

Go:   // 手写 map[T]int
来源：http://hz.ppjwa.cn/gtwompjrcz.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtgwdwoxtf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtdawdpaqg.html

[D21] 判断是否包含某元素
来源：http://hz.chenzaomai.com/gtmkbznjcg.html

Py:   x in arr
来源：http://hz.zhaomingkeji.xyz/gtmlganjwt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtlanvnorr.html

JS:   arr.includes(x)
来源：http://hz.redwolf501.top/gtbtpmyrwt.html

TS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gtyipcailj.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtyihjjpop.html

Go:   slices.Contains(arr, x)
来源：http://hz.feifeiyinyue.top/gtayegkvei.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gthxhgklxp.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtbyajsejy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gtouhacknh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhoulong.xyz/gtqqlbioyg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gotoacloud.top/gtxonrxgux.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangshuangyany.cn/gtysjrliiq.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtrzbrewxc.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtwsgsmxap.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.redwolf501.top/gtxyvqzvsm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gthgdyaivs.html

C#:   new List<int>(list);
来源：http://hz.zhaomingkeji.xyz/gtlqsexsiq.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gthqevarki.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sufxvd.cn/gtoxejvmhj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtbtexmrbc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtzdwexmwb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtiuntwotb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gtwtmoohoe.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtnbtzygdx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtuazzbtxt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.feifeiyinyue.top/gtjycchnmt.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtdobwcrvk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.havefunace.top/gtbcqwnroz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.52xcode.cn/gtmrbubbyu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtespfdmfl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gtwbdgjflt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.svipenyu.cn/gtffjyzjys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.redwolf501.top/gtpykdahnz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinghuilouyu.cn/gtcthzsbig.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydzc1.top/gtvejtmuns.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangtech.top/gtfemjqkfh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gthuwegljn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangtech.top/gtwkgomuzp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtugpadfee.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guannengcc.top/gtkznqwavm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ivvv.top/gtxmmjlsok.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtntpmqpxp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.smart0.xyz/gtsvxrytvr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtmtehwxda.html

[D26] 数组转字符串
来源：http://hz.haohaochexian.top/gtmltcszpd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtayrikzsy.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258.top/gtidboybys.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtytnspoab.html

TS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gttzyzutoa.html

Java: String.join(", ", list)
来源：http://hz.xinyue.icu/gtvssmcokn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gthkxlukqw.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gtysqiamsc.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gthfypktxg.html

================================================================================
来源：http://hz.ehwqpu.com/gtwzsbqvta.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gteslsoewg.html

================================================================================
来源：http://hz.wangdashe.top/gtoamjdyet.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gttcyyeiva.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.snrcjt.cn/gtkvnizese.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sufxvd.cn/gtxchwxoix.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtrtnpoeqe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtneexbfzo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xingfuxueyuan.xyz/gtfkvvctfr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pycfn.com/gtythoqjdk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxinkj.top/gtictdynbt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.guowangkeji.top/gtukgjcifu.html

[E02] 重复字符串
来源：http://hz.chenlongwang.top/gtbdjdfzmt.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtnaxpcxus.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xinyue.icu/gtvbmiceks.html

JS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtkowzkjmm.html

TS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtdzbozeyl.html

Java: "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtvssauamt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.mhx1999.top/gtmrdouljd.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtlsmyorji.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guannengcc.top/gtgheydxsi.html

[E03] 截取子串
来源：http://hz.yuxming.cn/gtbweizlje.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xingfuxueyuan.xyz/gtwtewdnvk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.52xcode.cn/gtslznpbsj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.52xcode.cn/gtzqltvhfu.html

TS:   s.slice(1, 4)
来源：http://hz.tian-w.cn/gtjaqqdafh.html

Java: s.substring(1, 4)
来源：http://hz.tanke756.top/gtovrcgwbw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtikborrzo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtofycoccq.html

C#:   s.Substring(1, 3)
来源：http://hz.yuanzhike.top/gtgixgauyi.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtmeamrgkb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gteuxgozwc.html

PHP:  strpos($s, "x");
来源：http://hz.zhixingplan.top/gtufrfspvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.birdmap.top/gtotgyvfpg.html

TS:   s.indexOf("x")
来源：http://hz.birdmap.top/gtkfeexmpt.html

Java: s.indexOf("x")
来源：http://hz.yangfankeji.com/gtejrbruzq.html

Go:   strings.Index(s, "x")
来源：http://hz.hongshengwenyu.top/gtgvbkwtpy.html

Ruby: s.index("x")
来源：http://hz.tanke756.top/gtzghejyfm.html

C#:   s.IndexOf("x")
来源：http://hz.shzxlz.cn/gtquroednv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtyngzuyou.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tian-w.cn/gtchxmicyk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yongpay.top/gtwbzcsjsl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guowangkeji.top/gtpoufapqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jiagoushi.top/gtbsuqadxa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtewskscvb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guowangkeji.top/gtuxcuydxc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenjidiqi.icu/gtweqnlund.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gaohongyu789.top/gtsekjhfrc.html

[E06] 替换子串
来源：http://hz.jinyuanbaomall.cn/gtbpmyntix.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sysykeji.top/gtpeucfkiy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenlongwang.top/gtxjkhdsvb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gthywvtlob.html

TS:   s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gteracxquk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtszhizzsv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuanzhike.top/gtdhkhpwsz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pycfn.com/gtrczcveec.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtjwcrbiow.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtfnlbivuf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shzxlz.cn/gtskatyymz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgfzy.top/gtctjsgddo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtvxlvhhll.html

TS:   s.split(",")
来源：http://hz.yuxming.cn/gtuvfcclcw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenlongwang.top/gtfmiczvcl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gtqtmiejou.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gtzxdhvorq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenjidiqi.icu/gtqjisbion.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtehdevllu.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gtsgedbmse.html

PHP:  implode(",", $items);
来源：http://hz.shangyingyoupin.top/gtfkndwuay.html

JS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtkpaadidz.html

TS:   items.join(",")
来源：http://hz.shzxlz.cn/gtipjffyqk.html

Java: String.join(",", items)
来源：http://hz.sweek.top/gtpvicujvs.html

Go:   strings.Join(items, ",")
来源：http://hz.dashuyun.cn/gtdzabglrs.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtdnpngjtq.html

C#:   string.Join(",", items)
来源：http://hz.tianlin.xyz/gtgzizhtbt.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtrdmnmomw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daxiang520.top/gtunhmnipg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhixingplan.top/gtxhidnord.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtokmmuraq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xingfuxueyuan.xyz/gtsbckrltz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtmjdnlffw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhijiandao.cn/gtveiulxxy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.svipenyu.cn/gtnxvhtynp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigfzy.top/gtdgfgmukp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tanke756.top/gtyxhucacm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtueytqekr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtvbrccjwq.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtgirhmsts.html

TS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtcnhszsmr.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtgwrxikjt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.meibo888.top/gtanalnnxv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.52xcode.cn/gtjtpmgzik.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgufenzy.top/gtwmfuhybf.html

[E11] 反转字符串
来源：http://hz.chenzaomai.com/gtnrosegta.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gthbsblphc.html

PHP:  strrev($s);
来源：http://hz.yj20258888.top/gtcxvwcbqc.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtomvbfrpt.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtsaxafonz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtzekebdju.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtwvuxjzsj.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtdnkblaao.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtmztlidxz.html

[E12] 统计某字符出现次数
来源：http://hz.gzhubu.top/gtqyevltrf.html

Py:   s.count("a")
来源：http://hz.nanxinkj.top/gtrzjwyunx.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gtqhavwbha.html

JS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtkfkflonq.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gtlbdnbrbg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenzaomai.com/gtxzhzpisy.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtyvdtvmvj.html

Ruby: s.count("a")
来源：http://hz.dianchejie.cn/gtjbeocevr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtcxejgfkg.html

[E13] 逐字符遍历
来源：http://hz.zhixingplan.top/gtmkwzevco.html

Py:   for ch in s: print(ch)
来源：http://hz.cucudq.cn/gtahmffpue.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gzhubu.top/gttrercvso.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtejcfsdtm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtgrwrkves.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ehwqpu.com/gtxolhhkir.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.316326.xyz/gtrhogazfw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cucudq.cn/gtkynuyvng.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gtioeloazt.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtkfgcaudf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yongpay.top/gtuhymeqdy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtltgawamh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtaowutqac.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gtyekwzsqq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtmjscvlwg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zycfv.cn/gtxfcrxblg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtveibqaim.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhiwuduotai.top/gtogvjnvmv.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gthldvcuia.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gtjvdhzxgs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gtpmsymnph.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxinkj.top/gtxxdnmqtj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gttlychsxr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtufrbziwv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fengsongda.top/gtnytjbcwv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinghuilouyu.cn/gtosljawbd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtyjrmieeh.html

[E16] 数字千分位
来源：http://hz.316326.xyz/gtobpwtpnz.html

Py:   f"{1234567:,}"
来源：http://hz.cheryme.top/gtzcuhmjgh.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtggkiqwxy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtclmlblmm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtceewjjzm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xylfe.cn/gtkvnunwew.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtynujaqkz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuanzhike.top/gtlbmhiioz.html

C#:   1234567.ToString("N0")
来源：http://hz.zhixingplan.top/gtdhwhjpvj.html

[E17] 首字母大写
来源：http://hz.hnqzz.top/gtjwltdwiq.html


<!-- 参考信息 -->