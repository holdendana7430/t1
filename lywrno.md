代发 wailian999

Ruby: arr.index(x)
来源：http://hz.shanyushiyangkeji.top/gtwwvouduo.html

C#:   list.IndexOf(x);
来源：http://hz.xingfuxueyuan.xyz/gtojglwbly.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pycfn.com/gtpvxubgkz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinghuilouyu.cn/gtbtodalpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtjrngrixn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtkzeiiazt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtisxnxzzd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhengqikj.top/gttxisjzwy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fengsongda.top/gtowwnjmtl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tanke756.top/gtygcmvafz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtseukubuz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.svipenyu.cn/gtpjelrnxt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guowangkeji.top/gtgswmvdwe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guannengcc.top/gtyhctdwsd.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtvkvujndg.html

TS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtdedurrtd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ywan-chungtsiang.top/gtqzitcchx.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtspjteord.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtxhfjicuk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sxryk.cn/gtvinvykkx.html

[D15] 去重
来源：http://hz.hfpthk.cn/gtkazuspmq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtucmumvcw.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtjftsbnln.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtkargfqnd.html

TS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtdtxkfqjy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtqdckjshr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtuldqppub.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtwtephvwj.html

C#:   list.Distinct().ToList()
来源：http://hz.nwbrower.top/gtpfawtzqf.html

[D16] 求和与平均值
来源：http://hz.yj20258888.top/gtedetyhex.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtxxnapiqn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtcdrvoooj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtotetwkgt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtzpsijabp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtvkfjbyrh.html

Go:   // 手写循环累加
来源：http://hz.smart0.xyz/gthxxzbpci.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtlwijrjyv.html

C#:   list.Sum();  list.Average()
来源：http://hz.jianghu66.top/gtgtayycwt.html

[D17] 最大值与最小值
来源：http://hz.xingfuxueyuan.xyz/gtuqpwgyki.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtxorbejhb.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtcjxlsmsb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtxgpmzhhr.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gtvbclkneu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gtjysydwae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtlssnsexi.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtkulugrvp.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgfzy.top/gtxoycsahz.html

[D18] 扁平化嵌套数组
来源：http://hz.xziqi.cn/gtsxiknaxa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtzvsonzbc.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtefnqavfb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtwiupqzhv.html

TS:   nested.flat();
来源：http://hz.hfpthk.cn/gtwruxllte.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.feifeiyinyue.top/gtzfcixxbm.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtnpfghhnc.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtffrohddw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sysykeji.top/gteyymuyef.html

[D19] 按字段分组
来源：http://hz.tian-w.cn/gtfznrravu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtkfxyuums.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gthwkvmyis.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtbosgzhnx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtjxysfdks.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guannengcc.top/gtgyhfuupu.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gtwfgkrzys.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydzc1.top/gtnqavkqqu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtljggcigx.html

[D20] 统计每个元素出现次数
来源：http://hz.fengsongda.top/gtxpjcittb.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtydazogon.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258888.top/gtyqxsxhub.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtheddlber.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtdjujvocz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sysykeji.top/gtccwgfwos.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtpdhxyadp.html

Ruby: arr.tally
来源：http://hz.aibaodan.cn/gthkasocop.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtwfzneume.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtvsotmqxk.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtjxiwigiw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aizwys.cn/gtxjvwxgzr.html

JS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtznvtkquf.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtazfcdkgo.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtuxyqdbtk.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangshuangyany.cn/gtfiyiqtim.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtuljtqwws.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gtlrnjmofz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtybetkkkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuetiantiany.cn/gtdeyegvdy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtjwaynfkh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtbbeixutl.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtozrbybwy.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtuzmsyjsw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtbhnprskg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtzzrczxse.html

C#:   new List<int>(list);
来源：http://hz.c1oappe.top/gtidsrvojd.html

[D23] reduce 累积计算
来源：http://hz.aizwys.cn/gtnkduornl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tian-w.cn/gtqoxsckzu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtejtgnnlq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtodujudav.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtlyocnugd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.havefunace.top/gtaahmnpct.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gteqfaibvm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fengsongda.top/gtwopfgtda.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gotoacloud.top/gtfcqcmxsr.html

[D24] 字典 / Map 基本操作
来源：http://hz.snrcjt.cn/gtlpjyfooz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tian-w.cn/gtksachaph.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtiyhwzihy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtveavxqic.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtjawqxthn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258888.top/gtmxuvpapj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtvayshzxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shangyingyoupin.top/gtiraasglp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtddwiarpp.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtdqhyvlur.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenzaomai.com/gtatxybukj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cucudq.cn/gtmipxzwgi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shangyingyoupin.top/gthhhahlmx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuanzhike.top/gtmrjfschu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhaomingkeji.xyz/gtnhyyykfg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtfymajoug.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuanzhike.top/gtesvzrhai.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtelmawkdo.html

[D26] 数组转字符串
来源：http://hz.nanxinkj.top/gtbpnrxbws.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtifbanzyz.html

PHP:  implode(", ", $arr);
来源：http://hz.havefunace.top/gtdrxhjpmh.html

JS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtdyydbsrf.html

TS:   arr.join(", ")
来源：http://hz.hammf.cn/gtksxqdbta.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtjiljvuqd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtzlfiiaep.html

Ruby: arr.join(", ")
来源：http://hz.ehwqpu.com/gtbktiqlyg.html

C#:   string.Join(", ", list)
来源：http://hz.sweek.top/gtvyaifyoh.html

================================================================================
来源：http://hz.tian-w.cn/gtgmonsizx.html

E. 字符串处理
来源：http://hz.jianghu66.top/gtxigwkfec.html

================================================================================
来源：http://hz.nanxinkj.top/gtppuerwnv.html

[E01] 拼接字符串
来源：http://hz.havefunace.top/gtvkwllvvk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydzc1.top/gthffzwknb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gthwmbhcfr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtwsevrysy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtncrorzco.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cqqwz.cn/gtzqkgwrst.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhoulong.xyz/gtltdivgcd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtzsuvybzl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cdnleiting.top/gtdyskuylp.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtdvmkglqc.html

Py:   "ab" * 3
来源：http://hz.jqgfzy.top/gtwwusfluw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhaomingkeji.xyz/gtcowuwkgp.html

JS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtglsqwovi.html

TS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtfnswqxog.html

Java: "ab".repeat(3)
来源：http://hz.sweek.top/gtpjxtiniq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hammf.cn/gtymznfdjn.html

Ruby: "ab" * 3
来源：http://hz.nwbrower.top/gtwwyjqpdz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtnxjrgbgc.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtgczphrzu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtbdwtrzro.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtnkvtfzpn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtsloyhwvn.html

TS:   s.slice(1, 4)
来源：http://hz.zhengqikj.top/gtdzrkajbs.html

Java: s.substring(1, 4)
来源：http://hz.yj20258.top/gtabocemao.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gotoacloud.top/gthxqkbpuh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gtkqpjordv.html

C#:   s.Substring(1, 3)
来源：http://hz.mhx1999.top/gtfdlklial.html

[E04] 查找子串位置
来源：http://hz.fengsongda.top/gtubraxgmd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhiwuduotai.top/gtpoqmchcs.html

PHP:  strpos($s, "x");
来源：http://hz.ydzc1.top/gtxjhhcdul.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxuanxn.top/gtwwqkcjcy.html

TS:   s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtfkrbbdmb.html

Java: s.indexOf("x")
来源：http://hz.jianghu66.top/gtmsetnoup.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gttfadfmdt.html

Ruby: s.index("x")
来源：http://hz.zhongyouzk.top/gtbfrcwkal.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtbpjgxcdz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydzc1.top/gtfcxqeusy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ivvv.top/gtjpfpatme.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangshuangyany.cn/gtdwgnkkai.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangdashe.top/gtqgieyeyg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.316326.xyz/gtlfpracxt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtkaipsqej.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhongyouzk.top/gtjilyvbjb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenzaomai.com/gtwgwqrfqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgufenzy.top/gtqiypqhpo.html

[E06] 替换子串
来源：http://hz.hammf.cn/gtfddteasl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sxryk.cn/gtqnbtenry.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtjbgemxme.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtyrevujfi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gttohajhgs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtntbkfjqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtskxvailk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtwjvqjwln.html

C#:   s.Replace("a", "b")
来源：http://hz.ivvv.top/gtoojehqaf.html

[E07] 按分隔符拆分
来源：http://hz.snrcjt.cn/gtkzwezfus.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtksdjxgnv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dianchejie.cn/gtcawqubmo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.vqdsnc.cn/gtwtjcwdbi.html

TS:   s.split(",")
来源：http://hz.andypj.xyz/gtkpohvdxq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aizwys.cn/gtutxpeuyq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtarxwvygw.html

Ruby: s.split(",");  s.split
来源：http://hz.hfpthk.cn/gtpiqtgghy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daxiang520.top/gtlucpvktv.html

[E08] 数组按分隔符合并
来源：http://hz.feifeiyinyue.top/gtwvfixlqf.html

Py:   ",".join(items)
来源：http://hz.andypj.xyz/gtdtispuee.html

PHP:  implode(",", $items);
来源：http://hz.yueranfly.top/gtxverkvcc.html

JS:   items.join(",")
来源：http://hz.iojbl.cn/gtljjwtchi.html

TS:   items.join(",")
来源：http://hz.redwolf501.top/gtqtdlrokl.html

Java: String.join(",", items)
来源：http://hz.hywenlv.cn/gtezoxyweg.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gtzbbsvcmd.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gtmcouiksu.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtyncshdzb.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtkxmppoza.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtfjiczmyl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinyuanbaomall.cn/gtdujqbbeq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtoltnngoo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtnvgnvwow.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtawuvzgrw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gotoacloud.top/gtrbigwbxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtfnxnmlmu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangshuangyany.cn/gtvornvfxt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.iojbl.cn/gtqrftnfdh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtgkpetpsc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtjuhibvxk.html

JS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtjhoefwid.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gthdaxudeo.html

Java: String.format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtnqhguaxp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtisttxawi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.52xcode.cn/gtluwjiwcn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gotoacloud.top/gttdvwtqiq.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtijcyjmnn.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtjjpsqcif.html

PHP:  strrev($s);
来源：http://hz.yj202588.top/gtqlxbcemw.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtudqlcbro.html

TS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtcjheyotc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hfpthk.cn/gtpvtcezig.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtwmcqxbnm.html

Ruby: s.reverse
来源：http://hz.c1oappe.top/gtjkkwnape.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtvqlzcwbw.html

[E12] 统计某字符出现次数
来源：http://hz.guannengcc.top/gtsevpqrxz.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtrndnfjqa.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxuanxn.top/gtieyosevi.html

JS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtzuzbdtuj.html

TS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtqxinygad.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtaohubpwo.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtvilorpwz.html

Ruby: s.count("a")
来源：http://hz.birdmap.top/gttgfointu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daxiang520.top/gthuhslxdt.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gteziljfxo.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtseegnhhz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydzc1.top/gtelyuowph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtlpomqkek.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtucmexeob.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtvfcgshfb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jianghu66.top/gtehxmzbbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtyrscsvpc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtusiqqpku.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtuwgqfiib.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gtlghidsge.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nwbrower.top/gthavrrajx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gtgqzduwsy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gtgbkmfgbv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yueranfly.top/gtkpubhdbi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ywan-chungtsiang.top/gtaferpjgh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258888.top/gtqftmlrmx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtpqxdlylf.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtrzwhoijm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xziqi.cn/gtwizzuqeu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtzhnzxwel.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.c1oappe.top/gtgvksjgdr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtrxxviitz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cdnleiting.top/gtpikusueo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtyalbmvtt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtzvnahxmc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtuatveqlq.html

[E16] 数字千分位
来源：http://hz.zhengqikj.top/gtmuccvpwq.html

Py:   f"{1234567:,}"
来源：http://hz.chenlongwang.top/gtoeogzjat.html

PHP:  number_format(1234567);
来源：http://hz.ybcxt.top/gtaqvyirse.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtjalmwwbl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtcogenkkf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.316326.xyz/gtbsmaiknh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.snrcjt.cn/gtmtdibkmm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinghuilouyu.cn/gtdewmvilr.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtsxtvxrkn.html

[E17] 首字母大写
来源：http://hz.yanxiufei.cn/gtihbsbusr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.vqdsnc.cn/gtxdfhoewb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gtmuukmclg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gthqmffnmm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtdawbjuul.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zdqjudy.top/gtytxhynnj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tianlin.xyz/gtugjaezsv.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gttqwigjmn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gtljzimhvu.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtkeypwneo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtznbfyhah.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtbjkpqygt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtkqrimisz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gtrhwwwvbe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhixingplan.top/gtjpfdhflq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtooxzuqqp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtlbbybymr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gtyibnvwys.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtnqdxxitm.html

Py:   s.splitlines()
来源：http://hz.52xcode.cn/gtzqspowjw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtymhymvhz.html

JS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtkjxtqbqp.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtmtxmqpgk.html

Java: s.lines().toList()
来源：http://hz.shzxlz.cn/gtqgzqkgua.html

Go:   strings.Split(s, "\n")
来源：http://hz.ppjwa.cn/gtsdwsqeif.html


<!-- 参考信息 -->