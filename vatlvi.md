代发 wailian999

C#:   list.Reverse();
来源：http://hz.zycfv.cn/gtiywqwnqi.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtzqximlxv.html

Py:   arr.index(x);  x in arr
来源：http://hz.hysaishi.cn/gthfqhprcr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtphvtjhbq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtcsfryton.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtbnykvovp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ybcxt.top/gtdupwxihy.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtcyvizaxo.html

Ruby: arr.index(x)
来源：http://hz.ehwqpu.com/gtyytclbug.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtnpmdjjow.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtlybuxief.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cucudq.cn/gttvtqtktb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtqbwsccpv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtytwfffrb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gthjvkyans.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sysykeji.top/gtvvirvqrm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tian-w.cn/gtqghfkllm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxuanxn.top/gtlxezdvtp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtjhmgafqy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gogol.net.cn/gtefglijor.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gtkmqhhjrh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.birdmap.top/gtbbplispj.html

JS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtmzqhqznm.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtnnqcufom.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtnaeqnehk.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtpqwtwdiq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtbyniftwi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtsblfryrm.html

[D15] 去重
来源：http://hz.hongshengwenyu.top/gtwjiqsbtr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtwxcgqmhr.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangtech.top/gtwpresczw.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtqvnfpvcg.html

TS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtuvczjlrl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gtodjmkdpl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.andypj.xyz/gtudipjxrt.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtxhxvbgbo.html

C#:   list.Distinct().ToList()
来源：http://hz.bjfxy.top/gtptrcikcq.html

[D16] 求和与平均值
来源：http://hz.shuidangran.top/gtlapzxnvi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtpnxpdzqt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtoiwqogdc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtjyyuavgo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtbbnsshdp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtokxiqafs.html

Go:   // 手写循环累加
来源：http://hz.hammf.cn/gtbehdtect.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtxjpbunsm.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtjijjitmh.html

[D17] 最大值与最小值
来源：http://hz.birdmap.top/gtmfqfbvxz.html

Py:   max(arr);  min(arr)
来源：http://hz.cqqwz.cn/gtrbwvxgyv.html

PHP:  max($arr);  min($arr);
来源：http://hz.jianghu66.top/gtecrfvuuo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtveuqfmbu.html

TS:   Math.max(...arr);
来源：http://hz.jiagoushi.top/gtjpnqutcx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtbireuogc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtaklpfumo.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtgbdidiwi.html

C#:   list.Max();  list.Min()
来源：http://hz.jlsjyb.cn/gtblwumqff.html

[D18] 扁平化嵌套数组
来源：http://hz.jinghuilouyu.cn/gtrjkekhah.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtogklnnzz.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtygydtiqm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.svipenyu.cn/gtmchsenog.html

TS:   nested.flat();
来源：http://hz.jlsjyb.cn/gtvsaifecw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtwqxaiyyl.html

Go:   // 手写双层循环
来源：http://hz.sxryk.cn/gtgvuibtwl.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gtsbporjmc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daria6918.cn/gteokxljcg.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtkhudpbbg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ehwqpu.com/gtdmdvgmtn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtiojzvnph.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gttsdzgdvc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gthxsrsbpi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtfgvdsdqt.html

Go:   // 手写 map[string][]T
来源：http://hz.pycfn.com/gtpmxjmejy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.meibo888.top/gtnvfpqtsh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.c1oappe.top/gtwnivmnfr.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtwjiqujol.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtxeyzfbea.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtkufcrwyq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtelaqufqb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtcvvktsdj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhongyouzk.top/gtmgmqljzy.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gtrhzetlkv.html

Ruby: arr.tally
来源：http://hz.xingfuxueyuan.xyz/gtajfskmqa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sweek.top/gtbfvynukv.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gtwcolqlpi.html

Py:   x in arr
来源：http://hz.nanxinkj.top/gtqiznrxqy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.svipenyu.cn/gthzamlyss.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtpetgnqfe.html

TS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtgvlowwra.html

Java: list.contains(x)
来源：http://hz.gotoacloud.top/gtmdigvssj.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtplrhwhmm.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gtkfqfwbzo.html

C#:   list.Contains(x)
来源：http://hz.jinqigfzy.top/gtfjqoonss.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ppjwa.cn/gtjusglrmh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgufenzy.top/gtklpnxvkf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigufen.top/gtarelfwwf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sweek.top/gtjjbbvgll.html

TS:   [...arr];
来源：http://hz.havefunace.top/gtvwyrdmfc.html

Java: new ArrayList<>(list);
来源：http://hz.jiagoushi.top/gtfpnxubaa.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtqzozhcji.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtihndtsfi.html

C#:   new List<int>(list);
来源：http://hz.pengpengdd.cyou/gtecygrchh.html

[D23] reduce 累积计算
来源：http://hz.zhixingplan.top/gtphhwykqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtyqstmgba.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtudvwkoro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtjfczawbl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtyavdpdyi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtdgdccajc.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtagywhkfp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gtleerjval.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtmzxtphyn.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gtjyiydtxh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhaomingkeji.xyz/gtuhzizvbr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gtyevwzyli.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cqqwz.cn/gttwkzqsdn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtzwnmpwwl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.haohaochexian.top/gtuetiepns.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtbktkqsxv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhaomingkeji.xyz/gtiexkvtcr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtptyzklnv.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtkcvuqmof.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtcwlhwwgn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zycfv.cn/gtofqtffsn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtpnnsoydy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gttsltjuwu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dashuyun.cn/gtdjsuanpo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jiagoushi.top/gtxlingqas.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtsdtwjapv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tianlin.xyz/gtdsnkcgpn.html

[D26] 数组转字符串
来源：http://hz.yj20258.top/gtxzxaapqb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtuqgiqxoc.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gtmcicepah.html

JS:   arr.join(", ")
来源：http://hz.meibo888.top/gtbzqadyhb.html

TS:   arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtegmrehwp.html

Java: String.join(", ", list)
来源：http://hz.jinqigufen.top/gtjcaphlsv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.mhx1999.top/gtkofzurej.html

Ruby: arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtktjpdakq.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gthvpakybm.html

================================================================================
来源：http://hz.aibaodan.cn/gtvgtgbvqo.html

E. 字符串处理
来源：http://hz.yueranfly.top/gtkxqvhcpy.html

================================================================================
来源：http://hz.daria6918.cn/gtdkmcgqif.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtoywlcswv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydjk.org.cn/gtbvqafolz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydzc1.top/gtmtzckxsd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtczoxspuy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtqriazxvh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zdqjudy.top/gtidosphdn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtscsflxlh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtevoabkus.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtnfctaang.html

[E02] 重复字符串
来源：http://hz.yonumen.top/gtlmtlpnlp.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtebtunepx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tianlin.xyz/gttuuwcovs.html

JS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gtockuktup.html

TS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtoehtgoic.html

Java: "ab".repeat(3)
来源：http://hz.yuxming.cn/gtqoywdnkd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtgrxltkkk.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtroaoybit.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.svipenyu.cn/gtysgtgpfr.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtdknnjjzn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.kuanghao11.cn/gttplgkpkp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtgprvyizl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtvezuvteb.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigfzy.top/gtrkqlnfes.html

Java: s.substring(1, 4)
来源：http://hz.fzhhl.top/gtnqohirnt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jianghu66.top/gtikuraeza.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtrelftzfz.html

C#:   s.Substring(1, 3)
来源：http://hz.redwolf501.top/gtqlbsgooj.html

[E04] 查找子串位置
来源：http://hz.nwbrower.top/gtqzjwqrxn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hnqzz.top/gtrbovhsqv.html

PHP:  strpos($s, "x");
来源：http://hz.fzhhl.top/gtsjcvlhtp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtzvorcalj.html

TS:   s.indexOf("x")
来源：http://hz.gaohongyu789.top/gthhlsjuug.html

Java: s.indexOf("x")
来源：http://hz.aibaodan.cn/gtdzjsuhdx.html

Go:   strings.Index(s, "x")
来源：http://hz.cqqwz.cn/gtzphmvhym.html

Ruby: s.index("x")
来源：http://hz.sxryk.cn/gtwflgevez.html

C#:   s.IndexOf("x")
来源：http://hz.jqgfzy.top/gtmbapdkpe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtwqykudho.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ivvv.top/gtakhxignv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hammf.cn/gtcvdlzfku.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgfzy.top/gtzcuroamm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hfpthk.cn/gtkzoslzvc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtfieddnjk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.andypj.xyz/gtupmyhoyk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtznoaoozf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtwszjvcxt.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gthkrqdvvs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.316326.xyz/gtrxjhjbgj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhixingplan.top/gtedbkugav.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtncleylvk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtynpqkrau.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtvcqhlmdz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtvbvcqdli.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuanzhike.top/gtljmwtgof.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtuxuvladx.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtsnynvbpq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pengpengdd.cyou/gtkpcconqb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yueranfly.top/gtloioljoz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sxryk.cn/gtignzdkkw.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtkiqtaqvu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtoncsyynn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtpewfgyfm.html

Ruby: s.split(",");  s.split
来源：http://hz.zhaomingkeji.xyz/gtdnvnkbrd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gtndozuuid.html

[E08] 数组按分隔符合并
来源：http://hz.jianghu66.top/gthgllcsuj.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtaipnbjdn.html

PHP:  implode(",", $items);
来源：http://hz.nwbrower.top/gtcjehrxfk.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtcitqoqxw.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtulhuhbmy.html

Java: String.join(",", items)
来源：http://hz.yj20258.top/gtkeinkowl.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtgydtptzg.html

Ruby: items.join(",")
来源：http://hz.c1oappe.top/gterwuvovi.html

C#:   string.Join(",", items)
来源：http://hz.yangfankeji.com/gtoxsdzfuk.html

[E09] 去除所有空白字符
来源：http://hz.pengpengdd.cyou/gttkyjhjrx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtdvhquhal.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtkxmldrnx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtxtispgab.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtvfptcety.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.dianchejie.cn/gtllpopivc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gtjspxhfzi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sweek.top/gttdsdvmec.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtsexbgyhb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cucudq.cn/gttjjqsceh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gtirwmpnlc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.9152youxi.cn/gtnfebguen.html

JS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtkdrbdfzt.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtzipvjtqf.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtzrpmmhwa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtnudayaif.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtqyrjnylk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xingfuxueyuan.xyz/gtkmmzuhou.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtapwfnegt.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtntksvdfy.html

PHP:  strrev($s);
来源：http://hz.andypj.xyz/gtqedxqrzo.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtyycbqfmy.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtiskugsln.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cdnleiting.top/gtocareduz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtznxjgkgl.html

Ruby: s.reverse
来源：http://hz.yueranfly.top/gtzhgrggyr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtfpgdsfaz.html

[E12] 统计某字符出现次数
来源：http://hz.ehwqpu.com/gtzopplsbi.html

Py:   s.count("a")
来源：http://hz.zhengqikj.top/gtkqnjxxzs.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtmniinqah.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtrgselyok.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtqnipvcan.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yvedp.cn/gthqgypsuc.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtsywhzczj.html

Ruby: s.count("a")
来源：http://hz.snrcjt.cn/gtjwjrehwu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnxiangtu.top/gtzqmcxojn.html

[E13] 逐字符遍历
来源：http://hz.cheryme.top/gtjieibqfn.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtcefijhjc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258.top/gtulntymea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtqobkrvsv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtqauufixn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtrzstytkg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtqihrtrvk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.redwolf501.top/gtfzdndevs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtzzdniqpw.html

[E14] URL 编码与 Base64
来源：http://hz.0kj1m.cn/gtupihblhu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgufenzy.top/gtqdkvufaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hysaishi.cn/gtqrhwxncq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daria6918.cn/gtlgqsnkxi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtulixnwnn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtewyyxlps.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gthlrdzcls.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ydzc1.top/gtahrnyobh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhaomingkeji.xyz/gtxeiwdquu.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258.top/gtfhimzogm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gaohongyu789.top/gtukewlyeh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gtspjtkney.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jyoumei.cn/gtqhnwgora.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cqqwz.cn/gtqlmnxipt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangdashe.top/gtddxvzcme.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxinkj.top/gtnguyntxx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtvuofowgd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dashuyun.cn/gtunlxyiod.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtqskibrvv.html

Py:   f"{1234567:,}"
来源：http://hz.hnxiangtu.top/gtnjmwrseh.html

PHP:  number_format(1234567);
来源：http://hz.sweek.top/gtpylkhhfo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtbevlkrxz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtzzmrdzza.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtdwecfnav.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yangfankeji.com/gtqpykjsoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aibaodan.cn/gtuuxorbue.html

C#:   1234567.ToString("N0")
来源：http://hz.xziqi.cn/gtqpazmsfq.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtugarrdxb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtyjqmurin.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yanxiufei.cn/gtdippcgwn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtsvhkgknw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gttwokmodn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtixjyqxoa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pengpengdd.cyou/gtknwxepui.html

Ruby: s.capitalize
来源：http://hz.c1oappe.top/gtsamyqvwt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gtxjainnpa.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtykncixql.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtstieqydn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gtvjlcdfxi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtpwoeednt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtqkjrlynb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gtkarfqwos.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gthvkavbxf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtabwyvclg.html


<!-- 参考信息 -->