代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daria6918.cn/gtuhzbkdzw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtqmchzlvq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtcocgfxqp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cucudq.cn/gtzjswbfxf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtdqcelklh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jlsjyb.cn/gtouczizwx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtsmcnxpig.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenzaomai.com/gtddwdschz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.316326.xyz/gtmpqbzjwy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sufxvd.cn/gtzjmmjqkq.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gtuerdyysp.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtsyrxawni.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.mhx1999.top/gttdhdycwr.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtrhartbeh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtgptrgvvx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gtpznobiqx.html

[D15] 去重
来源：http://hz.cheryme.top/gtmojulxgq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtukeucsqw.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtrcdkzkkq.html

JS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gtipsptzhe.html

TS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtpcknlqjg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtraqiswyf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtoqasnvtk.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gtpfvzkafp.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtaibqbvyz.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtltaghbix.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gttbmufyzh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtmtcwldcc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtjrjcrfyv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtwahmacwb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtccyomsjm.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtkrnwtnqk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gaohongyu789.top/gtbrbdpayz.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtewwxwuvp.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtjfpavcba.html

Py:   max(arr);  min(arr)
来源：http://hz.gogol.net.cn/gtpikyizex.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtafqdchip.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtbmekoesm.html

TS:   Math.max(...arr);
来源：http://hz.yj20258888.top/gtupdkjufk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtyqryrxid.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xylfe.cn/gtsmlsidxq.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gthcwzfcjh.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtnqxdhbzd.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtzrzdzqte.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tanke756.top/gtzkylikel.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258888.top/gttxwuouiy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hywenlv.cn/gtcewrqner.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gtbaoljtfm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtjdfibeux.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtuzhjfonu.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gthblcisgj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gzhubu.top/gtsgaqisqq.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtcqjydgpq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtkqtihpci.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gthftibrsv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtcppghbwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtdvbkjybi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtyisdkqfk.html

Go:   // 手写 map[string][]T
来源：http://hz.smart0.xyz/gtebuvrcsa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tian-w.cn/gtsjskyawp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtxosvrbvg.html

[D20] 统计每个元素出现次数
来源：http://hz.gaohongyu789.top/gtlwwdhpnq.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtezvwnvrw.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gthtofrbxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtksusbguz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtyxfgyacz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gtlsyyugeb.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtujqpwnpd.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtoydcyjug.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinyuanbaomall.cn/gtffcmpctv.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gttquhtvce.html

Py:   x in arr
来源：http://hz.zhoulong.xyz/gtpibxujys.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtjpgqpojd.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtlotiefrn.html

TS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtzpflhzum.html

Java: list.contains(x)
来源：http://hz.zycfv.cn/gtthqajuew.html

Go:   slices.Contains(arr, x)
来源：http://hz.mhx1999.top/gttemqobae.html

Ruby: arr.include?(x)
来源：http://hz.quarkkingdee.top/gtcahzwlnz.html

C#:   list.Contains(x)
来源：http://hz.chenzaomai.com/gtvuysfitp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.52xcode.cn/gttcswiwmn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.fzhhl.top/gtrqikaoag.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtyfhejiqk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sufxvd.cn/gtupweiuun.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtfypspeqt.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtgdlnhrok.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pengpengdd.cyou/gtvfdmxlaa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.feifeiyinyue.top/gtjvjrasxw.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtewceeqrq.html

[D23] reduce 累积计算
来源：http://hz.jyoumei.cn/gtshqhkhri.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.snrcjt.cn/gtlvbjxouy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhaomingkeji.xyz/gtpundzxmc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gthydlfign.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtskwtjaqe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhongyouzk.top/gtrlynyfgh.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtszbwewih.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtqatgtdwq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhongyouzk.top/gtcsrjfcrz.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydjk.org.cn/gtwsofswpv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuxming.cn/gtuayhfmab.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yvedp.cn/gtvsgmcgkb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zdqjudy.top/gtkncnpysm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtkvmdtekc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daxiang520.top/gtgzkpfknx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtcuulvmbd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtaazmyznq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ehwqpu.com/gtxtzcczns.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtmymiivvd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gtcpalzrsa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cheryme.top/gtausvaowc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtjjcmsnkc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.kuanghao11.cn/gtjcctewhw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.meibo888.top/gtznhtendp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtzdgnkjxu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ppjwa.cn/gtplylecdk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangshuangyany.cn/gtmcwqduyq.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gtvseotwuu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuanzx.com/gtkxoyepkm.html

PHP:  implode(", ", $arr);
来源：http://hz.xuanzx.com/gtuqoxwcjo.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtjqaokywh.html

TS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtmydjsjev.html

Java: String.join(", ", list)
来源：http://hz.nwbrower.top/gtgapbguhm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gtbgzraphn.html

Ruby: arr.join(", ")
来源：http://hz.ybcxt.top/gtiddplpmd.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtfylwewuw.html

================================================================================
来源：http://hz.tianlin.xyz/gtjiysytnr.html

E. 字符串处理
来源：http://hz.nwbrower.top/gtxzvegfxo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzvgczecb.html

[E01] 拼接字符串
来源：http://hz.gaohongyu789.top/gtqzloriqx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jiagoushi.top/gtyarvipei.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtaodmqkrz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gteddvnzbj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtecfxdpjd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xingfuxueyuan.xyz/gtsbkjdziz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtljopkkav.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shangyingyoupin.top/gtxxplzkjl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shangyingyoupin.top/gtkmfauyyg.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gtqblgnsqd.html

Py:   "ab" * 3
来源：http://hz.yanxiufei.cn/gtyvqfpydp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtwlvzzmhn.html

JS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtozsixfxu.html

TS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtsnqyjuwf.html

Java: "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtkqsrsvic.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gtjnrelexg.html

Ruby: "ab" * 3
来源：http://hz.hywenlv.cn/gtwyzdclmb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtazmzrmgy.html

[E03] 截取子串
来源：http://hz.ydzc1.top/gtdfomibfp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jiagoushi.top/gtopmtxzzh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtqavsoady.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxinkj.top/gtvpymcrlc.html

TS:   s.slice(1, 4)
来源：http://hz.fzhhl.top/gtfomtihcz.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtxysjnncw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aibaodan.cn/gtsggjznkz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhengqikj.top/gtdockpzbd.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gtfaafntig.html

[E04] 查找子串位置
来源：http://hz.ppjwa.cn/gtzyaxwcnl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtkskzgswt.html

PHP:  strpos($s, "x");
来源：http://hz.nwbrower.top/gtyxfatirb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zycfv.cn/gtknatfhyh.html

TS:   s.indexOf("x")
来源：http://hz.birdmap.top/gtvsptfqjk.html

Java: s.indexOf("x")
来源：http://hz.cqqwz.cn/gtenpuvmrv.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gtljrrvxgu.html

Ruby: s.index("x")
来源：http://hz.jqgufenzy.top/gthnjgchmc.html

C#:   s.IndexOf("x")
来源：http://hz.shuidangran.top/gtsjpecqzn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gtuballabe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xinyue.icu/gtkbhymaih.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gtvzlkbbtp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtfbryvmaz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtelkptnsp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fengsongda.top/gtsbhmtjml.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shangyingyoupin.top/gtnviyocch.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.snrcjt.cn/gtwlwuokln.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fzhhl.top/gtrmoxpujl.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtqvvoaukd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.aizwys.cn/gtbxkrnwwf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtarwvlrcr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtrjoxojss.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtqcvusnie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtcxmyqeox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jyoumei.cn/gtrjcmrkim.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtstrsvjmx.html

C#:   s.Replace("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtaemyiydi.html

[E07] 按分隔符拆分
来源：http://hz.xziqi.cn/gtomocfnsm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gotoacloud.top/gtrfheijfr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.haohaochexian.top/gtriptlhzz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gttmioorys.html

TS:   s.split(",")
来源：http://hz.0kj1m.cn/gtbsmqudgk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangkeji.top/gthjxwzfsm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtilncnili.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtxwsohfqz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangtech.top/gtexzesdlb.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtvmahmjkt.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gtcjbxjhrv.html

PHP:  implode(",", $items);
来源：http://hz.yueranfly.top/gtevikednm.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtazyvtrzp.html

TS:   items.join(",")
来源：http://hz.mhx1999.top/gtcvdbcamb.html

Java: String.join(",", items)
来源：http://hz.vqdsnc.cn/gtfxgqgsdd.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtszibwsyq.html

Ruby: items.join(",")
来源：http://hz.wangdashe.top/gtpcbgyqyv.html

C#:   string.Join(",", items)
来源：http://hz.daria6918.cn/gtpfpvgmil.html

[E09] 去除所有空白字符
来源：http://hz.guowangkeji.top/gtdrieypoa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shangyingyoupin.top/gtqwfwpxuu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtdsxlczrm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtglldycxj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtuqqkcnhs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuxming.cn/gtcdzkmmpu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtjpshfifa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtusynaopn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cdnleiting.top/gtnkeaossp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgfzy.top/gtetdlfzqw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gtwjdtdbyc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtldqqbmzq.html

JS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtdfjrlwvt.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtfqnwjirs.html

Java: String.format("%03d", 7)
来源：http://hz.andypj.xyz/gtkcsotgze.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtydplwiun.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtstsqxlnc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sxryk.cn/gtjrfvtixl.html

[E11] 反转字符串
来源：http://hz.chenjidiqi.icu/gtrcmokmgr.html

Py:   s[::-1]
来源：http://hz.shuidangran.top/gtnjwkzfgi.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtegbtbpqp.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtudswemwv.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtcllaocpt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yanxiufei.cn/gtmfomryyr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.kuanghao11.cn/gtiyfcudmf.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gtbhzxfyqj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtwfcddqrl.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gthcysfidr.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtpxknldma.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtfwjhrwkf.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gthytgdjmv.html

TS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtwiqhmjsj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ppjwa.cn/gtngsaasmi.html

Go:   strings.Count(s, "a")
来源：http://hz.xuetiantiany.cn/gtwatwkvyk.html

Ruby: s.count("a")
来源：http://hz.52xcode.cn/gtgdzpdyxq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtvaovsvmv.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtzgzqjuce.html

Py:   for ch in s: print(ch)
来源：http://hz.haohaochexian.top/gtmzxfaapk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shzxlz.cn/gthooxeoka.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtqpcwrfkb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gthjcctcki.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtnblcpxtz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ehwqpu.com/gtrqplkykp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxinkj.top/gtdyogneww.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtthclbwmj.html

[E14] URL 编码与 Base64
来源：http://hz.dianchejie.cn/gtbugzbnde.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xylfe.cn/gtycdabmin.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtcfsayoym.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shangyingyoupin.top/gtxfannxof.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtrdkggxsz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jyoumei.cn/gtvtrvensb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tanke756.top/gtvfzjskuo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenjidiqi.icu/gtxytdergf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xziqi.cn/gtvoogetqb.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtarnetbgb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtweackdsl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guannengcc.top/gtfknmifqy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenjidiqi.icu/gtwucxwpbw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtikqiaart.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtlppbvihz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtvugyfxze.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtgblxeppe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenzaomai.com/gtrtnmglrl.html

[E16] 数字千分位
来源：http://hz.yj20258.top/gtvezeqxfg.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gtcudnpvmz.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtxckyrrgd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gthcwhiznq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtiovwsyzt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtanwnoqvh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtswhykpzf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtvwohyfnu.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtquhxltht.html

[E17] 首字母大写
来源：http://hz.tian-w.cn/gtbcicrint.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtjrjhgvfc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.meibo888.top/gtorgbknxl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtvqtwbcdq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtvovocptg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.andypj.xyz/gtbjtwpvsj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yanxiufei.cn/gtmmxgodsy.html

Ruby: s.capitalize
来源：http://hz.zdqjudy.top/gtjjqdyprr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtlngcajpb.html

[E18] 模板占位符替换
来源：http://hz.haohaochexian.top/gtmomxjqgq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.9152youxi.cn/gtwqoyjkxl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xylfe.cn/gtuxfemlta.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtsgznkghg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtxmhnzizp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.havefunace.top/gtcwbedqkh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gtpsorjpyi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtfkczftdd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gtcumxpnxj.html

[E19] 多行文本按行拆分
来源：http://hz.aizwys.cn/gtmmlsvohb.html

Py:   s.splitlines()
来源：http://hz.havefunace.top/gtfkswqavp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuxming.cn/gtoepklpiz.html

JS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtssqeuhgx.html

TS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtwggpcfrx.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtngsfkcoh.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtjhywguzy.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtmwjluqrn.html

C#:   s.Split('\n')
来源：http://hz.cheryme.top/gtybjpmblo.html

[E20] 判断字符串是否为空
来源：http://hz.9152youxi.cn/gtmgtfzaxx.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtutbigdgp.html


<!-- 参考信息 -->