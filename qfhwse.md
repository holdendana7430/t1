代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hongshengwenyu.top/gtsililurf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.mhx1999.top/gtjgvuywlt.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtppgjvmov.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtjpixxqjz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gthbfuvboq.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtugliovvr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtzutrnqrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guannengcc.top/gtdjebmikc.html

[D15] 去重
来源：http://hz.guannengcc.top/gtmbdigagb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhengqikj.top/gtqsfmubca.html

PHP:  array_unique($arr);
来源：http://hz.nanxuanxn.top/gtvrueifbi.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtkqjnpddn.html

TS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtwntbchep.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gttrpwgfqq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtkwkiznrr.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gtvtaakqgg.html

C#:   list.Distinct().ToList()
来源：http://hz.wangshuangyany.cn/gtjrfkksii.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gtqfzldsiv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtfkxhtwpl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sweek.top/gtpgewpbkx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtxwmdxyxz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtopayxypw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtrautzjkb.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtzaorqwse.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtzsphalbg.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydzc1.top/gtvcybyqel.html

[D17] 最大值与最小值
来源：http://hz.pycfn.com/gtgxyjndvb.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtsctfktqf.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gtwkhkudlo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gturqnyeao.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gtagbfsnkv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtgdgeklmv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigfzy.top/gtoduufcob.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtwsmcmgll.html

C#:   list.Max();  list.Min()
来源：http://hz.yj202588.top/gtifrezidh.html

[D18] 扁平化嵌套数组
来源：http://hz.zdqjudy.top/gtlpscozav.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtukirkwdu.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtlzrbaksg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cqqwz.cn/gtrgmmcmux.html

TS:   nested.flat();
来源：http://hz.bjfxy.top/gtvlppxyea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtsejsvlsa.html

Go:   // 手写双层循环
来源：http://hz.52xcode.cn/gtulmgihou.html

Ruby: nested.flatten
来源：http://hz.xziqi.cn/gthcoujhnc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258.top/gtacuylklo.html

[D19] 按字段分组
来源：http://hz.iojbl.cn/gtyocjypdf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gtayawytaz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtpajpnxrn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xylfe.cn/gteyepajth.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtmjfggwka.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtyxowtfui.html

Go:   // 手写 map[string][]T
来源：http://hz.hnxiangtu.top/gtkpvbqzee.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtcidxkeug.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtgfvkhwpz.html

[D20] 统计每个元素出现次数
来源：http://hz.quarkkingdee.top/gtgdoeitos.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtiqshwezp.html

PHP:  array_count_values($arr);
来源：http://hz.c1oappe.top/gtasnhxnny.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gttcnloajr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtyxurgfyl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtrogbasae.html

Go:   // 手写 map[T]int
来源：http://hz.yangfankeji.com/gtemskqycd.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtmrkgrwzv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtmzpanurn.html

[D21] 判断是否包含某元素
来源：http://hz.cqqwz.cn/gtopufvhpv.html

Py:   x in arr
来源：http://hz.feifeiyinyue.top/gtaeonaobx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtucohsjys.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtcehpdhna.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gtfogftaes.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gttkjfmusp.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtomnydbbo.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtszmytbgz.html

C#:   list.Contains(x)
来源：http://hz.havefunace.top/gtwemkwbpd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gteelxvmmq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhiwuduotai.top/gtbvhgpvjb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtcfwgdftn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtxfxktvbu.html

TS:   [...arr];
来源：http://hz.gogol.net.cn/gtxrxeirzo.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtrgssgtgw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenzaomai.com/gtptyyjauf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cdnleiting.top/gtfefgglcm.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtsibyryxh.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gtaaugnzca.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtypgnkbqj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hfpthk.cn/gtzodvdbgc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtrcobulco.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtivneurss.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cheryme.top/gtsknviifu.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtmgpjbicl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtqcixlihk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtifpkwtqt.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gtgewsdzyf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gtdentrhtk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yonumen.top/gtgtoxjbnv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cashguo.top/gtmqfqsuym.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gtawvnllgv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gaohongyu789.top/gtskwmxbwb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tianlin.xyz/gtuuxwvpmy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtsafehkgd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtppysxgza.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtwsbcsnzk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gtjmyjaphv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dianchejie.cn/gtplzqfptt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhaomingkeji.xyz/gtbjxsjbxk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tianlin.xyz/gtqhcvupol.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtulnmbbsj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtediztjfr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gzhubu.top/gtwvkluclw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gtstsoocfq.html

[D26] 数组转字符串
来源：http://hz.fzhhl.top/gtsteffeuz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xziqi.cn/gthsscwppx.html

PHP:  implode(", ", $arr);
来源：http://hz.dashuyun.cn/gtggayzxvk.html

JS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtluzuvnby.html

TS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtqywjxpvl.html

Java: String.join(", ", list)
来源：http://hz.xuetiantiany.cn/gtynvqqvpb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuetiantiany.cn/gtkjoozdtz.html

Ruby: arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtzgnjtwgv.html

C#:   string.Join(", ", list)
来源：http://hz.iojbl.cn/gtoocchpsp.html

================================================================================
来源：http://hz.yanxiufei.cn/gtccdcrrrn.html

E. 字符串处理
来源：http://hz.meibo888.top/gtzevbobvh.html

================================================================================
来源：http://hz.gzhubu.top/gthwwybzrs.html

[E01] 拼接字符串
来源：http://hz.iojbl.cn/gtcqaxjbso.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtuqlhbjiz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.kuanghao11.cn/gtjkxbnxwe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtwgffhlhk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gttkjkmgwf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangkeji.top/gtuwuvlazd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gttheoscwv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gtgarcbrjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnxiangtu.top/gtbeceetds.html

[E02] 重复字符串
来源：http://hz.shuidangran.top/gtmzcnthjt.html

Py:   "ab" * 3
来源：http://hz.yangfankeji.com/gtsldvhhsp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jiagoushi.top/gtyvrmvjnx.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtgfjefdid.html

TS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtriqmvfja.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtdizkkzvm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtiunpjsfr.html

Ruby: "ab" * 3
来源：http://hz.svipenyu.cn/gtqqitcvqv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gtjhajibol.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtjnfdbhch.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtnxeiarse.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtvywvdfaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daria6918.cn/gtcwhkhsmw.html

TS:   s.slice(1, 4)
来源：http://hz.gogol.net.cn/gtqncpjyio.html

Java: s.substring(1, 4)
来源：http://hz.yueranfly.top/gttjyenufw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cdnleiting.top/gtzjdgagmd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ybcxt.top/gtmrvqccxh.html

C#:   s.Substring(1, 3)
来源：http://hz.yangfankeji.com/gtzidbogri.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtlcwkbhai.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtttesqpol.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtxtetasuh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtdwydsozx.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtyabkfcfb.html

Java: s.indexOf("x")
来源：http://hz.xylfe.cn/gtenumkvpx.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtusgsbatq.html

Ruby: s.index("x")
来源：http://hz.pycfn.com/gtkbtnqdbt.html

C#:   s.IndexOf("x")
来源：http://hz.dianchejie.cn/gtaudryupk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxuanxn.top/gtbhsydssh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sufxvd.cn/gtyfdhjurr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pengpengdd.cyou/gtuwlopmsl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtzkcegoys.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hfpthk.cn/gtjksxcqxn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtqajobwzm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhiwuduotai.top/gtvfhlvoyj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.0kj1m.cn/gtyasfhlmu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.bjfxy.top/gtizpyiibc.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gttqobmoaa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yangfankeji.com/gtjqkhatug.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sxryk.cn/gtprfiexqf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtmhogfsso.html

TS:   s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtjbrslaex.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gttvbcqcjw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydjk.org.cn/gttunjucbn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtkghozwvh.html

C#:   s.Replace("a", "b")
来源：http://hz.quarkkingdee.top/gtbtqbsxjp.html

[E07] 按分隔符拆分
来源：http://hz.tianlin.xyz/gtbfpxhhry.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hysaishi.cn/gtfcdlustg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.52xcode.cn/gtvnrcpzyg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.c1oappe.top/gtonkflsph.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtgdadprbk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtmqnsvcwu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ywan-chungtsiang.top/gtrqtexprt.html

Ruby: s.split(",");  s.split
来源：http://hz.zdqjudy.top/gtdrbbinuh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hammf.cn/gtepsjvrii.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtputgrpab.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtgsomjkff.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtaolidrpn.html

JS:   items.join(",")
来源：http://hz.shuidangran.top/gtdzbjenhc.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtqcgqvxvs.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtjyzvzmlm.html

Go:   strings.Join(items, ",")
来源：http://hz.nwbrower.top/gtgwihmpnf.html

Ruby: items.join(",")
来源：http://hz.gogol.net.cn/gtcisqansi.html

C#:   string.Join(",", items)
来源：http://hz.feifeiyinyue.top/gtctdamqwq.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtqtjybgog.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtyqxnfxan.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.316326.xyz/gtiisvyxez.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtkisyrlwf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtjwipypal.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gtppajchun.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgfzy.top/gtloablagi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.316326.xyz/gtbzmjlbzk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtlysfudkb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtcufqnuhq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.52xcode.cn/gtzgslbxvb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xziqi.cn/gtiafxcjgb.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtoyfgifvk.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtutulhifn.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gttuuenobc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtbfqwjiuh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtvyaqgixl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.mhx1999.top/gtkordvqrw.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtgrkwyeje.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtheytpygg.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtvijvizgy.html

JS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtasmfzqck.html

TS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtnudbkmjd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnxiangtu.top/gtovexwlrf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgfzy.top/gtdniamqjt.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gthyfjawoh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gthnycvhfo.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtskxydgmh.html

Py:   s.count("a")
来源：http://hz.vqdsnc.cn/gtnkskcumt.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtxgeeqeyc.html

JS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gteqgyvttw.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtguqbvykb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtjqogwzzv.html

Go:   strings.Count(s, "a")
来源：http://hz.cdnleiting.top/gtbollolfp.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtbbumidws.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tianlin.xyz/gtobmbgnsi.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtpsbspsyy.html

Py:   for ch in s: print(ch)
来源：http://hz.yanxiufei.cn/gtwranduhg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zycfv.cn/gtnybzinft.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtsvjkhemp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtmmalzlzn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shangyingyoupin.top/gtsokqdniq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtbzxulfft.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gttkeshyge.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yanxiufei.cn/gtutecjrjm.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtlmqxzggm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhongyouzk.top/gtjdsjjnmi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cqqwz.cn/gtvdvxtwiz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ehwqpu.com/gtddascwma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhiwuduotai.top/gtoqbtybko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gthbhigpjw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtozfydttx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daria6918.cn/gtkxyhvyod.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtudzdhpxe.html

[E15] HTML 转义 / 反转义
来源：http://hz.gotoacloud.top/gtwfhvuqef.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtnsrrwail.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daxiang520.top/gtqnrhybko.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daxiang520.top/gteggvyteh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gthozqtldt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuanzhike.top/gtaxponhqj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hysaishi.cn/gtuhwoilyo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangkeji.top/gtwnewyxej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gtbftgisqb.html

[E16] 数字千分位
来源：http://hz.0kj1m.cn/gtlyjbskqc.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtnqqhzdcl.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtzaonsxqw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtemoyqhhu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtngqqpxyp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtvcwxonip.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guowangkeji.top/gttltkznzh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fengsongda.top/gteueqmkkk.html

C#:   1234567.ToString("N0")
来源：http://hz.zdqjudy.top/gtbgtdpatf.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtwfhdhclv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtzkiggtrq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtryxdpsqx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtbvtrhevw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtuizkazhz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtzmcrzhem.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gtchddlrot.html

Ruby: s.capitalize
来源：http://hz.cdnleiting.top/gtyeppzvtw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ppjwa.cn/gtxjvzendm.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtgoudtute.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.havefunace.top/gtqidmymhl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aibaodan.cn/gtqealrydr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtoljiygzy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtiprvahuk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtncgtrpzd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hywenlv.cn/gtjczzklpm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtqoflzxcl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnxiangtu.top/gtsehjgpjt.html

[E19] 多行文本按行拆分
来源：http://hz.ywan-chungtsiang.top/gthmzeqdrj.html

Py:   s.splitlines()
来源：http://hz.chenlongwang.top/gtnhxroktc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fengsongda.top/gtcsgzmrgi.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtklrjexwi.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gttavoqstp.html

Java: s.lines().toList()
来源：http://hz.jiagoushi.top/gtgyxgldpc.html

Go:   strings.Split(s, "\n")
来源：http://hz.birdmap.top/gtclzlvifw.html

Ruby: s.lines
来源：http://hz.havefunace.top/gtwuhluyhw.html

C#:   s.Split('\n')
来源：http://hz.guannengcc.top/gtagrdajdn.html

[E20] 判断字符串是否为空
来源：http://hz.aibaodan.cn/gtenkzopqo.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtykxokhpk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtyitbctms.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtkjrzjzzc.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtmhqvbpgb.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtddtygfzh.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtjdpxwrut.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtztfpwevp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtvwkkcjsc.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtppumbckv.html


<!-- 参考信息 -->