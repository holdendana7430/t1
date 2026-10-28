代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtkisamtlv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtntlqxqkh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtkidurcyi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtyfzchasx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtyazonutv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenjidiqi.icu/gtefyvenhi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenlongwang.top/gtecrmwhhu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtdvexkwvm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258888.top/gtsrvwclum.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gttydysuli.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtagddnqbc.html

TS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gtdxigwkwc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hongshengwenyu.top/gtcuwyfpdl.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtxybkftpj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ehwqpu.com/gtyanabnkz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtqcxaldsa.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gttfgqhuud.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtepikxkeu.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtesgemvhh.html

JS:   [...new Set(arr)]
来源：http://hz.fengsongda.top/gtnvyvgjze.html

TS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtopugdsas.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtfofhtoct.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hysaishi.cn/gtlglzszfx.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtixsmpjug.html

C#:   list.Distinct().ToList()
来源：http://hz.vqdsnc.cn/gtlrdkiaya.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gthskvyjbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtkhzbmhoh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgfzy.top/gtbgwwoqqv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtvwgpndns.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtxgvlyksr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinghuilouyu.cn/gtjghoptgf.html

Go:   // 手写循环累加
来源：http://hz.cashguo.top/gtgaiqugdl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gterxqvsae.html

C#:   list.Sum();  list.Average()
来源：http://hz.9152youxi.cn/gteseolqzh.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtnwrxnhzs.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gtxmuialnr.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtslspytny.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.smart0.xyz/gtngsfsnup.html

TS:   Math.max(...arr);
来源：http://hz.sweek.top/gtuyxfsgvv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gthuzvkuue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuxming.cn/gtjnywxisu.html

Ruby: arr.max;  arr.min
来源：http://hz.dianchejie.cn/gtuyylhjof.html

C#:   list.Max();  list.Min()
来源：http://hz.smart0.xyz/gtmukzqjul.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtyiserwgw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gtlwhzjbuu.html

PHP:  array_merge(...$nested);
来源：http://hz.zhijiandao.cn/gtufxevnto.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj202588.top/gtypvqvwwp.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtfrzdfzip.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sweek.top/gtyaumrebz.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtwizvgnrp.html

Ruby: nested.flatten
来源：http://hz.ywan-chungtsiang.top/gtoreauxye.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtuvehyets.html

[D19] 按字段分组
来源：http://hz.svipenyu.cn/gtqsfwxnip.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gtnzmlkdgu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtpcbuqqre.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hysaishi.cn/gttbxfvtko.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtkxjayems.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtpcifoxus.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gthdlhqyav.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yanxiufei.cn/gtghencxpx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pycfn.com/gtezlshjjz.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtgwxgiopt.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gthpxcmzbw.html

PHP:  array_count_values($arr);
来源：http://hz.yueranfly.top/gtlpnfqbbj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtawzrfgwt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtmhxxybtq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gtwsxtqubp.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtiryjvuwj.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gtbhxfnswg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gaohongyu789.top/gtiobnwral.html

[D21] 判断是否包含某元素
来源：http://hz.shangyingyoupin.top/gtqjkwskow.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gttlaxiwhq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtkzegsbid.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtdvzddneg.html

TS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtnigxsetj.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtzqqsmdnm.html

Go:   slices.Contains(arr, x)
来源：http://hz.ybcxt.top/gtsztlcpmu.html

Ruby: arr.include?(x)
来源：http://hz.jianghu66.top/gtmyreoxeh.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtxuekxlfg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtmczjwgtf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtdqotjwpc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gotoacloud.top/gtvggygzno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtcutsideg.html

TS:   [...arr];
来源：http://hz.nwbrower.top/gtqbyzwppe.html

Java: new ArrayList<>(list);
来源：http://hz.yueranfly.top/gtzxgalzsx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tanke756.top/gtdirmhtzc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258888.top/gtzmrovloe.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtvvqwnvry.html

[D23] reduce 累积计算
来源：http://hz.daria6918.cn/gtiwuvsxwr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtsmuihyfx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xylfe.cn/gtydwntaeh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtpgqmdwyz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtsvibhwpd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtmtkmlqny.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtkxxmxyaq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jianghu66.top/gtiexiroxi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtrgakoqcp.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtraezplyi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtzvunfmdy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gtccmqhioq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cheryme.top/gtmtyealto.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinqigufen.top/gtnejvniog.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pycfn.com/gtmaifwdnm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gtoixkqikf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ivvv.top/gtomwpokfg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.redwolf501.top/gthtncfouv.html

[D25] Set 集合去重与交并差
来源：http://hz.hfpthk.cn/gtmezwritm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.aizwys.cn/gtakvqgxxd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtjpcbustz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gtmlvwziqc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuanzx.com/gtwoekpwis.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtdgqdtuge.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtosbahvas.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnqzz.top/gtrsjokiok.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangkeji.top/gtzwbsyjvr.html

[D26] 数组转字符串
来源：http://hz.cashguo.top/gtpofvfsfr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zycfv.cn/gtwbiwgnvc.html

PHP:  implode(", ", $arr);
来源：http://hz.jinghuilouyu.cn/gthmxwuvnm.html

JS:   arr.join(", ")
来源：http://hz.meibo888.top/gtlctvifxy.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtrcovahlr.html

Java: String.join(", ", list)
来源：http://hz.zhiwuduotai.top/gtrfumhzkc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtgbnwnysf.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gttnvnpnyk.html

C#:   string.Join(", ", list)
来源：http://hz.jianghu66.top/gtuwdtkdco.html

================================================================================
来源：http://hz.daria6918.cn/gtsgsxvzgn.html

E. 字符串处理
来源：http://hz.gotoacloud.top/gtzkvkkpki.html

================================================================================
来源：http://hz.jianghu66.top/gtojvotlsq.html

[E01] 拼接字符串
来源：http://hz.gogol.net.cn/gtvbhmqtqm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.vqdsnc.cn/gtafqkyoql.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cheryme.top/gtxugqwvgx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtrjbyapcd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtwwvnruzt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigfzy.top/gtoriaxuij.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtgahinhrd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.redwolf501.top/gtxyfiyuas.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtxbfazotl.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gthckjeeik.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtypdxqhup.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sufxvd.cn/gtywcyyuul.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtisedqqxi.html

TS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtltzogyxk.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtwdmkxcon.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gtmrnzsjdq.html

Ruby: "ab" * 3
来源：http://hz.cdnleiting.top/gtjmtreihi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gtyoavlukl.html

[E03] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtmfiwvrjo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhengqikj.top/gtfhbhxsny.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtxlsrkqsr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtvryrpeux.html

TS:   s.slice(1, 4)
来源：http://hz.fzhhl.top/gtobturfwt.html

Java: s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtuxovojna.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fengsongda.top/gtbgfilobg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtywkldcbv.html

C#:   s.Substring(1, 3)
来源：http://hz.chenlongwang.top/gthsombeau.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtzwolhqoy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhengqikj.top/gtcudgcjbq.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtuaaaixzy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jianghu66.top/gtvvnhcxck.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtxosxrcwf.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gtosdhbxfq.html

Go:   strings.Index(s, "x")
来源：http://hz.ehwqpu.com/gtpjwwkpbu.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtwdujpymn.html

C#:   s.IndexOf("x")
来源：http://hz.quarkkingdee.top/gtojwipkju.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.redwolf501.top/gtcrpnjisq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sxryk.cn/gtdblogifw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sweek.top/gtyuqfyklm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtqdyrfgmp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yvedp.cn/gtbveqtkml.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtxunuqfuq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gtpjpltcna.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtpdwrkcjq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenzaomai.com/gtqxvysitl.html

[E06] 替换子串
来源：http://hz.nanxuanxn.top/gtkixuagvn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xylfe.cn/gtquexqgsw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigfzy.top/gtrxvzmmei.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtfjrbmjuc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtwvixdfzm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtsksrxcav.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgufenzy.top/gtjnkfkpnb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gtpsjwxlgo.html

C#:   s.Replace("a", "b")
来源：http://hz.yuanzhike.top/gtibkijpwm.html

[E07] 按分隔符拆分
来源：http://hz.zhijiandao.cn/gtjqhbzajh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnxiangtu.top/gthxavwjpj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtyjpmgwpw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sxryk.cn/gtimdjdony.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtffnuvkur.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hfpthk.cn/gtkedgknxt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtbxgyuzbx.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gttgfyljep.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhiwuduotai.top/gtxyfxgyea.html

[E08] 数组按分隔符合并
来源：http://hz.zycfv.cn/gtsyqjlxhl.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtrskascgf.html

PHP:  implode(",", $items);
来源：http://hz.iojbl.cn/gteksigjqm.html

JS:   items.join(",")
来源：http://hz.haohaochexian.top/gtumvxvjrx.html

TS:   items.join(",")
来源：http://hz.guannengcc.top/gtsrkikwla.html

Java: String.join(",", items)
来源：http://hz.zhongyouzk.top/gtiieriysp.html

Go:   strings.Join(items, ",")
来源：http://hz.zhaomingkeji.xyz/gtixrqtnrd.html

Ruby: items.join(",")
来源：http://hz.zycfv.cn/gtmexijbok.html

C#:   string.Join(",", items)
来源：http://hz.gotoacloud.top/gtuwpubnns.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangkeji.top/gtdhmghsxz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtuoolkwrf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cheryme.top/gtsbsgzjus.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtyabryiud.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtsiqibrvb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtrrzfigrk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gzhubu.top/gtopzitnfg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pengpengdd.cyou/gtvlencqht.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.316326.xyz/gtaxrejbor.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtqynrxjsc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtevkgupym.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtzsufjyls.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtbquknnqx.html

TS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtqeqxswrq.html

Java: String.format("%03d", 7)
来源：http://hz.yuxming.cn/gtzpajaekp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ivvv.top/gtulidiazo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sysykeji.top/gtygtkxhpd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtjysocxon.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtchgmwczc.html

Py:   s[::-1]
来源：http://hz.wangshuangyany.cn/gtkfhpmcfn.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gttivjsvva.html

JS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtgevnmqfu.html

TS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtyoezoulv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.vqdsnc.cn/gttkqfiera.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gthpqwsxkf.html

Ruby: s.reverse
来源：http://hz.yanxiufei.cn/gtzvkcthxz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gthmoeazlg.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigfzy.top/gtfyxqsnlg.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gteadpiaez.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgufenzy.top/gtgmqoiszx.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtepctflgj.html

TS:   s.split("a").length - 1
来源：http://hz.ywan-chungtsiang.top/gtxtkwfqpl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yongpay.top/gtcdcyrqrr.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtazhxjesy.html

Ruby: s.count("a")
来源：http://hz.fengsongda.top/gtwhnineki.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtadzsxduu.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtfzadnidk.html

Py:   for ch in s: print(ch)
来源：http://hz.snrcjt.cn/gthegonlop.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gtvdobbrkk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtdtsqqzjt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtzbcbivqm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtaorudcxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtaehdanhe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aibaodan.cn/gtubxnkjdh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gtsedeemgv.html

[E14] URL 编码与 Base64
来源：http://hz.chenlongwang.top/gtcfyddukm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtqrfmhaye.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yongpay.top/gtnqccktqw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.vqdsnc.cn/gthzlgaksp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtytiesjfg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuetiantiany.cn/gthffbsxgt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258.top/gtquxbyzkz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.snrcjt.cn/gtkxtilezo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtowgvrzgt.html

[E15] HTML 转义 / 反转义
来源：http://hz.hnqzz.top/gtagxzctgp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dianchejie.cn/gtqgjzkdoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtwqzaebyh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtvlxsmpls.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gogol.net.cn/gtllojpiqh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gtwaixjgii.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.316326.xyz/gtasoidzmn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtoanmxmjs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.meibo888.top/gtqxxcfhno.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtxrdpsdas.html

Py:   f"{1234567:,}"
来源：http://hz.ydzc1.top/gtieolngfc.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtbllebfrd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtmqybnmbm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtyibqrxtn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gteiidsoni.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gtpyistwcz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigufen.top/gtyyeodfbz.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtrnmjcvxc.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtgorsrlpi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cucudq.cn/gtgxdccwsl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtwgbnmmly.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtodwcpasd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtuyugybmy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtjixlnkhy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yongpay.top/gtabninmox.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtgpbvdick.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ydzc1.top/gtwahugbjz.html

[E18] 模板占位符替换
来源：http://hz.bjfxy.top/gtzhxxhsiw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangdashe.top/gtypeggvaa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinghuilouyu.cn/gtmfhuhojs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gtzhlarzpw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtazpphyoz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtoqaetlxx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtwpmbsfcp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtnbdpqovh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtnjmbkune.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtxqmfoadx.html

Py:   s.splitlines()
来源：http://hz.sufxvd.cn/gtfzjkbdmz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.andypj.xyz/gtwhgskigp.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtljupvnlr.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtqmdgelpk.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gtbuwtomua.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhengqikj.top/gtgafnfwom.html

Ruby: s.lines
来源：http://hz.jinqigfzy.top/gtlbanwjyj.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtaityxfoo.html

[E20] 判断字符串是否为空
来源：http://hz.jinyuanbaomall.cn/gtcwvxmekd.html

Py:   if not s:
来源：http://hz.sweek.top/gtqbxfoopc.html


<!-- 参考信息 -->