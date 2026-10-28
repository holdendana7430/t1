代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jiagoushi.top/gtqwifudpr.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtiyrccqcx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hywenlv.cn/gtzbxvjlgu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtakgesnfl.html

[D15] 去重
来源：http://hz.yuanzhike.top/gtlsrtmyuu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtgomkxsuf.html

PHP:  array_unique($arr);
来源：http://hz.shangyingyoupin.top/gtybqbkzxp.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtcfnycggu.html

TS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtayifpokn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtfvrmjawv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtzejoxdig.html

Ruby: arr.uniq
来源：http://hz.jinghuilouyu.cn/gtgutevsmg.html

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtwoikwhej.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gtandxucnv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydjk.org.cn/gtsgvkblbl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.smart0.xyz/gtnogwucig.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtbnkqdgwf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtclomdpcm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yongpay.top/gtbzpzeicr.html

Go:   // 手写循环累加
来源：http://hz.ehwqpu.com/gtqhdwomct.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.316326.xyz/gtxlfsjxhx.html

C#:   list.Sum();  list.Average()
来源：http://hz.pengpengdd.cyou/gtjkoyhprx.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtznyacgvm.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgfzy.top/gtbrdjqtpt.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtdozkszfg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtonykroii.html

TS:   Math.max(...arr);
来源：http://hz.yj202588.top/gtjjtdrkhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenlongwang.top/gtyzgqlusg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtcpwjudea.html

Ruby: arr.max;  arr.min
来源：http://hz.daxiang520.top/gthhehjvmm.html

C#:   list.Max();  list.Min()
来源：http://hz.jiagoushi.top/gtnrfngvpp.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gtuehhapoc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.c1oappe.top/gtozjtvlmv.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtwyguzvdx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daxiang520.top/gtoofwajzh.html

TS:   nested.flat();
来源：http://hz.zdqjudy.top/gtacprkerz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hongshengwenyu.top/gtwxeaierv.html

Go:   // 手写双层循环
来源：http://hz.pycfn.com/gtliluawlo.html

Ruby: nested.flatten
来源：http://hz.9152youxi.cn/gttlqszctr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtogodwlrs.html

[D19] 按字段分组
来源：http://hz.zhongyouzk.top/gtjqjgjtoz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.smart0.xyz/gtdfewdhyo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hammf.cn/gtrxjuxcio.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtcuxbppcx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtxohxivvr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gtfacnpgpn.html

Go:   // 手写 map[string][]T
来源：http://hz.ydzc1.top/gtxgmfgivs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gtabxyoeyd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.52xcode.cn/gtarrqavxs.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gttmcytsal.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtgfqnkhwo.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gtgikvyvdd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtxrnvbmyt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtzgyabpsd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtgfjhelhc.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtdhtaqybq.html

Ruby: arr.tally
来源：http://hz.ehwqpu.com/gtfuygybou.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtneiozlrw.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtjiogdlqb.html

Py:   x in arr
来源：http://hz.hywenlv.cn/gtyuqqeqdu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shanyushiyangtech.top/gtuxvdzglk.html

JS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtpsoqsnsu.html

TS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtmotmdbup.html

Java: list.contains(x)
来源：http://hz.jiagoushi.top/gtcjvfpcmv.html

Go:   slices.Contains(arr, x)
来源：http://hz.hysaishi.cn/gtmvcdeybt.html

Ruby: arr.include?(x)
来源：http://hz.snrcjt.cn/gtbvpvjadj.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtamyfokio.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtibsbdmeh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gaohongyu789.top/gtlcvuihnh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xziqi.cn/gtqxwdumrc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gttatjvznd.html

TS:   [...arr];
来源：http://hz.hnqzz.top/gtjaqexube.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtkrcrlwve.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.wangdashe.top/gtmabbwyvy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hnqzz.top/gtjhlxlbex.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtjoupvxue.html

[D23] reduce 累积计算
来源：http://hz.jinyuanbaomall.cn/gtohhekiof.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.kuanghao11.cn/gtzqutnemi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtyltcjzcs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtvwqvazta.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtrmjctvqk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aibaodan.cn/gtolygmhqi.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtmavbbruf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nwbrower.top/gtnbxptxfm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuanzhike.top/gtxouygbly.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtnacsgfwh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gtunaigmpk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gteppdurin.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenjidiqi.icu/gtpuozmpel.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.snrcjt.cn/gtwuclleqj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtufmswmaz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtcuspesvv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cheryme.top/gtthahdakf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gttfkpkizd.html

[D25] Set 集合去重与交并差
来源：http://hz.hysaishi.cn/gtnmvefwyh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gtsfxahron.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yangfankeji.com/gtkssruuml.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtvnykthvs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.kuanghao11.cn/gtdgcciotc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtvxxcqezm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtfalnqwen.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shzxlz.cn/gtjukdmfbh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtjpydcdso.html

[D26] 数组转字符串
来源：http://hz.haohaochexian.top/gtircdbggx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtxludzkrd.html

PHP:  implode(", ", $arr);
来源：http://hz.nwbrower.top/gtezqcejon.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtmrrkogbg.html

TS:   arr.join(", ")
来源：http://hz.aizwys.cn/gthzsfulcw.html

Java: String.join(", ", list)
来源：http://hz.tanke756.top/gtdnfkczkb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnqzz.top/gthhiveycr.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gtpgicyfim.html

C#:   string.Join(", ", list)
来源：http://hz.sweek.top/gtivwthjcq.html

================================================================================
来源：http://hz.jiagoushi.top/gttntipszv.html

E. 字符串处理
来源：http://hz.xziqi.cn/gthqfazjlf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfdayqerp.html

[E01] 拼接字符串
来源：http://hz.ydzc1.top/gtxaauycvp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydjk.org.cn/gthlgffabp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtxnqqzzej.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gttqvjqwiq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtnfllvpfv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gthytgznau.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.andypj.xyz/gtiwoocxxp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gogol.net.cn/gtyledwsej.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtfoeesduj.html

[E02] 重复字符串
来源：http://hz.shuidangran.top/gtwwdbfkod.html

Py:   "ab" * 3
来源：http://hz.zhoulong.xyz/gtschkazbn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtooeuuiju.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtvbcbrxif.html

TS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtxakxklrm.html

Java: "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtlgtmepxd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xylfe.cn/gtqxzgqgas.html

Ruby: "ab" * 3
来源：http://hz.wangdashe.top/gtbmvecuyy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtjuqnxwqe.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtfwxhrvbq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxuanxn.top/gtsnanlnlf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenlongwang.top/gtekkfzeum.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtdaxciexh.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258.top/gtsrsyzcpz.html

Java: s.substring(1, 4)
来源：http://hz.jianghu66.top/gtjfxvujli.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtuilvigkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gthntwfbil.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtbpgfejgh.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtwcxgvlwp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.andypj.xyz/gtltjszicv.html

PHP:  strpos($s, "x");
来源：http://hz.hysaishi.cn/gtuofrvydj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xziqi.cn/gtcovjofhg.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtgmgnyakl.html

Java: s.indexOf("x")
来源：http://hz.aibaodan.cn/gtkgpmqgix.html

Go:   strings.Index(s, "x")
来源：http://hz.zdqjudy.top/gtucneaiml.html

Ruby: s.index("x")
来源：http://hz.ppjwa.cn/gtmqfozudt.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtqfggbgpr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.birdmap.top/gtaxfapnfq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gtzcexejir.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cashguo.top/gtxvvsjgpw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtoixrwsvo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.9152youxi.cn/gtmpklwxfk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtprfwgkki.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.pycfn.com/gtovsazsjr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ehwqpu.com/gtbuomohwb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtezboqckd.html

[E06] 替换子串
来源：http://hz.yangfankeji.com/gtragmpyjf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.vqdsnc.cn/gttcbtdhtz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtrkujondu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtlueyywor.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtkplqxvgw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtorvpzqni.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.0kj1m.cn/gtrcesrjgj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cdnleiting.top/gtvpmuxpka.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gtbfpjpokg.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangkeji.top/gtxdsjckig.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daria6918.cn/gtbicfamey.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gttqueqexz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtbbuxoqrn.html

TS:   s.split(",")
来源：http://hz.jqgufenzy.top/gtaqriaqhk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gtadzzpvcp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtioyyoijd.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtdqkvlryj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cucudq.cn/gtehaafemm.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gtxisylafc.html

Py:   ",".join(items)
来源：http://hz.chenjidiqi.icu/gtbipolglz.html

PHP:  implode(",", $items);
来源：http://hz.zhixingplan.top/gtckdduprj.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtbcahowvn.html

TS:   items.join(",")
来源：http://hz.nwbrower.top/gtbxienoco.html

Java: String.join(",", items)
来源：http://hz.dashuyun.cn/gtsbtrsngg.html

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gthkzkphud.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtdrcpsguu.html

C#:   string.Join(",", items)
来源：http://hz.316326.xyz/gtanaviekg.html

[E09] 去除所有空白字符
来源：http://hz.9152youxi.cn/gtrlqasnox.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgufenzy.top/gtwpxoqpbp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cheryme.top/gtddezbjqi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtschynvpc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtyubyjdea.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtoxmaowqm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtdsifjsys.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtxmurmjuk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtrtnzsdcq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtkefpfdcc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gtnnwbieoy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuxming.cn/gtlndnhvcw.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gtpdsllyvk.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtpxgsyteb.html

Java: String.format("%03d", 7)
来源：http://hz.zhengqikj.top/gtmnmkjnoi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtjsdrmbgo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtgfpjqeoq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuanzx.com/gtropwsxef.html

[E11] 反转字符串
来源：http://hz.gaohongyu789.top/gtnyzlvujx.html

Py:   s[::-1]
来源：http://hz.xziqi.cn/gtmmroosjv.html

PHP:  strrev($s);
来源：http://hz.yueranfly.top/gtmetxhjiw.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtchfjbajm.html

TS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtzmazivlw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gttkgixvbw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sufxvd.cn/gtxgxhwknp.html

Ruby: s.reverse
来源：http://hz.jianghu66.top/gthdzydnpu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtebktzkas.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtgimvczqc.html

Py:   s.count("a")
来源：http://hz.aizwys.cn/gtfhlozsny.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtonarcdql.html

JS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtskgumguk.html

TS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtwaozbbhw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtmrqkqvyv.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtojggbwai.html

Ruby: s.count("a")
来源：http://hz.sysykeji.top/gthawjeagi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pengpengdd.cyou/gtfwytrwvi.html

[E13] 逐字符遍历
来源：http://hz.dashuyun.cn/gteyzhwskw.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtlbmtkksv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.snrcjt.cn/gtstaypcbf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fzhhl.top/gtlqixcstv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtvbqcvbam.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.quarkkingdee.top/gthpwskyhe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangshuangyany.cn/gtexkaddke.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtdaekyrro.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zycfv.cn/gtjyhztwel.html

[E14] URL 编码与 Base64
来源：http://hz.ivvv.top/gtfqvesmyp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hongshengwenyu.top/gtagmtemji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtjkncrddr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xylfe.cn/gtzwzphfsh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.c1oappe.top/gtxljtcczm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtgkaczcol.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gthxldcosh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangtech.top/gtnroppcvw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shangyingyoupin.top/gtzcgqwxkz.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhijiandao.cn/gtpnlcahhl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuanzhike.top/gtwtlbgfxr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gtqlxdwcyn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtthcsnunb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.kuanghao11.cn/gtqobeyvuz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangkeji.top/gtdtsaotff.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtsafwpbqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhengqikj.top/gtemfmyssc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtrduyntpl.html

[E16] 数字千分位
来源：http://hz.xuanzx.com/gtpjmvdltq.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtdvpjccfv.html

PHP:  number_format(1234567);
来源：http://hz.xinyue.icu/gtlqocasjg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtrgwukhrf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtyienvrpg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtpjwgzwcv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtzcnjdyip.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtbkynubla.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtsspuutmy.html

[E17] 首字母大写
来源：http://hz.chenlongwang.top/gtnxywgejw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtqzyliowf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtqpizqwqu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtdhiipple.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtzratxvyx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtxgzvlojm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xziqi.cn/gtwmtuzkjp.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtntffobzu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtydzvjxog.html

[E18] 模板占位符替换
来源：http://hz.sysykeji.top/gtbjjhzrtf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtnefndxee.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hongshengwenyu.top/gtbdydtkac.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gthnfrsgdq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtfgjjqjdq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xylfe.cn/gtesfwvpga.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnxiangtu.top/gtrawvdfvc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtmidfbfep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.andypj.xyz/gtzjmlthss.html

[E19] 多行文本按行拆分
来源：http://hz.jqgufenzy.top/gtbdohwmxx.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtbceovrid.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gtfupdgkke.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtwkodpqzc.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtpkgbqryb.html

Java: s.lines().toList()
来源：http://hz.gotoacloud.top/gtscngteon.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtotwcjarv.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtkzsstlwl.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtsusudkfw.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gtqodnpclw.html

Py:   if not s:
来源：http://hz.xziqi.cn/gtwzfrpppp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gtpnvdsduz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtdngaxqmz.html

TS:   if (s === "") {}
来源：http://hz.chenjidiqi.icu/gtukjpnakq.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtarwrfmoy.html

Go:   if s == "" {}
来源：http://hz.tanke756.top/gtivgpakzj.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gthcjdkbtk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xziqi.cn/gtuvmqhuxa.html

[E21] 超长截断加省略号
来源：http://hz.hongshengwenyu.top/gtfjacyoeb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gthqgdvmpv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhijiandao.cn/gtaclngdgx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtfjjpujbi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtnpsxbrlk.html


<!-- 参考信息 -->