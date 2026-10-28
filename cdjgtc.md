代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtvqokydin.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtggihlamo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dashuyun.cn/gtqhusmiwo.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtrfkhqwmx.html

Ruby: arr.index(x)
来源：http://hz.fengsongda.top/gtfgiejqsm.html

C#:   list.IndexOf(x);
来源：http://hz.zhaomingkeji.xyz/gtwatsfskj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtjrqispko.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.redwolf501.top/gtvftwjies.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.c1oappe.top/gtsjbxlyqt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtotzxpcuo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtmqgwafoz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtoaflovhc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guowangkeji.top/gtgvqbnete.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shangyingyoupin.top/gtdnlkytof.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtosuufymz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gtyobwpmew.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtufczhmas.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tianlin.xyz/gtsfmephjo.html

JS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtdioolbne.html

TS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtvgffwsqd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ywan-chungtsiang.top/gtmxquzqxn.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtvwyktgpb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhiwuduotai.top/gtmjjstfxw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.meibo888.top/gtvsqfhrce.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtectejtur.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigfzy.top/gtfgzekxti.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtwtrjaeoz.html

JS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtngredojs.html

TS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gttzatnyfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jlsjyb.cn/gtxfdqndtl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhaomingkeji.xyz/gtlpxqwifr.html

Ruby: arr.uniq
来源：http://hz.jianghu66.top/gtexzmeviy.html

C#:   list.Distinct().ToList()
来源：http://hz.9152youxi.cn/gtvurdtnfp.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtfpjglgal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtcnqbgzfw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ehwqpu.com/gtxkblmmog.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gturfuiswe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtpucvvufk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtkldakwrd.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtzjyjswda.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yuanzhike.top/gtbjqmdams.html

C#:   list.Sum();  list.Average()
来源：http://hz.guannengcc.top/gtacdxvxcd.html

[D17] 最大值与最小值
来源：http://hz.zhengqikj.top/gtmmwyxrms.html

Py:   max(arr);  min(arr)
来源：http://hz.feifeiyinyue.top/gtmbdtnqnc.html

PHP:  max($arr);  min($arr);
来源：http://hz.tanke756.top/gtpwfkwvwc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangtech.top/gtznyhivhq.html

TS:   Math.max(...arr);
来源：http://hz.mhx1999.top/gtpmvsmfkq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj202588.top/gtdwqgdqdx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtovagkdjj.html

Ruby: arr.max;  arr.min
来源：http://hz.jiagoushi.top/gthzgospfp.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtatavbvef.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtjvbwnmpc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtmhyuozou.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gteqklsixm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258888.top/gtbjpeulib.html

TS:   nested.flat();
来源：http://hz.smart0.xyz/gtbqoezvyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtbfkvcmmk.html

Go:   // 手写双层循环
来源：http://hz.bjfxy.top/gtfcaytpoq.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtldukuvuh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtrzkpdceg.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtkyefepfk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtzbdemsvv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtrvnzrzyc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtfwmhomyk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtlyrybrvg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtfzgitxyb.html

Go:   // 手写 map[string][]T
来源：http://hz.ybcxt.top/gtxueihokv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtvqdrzixw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.andypj.xyz/gtdlzjoxfj.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtoydftlak.html

Py:   Counter(arr)
来源：http://hz.gotoacloud.top/gtdpusdrqt.html

PHP:  array_count_values($arr);
来源：http://hz.ehwqpu.com/gtxakihksz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtrwistgyc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtnmmnnuhy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hongshengwenyu.top/gteczhxdxi.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtdhtostrr.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gtwbmrmobd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yonumen.top/gtfsebstnz.html

[D21] 判断是否包含某元素
来源：http://hz.andypj.xyz/gthxkhulxm.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtvumhiahf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.vqdsnc.cn/gtcvvcroqb.html

JS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtvoopdsqb.html

TS:   arr.includes(x)
来源：http://hz.316326.xyz/gtdpsngzrs.html

Java: list.contains(x)
来源：http://hz.c1oappe.top/gttdxpabxx.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnqzz.top/gtkmbrxicl.html

Ruby: arr.include?(x)
来源：http://hz.hywenlv.cn/gtvvwzyfvm.html

C#:   list.Contains(x)
来源：http://hz.gaohongyu789.top/gthszoamln.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yongpay.top/gtsdfvqdcg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hysaishi.cn/gtgknxpolf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenzaomai.com/gtrhefheis.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.mhx1999.top/gtbfrohglm.html

TS:   [...arr];
来源：http://hz.birdmap.top/gtvpzpbnby.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangtech.top/gtgktniowh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zycfv.cn/gtzeucvrqx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cashguo.top/gtckrmsyyt.html

C#:   new List<int>(list);
来源：http://hz.52xcode.cn/gtmegrrbnl.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtemockrhx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtzjqjnpmu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gtjzhlaohr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtudwmphww.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtwnjzregd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yanxiufei.cn/gtyfxqhiwk.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtcsczikiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gtkhewoedm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nanxinkj.top/gtvjocikos.html

[D24] 字典 / Map 基本操作
来源：http://hz.tian-w.cn/gtqokyfzyy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtlvalrkfa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtrvylojox.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinghuilouyu.cn/gtjsfwaarm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.kuanghao11.cn/gtgoulbzqt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gtugxrcajb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtafnkmaeo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tanke756.top/gtvpyiejtp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.bjfxy.top/gtkkylbxrn.html

[D25] Set 集合去重与交并差
来源：http://hz.hnxiangtu.top/gtohrdrgej.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtaqqkipgv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gthoyhodbk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtbqmbrlov.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.svipenyu.cn/gtrpsiwxzr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgfzy.top/gtxgnxfciq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hywenlv.cn/gtmojlzkxe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shangyingyoupin.top/gtxvahsuew.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gtpjcjjyiu.html

[D26] 数组转字符串
来源：http://hz.haohaochexian.top/gtkgyrwutj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtjwoqrzmc.html

PHP:  implode(", ", $arr);
来源：http://hz.andypj.xyz/gtjmjadeir.html

JS:   arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtscgjywpf.html

TS:   arr.join(", ")
来源：http://hz.316326.xyz/gtteiznsph.html

Java: String.join(", ", list)
来源：http://hz.xziqi.cn/gtzxeohewi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenjidiqi.icu/gtlwybctvm.html

Ruby: arr.join(", ")
来源：http://hz.yanxiufei.cn/gtqkrguzum.html

C#:   string.Join(", ", list)
来源：http://hz.wangshuangyany.cn/gticzsilrx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtncemyxdk.html

E. 字符串处理
来源：http://hz.zhongyouzk.top/gtbytfqgup.html

================================================================================
来源：http://hz.hysaishi.cn/gtpauhpdid.html

[E01] 拼接字符串
来源：http://hz.zhoulong.xyz/gtmngmissn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.quarkkingdee.top/gtbgddkxwg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtvegowyhv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtbirxujsv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtuowuyffi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yongpay.top/gtrqsxxeoq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aibaodan.cn/gtrloodqjx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gthjpzebgb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhongyouzk.top/gtksapjwhi.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtwqvjphej.html

Py:   "ab" * 3
来源：http://hz.jiagoushi.top/gtoxogxddq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtvrfoscjb.html

JS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtetcirhyx.html

TS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtnareojep.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtxslwjmgy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtroellscs.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gthcaejzii.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hfpthk.cn/gtvbwumrgc.html

[E03] 截取子串
来源：http://hz.cdnleiting.top/gtcipvfpee.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shzxlz.cn/gtgqnxymym.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gogol.net.cn/gtbbvdvcqv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.smart0.xyz/gtxfkcxwhh.html

TS:   s.slice(1, 4)
来源：http://hz.aizwys.cn/gtprwplpjp.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtartrfwax.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtfevkdoua.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigfzy.top/gtokvrzzbv.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtnmkxnhyq.html

[E04] 查找子串位置
来源：http://hz.vqdsnc.cn/gtcsgnqrqt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtophgpynv.html

PHP:  strpos($s, "x");
来源：http://hz.hongshengwenyu.top/gtgtcbhhft.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gtswtqgcbi.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtpdmrhiuk.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtfavvpaoc.html

Go:   strings.Index(s, "x")
来源：http://hz.hongshengwenyu.top/gtqsfdaizg.html

Ruby: s.index("x")
来源：http://hz.mhx1999.top/gtlfkdshfn.html

C#:   s.IndexOf("x")
来源：http://hz.yonumen.top/gtodoxzwxk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fzhhl.top/gtueligout.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gthopwfncg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj202588.top/gtioioteuh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtywpsdncn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinyuanbaomall.cn/gttfiyfyvj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtnjpgeljd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hammf.cn/gtnhjqbavv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gtsrcueeid.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtqdqawmtq.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtoqwvtaxn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtutghrnws.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtkkvzbtor.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtnpmscwhr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtebmqrndz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtdmwbduqt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuanzx.com/gtvaaourft.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj202588.top/gtkqxwvtpa.html

C#:   s.Replace("a", "b")
来源：http://hz.zhoulong.xyz/gtnkjzwget.html

[E07] 按分隔符拆分
来源：http://hz.yj202588.top/gtlmxotwxw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtysrhizmg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenjidiqi.icu/gtyiisfqyl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtioknrpjg.html

TS:   s.split(",")
来源：http://hz.jqgfzy.top/gtgwtkquva.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtbnezbemp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fengsongda.top/gtdupsmrdy.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gttqjcmvvw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhixingplan.top/gtcjuaqjhl.html

[E08] 数组按分隔符合并
来源：http://hz.hammf.cn/gttcfjigll.html

Py:   ",".join(items)
来源：http://hz.jqgufenzy.top/gtvfefasiu.html

PHP:  implode(",", $items);
来源：http://hz.hnqzz.top/gtmytxcaqc.html

JS:   items.join(",")
来源：http://hz.cheryme.top/gtiimnnucd.html

TS:   items.join(",")
来源：http://hz.dianchejie.cn/gtnqhimlcg.html

Java: String.join(",", items)
来源：http://hz.xuanzx.com/gtqbzhwdkl.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtbhbojdoh.html

Ruby: items.join(",")
来源：http://hz.daria6918.cn/gtglhgwchg.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtttennssf.html

[E09] 去除所有空白字符
来源：http://hz.guowangkeji.top/gtylznmzli.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtjpgdjiao.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ywan-chungtsiang.top/gtuyhsrffe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtqbuwrrlj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtnqbuksxr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gtcbqrqmdl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtbnvpsmnt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ivvv.top/gtxcrfhdmo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtuqfnqoid.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yongpay.top/gtupppndqf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj20258888.top/gthgraxowt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xinyue.icu/gtmdhpdktg.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gtlpjwvqwn.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtbujcjodh.html

Java: String.format("%03d", 7)
来源：http://hz.yongpay.top/gtovtgxfwp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtoddsjrvv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gtaydsmjsl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtqkuyblwv.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtiyjrbpti.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtxfufukcg.html

PHP:  strrev($s);
来源：http://hz.yj20258.top/gtmbhvuvyv.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtrjjnfrxx.html

TS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtoyihqrwh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gthlibvjie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zycfv.cn/gtzgspmkuf.html

Ruby: s.reverse
来源：http://hz.bjfxy.top/gtiprvurmd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtdjpcbouj.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtsrxwmxyl.html

Py:   s.count("a")
来源：http://hz.cqqwz.cn/gthvoylvdf.html

PHP:  substr_count($s, "a");
来源：http://hz.xylfe.cn/gtppnlvede.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtcvrdoeig.html

TS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtijjycpat.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gteccciudj.html

Go:   strings.Count(s, "a")
来源：http://hz.cdnleiting.top/gtdmbwisfe.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtbqqnbqdt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhixingplan.top/gthdtcgjjx.html

[E13] 逐字符遍历
来源：http://hz.52xcode.cn/gtiqcgfhey.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtowdzfnjg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gtvncthvrv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtppozsyuk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtmsghkopl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhengqikj.top/gtmckanymz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tian-w.cn/gtcjaeliwh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gotoacloud.top/gteygtndgx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhongyouzk.top/gthdsbcpxl.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtsejhioai.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.bjfxy.top/gtlosvjysb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.feifeiyinyue.top/gtjaxeuxgq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtfsfhysdi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxuanxn.top/gtmafaalom.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtclpxerln.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtfipdhulm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gtvfenthyt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtliqdxsgh.html

[E15] HTML 转义 / 反转义
来源：http://hz.quarkkingdee.top/gttoqozhru.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hfpthk.cn/gtjamhxefu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtaimelskh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gttaobiirj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtxtmlusmg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtuvndstxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gtetckvlff.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhaomingkeji.xyz/gthxcgnwcq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtmihyjcbc.html

[E16] 数字千分位
来源：http://hz.gotoacloud.top/gtfdcnpbrr.html

Py:   f"{1234567:,}"
来源：http://hz.ehwqpu.com/gtzxmofgkr.html

PHP:  number_format(1234567);
来源：http://hz.nanxinkj.top/gtserqjfze.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtcodkwphr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtxxdfatzo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gtedapotmy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cucudq.cn/gtfwlusuag.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xuetiantiany.cn/gtdkemhzqu.html

C#:   1234567.ToString("N0")
来源：http://hz.bjfxy.top/gtizuolbma.html

[E17] 首字母大写
来源：http://hz.vqdsnc.cn/gtoouswnkw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hammf.cn/gtlaoudilr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yangfankeji.com/gtwogeukhv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtskpjllpt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtkqsutbsz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtxdgfkdnt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ybcxt.top/gtcstlgwuq.html

Ruby: s.capitalize
来源：http://hz.guowangkeji.top/gthjimbrxl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ywan-chungtsiang.top/gthyhbkgyf.html

[E18] 模板占位符替换
来源：http://hz.yongpay.top/gtopamchgl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtzsminnjo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtppargqrx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtipgzhzwr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtzfsowjok.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtgnagntqw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtshprvesa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtwetjxnzx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xziqi.cn/gtwlrttged.html

[E19] 多行文本按行拆分
来源：http://hz.fengsongda.top/gtdvcmerbv.html

Py:   s.splitlines()
来源：http://hz.nanxinkj.top/gtunujkimb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tianlin.xyz/gttfhviksg.html


<!-- 参考信息 -->