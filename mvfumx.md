代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtzpeddoid.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gturtwcosb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtskylypin.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tianlin.xyz/gteqdtnlkc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigufen.top/gtgozyqlor.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtrvtgtqmc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.guowangkeji.top/gtdyrmwxtd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtvvlaabip.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtqyjtoeoq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtjkwhknvv.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtqowhhqcd.html

TS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtskrwhmxr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.havefunace.top/gtpdclslvm.html

Go:   // 手写循环
来源：http://hz.quarkkingdee.top/gtneenqgey.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtlilgdfgz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhiwuduotai.top/gtlgjygaga.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtxetgjuaq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtbofyrcys.html

PHP:  array_unique($arr);
来源：http://hz.gaohongyu789.top/gtsxufmidy.html

JS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtyqrpqypl.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtaeftvtzp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.andypj.xyz/gtmlrxibgd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.quarkkingdee.top/gtfwfyfhgn.html

Ruby: arr.uniq
来源：http://hz.ehwqpu.com/gtvbmowpbt.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxuanxn.top/gtqdjasgbu.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtsnjfihda.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtxgvzsqcr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cdnleiting.top/gtmnywuolg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gttwwijqpz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtybpypczc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jyoumei.cn/gtaolbrhxe.html

Go:   // 手写循环累加
来源：http://hz.sxryk.cn/gthhxbrlkd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tian-w.cn/gtospchqbw.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtkiwhfjag.html

[D17] 最大值与最小值
来源：http://hz.hysaishi.cn/gtnrjxnnvh.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtnsocfgpf.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtwttidtyc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtoxkmiprd.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangkeji.top/gtctftcszf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cqqwz.cn/gtusjvobfy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhijiandao.cn/gtovhyxzli.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtnxohhesp.html

C#:   list.Max();  list.Min()
来源：http://hz.havefunace.top/gtobnmcwlq.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtljngobns.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhengqikj.top/gtqqzqojll.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtdnmsorjt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtbrdtcrma.html

TS:   nested.flat();
来源：http://hz.ydzc1.top/gtrlnefqdm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.0kj1m.cn/gteubudglv.html

Go:   // 手写双层循环
来源：http://hz.zdqjudy.top/gtvalzhhdi.html

Ruby: nested.flatten
来源：http://hz.guannengcc.top/gtoxcvnwge.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.bjfxy.top/gtzjtzmsdg.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtppqaqjyc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xylfe.cn/gtlbubalnb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtwowevtqy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtonhggcjm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtsiujwena.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnxiangtu.top/gtabpuliyt.html

Go:   // 手写 map[string][]T
来源：http://hz.zhengqikj.top/gtqeczskqj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sysykeji.top/gtbguwpyna.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangshuangyany.cn/gttbnthuvd.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtgqnfmdxy.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gttkenypyb.html

PHP:  array_count_values($arr);
来源：http://hz.yuxming.cn/gtyrjwcyzs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtehvxlfrn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtofcloxeg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cashguo.top/gtztmkwjut.html

Go:   // 手写 map[T]int
来源：http://hz.gogol.net.cn/gtglmkpcho.html

Ruby: arr.tally
来源：http://hz.jinqigfzy.top/gtlkxoejcp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.52xcode.cn/gtcffapyoq.html

[D21] 判断是否包含某元素
来源：http://hz.tian-w.cn/gtkuzgsbbo.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtkmbzgkix.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gtcmlzkrmp.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtkpkcpwxf.html

TS:   arr.includes(x)
来源：http://hz.316326.xyz/gtwfzzoyqi.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtwfpvbkos.html

Go:   slices.Contains(arr, x)
来源：http://hz.316326.xyz/gtuqeesrdm.html

Ruby: arr.include?(x)
来源：http://hz.meibo888.top/gtgcyenvkz.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtosdbwfzk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhoulong.xyz/gtotaalieo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtrenaqncx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gttftllfvt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guowangkeji.top/gtwagckyvl.html

TS:   [...arr];
来源：http://hz.birdmap.top/gtdriehdor.html

Java: new ArrayList<>(list);
来源：http://hz.ehwqpu.com/gtjfwoleiz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtsflplfzx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gttomvxdpb.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gttsxigsbn.html

[D23] reduce 累积计算
来源：http://hz.xinyue.icu/gtjwonkrdw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtlwhiixrv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhixingplan.top/gtwaczkuwf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtirpsnjjg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtzjyzmqlu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtarwsmtse.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtoyancjgo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtqevbwwge.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangshuangyany.cn/gtpkxqvouh.html

[D24] 字典 / Map 基本操作
来源：http://hz.jianghu66.top/gtnjooyhqe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtquwmyocd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtlrkasgfq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yongpay.top/gtftysyshm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenlongwang.top/gtizckvspq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xylfe.cn/gtayvkzgmb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhijiandao.cn/gtgtobgryc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gzhubu.top/gtgkhlqqzn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtxqepolju.html

[D25] Set 集合去重与交并差
来源：http://hz.zhixingplan.top/gtzrfqdqbk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.c1oappe.top/gtxwujuqay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtwkbsfytx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtoyjznyzd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gtjvkievkd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gteemgzdhq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtgkjbofzv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydzc1.top/gtxnwkaqdz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangtech.top/gtscahgjso.html

[D26] 数组转字符串
来源：http://hz.pycfn.com/gtwtwgrlbh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtfiwiwidu.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gtjgfkujat.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtqdstezaz.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gttipjyznh.html

Java: String.join(", ", list)
来源：http://hz.havefunace.top/gtokcplwnx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtgxaldzvj.html

Ruby: arr.join(", ")
来源：http://hz.xuanzx.com/gtxqxjbwdf.html

C#:   string.Join(", ", list)
来源：http://hz.wangshuangyany.cn/gtkkququfj.html

================================================================================
来源：http://hz.jiagoushi.top/gtmfouwcgn.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtxcpndvcn.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzutmeqze.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtfjypiyaf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenjidiqi.icu/gtqlradoom.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtrqrgcwut.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtoaewwfqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtkcyjtoso.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtvqqthhlt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgufenzy.top/gtnzrheink.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigfzy.top/gtzeojfmph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangtech.top/gtjrceazcv.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gtzdowofgd.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtynpffplq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtmvkxfsrk.html

JS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gtfpjkbtdp.html

TS:   "ab".repeat(3)
来源：http://hz.yj20258888.top/gtubkbldaf.html

Java: "ab".repeat(3)
来源：http://hz.aibaodan.cn/gthqqaojkj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gtjgyguoyy.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtfqosihur.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gzhubu.top/gtowrashow.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtqdeqzxgn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtutjnmhil.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gtihjvqphm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtbaxgelon.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtvstfculr.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtcqbrovwi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtnbhivnoh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hongshengwenyu.top/gtyfdqismz.html

C#:   s.Substring(1, 3)
来源：http://hz.jianghu66.top/gttgwztpti.html

[E04] 查找子串位置
来源：http://hz.sweek.top/gtiwrddyor.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtikabuxlw.html

PHP:  strpos($s, "x");
来源：http://hz.sxryk.cn/gtlrzihggs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.mhx1999.top/gtlcpffjbj.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtsrcnjeup.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtviraacyh.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtmykkbrfg.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gticebnhxk.html

C#:   s.IndexOf("x")
来源：http://hz.daria6918.cn/gtlbcrpcif.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtlkaxunxo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydzc1.top/gtyiufqbnq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhoulong.xyz/gtliatakrs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtnnjrivvr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ivvv.top/gthrzudrhy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtxsxklrlv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinyuanbaomall.cn/gtnqydussq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenjidiqi.icu/gtazaxajnu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gtvpzecxqa.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtzrjmcscu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtlxaigyxs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydzc1.top/gtkbgxqbmg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtukxnevfq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtukjulepf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtxntoqvum.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtyuirgnxp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cqqwz.cn/gtqgmadijl.html

C#:   s.Replace("a", "b")
来源：http://hz.52xcode.cn/gtcewtvhxp.html

[E07] 按分隔符拆分
来源：http://hz.daxiang520.top/gtmbacdppd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtnvwbsare.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.havefunace.top/gtvbbaszyu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gtmaqtjcrh.html

TS:   s.split(",")
来源：http://hz.smart0.xyz/gtsisrizaj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gthilkmjxf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hfpthk.cn/gtatiyojmg.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtiimqdrob.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgufenzy.top/gtodsrcfik.html

[E08] 数组按分隔符合并
来源：http://hz.guannengcc.top/gtrmyutpiy.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtfijvakuo.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gtrtlbemum.html

JS:   items.join(",")
来源：http://hz.hysaishi.cn/gtvhpuuvek.html

TS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtsyapjkzq.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gtsegleahv.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtwhlmsrfl.html

Ruby: items.join(",")
来源：http://hz.zhijiandao.cn/gtjcqadwhe.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gthelwkskn.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gtxvfteexy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtagerkryq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.haohaochexian.top/gtzifhnodw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtgojektsz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtpmdowmot.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhoulong.xyz/gtirgudyzb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtdmbnbtxb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtqkvdblyn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtnyeohhbs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gtwoycvxem.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhiwuduotai.top/gtgxdeybxi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtydjjgrtc.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gthlpqhqkc.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtlcpbmtgk.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtkipwbzzj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.316326.xyz/gtlpqnemwr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gteyyiauzk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daria6918.cn/gtdmfpxkov.html

[E11] 反转字符串
来源：http://hz.nanxuanxn.top/gtrzirohda.html

Py:   s[::-1]
来源：http://hz.nanxinkj.top/gtpzinmjsk.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtykvxiqnl.html

JS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtfgqbgohc.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtbcaubysx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhijiandao.cn/gtctqzvmnb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pengpengdd.cyou/gtqywhrlxn.html

Ruby: s.reverse
来源：http://hz.svipenyu.cn/gtazxkdszh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtdwcbtmqx.html

[E12] 统计某字符出现次数
来源：http://hz.chenjidiqi.icu/gtyxpismmv.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gtecelwkna.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtbpazlcvs.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtlgmhxxrz.html

TS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtvgiftzlh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.snrcjt.cn/gtbarbexgs.html

Go:   strings.Count(s, "a")
来源：http://hz.sxryk.cn/gtrhhlhtkv.html

Ruby: s.count("a")
来源：http://hz.sxryk.cn/gtorbzihdz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangtech.top/gtlhvtgbpc.html

[E13] 逐字符遍历
来源：http://hz.birdmap.top/gtxipemeoi.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtrbnjamjy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shuidangran.top/gtksoidyuo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtlelurxlx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtuvvptfre.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.0kj1m.cn/gtankimypb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhongyouzk.top/gtimzcmupt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cheryme.top/gtyuxtlffa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zdqjudy.top/gtlkbupnez.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtbxcjjsvz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xziqi.cn/gtqtnzyrmj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhoulong.xyz/gtxgyaudtd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtnlmuvzjs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.52xcode.cn/gtlroiutyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daria6918.cn/gtoeqtkacn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangshuangyany.cn/gthbmriddj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtuwmzmqyb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shangyingyoupin.top/gtzipurlyp.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuanzx.com/gtffckpoky.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.52xcode.cn/gtdtcfxfcd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtzfkgjlgc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtkhzfedmd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hywenlv.cn/gtwahxqjac.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuxming.cn/gtweuhhblz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hywenlv.cn/gtfrebulht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtuxwnnobe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cucudq.cn/gthqiozdnr.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtdbxinmyu.html

Py:   f"{1234567:,}"
来源：http://hz.guowangkeji.top/gtkdiwtyhu.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtwncmqkum.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cdnleiting.top/gtubyicsrq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gthhjcnqur.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtrswesgut.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gtlbjeozxx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.andypj.xyz/gtdmwuiiix.html

C#:   1234567.ToString("N0")
来源：http://hz.aizwys.cn/gtccquohog.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtasckszcu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhiwuduotai.top/gthjtvqlwd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtpuwynzdz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtkrcyftgl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtswkmtbeu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.mhx1999.top/gtckmxgyhg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zycfv.cn/gtlberhkya.html

Ruby: s.capitalize
来源：http://hz.shzxlz.cn/gtumtbswyk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtjgawzgrm.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gteouqgldz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zycfv.cn/gtkwrxrruk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ehwqpu.com/gtnvdmeruf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtbnyplqeh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtsfalidpq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cdnleiting.top/gtgteoirfx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shuidangran.top/gtqjdutjed.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gttgxirihv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gthcfqixuk.html

[E19] 多行文本按行拆分
来源：http://hz.quarkkingdee.top/gtwwbjhkzq.html

Py:   s.splitlines()
来源：http://hz.zhengqikj.top/gtfobvyghy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtciaphzqe.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtmwyawmxu.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtgdqhesrs.html

Java: s.lines().toList()
来源：http://hz.sysykeji.top/gtlydasswi.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtnnonmghq.html

Ruby: s.lines
来源：http://hz.mhx1999.top/gttlrktshf.html

C#:   s.Split('\n')
来源：http://hz.316326.xyz/gtnmxjjahu.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtkfcqjrzv.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtylpssuuo.html


<!-- 参考信息 -->