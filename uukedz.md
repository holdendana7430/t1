代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gtqftohmiq.html

[D16] 求和与平均值
来源：http://hz.iojbl.cn/gtwewwiapg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ywan-chungtsiang.top/gtpekzlpqd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtawebxxsl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtkinvtkzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtggftxmor.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtiqivariu.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gttapxvnls.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtrvfbbyul.html

C#:   list.Sum();  list.Average()
来源：http://hz.daria6918.cn/gtkbibmwzh.html

[D17] 最大值与最小值
来源：http://hz.pycfn.com/gtmrakonvh.html

Py:   max(arr);  min(arr)
来源：http://hz.dashuyun.cn/gtpyjnsxjg.html

PHP:  max($arr);  min($arr);
来源：http://hz.hywenlv.cn/gtvqoijwyb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daria6918.cn/gtmkfwwgsq.html

TS:   Math.max(...arr);
来源：http://hz.52xcode.cn/gtqnevawzw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.kuanghao11.cn/gtkqlcpsrh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtvxzfqyfy.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtzdszzhge.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtoejxlyjc.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtenoxefkl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cheryme.top/gtvdfqavmo.html

PHP:  array_merge(...$nested);
来源：http://hz.svipenyu.cn/gtlcvhajcs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuanzhike.top/gtbmmszcvd.html

TS:   nested.flat();
来源：http://hz.tian-w.cn/gtixcbzuya.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gtlvwcnago.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gtvuhciqwt.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtfmsjpzbk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtjqguaauz.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtgforytmr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydzc1.top/gtnqbswctm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinghuilouyu.cn/gtihfvdplj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sysykeji.top/gtcdrbmupg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gthsiyhgqm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtbhcibxgy.html

Go:   // 手写 map[string][]T
来源：http://hz.xingfuxueyuan.xyz/gtdfogxbmj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gteyfgafnv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gtgfdaihfj.html

[D20] 统计每个元素出现次数
来源：http://hz.yanxiufei.cn/gtloqcfvaa.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtbeftytqz.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gttylxxcrr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtgebmlhto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtxzyyxyvp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gtwyjuysqo.html

Go:   // 手写 map[T]int
来源：http://hz.aibaodan.cn/gtftglxddj.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtuiyfedcf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gttxflttdp.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtvtqbhzxt.html

Py:   x in arr
来源：http://hz.shanyushiyangtech.top/gtxyspbivd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtgsobtael.html

JS:   arr.includes(x)
来源：http://hz.wangshuangyany.cn/gtbxwpdgjl.html

TS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtfgwldjsk.html

Java: list.contains(x)
来源：http://hz.xinyue.icu/gtsvhzrfsj.html

Go:   slices.Contains(arr, x)
来源：http://hz.52xcode.cn/gtsnjizyqo.html

Ruby: arr.include?(x)
来源：http://hz.ivvv.top/gtciuarxcg.html

C#:   list.Contains(x)
来源：http://hz.52xcode.cn/gtqsvbqpog.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtdkptzvqv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.svipenyu.cn/gtnlukteud.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gtrtfxpmff.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtdvgrdhur.html

TS:   [...arr];
来源：http://hz.ivvv.top/gtxgvrdbwj.html

Java: new ArrayList<>(list);
来源：http://hz.ywan-chungtsiang.top/gtqpkedxdq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.wangshuangyany.cn/gtbuusmydh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guannengcc.top/gtvztvrzjf.html

C#:   new List<int>(list);
来源：http://hz.hfpthk.cn/gtdzgfmwsu.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gtscwysjac.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.316326.xyz/gtakxyebmv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtimnunmws.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtgtpiwotg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gogol.net.cn/gtegcwzkbt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtlcmuqcjm.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtmgoztkty.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtsvanvayg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gthqfottor.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtcvcajeyx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangkeji.top/gtcdeweusq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jlsjyb.cn/gtuqdrdcgy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gttsanhuyh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtknprexye.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gttzpopkgn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhiwuduotai.top/gtpcmulany.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xingfuxueyuan.xyz/gtlehclxoe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenzaomai.com/gtoaboewsl.html

[D25] Set 集合去重与交并差
来源：http://hz.daria6918.cn/gtyzbtstdh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtepduizro.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtnuglpeiu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigufen.top/gtiefmcrcq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guannengcc.top/gtctcqxwyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tian-w.cn/gtyetmkkwv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.kuanghao11.cn/gtpfxdvxsq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gtnteurxnc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.vqdsnc.cn/gtapnmskox.html

[D26] 数组转字符串
来源：http://hz.cucudq.cn/gtekbotmjm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtyyzklwcr.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtcuyhxwzw.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtevpmyiwn.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtacgbhlmy.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtkpyogorg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jianghu66.top/gtymltubuo.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtaqqnwdce.html

C#:   string.Join(", ", list)
来源：http://hz.yueranfly.top/gtporvxewp.html

================================================================================
来源：http://hz.gogol.net.cn/gtesuhyrsx.html

E. 字符串处理
来源：http://hz.tianlin.xyz/gteyopgrdi.html

================================================================================
来源：http://hz.cucudq.cn/gtrmnrihce.html

[E01] 拼接字符串
来源：http://hz.zhongyouzk.top/gtqtskdlib.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinghuilouyu.cn/gtdlfjinkx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtvlijuvce.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtsvwvmpug.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtcjderdka.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj20258.top/gtdndkfsbz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.316326.xyz/gtijjgpain.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gtzgvbxsnc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhongyouzk.top/gtvlywsckg.html

[E02] 重复字符串
来源：http://hz.yj20258.top/gttedlwshq.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gteveqodqo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gtkjksgcqy.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gttsshvubs.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtcvhrnfob.html

Java: "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtxxjnctdc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtkukvjysu.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gttnthzubd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.meibo888.top/gttnhuhxzx.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtzzgwqgwz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangtech.top/gtsthhyjyx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtqyoufatb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sysykeji.top/gtcqhfkzmv.html

TS:   s.slice(1, 4)
来源：http://hz.redwolf501.top/gtsaheeknm.html

Java: s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtkdahvpob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gtvhnjbmjh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.andypj.xyz/gtzumxivqa.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtodhuemih.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtjtkmxwzq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yonumen.top/gtoydtkteo.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtiuifiwuy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtimsolamn.html

TS:   s.indexOf("x")
来源：http://hz.cashguo.top/gtqeptbosy.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtfzyhvlyn.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtsmxueibw.html

Ruby: s.index("x")
来源：http://hz.sweek.top/gtizbndmwp.html

C#:   s.IndexOf("x")
来源：http://hz.andypj.xyz/gtuajmbqbp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xylfe.cn/gtdqajcide.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sysykeji.top/gtipbmofwv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gtmqlckqqy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtejlcfijj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yvedp.cn/gtdjlslbtf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtmtrhoaqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.haohaochexian.top/gtmghacfdg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258.top/gtqqhpiufj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxinkj.top/gttdvlwlgc.html

[E06] 替换子串
来源：http://hz.xylfe.cn/gtiozeoacp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xziqi.cn/gthdieqdoe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.smart0.xyz/gtpzrwjkze.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtqugydhiw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtwsbzhzlo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtzbkuzbuo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.0kj1m.cn/gthseqsgdb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ybcxt.top/gtipdbpqpm.html

C#:   s.Replace("a", "b")
来源：http://hz.sufxvd.cn/gtgwzoyefh.html

[E07] 按分隔符拆分
来源：http://hz.pycfn.com/gtufgzytxe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgufenzy.top/gtxavkycgt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtjexjlivf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ehwqpu.com/gtsropcbep.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtyrrmrgww.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtxpooszvc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tianlin.xyz/gtrowcfjzm.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtnwwcvfjd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtceejiwzj.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtqofhrkul.html

Py:   ",".join(items)
来源：http://hz.c1oappe.top/gtigeekhha.html

PHP:  implode(",", $items);
来源：http://hz.ydjk.org.cn/gtlwirvcoz.html

JS:   items.join(",")
来源：http://hz.hfpthk.cn/gtnlwmhpur.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtyapiygrl.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtplhfnucn.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtxneqmeir.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gtqxkloojo.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtegzzcrmd.html

[E09] 去除所有空白字符
来源：http://hz.zhoulong.xyz/gtzwsoqrpg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuxming.cn/gtuqpswhjj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sxryk.cn/gtfvewvmyu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gthutuqvyv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gtiedkxrpj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cashguo.top/gtyoxoslvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtzkoyesir.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gaohongyu789.top/gtkfdejedo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zdqjudy.top/gtsxxfgnny.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gtvdtbdfjd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtdkeqntwf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gttsdfsocb.html

JS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtmhbtylqn.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtskyaszqk.html

Java: String.format("%03d", 7)
来源：http://hz.xinyue.icu/gtchtrnuav.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtclubrecn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtfklkqgug.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xinyue.icu/gtbrdwqmxu.html

[E11] 反转字符串
来源：http://hz.gogol.net.cn/gtyuwkzkym.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtluimlxma.html

PHP:  strrev($s);
来源：http://hz.yj20258888.top/gtrgvnfevz.html

JS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtubvhecfo.html

TS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtgdghbwma.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenzaomai.com/gtfegodqpa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gtuwpzllno.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtwnhdjhel.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtunifjjeh.html

[E12] 统计某字符出现次数
来源：http://hz.sweek.top/gtiaptdnih.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gthijictew.html

PHP:  substr_count($s, "a");
来源：http://hz.sweek.top/gthtmnyldz.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtrsbxmjzt.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtrnunynmh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.0kj1m.cn/gtofkynvyg.html

Go:   strings.Count(s, "a")
来源：http://hz.hongshengwenyu.top/gtjtgzjrih.html

Ruby: s.count("a")
来源：http://hz.chenzaomai.com/gtzpjpswgq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtyzcqlzua.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtwgbijxhc.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgufenzy.top/gthvagiqvx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gttbfjjdyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtmxnzaomn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtumxemffj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtwplyvvse.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtehodrdzy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daria6918.cn/gtgeyshasc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtvmetuzor.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtcunciefs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxuanxn.top/gtkgcoxknk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtdlibjjqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gttbahhcio.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhaomingkeji.xyz/gtuofbhzrm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sufxvd.cn/gtrwawsivf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jlsjyb.cn/gtudzyatcw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnqzz.top/gtvbyqtmop.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhaomingkeji.xyz/gtoxpmznbk.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtywkykhzq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zdqjudy.top/gtlrqtqtaj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhaomingkeji.xyz/gtqqqecqug.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhixingplan.top/gtbkelojzc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinghuilouyu.cn/gtvolqcdzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtiejhppkj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.meibo888.top/gtknkiwhtt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhixingplan.top/gtkzwvboxe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinghuilouyu.cn/gtbtxwyews.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtwmwwilnr.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtcsmlyduj.html

PHP:  number_format(1234567);
来源：http://hz.nanxinkj.top/gtzfglvkqv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtxiajudph.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtuezvextq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cashguo.top/gtgybksang.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtmjxrxity.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtzkfovmbn.html

C#:   1234567.ToString("N0")
来源：http://hz.yuanzhike.top/gtfllbydwj.html

[E17] 首字母大写
来源：http://hz.andypj.xyz/gtkeorfdmt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dashuyun.cn/gtedreoyrb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gttorwbnmq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtrugelpxc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtqobwhshf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtqsmxrkoa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ybcxt.top/gtufujcwqe.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtwsbqhggr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtaiiuschf.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtfrjujgci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxuanxn.top/gtpamhrtsj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gzhubu.top/gtwnypdxdy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtvdtkvfbs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gthurepgvy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gttgzapsez.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daxiang520.top/gttsmekuul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dianchejie.cn/gtaxzisrym.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtadzpbgnz.html

[E19] 多行文本按行拆分
来源：http://hz.yanxiufei.cn/gtquvuuqbi.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtiibmieyp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yangfankeji.com/gtrdapdeqs.html

JS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gthlbvgezt.html

TS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtchrclyck.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtlqfkbhlj.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gtozrzearc.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtonprsadc.html

C#:   s.Split('\n')
来源：http://hz.xinyue.icu/gtbkikxqvb.html

[E20] 判断字符串是否为空
来源：http://hz.nanxinkj.top/gtloduxmow.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gtvvrxgtrq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtyhxjkmgn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gtefavbwjy.html

TS:   if (s === "") {}
来源：http://hz.hnxiangtu.top/gttqmsomyr.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtjhntburl.html

Go:   if s == "" {}
来源：http://hz.ivvv.top/gtopascryg.html

Ruby: if s.empty?
来源：http://hz.cdnleiting.top/gtzjugtxzk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtgyxqdgfr.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gtfjivlkqx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtymsnufom.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtvutmouln.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtlpnbhmjt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtykepeshh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtabninfjh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.kuanghao11.cn/gtxiuqmifo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ehwqpu.com/gtwyneflmz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtunjzhqrw.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtknrfmrjf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtavmtxiii.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtdzlqiuor.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gteqibimed.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtbilrlxrv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gtsaxhswoo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtbwxhfulb.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtgvuewglx.html


<!-- 参考信息 -->