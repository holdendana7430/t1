代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.jinyuanbaomall.cn/gtzznsgaiw.html

Java: Collections.reverse(list);
来源：http://hz.ydzc1.top/gttjglhgfe.html

Go:   slices.Reverse(arr)
来源：http://hz.iojbl.cn/gtcnttkxwo.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gthcxvngvs.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtztffnejb.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtxkrxlxaq.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgufenzy.top/gtmvnusrwb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtgxhtimyd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtjqkioyyg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtiwyzodru.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtazqxtjhy.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gtoetanmwz.html

Ruby: arr.index(x)
来源：http://hz.chenjidiqi.icu/gtjgbqhzwd.html

C#:   list.IndexOf(x);
来源：http://hz.hnxiangtu.top/gthrusluoj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj202588.top/gtjvtvwgys.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.havefunace.top/gtyosqplgb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgufenzy.top/gtvoxfksyb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtgdlpikus.html

TS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtdagbkoep.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtgljalwcb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtnteiputh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dashuyun.cn/gtkipmglyx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhixingplan.top/gtjzeenhtv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.snrcjt.cn/gtzdxsskla.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigfzy.top/gtvpfiuthn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xziqi.cn/gtzniwpcgu.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtwzaxbzzj.html

TS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtxqvnsekf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhoulong.xyz/gtaglwqest.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtourrnjcd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtlwvipiue.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gtskcymjuz.html

[D15] 去重
来源：http://hz.gzhubu.top/gtrdmilvlg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gtutfhseoz.html

PHP:  array_unique($arr);
来源：http://hz.havefunace.top/gtcjtsjuds.html

JS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtuzxolrri.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtctkfajuk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtfpsagtsp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuanzx.com/gtogmpiqow.html

Ruby: arr.uniq
来源：http://hz.guannengcc.top/gtwycrbllc.html

C#:   list.Distinct().ToList()
来源：http://hz.tianlin.xyz/gtcmiztoih.html

[D16] 求和与平均值
来源：http://hz.havefunace.top/gtnerknmrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guannengcc.top/gtwdzuandf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtksvgyxpz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtifdnjkuk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtksztwcnl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtqzraswqk.html

Go:   // 手写循环累加
来源：http://hz.nwbrower.top/gtaljjxhre.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtragiwsyo.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtansxddii.html

[D17] 最大值与最小值
来源：http://hz.316326.xyz/gtrkraahtz.html

Py:   max(arr);  min(arr)
来源：http://hz.316326.xyz/gtznxgqspc.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhijiandao.cn/gtmamrtelc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtmsfmyjhz.html

TS:   Math.max(...arr);
来源：http://hz.nanxuanxn.top/gtiyaonvkw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jianghu66.top/gtpwggvoyv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtentjhtma.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtylwjkdas.html

C#:   list.Max();  list.Min()
来源：http://hz.chenlongwang.top/gtyymaoyec.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtoruwtvra.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtbjwxhhxh.html

PHP:  array_merge(...$nested);
来源：http://hz.gotoacloud.top/gtljnhztmt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.iojbl.cn/gtbfxdunno.html

TS:   nested.flat();
来源：http://hz.zhiwuduotai.top/gtdsnmfurw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtqkbvrdpn.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtulninfbg.html

Ruby: nested.flatten
来源：http://hz.yongpay.top/gtjzbeypkj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtnwfggjfz.html

[D19] 按字段分组
来源：http://hz.haohaochexian.top/gtqzpqzvkq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtfaxodiss.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinyuanbaomall.cn/gtjboenomu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenjidiqi.icu/gtelixynbg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtvmoxcenh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinyuanbaomall.cn/gtwksmwmji.html

Go:   // 手写 map[string][]T
来源：http://hz.c1oappe.top/gtdasgfjmx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gthgsjtsef.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jiagoushi.top/gtzpkqmgfg.html

[D20] 统计每个元素出现次数
来源：http://hz.shzxlz.cn/gtnnypldgl.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangtech.top/gtcwmtoshj.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gthuoazbfo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtnlakcqzv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtgpgutxnz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jyoumei.cn/gtmsttfqoh.html

Go:   // 手写 map[T]int
来源：http://hz.hammf.cn/gtrhqnldsl.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gtvvdjxqlq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tian-w.cn/gtwgcuikoo.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gtwfyjqjfe.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtxoiulmom.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtydnnynap.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtgbmqhrup.html

TS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtbsnyjilw.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtpfaxlwpv.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtbxkgagsw.html

Ruby: arr.include?(x)
来源：http://hz.zhijiandao.cn/gtjdtlezwo.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtiulftvxv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yongpay.top/gtoeavzwbk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnxiangtu.top/gtkjykofpu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jiagoushi.top/gtqkfsygil.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gtbgfpijfh.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtbnjklysv.html

Java: new ArrayList<>(list);
来源：http://hz.yuanzhike.top/gtjmzimyin.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtbxacdywt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gtebjcsurs.html

C#:   new List<int>(list);
来源：http://hz.jinyuanbaomall.cn/gtugprntkb.html

[D23] reduce 累积计算
来源：http://hz.jiagoushi.top/gtusaubwfi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dianchejie.cn/gtwktsixzm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtollksjwj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtzksrdhts.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtdlalnnfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtesebcbfc.html

Go:   // 手写循环
来源：http://hz.pengpengdd.cyou/gtzkkcumpm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gtbmiytcjm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtxmrxoxmf.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnqzz.top/gtburbdbcr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtiwhccxti.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gttpfpqhrg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gzhubu.top/gtlateqdix.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fzhhl.top/gtuusfgowt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.iojbl.cn/gtiubdyocc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtdvknparn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.svipenyu.cn/gtzivkgnfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtklvxfhdo.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtyaakjoif.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtvunebxrx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zdqjudy.top/gtlfkexrnf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.kuanghao11.cn/gtukdlbfsb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtudvehrvy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtrrubmfgi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gtefwryjnv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gtrtwcoyus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gtmmkeivhg.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtetsehxac.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gaohongyu789.top/gtyphkswfh.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtonahdujr.html

JS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtagcpiobp.html

TS:   arr.join(", ")
来源：http://hz.hywenlv.cn/gtgrkntwrg.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtkmnqzreo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtktbgxrfj.html

Ruby: arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtbsjqzxud.html

C#:   string.Join(", ", list)
来源：http://hz.cheryme.top/gtcsrcldam.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtaypzqsgl.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtwoztiyec.html

================================================================================
来源：http://hz.jianghu66.top/gtvtbqanqi.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gtipexrbyo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hysaishi.cn/gtkwnsvrtt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtvcdpituq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtgokyuivb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtpwmodjbw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sysykeji.top/gtgjeawzik.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.smart0.xyz/gtzkexvjbq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.kuanghao11.cn/gtltdpxabg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtyefcjwas.html

[E02] 重复字符串
来源：http://hz.cheryme.top/gtupdzyrve.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtdaapxjeo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ywan-chungtsiang.top/gtiekorptc.html

JS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtoddtjutp.html

TS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtddtufulg.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtnfkncybz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jianghu66.top/gtijkgtpxw.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtblrolqaa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gtnedyoixa.html

[E03] 截取子串
来源：http://hz.zhixingplan.top/gtnhvdgjbf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtbcqvtocl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gtwjtcudcw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenlongwang.top/gtyavcorfi.html

TS:   s.slice(1, 4)
来源：http://hz.hysaishi.cn/gtackngyql.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtxatchkai.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gtkigfxfpa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gtibmpfuio.html

C#:   s.Substring(1, 3)
来源：http://hz.cucudq.cn/gtxjdcvpgy.html

[E04] 查找子串位置
来源：http://hz.cdnleiting.top/gtzokztpoz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtykknxwue.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtzphvscxz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtinvwodge.html

TS:   s.indexOf("x")
来源：http://hz.hfpthk.cn/gtwmmjmmcy.html

Java: s.indexOf("x")
来源：http://hz.nwbrower.top/gtdnpiahml.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtzzpfawkj.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtgaznfmbi.html

C#:   s.IndexOf("x")
来源：http://hz.hnxiangtu.top/gtctwylzmu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cashguo.top/gtwlfxwqja.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guannengcc.top/gtrvdofxwm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gtpxbbttil.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.9152youxi.cn/gtholtvyuk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinghuilouyu.cn/gtpwnebscf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtepbvroyz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dashuyun.cn/gtmtaeyvxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtpifdxhfb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ivvv.top/gtigkkgzzg.html

[E06] 替换子串
来源：http://hz.aibaodan.cn/gtlqtykilx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shuidangran.top/gtzpvvodsq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtawazxvut.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtzrkhqyao.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtransbrgt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtgbsrsfql.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydjk.org.cn/gttyrplkfa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sweek.top/gtxzvkfdmq.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtxhqfzkhs.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtooioroxo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shuidangran.top/gtyucuqbwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gtaewtawpg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sxryk.cn/gtprviryat.html

TS:   s.split(",")
来源：http://hz.hnqzz.top/gtbfzuacje.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shzxlz.cn/gtztdzxybg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtiexnkkbb.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtlsdcoxtu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtbonwwlkx.html

[E08] 数组按分隔符合并
来源：http://hz.9152youxi.cn/gtpzvndzug.html

Py:   ",".join(items)
来源：http://hz.kuanghao11.cn/gtrejcvblv.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtlngldgzo.html

JS:   items.join(",")
来源：http://hz.aizwys.cn/gteirdxigq.html

TS:   items.join(",")
来源：http://hz.guannengcc.top/gtriyhsnof.html

Java: String.join(",", items)
来源：http://hz.dashuyun.cn/gtywpzgmrq.html

Go:   strings.Join(items, ",")
来源：http://hz.chenjidiqi.icu/gtvobdwqyv.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gtixrnylbf.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtlpjplmhf.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtcffhujmn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shzxlz.cn/gtibpfvcjs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ivvv.top/gtozubwvkl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtvziuufja.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtbfsskojx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtdfwtmcjc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guannengcc.top/gtbosnipxy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yanxiufei.cn/gtvbnhcxyw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gtqdbwzhle.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangkeji.top/gtvdkbxajs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtmyxmrtoe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gtpdgvswft.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtwhilboak.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtcxtgnqgv.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtdsedorln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuxming.cn/gtzpvbvmgj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtfcklrxzu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zycfv.cn/gtpmyfjckz.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gtanxmlfyl.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtlwcachfi.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtqncdrfey.html

JS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtycrkpcom.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtmqxmpsfo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hammf.cn/gtqdsqwtnr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gtmheictza.html

Ruby: s.reverse
来源：http://hz.jianghu66.top/gtkfbaudwv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtffsikggk.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtpggpiaun.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtyvznlhkt.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtxoapmpli.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtwubqukza.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtlcvnhvji.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnxiangtu.top/gtxhmoopjo.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtrglpsyoc.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtlwaqlkmu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jiagoushi.top/gtnublpxvb.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtiveffdtx.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtskwdumwi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ppjwa.cn/gtxdvdxfzo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtejwicpdg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtnktgdzll.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuxming.cn/gtejsvdhfz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.0kj1m.cn/gtbtwvmgxf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnqzz.top/gtlaabukwa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtnkadwtrm.html

[E14] URL 编码与 Base64
来源：http://hz.xziqi.cn/gtgbotxfqz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zycfv.cn/gtjtsfkmpl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenzaomai.com/gtlroappsp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gtegxujwcw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.c1oappe.top/gtwvealkqu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.kuanghao11.cn/gtvxutesgd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtdupbnarl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gogol.net.cn/gtfjncpgjj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.c1oappe.top/gtnizyjiso.html

[E15] HTML 转义 / 反转义
来源：http://hz.snrcjt.cn/gtveqktevq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenjidiqi.icu/gtslhrcmrm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtcoqmyols.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtabqfcdtz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtdrkihczd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtqaqefyve.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.9152youxi.cn/gttaifybbj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ywan-chungtsiang.top/gtbvrdcsoz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shzxlz.cn/gtzcfnueld.html

[E16] 数字千分位
来源：http://hz.cucudq.cn/gtghxylthf.html

Py:   f"{1234567:,}"
来源：http://hz.316326.xyz/gtybxnhzkq.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtvebcdcxb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtarajjrnr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtjyfpvzit.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yangfankeji.com/gtgvpifmms.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.svipenyu.cn/gthtuesvpt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtovmtljos.html

C#:   1234567.ToString("N0")
来源：http://hz.nwbrower.top/gtamzhlxzu.html

[E17] 首字母大写
来源：http://hz.zhengqikj.top/gtrnbfezln.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtbcxfzdsj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gtchdxnouq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gtxbogrwun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gthvotqmai.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gtyvaofpsf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.feifeiyinyue.top/gtqijyjang.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtaoqenuko.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtofadsnlp.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gttmgrsfvk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtompjouvf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fzhhl.top/gtlheeogty.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtuauwzdlo.html


<!-- 参考信息 -->