代发 wailian999

[D15] 去重
来源：http://hz.yangfankeji.com/gtdcwwxayw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtvbuoerwt.html

PHP:  array_unique($arr);
来源：http://hz.fengsongda.top/gtfogoiiaa.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtjjhccfju.html

TS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gttzdesogz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuanzhike.top/gtgkycjdzo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtczqyyvjd.html

Ruby: arr.uniq
来源：http://hz.jlsjyb.cn/gttxsyihht.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxuanxn.top/gtchirrjrs.html

[D16] 求和与平均值
来源：http://hz.hnqzz.top/gtpegznrxt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zycfv.cn/gtkjrvwsyx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shuidangran.top/gtnmfzcsup.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtkuwmadux.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtqetfklad.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dashuyun.cn/gtbbjjhpjh.html

Go:   // 手写循环累加
来源：http://hz.hfpthk.cn/gtovyywiod.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.9152youxi.cn/gtmugwzfon.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258.top/gtkhbpwmpc.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtftaizxts.html

Py:   max(arr);  min(arr)
来源：http://hz.zhongyouzk.top/gtkumbnajy.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtdrdljyey.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangtech.top/gtbpyigdgt.html

TS:   Math.max(...arr);
来源：http://hz.sufxvd.cn/gttunnjozl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ywan-chungtsiang.top/gtmkqrxndr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtaruocxya.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gthnambfyl.html

C#:   list.Max();  list.Min()
来源：http://hz.zhiwuduotai.top/gtextezqkf.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtxdmbkvve.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtxrcrebin.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gthpbmgioz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shzxlz.cn/gtltmjkvfc.html

TS:   nested.flat();
来源：http://hz.cucudq.cn/gtvbicnoil.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yangfankeji.com/gtgizzswcr.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtoqlawrwq.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtbdeyoffz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ybcxt.top/gtmohotrvn.html

[D19] 按字段分组
来源：http://hz.jinqigufen.top/gthhozzdhi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258.top/gtyjhogowv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtplmclbnx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gogol.net.cn/gtbaypdyhh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtswdkxbbu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtoaepngyt.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtmepplwdq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yvedp.cn/gtpzagyept.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtnvhmcxtw.html

[D20] 统计每个元素出现次数
来源：http://hz.sysykeji.top/gtnyjxmbkt.html

Py:   Counter(arr)
来源：http://hz.cucudq.cn/gtugdeuvdi.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtckustpbk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtfahmgzgg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtslzcdghh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtpsibemze.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gtbrbiyxwb.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtkmkptejf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pengpengdd.cyou/gtsoqaojzg.html

[D21] 判断是否包含某元素
来源：http://hz.kuanghao11.cn/gtcgkcnyni.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gtdyjekdka.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgfzy.top/gtmgifsick.html

JS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtearmozmu.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gtsjlfxpih.html

Java: list.contains(x)
来源：http://hz.yvedp.cn/gtrwovfpcn.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtbluixwzv.html

Ruby: arr.include?(x)
来源：http://hz.xziqi.cn/gtecyegdzk.html

C#:   list.Contains(x)
来源：http://hz.nwbrower.top/gtalxbspxn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tanke756.top/gtxerfoddy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sysykeji.top/gtbvicqtjt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.mhx1999.top/gtirtztgzw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtwqptsdul.html

TS:   [...arr];
来源：http://hz.tanke756.top/gtgbccrxer.html

Java: new ArrayList<>(list);
来源：http://hz.zhijiandao.cn/gtlpandwpg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtvinvnram.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gtnuliehun.html

C#:   new List<int>(list);
来源：http://hz.hongshengwenyu.top/gthqqxmqfb.html

[D23] reduce 累积计算
来源：http://hz.meibo888.top/gtamrbsbdr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cucudq.cn/gtmnxljdut.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gtefnycirv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nwbrower.top/gttecealdm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtqsyurvvy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtmtsaxaui.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtqyhtwnll.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xylfe.cn/gtmuazetcv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gtiomelkta.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gturltinkb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gaohongyu789.top/gthkyahxrs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtrksdrvvk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nwbrower.top/gtimjycrff.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gtvmrzcbqe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.birdmap.top/gtzmqoazov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gzhubu.top/gtcsxxadoy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.mhx1999.top/gtlpjpahwf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhiwuduotai.top/gtjhmgdexo.html

[D25] Set 集合去重与交并差
来源：http://hz.xinyue.icu/gtmdczssnx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenjidiqi.icu/gtxbqphtoj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj202588.top/gtcwojiqrc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yongpay.top/gtkcatfjur.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dianchejie.cn/gtsxdgnusx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj20258888.top/gtatyuivmo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtwteaftkb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gtwpwbhfiv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhijiandao.cn/gtsbktyhkt.html

[D26] 数组转字符串
来源：http://hz.ppjwa.cn/gtlckobvcr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenjidiqi.icu/gtqynqxdje.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtlyeawmwx.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtvjrdeimi.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtkeatigsf.html

Java: String.join(", ", list)
来源：http://hz.yongpay.top/gtckgzxegh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.birdmap.top/gthtjkxjbt.html

Ruby: arr.join(", ")
来源：http://hz.yj202588.top/gtwkwgcqgv.html

C#:   string.Join(", ", list)
来源：http://hz.guannengcc.top/gtfyqufsgw.html

================================================================================
来源：http://hz.andypj.xyz/gtkjlmidnw.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtbcfznohn.html

================================================================================
来源：http://hz.zycfv.cn/gtfvpzfjqi.html

[E01] 拼接字符串
来源：http://hz.gogol.net.cn/gtjcicodod.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.c1oappe.top/gtftqmkeul.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtpncswxly.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gturatdhng.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtvlrsyqhl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigufen.top/gtfvkylyyy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangdashe.top/gtgulgjbot.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gthuwqqbky.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhongyouzk.top/gtjnqparwn.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtlxhgbwpb.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtyckipter.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sxryk.cn/gtkdzyewbe.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtmcaidjzt.html

TS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtrwkognyz.html

Java: "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtjszykmus.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydjk.org.cn/gtmqhmzqol.html

Ruby: "ab" * 3
来源：http://hz.316326.xyz/gtbzucydwd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj202588.top/gtfqfouevj.html

[E03] 截取子串
来源：http://hz.vqdsnc.cn/gtuerkqerr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yangfankeji.com/gtangotlje.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gotoacloud.top/gtawxxtdxw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj202588.top/gtocvcjzue.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtjpetahqj.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtzansnmic.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cheryme.top/gtgsqrcycj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sweek.top/gtqziiugve.html

C#:   s.Substring(1, 3)
来源：http://hz.tian-w.cn/gtxhbmzibz.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtkcawbysh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtgfktzzvf.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigufen.top/gtqzuutzom.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhoulong.xyz/gtyawrdaju.html

TS:   s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtemnehbqf.html

Java: s.indexOf("x")
来源：http://hz.haohaochexian.top/gtfgskxwhv.html

Go:   strings.Index(s, "x")
来源：http://hz.shuidangran.top/gtakceqlkh.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtpwqmkrge.html

C#:   s.IndexOf("x")
来源：http://hz.hammf.cn/gtjzztvipn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnqzz.top/gtsszwqhex.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gtuacyqvwt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hywenlv.cn/gtnxmdskxq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtiwtkpcov.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtyuxhhtiz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtetzgcvgw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gthkzhvies.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gaohongyu789.top/gthfuwewrw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtblvtkgow.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtpzfufrid.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtitfvnacx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtqekjhslf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gthcmoycgu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtcrkpnoxb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtfbjllnru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj20258888.top/gttzsxbdxe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydzc1.top/gtpfkkwtrv.html

C#:   s.Replace("a", "b")
来源：http://hz.gogol.net.cn/gtxqygrvda.html

[E07] 按分隔符拆分
来源：http://hz.316326.xyz/gtywqapxxp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zycfv.cn/gtuqlqwrgj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gtxdzqkvrr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuanzx.com/gtbwqlvxpy.html

TS:   s.split(",")
来源：http://hz.aizwys.cn/gtwjodfjci.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cashguo.top/gtdqkarztn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hysaishi.cn/gtrihirmck.html

Ruby: s.split(",");  s.split
来源：http://hz.zhijiandao.cn/gtqzcrqsml.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.havefunace.top/gtjacqmfdb.html

[E08] 数组按分隔符合并
来源：http://hz.guowangkeji.top/gtdffhsbhe.html

Py:   ",".join(items)
来源：http://hz.gogol.net.cn/gtirkxnijs.html

PHP:  implode(",", $items);
来源：http://hz.ydjk.org.cn/gtuicrtwxo.html

JS:   items.join(",")
来源：http://hz.xylfe.cn/gtlyqofgrn.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtoodwxruj.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtxbctvmzz.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigfzy.top/gtunvvtfma.html

Ruby: items.join(",")
来源：http://hz.sxryk.cn/gtwvvtbbga.html

C#:   string.Join(",", items)
来源：http://hz.dianchejie.cn/gtpopirtja.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gteztutsik.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yangfankeji.com/gtmuzrzmbw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtpioxwogp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtuzrummlc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gtgxqvchsk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gtuzqhzaov.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtlgaanzus.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtwrimznsf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cheryme.top/gthcavcess.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtlplolrad.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.redwolf501.top/gtkuzwqowr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pycfn.com/gtnsgkmlge.html

JS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtnjbpiswb.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtgzpujdei.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gtsxfcnhvi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtvwijhldt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shuidangran.top/gtozlbmopy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shuidangran.top/gtuqigxjzb.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtgfnfcuhv.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gthgegcmei.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtuonkqyop.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gthunnwvxf.html

TS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtqmsypenj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jiagoushi.top/gthujryxhm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gtnuhxsrkr.html

Ruby: s.reverse
来源：http://hz.hfpthk.cn/gtdurfryjf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtoyzeymdx.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtgerhgwwh.html

Py:   s.count("a")
来源：http://hz.yanxiufei.cn/gtiuuyrpbr.html

PHP:  substr_count($s, "a");
来源：http://hz.iojbl.cn/gtcftdapji.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtatezofcl.html

TS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtlxxekwzd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gtwaoseyht.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258888.top/gtggfplkao.html

Ruby: s.count("a")
来源：http://hz.birdmap.top/gtrbfvfqkz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtfayfhrsx.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtuhsxmuka.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gtoctjiptu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daxiang520.top/gttvqoroga.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtibrtcwux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtlpockyaj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gtzagbhxyw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gotoacloud.top/gtinxwigpc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtfhxeshop.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jlsjyb.cn/gttdakswhp.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangkeji.top/gtmjzobubv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtlwvpahth.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtqfwltwgx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.vqdsnc.cn/gtujlmugfn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenzaomai.com/gtfbtudjbm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gogol.net.cn/gtmhbminpp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtqlaejeod.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.redwolf501.top/gtimdyhtcs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtxlgzkoeg.html

[E15] HTML 转义 / 反转义
来源：http://hz.cheryme.top/gtjlalydjr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.snrcjt.cn/gtvrsoirya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtscxtzlzo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gttxxkbvff.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gthxptxsmr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jiagoushi.top/gtjyjrznvn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gtpqxzhvli.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtipntcttl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtyvccuhbi.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtpsfjxymn.html

Py:   f"{1234567:,}"
来源：http://hz.yuanzhike.top/gtddruesan.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtticnxpcl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtjgbvvtcp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtyupiddot.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtudwkfqpl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtflterysk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtyxxhkbbc.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtfatbqgvh.html

[E17] 首字母大写
来源：http://hz.zhoulong.xyz/gtufrkwsuu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yvedp.cn/gtxrvioaes.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtrmxpbkey.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtgtpctuyd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtzykmxzyl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtcpfjfshj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtcqfhttkd.html

Ruby: s.capitalize
来源：http://hz.ydjk.org.cn/gtdenmarsj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenzaomai.com/gtbrptwalb.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtnzirgbkh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtgoblgapb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtcqgezboi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtqdegoywe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtyvpckliw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gtjmuzpjlw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtvhyuohne.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtxuelwzew.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhoulong.xyz/gtxsfgdjba.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtfsqqfdkd.html

Py:   s.splitlines()
来源：http://hz.hnqzz.top/gtszpmxwux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtothxypqn.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gthbnsmdou.html

TS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtwxnhyodk.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtwcfnksxf.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtjfhfyucp.html

Ruby: s.lines
来源：http://hz.gzhubu.top/gtshdsmeco.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtjlbcuuxu.html

[E20] 判断字符串是否为空
来源：http://hz.hnxiangtu.top/gtgarpfzuu.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtlkhywqri.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hysaishi.cn/gtnzhwdxjx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hfpthk.cn/gtklrivzfr.html

TS:   if (s === "") {}
来源：http://hz.pycfn.com/gtjyselyow.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtkfqbtfiv.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtzrlxzejm.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gtplmvwnxj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258.top/gtjwwzfxwf.html

[E21] 超长截断加省略号
来源：http://hz.ydzc1.top/gtyeyfepox.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hfpthk.cn/gtnhoogtkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dianchejie.cn/gtszwssyvp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtxsvquvau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtrqnawkdt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtqmmaplal.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtuplwntqf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtphlqxbce.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gtvczrvapo.html


<!-- 参考信息 -->