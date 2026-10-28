代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtolwlziky.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj20258.top/gtynnganrd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hysaishi.cn/gtqaqozpep.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tanke756.top/gtdstxoviy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cqqwz.cn/gtwdmabijf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shuidangran.top/gtjusbxxvj.html

JS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gtzzcdvlvc.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtdlbmmxlv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigufen.top/gtuyifxtdc.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtlczmyiqx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.andypj.xyz/gtlpocpxlu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yonumen.top/gtwtgkczbe.html

[D15] 去重
来源：http://hz.yuxming.cn/gtbnnskdsq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtcrcpkgxr.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtsczdybfv.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtgfjlosck.html

TS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtubukbtvl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gtjulxrnul.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuanzx.com/gtnljslipt.html

Ruby: arr.uniq
来源：http://hz.meibo888.top/gtbtrafjnz.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtqisbvbmr.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtfmiogibw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pengpengdd.cyou/gtdcpjwhbs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtyvpvpgjk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtgvtkeafm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtoohvrkko.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gtauahbkrk.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtdmplmpbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtbvtyjdaj.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtzftwjelm.html

[D17] 最大值与最小值
来源：http://hz.dashuyun.cn/gtlfhptyzp.html

Py:   max(arr);  min(arr)
来源：http://hz.cheryme.top/gtqzqqeycb.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtgwnswgoe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtzbsremvh.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtgaszjivy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.snrcjt.cn/gtduoewohs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtgtgliawn.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258888.top/gtqevlptkf.html

C#:   list.Max();  list.Min()
来源：http://hz.fzhhl.top/gttilixyij.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtudlmokot.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.feifeiyinyue.top/gtxumyaxrn.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gtezilngtc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtndrnista.html

TS:   nested.flat();
来源：http://hz.iojbl.cn/gthujfanob.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtnljhcvmq.html

Go:   // 手写双层循环
来源：http://hz.xuanzx.com/gtupivrwnc.html

Ruby: nested.flatten
来源：http://hz.gaohongyu789.top/gtfapvrgjn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hfpthk.cn/gtxfmpcgkf.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtqxnkuppi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtbdgkxsdg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangkeji.top/gtmdfhekel.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnqzz.top/gtrpivdfkf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gthqvduygg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtlufrkwxj.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtbbnzvmhs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtdgwgiawn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtvkritlji.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtkokangyk.html

Py:   Counter(arr)
来源：http://hz.xuetiantiany.cn/gtttgpapdx.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtfesqnjsh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtbfkaevrr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtkuhzqznr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtquujwpfi.html

Go:   // 手写 map[T]int
来源：http://hz.dashuyun.cn/gtfkdibmtk.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtcxickqtk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtgvpjjjxn.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtoculwbfz.html

Py:   x in arr
来源：http://hz.ppjwa.cn/gtpzuzxrkc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.snrcjt.cn/gtfcasliue.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtyjhlztyp.html

TS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtacgnevuv.html

Java: list.contains(x)
来源：http://hz.hammf.cn/gtykktuiit.html

Go:   slices.Contains(arr, x)
来源：http://hz.gaohongyu789.top/gtzkuxedty.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtukudfmrk.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gtmpmrpscq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigfzy.top/gtuuhwctlo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtbyqcgmmf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnxiangtu.top/gtidsuhhqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhaomingkeji.xyz/gtlfipxfwu.html

TS:   [...arr];
来源：http://hz.yuanzhike.top/gttbmhwzxm.html

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gtoqglhukx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.haohaochexian.top/gtgonkaljf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gtsdurgmqc.html

C#:   new List<int>(list);
来源：http://hz.wangdashe.top/gtzvibpkud.html

[D23] reduce 累积计算
来源：http://hz.feifeiyinyue.top/gtlkakqizv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtnlkktbdg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtfcbyyzad.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtyadtmvps.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtffkxodma.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenjidiqi.icu/gteiuilnoi.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtbmwrqmsr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtarcjrtvc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jlsjyb.cn/gtunckprli.html

[D24] 字典 / Map 基本操作
来源：http://hz.gaohongyu789.top/gtvgrxrcmt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydzc1.top/gtbxtgfucq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtmkbggrji.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gaohongyu789.top/gtqggmyfgb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtsyuezcxu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtyxadpyjy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtgsttimea.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinyuanbaomall.cn/gtxfxscrzd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtldhiugcy.html

[D25] Set 集合去重与交并差
来源：http://hz.yj202588.top/gtrtdfpkvz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258.top/gtywzijuzw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jyoumei.cn/gtymqtntdn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtyjrennrq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gtjhylbypi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtzeuohuql.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnqzz.top/gttnflszeu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gtilvczvzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtcetzirdv.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtyzstwywm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jyoumei.cn/gtczrwkzqh.html

PHP:  implode(", ", $arr);
来源：http://hz.cdnleiting.top/gtwwfhnuze.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtqemcxbwc.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtzrtsyauj.html

Java: String.join(", ", list)
来源：http://hz.sufxvd.cn/gtkarfaavg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtnvgiqmth.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtlggyxcql.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtpywheqmk.html

================================================================================
来源：http://hz.52xcode.cn/gtvwestjnn.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtoxoxbepl.html

================================================================================
来源：http://hz.shzxlz.cn/gtjmakyliz.html

[E01] 拼接字符串
来源：http://hz.316326.xyz/gtddmezpig.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtiyasmdzi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtqxmkvbmy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtgzbbucld.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtehzfvlhd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.mhx1999.top/gtiuixiiim.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.dianchejie.cn/gtvnhlbazf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gtajfkbmex.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gtthkcyxbq.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gtjdzijgyi.html

Py:   "ab" * 3
来源：http://hz.hfpthk.cn/gtozqipdlc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuetiantiany.cn/gtfyltcwdu.html

JS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtnbwmzuaz.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtudfuisxw.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtjhcqvvjx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yonumen.top/gtnhtlfjay.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gtojcaprbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtdbwbcbiw.html

[E03] 截取子串
来源：http://hz.hammf.cn/gtenwvxyvq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxuanxn.top/gtnamdyhrs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gtldigpysu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtyvimfoxb.html

TS:   s.slice(1, 4)
来源：http://hz.ivvv.top/gtzwufxgvy.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtcyapzkjm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gtsdyryatz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gogol.net.cn/gtzeyvujbt.html

C#:   s.Substring(1, 3)
来源：http://hz.hfpthk.cn/gtabogfrhq.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtceypnlpd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtkhmivnuy.html

PHP:  strpos($s, "x");
来源：http://hz.hfpthk.cn/gttqxptaae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtmqxczjwz.html

TS:   s.indexOf("x")
来源：http://hz.hywenlv.cn/gttpyzmnsm.html

Java: s.indexOf("x")
来源：http://hz.jyoumei.cn/gtzysceoif.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtlalyvxcv.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtmawrevay.html

C#:   s.IndexOf("x")
来源：http://hz.tianlin.xyz/gttufzuznk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gtaikcmkjo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnqzz.top/gtocrfyugf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtubohzfbu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtnsnjmyrb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sxryk.cn/gtqavveamk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtdoyzsjqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigufen.top/gtiyaegmjp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtpelznqbl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangdashe.top/gtawccmccs.html

[E06] 替换子串
来源：http://hz.yongpay.top/gtuyglhxkg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtteqikggt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtvzqeyjdq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtcnubeamk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtjvbhvcoe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtbknotzdt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuxming.cn/gtmrcvkkqi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.kuanghao11.cn/gtzurunown.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtzznoieaz.html

[E07] 按分隔符拆分
来源：http://hz.jqgfzy.top/gtbhixknxw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yvedp.cn/gtfcwaobbb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtlocggszd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtslqwfuri.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtgdlqkhhz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgufenzy.top/gtknycacly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sxryk.cn/gtrcjrepoh.html

Ruby: s.split(",");  s.split
来源：http://hz.yangfankeji.com/gtpcotourb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangkeji.top/gtjzxjbusk.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtccltovxd.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtmyvfxjei.html

PHP:  implode(",", $items);
来源：http://hz.daria6918.cn/gtnhrglnff.html

JS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtmqqwrgzz.html

TS:   items.join(",")
来源：http://hz.ydzc1.top/gtaopwkfxp.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtvtkdlazv.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtqanyaytr.html

Ruby: items.join(",")
来源：http://hz.hongshengwenyu.top/gtigtuotxl.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gtfnbqtdon.html

[E09] 去除所有空白字符
来源：http://hz.xuanzx.com/gtpdzmsbch.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangshuangyany.cn/gtpwoicaqg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gtnyhfcvqy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtttooutvu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtsucpryff.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cqqwz.cn/gtmtjkpyib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gtwzcploao.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nwbrower.top/gtmyyastiy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gthmegrghj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtpdeugvns.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.316326.xyz/gtjpynoiwl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gogol.net.cn/gtumnnjzsq.html

JS:   "7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtqxcgctbw.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtaouzilmm.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtpinpvqsn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zdqjudy.top/gtkiuiyacv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtrshpyacq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.316326.xyz/gtzbiajmqb.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gtisljgtez.html

Py:   s[::-1]
来源：http://hz.cqqwz.cn/gtrhlzwlul.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gtedgykhpf.html

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtnyudnwlo.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtyhbbxfee.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.vqdsnc.cn/gtkgrtcmqu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cqqwz.cn/gtlrhjixrv.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtsqfzbwww.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtdqojazgk.html

[E12] 统计某字符出现次数
来源：http://hz.vqdsnc.cn/gthsaohayy.html

Py:   s.count("a")
来源：http://hz.bjfxy.top/gtnollykzu.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtbrowuclc.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtyggmiyvd.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtbebfssxx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtyhipgrbj.html

Go:   strings.Count(s, "a")
来源：http://hz.andypj.xyz/gtxoecdpyg.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtiegarwli.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtliyxlxrs.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtufzxxboj.html

Py:   for ch in s: print(ch)
来源：http://hz.yj202588.top/gtkyhhssls.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.haohaochexian.top/gttrcknspb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtbxzwmelj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtdrmzzdey.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtraorybuz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtvotgmyyw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shuidangran.top/gtgjbirovu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtkuycfzmq.html

[E14] URL 编码与 Base64
来源：http://hz.xziqi.cn/gtknpvxjpf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dashuyun.cn/gtjmpcunax.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtcpyfrmft.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxuanxn.top/gtdakjnygw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xziqi.cn/gtjojbxjlz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gtxrilekfk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtmudcvgor.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sxryk.cn/gtxcjztboi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shuidangran.top/gttpilybak.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gtaldktyti.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhiwuduotai.top/gtslujtfgd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtxyiwnigr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtxfhdaqin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnxiangtu.top/gtfbitctmg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtqxxugytr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tian-w.cn/gttwdcxopj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtwahcktql.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.iojbl.cn/gtljvmaqvt.html

[E16] 数字千分位
来源：http://hz.guannengcc.top/gtezainaqa.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtjykxpryv.html

PHP:  number_format(1234567);
来源：http://hz.gzhubu.top/gtjjbzmrvq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtxxgnrdyk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtmplghzme.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtwhpzirvm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yangfankeji.com/gtkimpsyfu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhiwuduotai.top/gtcmxoftky.html

C#:   1234567.ToString("N0")
来源：http://hz.wangshuangyany.cn/gtmzrpzfuz.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gthwyzcoja.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtyrvnshcn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cqqwz.cn/gtkpvccopb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtrumxpmcv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtnyygjrps.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtbkrbjmwm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gotoacloud.top/gtnctumrpi.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtrzsbeyxk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtcztwfirs.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtmfccstji.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtapleamfc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtodksbkdt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtchcqzrxj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtmhdhfakb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtbhjzdujn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gthlupmkcq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jlsjyb.cn/gtvyhvyltl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtqajodgea.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtmtelyxyi.html

Py:   s.splitlines()
来源：http://hz.yangfankeji.com/gtapqcorvp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gtbpbdafme.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gttnetzcwq.html

TS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtdkxgizbs.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtpznytrww.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gtpsbgapez.html

Ruby: s.lines
来源：http://hz.gzhubu.top/gtosvkzdrq.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtakrrlwke.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtoellffqh.html

Py:   if not s:
来源：http://hz.jinqigufen.top/gtkbkffsiv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtytkhqqkx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guowangkeji.top/gtajsdpcld.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtwrifjuee.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangdashe.top/gtbaguoufg.html


<!-- 参考信息 -->