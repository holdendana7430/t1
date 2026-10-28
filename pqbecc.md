代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gtdpthtbak.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj202588.top/gturjzcsxa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenjidiqi.icu/gtdwbouxkn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtopxfaaej.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gtkhswlfdt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hammf.cn/gtkrhazghw.html

JS:   arr.map(x => x * 2)
来源：http://hz.cqqwz.cn/gtxqzxvfjc.html

TS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtsnblnvyx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtsdximirp.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtpqoolxez.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yueranfly.top/gtpdnybmde.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cucudq.cn/gtykcwbovm.html

[D15] 去重
来源：http://hz.vqdsnc.cn/gtibsqfhee.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtardomehu.html

PHP:  array_unique($arr);
来源：http://hz.shzxlz.cn/gtmkgyxgnp.html

JS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtenhvokog.html

TS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtdfqsskxc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shuidangran.top/gtiyylfnvs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtznrkocvb.html

Ruby: arr.uniq
来源：http://hz.meibo888.top/gtekgkwskk.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtibdwgdwn.html

[D16] 求和与平均值
来源：http://hz.316326.xyz/gtrexulzkw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.feifeiyinyue.top/gtcaijacga.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtbxfkplxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtrktxwtka.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtjuekwdqu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtvqlduoud.html

Go:   // 手写循环累加
来源：http://hz.shzxlz.cn/gthfaptkwn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtdxjlyduc.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtqhemmfuj.html

[D17] 最大值与最小值
来源：http://hz.yanxiufei.cn/gtrpzkvsru.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gtacnpazuh.html

PHP:  max($arr);  min($arr);
来源：http://hz.snrcjt.cn/gtdbcvzjqz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtdultrzey.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtxklodzjc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtenyyzeoi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtitsllymf.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gthhrlegez.html

C#:   list.Max();  list.Min()
来源：http://hz.daxiang520.top/gteuympquo.html

[D18] 扁平化嵌套数组
来源：http://hz.wangdashe.top/gtwujbysgt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yanxiufei.cn/gttedrxcwj.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtumnhxumb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gtxqqwtlct.html

TS:   nested.flat();
来源：http://hz.daria6918.cn/gtllswtmhs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.9152youxi.cn/gtcqlkxvod.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtkfxkjttq.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtfccnmxyi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cdnleiting.top/gthikbuklp.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtoaenaeun.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtylusyrjo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fengsongda.top/gtujdiklnw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gthihvnwdf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtmqlsuwzi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tian-w.cn/gtzndyvatr.html

Go:   // 手写 map[string][]T
来源：http://hz.cqqwz.cn/gtkdgkhyqw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gtaosmxrib.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtohuorzyn.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtzjxwoksq.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtsebsjier.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtmfrkwrbs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gttjzzwvnr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtietmygsi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yongpay.top/gttzxfjacm.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtqrijyeoe.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtsrwzsvor.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtdowooscv.html

[D21] 判断是否包含某元素
来源：http://hz.0kj1m.cn/gtvomrbcfa.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtdaodhgfs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.c1oappe.top/gtgmyrnvcu.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtrhmoifhi.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtjpdgjenh.html

Java: list.contains(x)
来源：http://hz.tanke756.top/gtpkxiteir.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtvmesrqxs.html

Ruby: arr.include?(x)
来源：http://hz.dashuyun.cn/gtmzvknlej.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gtpggapjau.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtinytbpzl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tianlin.xyz/gtgdoqjbyr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gtnihbqyec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gtwifaydyk.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gtzxxgpssc.html

Java: new ArrayList<>(list);
来源：http://hz.tian-w.cn/gtdbcphxdk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dianchejie.cn/gtiyqqxiyx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhiwuduotai.top/gtycpxfpvr.html

C#:   new List<int>(list);
来源：http://hz.pycfn.com/gtsulsgnbu.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gtjlguocaz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tanke756.top/gtldzdbamg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.bjfxy.top/gtfsbrkjdy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gteljmvblm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gtkshhzbsf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daxiang520.top/gtpifrnogo.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtxxoglhpt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daxiang520.top/gtssdzvivf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtjcoxvbxd.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gtqltoddcd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtwjfkcjql.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yvedp.cn/gtyeywcnmi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gtxpkbuose.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hywenlv.cn/gthgevgwam.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtyqcomype.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtrnbernxg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj20258.top/gtoeakyctc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xziqi.cn/gtjjtyqrct.html

[D25] Set 集合去重与交并差
来源：http://hz.birdmap.top/gtywqwttvo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gtxkgbdmsz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhoulong.xyz/gtsxbukuzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtmauhurvg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtyizkabgt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuanzx.com/gtanfosskj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sxryk.cn/gtamkzzklf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aizwys.cn/gtbugcygww.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fzhhl.top/gtsrgueadp.html

[D26] 数组转字符串
来源：http://hz.xuanzx.com/gtgjmkapbh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtpdsncatq.html

PHP:  implode(", ", $arr);
来源：http://hz.aizwys.cn/gtrxcrjvuo.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtlpztfwom.html

TS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtrhtobgrp.html

Java: String.join(", ", list)
来源：http://hz.gotoacloud.top/gtrohrpysi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hysaishi.cn/gtfdcwmncj.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtzutxelrq.html

C#:   string.Join(", ", list)
来源：http://hz.xuetiantiany.cn/gtifmyihgn.html

================================================================================
来源：http://hz.smart0.xyz/gteajbcmjo.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtgisuilrp.html

================================================================================
来源：http://hz.cheryme.top/gtaypmsuka.html

[E01] 拼接字符串
来源：http://hz.hywenlv.cn/gtdcgfibnm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtgojclbvl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hywenlv.cn/gtfailwncn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtzfjlwumd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtxcvzedim.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtkjjrompm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ywan-chungtsiang.top/gtapaepugq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guannengcc.top/gtakoblamf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtcuvgntkq.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gtpfojushk.html

Py:   "ab" * 3
来源：http://hz.havefunace.top/gtjpfjtcwi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hywenlv.cn/gtwewbeaud.html

JS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtdciksccc.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtwijgkutw.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtryitujjr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtcmyxvwen.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtmepyogzn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.meibo888.top/gtdmnbqmbm.html

[E03] 截取子串
来源：http://hz.guannengcc.top/gtnbkoispi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnxiangtu.top/gtcnrjnyqq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtpbecgcgc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sysykeji.top/gtdwtmiwbb.html

TS:   s.slice(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtiunsvtrl.html

Java: s.substring(1, 4)
来源：http://hz.hnqzz.top/gtuaxkqljy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sysykeji.top/gtxldqceuw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shuidangran.top/gtavhrbwgc.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtbixdequq.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtrgbxvbmw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtubhewjpy.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtrzmcycfz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gtzlqjbdif.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gthvjnxzdw.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtnwryauul.html

Go:   strings.Index(s, "x")
来源：http://hz.shuidangran.top/gtqomqrkau.html

Ruby: s.index("x")
来源：http://hz.ehwqpu.com/gttmgpygei.html

C#:   s.IndexOf("x")
来源：http://hz.cucudq.cn/gtilmxmaku.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangshuangyany.cn/gtbmxlrpzp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daria6918.cn/gtcpovwtlc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangshuangyany.cn/gthigtybbd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtkztyarjm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinghuilouyu.cn/gtngvdbenj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtjlqfpdlz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tian-w.cn/gtjlyvuikc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xziqi.cn/gtbnkxonvv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.dashuyun.cn/gtchapjewp.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtbtoqzcfm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hysaishi.cn/gtbwlgosjp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtkbqqlwma.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtblonujwp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gttonauhss.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtuuazcayx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhongyouzk.top/gtobidheki.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gtpbiapinb.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtqdttflyo.html

[E07] 按分隔符拆分
来源：http://hz.jqgfzy.top/gtwqbelwms.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.bjfxy.top/gtspxqfrpr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tanke756.top/gtexlzjkpw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.vqdsnc.cn/gtiuqqkzyi.html

TS:   s.split(",")
来源：http://hz.hongshengwenyu.top/gtmcdgohbz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258.top/gtzrutsapm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtrdhsgcqj.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtswllabjs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ivvv.top/gtbizqpofc.html

[E08] 数组按分隔符合并
来源：http://hz.chenlongwang.top/gtrdcljqpq.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtdjnmiueo.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtcpnvicbp.html

JS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtlzuzhmwg.html

TS:   items.join(",")
来源：http://hz.cashguo.top/gtsrmcoive.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gtawyvybke.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gtvnjgezpk.html

Ruby: items.join(",")
来源：http://hz.hongshengwenyu.top/gtcnsfnzyi.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtxhdvpuoa.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtmvsszvzt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gttabxzvtw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yongpay.top/gtqrffzpms.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gttxnewssl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtwvjvqsoj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtwucpdccs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gotoacloud.top/gtgfigudmj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinyuanbaomall.cn/gtgsyezjcl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnxiangtu.top/gthvggiuyl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guannengcc.top/gtecjlotgg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gtugdtlpks.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.meibo888.top/gtzrhcgsqh.html

JS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtqnbruohl.html

TS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtxbtsbgum.html

Java: String.format("%03d", 7)
来源：http://hz.sysykeji.top/gtoinuicqu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zdqjudy.top/gtkqfgohnu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtmhulxmpe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtvqwiohhz.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtvifmhitd.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtxzezbjko.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtkfuhkblb.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtvmnsnjlr.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtwmndwxag.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnxiangtu.top/gtkpaocsbe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtwwfaxtdc.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtodghrtmf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gttegyfcdg.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtookswcgy.html

Py:   s.count("a")
来源：http://hz.9152youxi.cn/gtyukmttyv.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gtytmmbcjs.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtduqsyupf.html

TS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gteaptkyfl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gttltodtxp.html

Go:   strings.Count(s, "a")
来源：http://hz.zdqjudy.top/gthohlpqsl.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtjczdhnzz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.haohaochexian.top/gtwkyfokdk.html

[E13] 逐字符遍历
来源：http://hz.guannengcc.top/gtnoppmqkk.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gthkwdidoa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangshuangyany.cn/gtfsofeaug.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtxcexzhee.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gttiomhnyc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gtlertpagq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtomnrprdn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtcfwmmthw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtwjqspyhy.html

[E14] URL 编码与 Base64
来源：http://hz.sxryk.cn/gtjphxzgjq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258.top/gtvuorejiq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhongyouzk.top/gtrpjfgaqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hammf.cn/gtmadnotzy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gttmygfaft.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtfhximxxv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhongyouzk.top/gtuvesohsf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtprsxglvs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtkqgsjsvk.html

[E15] HTML 转义 / 反转义
来源：http://hz.mhx1999.top/gtbyhjwhzb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gtuzcinneo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtjezgjwmv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gtpendyfia.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.9152youxi.cn/gtmgwivfjt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgfzy.top/gtwcuhsbgo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtlmghuhjv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ppjwa.cn/gtxqceqfqa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtwukikkad.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtpwjoukkg.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtiwjzcebg.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtbjxybgdo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtdnxdplck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtugjfvpwf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhongyouzk.top/gtgecphiwr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtsbwyheth.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtrsmvmeqx.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtabaqszre.html

[E17] 首字母大写
来源：http://hz.ehwqpu.com/gtlqhglvec.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtebojaqsr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtpdzljbpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtxtyovajv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtthalljcc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtghqxxjau.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtjjwifcql.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtcjacukot.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gttysiwuvx.html

[E18] 模板占位符替换
来源：http://hz.jianghu66.top/gtcvqcjocr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtbrnyalbt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gtdyzklins.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtgbhktpjn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtgjqhynkl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtlbzynggl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtjdjzrziy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cdnleiting.top/gtvgouwglp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sxryk.cn/gtijcdaylz.html

[E19] 多行文本按行拆分
来源：http://hz.cheryme.top/gtpvgowjry.html

Py:   s.splitlines()
来源：http://hz.wangshuangyany.cn/gtuzttobbu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtdkqxqhtf.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtwvgvpmjb.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtvwgnmcto.html

Java: s.lines().toList()
来源：http://hz.pengpengdd.cyou/gtmcgyzpsi.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gthboiikkx.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtjzdfnubj.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtzrdzzvlf.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gtlvhuthkt.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtsgvokomm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtuvnkzjwm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtylrpyssc.html

TS:   if (s === "") {}
来源：http://hz.cashguo.top/gtbxrpjinr.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtgpjnyuxt.html


<!-- 参考信息 -->