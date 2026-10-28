代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhijiandao.cn/gtuqwbzqxw.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtdrmlnwjw.html

C#:   list.Max();  list.Min()
来源：http://hz.fzhhl.top/gtqmxjyzde.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gteoeqfuam.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhijiandao.cn/gtxmvgmxre.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtkdnjfzum.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtdsufuccs.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtmbpywais.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtdledypov.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtibminhjz.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtrobhdjey.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxuanxn.top/gtcevxfhoo.html

[D19] 按字段分组
来源：http://hz.jianghu66.top/gttzwnbcvm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yonumen.top/gtfhajpwxr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtgqyklree.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtqtnlkbzr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gtzxqjgccv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtzeefcuia.html

Go:   // 手写 map[string][]T
来源：http://hz.ywan-chungtsiang.top/gtjpsoqpzd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtotarmjly.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgfzy.top/gtsdlyozsb.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtafjeorzo.html

Py:   Counter(arr)
来源：http://hz.ydzc1.top/gtdiquqwwr.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtnerkding.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gthokizsaw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtvrhlkxfa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.snrcjt.cn/gtimeslneh.html

Go:   // 手写 map[T]int
来源：http://hz.iojbl.cn/gtxtzutmmb.html

Ruby: arr.tally
来源：http://hz.tianlin.xyz/gtksquzljz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.redwolf501.top/gtwlbvbent.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtpcltauyo.html

Py:   x in arr
来源：http://hz.daria6918.cn/gtfcmkkaec.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gtxosbkzhh.html

JS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtyqzhmfwf.html

TS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtefrxskpb.html

Java: list.contains(x)
来源：http://hz.jinqigufen.top/gtlidseyxv.html

Go:   slices.Contains(arr, x)
来源：http://hz.mhx1999.top/gtgrwxdfkh.html

Ruby: arr.include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtizkflmna.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtpxuzuctk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hysaishi.cn/gteuajzfut.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtukltgrfz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuanzx.com/gtqpsebzbq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtasictmju.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtvgweftbx.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtqjcwnnam.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gthhpwxhlg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.meibo888.top/gtsjvigsge.html

C#:   new List<int>(list);
来源：http://hz.yongpay.top/gtvxupmknt.html

[D23] reduce 累积计算
来源：http://hz.cheryme.top/gtzvoflggc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ivvv.top/gtmmejnpey.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.9152youxi.cn/gtjvyknuqu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtqrealinp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtgmeprjpo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.bjfxy.top/gtemhcupbe.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtyrupemgx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fengsongda.top/gtcjxiqbpp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zdqjudy.top/gtgnjoonsp.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gtpchwvfow.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guowangkeji.top/gtyzefsxos.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zdqjudy.top/gtziukrkmk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinghuilouyu.cn/gtacvgpulu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hywenlv.cn/gtbsvnnksv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.aizwys.cn/gtoaqubnnh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtxqpuztms.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtznfwnmsu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtkednkiwa.html

[D25] Set 集合去重与交并差
来源：http://hz.hongshengwenyu.top/gtuyljxrhr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tianlin.xyz/gtldwgyjim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtiuozhqye.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtvtxuzckc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.redwolf501.top/gtwhazszja.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtfcqeyflb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtzaedfydt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.guannengcc.top/gtdvqxfqek.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gotoacloud.top/gtxxzimsef.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtyaqzeilw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtuvhjdowa.html

PHP:  implode(", ", $arr);
来源：http://hz.jinghuilouyu.cn/gtfnptlsle.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtvqefguax.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtqijwsjgp.html

Java: String.join(", ", list)
来源：http://hz.yuxming.cn/gtosflutjb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gtidgxjcbd.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtaapycvby.html

C#:   string.Join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtqbnebtzk.html

================================================================================
来源：http://hz.ydzc1.top/gtviderwgt.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtkmrondnb.html

================================================================================
来源：http://hz.yonumen.top/gtbirrqyiy.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtmowpjxcl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtcmuzrmpt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtnshfwskx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtxjghmqiu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtkywkscgd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nwbrower.top/gtpaixxtcg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtorbkuenb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gtxagdzwnl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cucudq.cn/gtawsapdug.html

[E02] 重复字符串
来源：http://hz.yueranfly.top/gtbxelpdri.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtbralkriu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.vqdsnc.cn/gtgcllbntt.html

JS:   "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtuvkpkuzu.html

TS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtsadwulog.html

Java: "ab".repeat(3)
来源：http://hz.andypj.xyz/gtuzkkgrtk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gtazirbsva.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gtxnugldaa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtbqpfjgsz.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtozpmwzxi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xinyue.icu/gtrqignyni.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtutrkzbjh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtkwkbnnzu.html

TS:   s.slice(1, 4)
来源：http://hz.xylfe.cn/gtmaxumygr.html

Java: s.substring(1, 4)
来源：http://hz.tian-w.cn/gthqaaqzfm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuxming.cn/gtzovhetuc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtmdimxgep.html

C#:   s.Substring(1, 3)
来源：http://hz.kuanghao11.cn/gtdqmrrfyl.html

[E04] 查找子串位置
来源：http://hz.zhaomingkeji.xyz/gtkcrszypi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sweek.top/gtyhllmzwg.html

PHP:  strpos($s, "x");
来源：http://hz.zhiwuduotai.top/gtxtrhhdhu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtumzmxzed.html

TS:   s.indexOf("x")
来源：http://hz.yonumen.top/gtrldkdwtz.html

Java: s.indexOf("x")
来源：http://hz.yongpay.top/gtwkdvavft.html

Go:   strings.Index(s, "x")
来源：http://hz.gzhubu.top/gtljgtflzw.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtxnaaffzg.html

C#:   s.IndexOf("x")
来源：http://hz.316326.xyz/gthkwsowgn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cashguo.top/gtfzwzdjmw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hongshengwenyu.top/gtuxzqhkhe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ehwqpu.com/gtrpwdetkz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gteednsjja.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.redwolf501.top/gtrfdegeqp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtbghpjxiz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fengsongda.top/gtanqnrijt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jianghu66.top/gtknbtaogv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cqqwz.cn/gtsufceouk.html

[E06] 替换子串
来源：http://hz.yongpay.top/gtixrpnsdn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.mhx1999.top/gtpbzzvowx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtmofoeftv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtiabodcgx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtadiraaaj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtcpxdzpzc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtkvyurpyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guowangkeji.top/gtzrspkexj.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gttrvhjjjg.html

[E07] 按分隔符拆分
来源：http://hz.zhixingplan.top/gtdtkmxjmi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.smart0.xyz/gtoolgiqyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtoztzpisa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinqigufen.top/gtlhkcaxbg.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtxjdtkjbs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zycfv.cn/gtrzdmqxsy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtclpwtdvo.html

Ruby: s.split(",");  s.split
来源：http://hz.nwbrower.top/gtpobrqnjn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhoulong.xyz/gtgdcakqgp.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtyjeckyce.html

Py:   ",".join(items)
来源：http://hz.fengsongda.top/gtmrwxkihe.html

PHP:  implode(",", $items);
来源：http://hz.smart0.xyz/gtsmbmuuwa.html

JS:   items.join(",")
来源：http://hz.316326.xyz/gtyyqgjkyh.html

TS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtpeoiklle.html

Java: String.join(",", items)
来源：http://hz.zhengqikj.top/gtnefdrsdi.html

Go:   strings.Join(items, ",")
来源：http://hz.hnqzz.top/gtoihheber.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtnpjssaqp.html

C#:   string.Join(",", items)
来源：http://hz.yj202588.top/gtndaixala.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtrtxylpjm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gtoumoawwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gtlzkmrcbh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtdgdshrxs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtqlkfbjyl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gteljfrywd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gtrgmtnbkg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.meibo888.top/gtclydeous.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.meibo888.top/gtpfxairzh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gttofklzgr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.feifeiyinyue.top/gtkpqacgfh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hysaishi.cn/gtkzjwhcyn.html

JS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtycqvrsqm.html

TS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gttmcrzmae.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtfcdhjyvw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gteghpzbpe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gttzbiheia.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gtfmrkqhiu.html

[E11] 反转字符串
来源：http://hz.dianchejie.cn/gtqkuuluxv.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtsqfxlawk.html

PHP:  strrev($s);
来源：http://hz.nwbrower.top/gtulesktzm.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtkzxhmoaj.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtzaspxcdw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangdashe.top/gtowmcrdym.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gtyugcnymq.html

Ruby: s.reverse
来源：http://hz.guannengcc.top/gtxwcdtilu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtxyebetwj.html

[E12] 统计某字符出现次数
来源：http://hz.jiagoushi.top/gtnbufjfub.html

Py:   s.count("a")
来源：http://hz.zhoulong.xyz/gtkfyvsrhq.html

PHP:  substr_count($s, "a");
来源：http://hz.hywenlv.cn/gtadrcpmke.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtnyikujvt.html

TS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gthhpmbklh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ehwqpu.com/gtfrzfqjlk.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtehotrqze.html

Ruby: s.count("a")
来源：http://hz.hywenlv.cn/gtipkuwama.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gzhubu.top/gtjzkwkvif.html

[E13] 逐字符遍历
来源：http://hz.xinyue.icu/gtxkdgqmpb.html

Py:   for ch in s: print(ch)
来源：http://hz.yj202588.top/gtxndprobb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangshuangyany.cn/gtjptnmigd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtshuqyvqj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtzrhuhkpy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtbcecoqfi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtstxrnnhe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yangfankeji.com/gtxbsonbpe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.meibo888.top/gtqwtgzqyq.html

[E14] URL 编码与 Base64
来源：http://hz.zhongyouzk.top/gtzsymxrjm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.snrcjt.cn/gtgwnbfxdf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gtagnqumxh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tanke756.top/gtwcvjtuzc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtumqnmgcd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtwnzrbhvf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.andypj.xyz/gtgzihigjz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtihxutsak.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgufenzy.top/gtgtzcmgjh.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gthgsgfloz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gtxskpttqs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sysykeji.top/gtmobrjunh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xinyue.icu/gtfjyteakb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtcrxhzdyi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtnoiigzfq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gthtrbxofd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangtech.top/gtgpdnmqfl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xziqi.cn/gtffvskswi.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtdzhxhhcy.html

Py:   f"{1234567:,}"
来源：http://hz.shzxlz.cn/gtauroeaki.html

PHP:  number_format(1234567);
来源：http://hz.hnqzz.top/gttulzztjw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtyrdmeeza.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtklhykbih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ybcxt.top/gtuvurdgwf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtbaaitnod.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hongshengwenyu.top/gtxmqrzenz.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtkgzzuuwn.html

[E17] 首字母大写
来源：http://hz.xingfuxueyuan.xyz/gtqspcaoil.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtaueqqmnw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangdashe.top/gtnithmwya.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtsgrjypml.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtgxchiqdu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtvoxuvgvm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nwbrower.top/gtqtqltsob.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtrislnazc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.52xcode.cn/gtrlnmsilf.html

[E18] 模板占位符替换
来源：http://hz.bjfxy.top/gtqigbguzy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ivvv.top/gtkitrmidy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pengpengdd.cyou/gtmmxtqfpl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtehwihajr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gttfqfmvyw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.havefunace.top/gtkembktux.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gtuqgmfowr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xziqi.cn/gtkinjmrwi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtpfgxiuzk.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtkdfrazkh.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtlthqmgjj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhongyouzk.top/gtwvummibh.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtcfbiwsic.html

TS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtoormqjep.html

Java: s.lines().toList()
来源：http://hz.nanxinkj.top/gtspkykrbv.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtttdgsrpz.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtqtwkilby.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gtcpovwmie.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtpkltziyd.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtdnldmruw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hammf.cn/gtqqyftwce.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtsylwlaez.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gtnwljukiq.html

Java: if (s.isEmpty()) {}
来源：http://hz.cashguo.top/gtjcphzjvl.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtyloikekr.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtchcmkavg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangshuangyany.cn/gtwnvfddcu.html

[E21] 超长截断加省略号
来源：http://hz.316326.xyz/gtenlxjozr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtggijrnwz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtbssqtota.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtqmumjaqd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtyjolgkbh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtrrvvfiso.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cucudq.cn/gthegohawx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9152youxi.cn/gtcoqipdyf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtpgcpiqkc.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtcrqvjibx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtzyweamge.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtwvdqqhbc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtznlmbusa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtgmlcjbcn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtdxfhfsgd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtkpydgvnq.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtjsmgzeme.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xinyue.icu/gtaakyotui.html

================================================================================
来源：http://hz.jqgfzy.top/gtondzjtyu.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtllvxbzbg.html

================================================================================
来源：http://hz.cdnleiting.top/gtgfcpikvn.html

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtdacshbiw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtbjawsqfi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinghuilouyu.cn/gtgbzjzzzj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.quarkkingdee.top/gtgdsykuqj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtbybpgwst.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtvugzqlys.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtbchatnwh.html

Ruby: File.read("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtihzoymby.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cashguo.top/gtgpmbgvcg.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtunuxhbwa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pengpengdd.cyou/gtupryparo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtsaflzibs.html


<!-- 参考信息 -->