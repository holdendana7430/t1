代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.vqdsnc.cn/gtlykjjenh.html

Java: Collections.reverse(list);
来源：http://hz.sweek.top/gtqkfpnito.html

Go:   slices.Reverse(arr)
来源：http://hz.smart0.xyz/gtqfqooawz.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gttydpjhoy.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtvauzuvcp.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtffrjkwom.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuanzhike.top/gtvqaqbhyu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.9152youxi.cn/gtkaugadyf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gttxdgcvmr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gttdigndry.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.bjfxy.top/gterthcaoc.html

Go:   slices.Index(arr, x)
来源：http://hz.jinghuilouyu.cn/gtwwdqyrai.html

Ruby: arr.index(x)
来源：http://hz.hongshengwenyu.top/gtxubtrkds.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtbvkzepdg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dianchejie.cn/gtnweamiop.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhongyouzk.top/gtwmtmxizi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtrznbcfej.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtozwqrddb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtwzsyrcam.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ivvv.top/gtekvnjgkx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.kuanghao11.cn/gtglkvioxz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gtrehcxgjf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pengpengdd.cyou/gtnxuiwtod.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtnkwqfpoe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yongpay.top/gtnsvgqsyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnxiangtu.top/gtmshzrsqu.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtixuperwj.html

TS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtzcinohye.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtljxhttkc.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtdkrthvzq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gtkskeomnv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigfzy.top/gtlvysmvzu.html

[D15] 去重
来源：http://hz.fengsongda.top/gtjixdnyfg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtovyzkooy.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtsqyizkzi.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtbvvcbyws.html

TS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtcjgwoyjb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhoulong.xyz/gtgthcfpcr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtjadnfcya.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtrawsdbdk.html

C#:   list.Distinct().ToList()
来源：http://hz.jiagoushi.top/gthuqokgra.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gtclgpfjtu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhijiandao.cn/gtiozzoqsq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtrtffxrno.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtolzjcifd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtgjogdujm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yonumen.top/gtdxefocvv.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtlmiisubd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtkemfszor.html

C#:   list.Sum();  list.Average()
来源：http://hz.daxiang520.top/gtlsszdiiq.html

[D17] 最大值与最小值
来源：http://hz.jinqigufen.top/gttpvppxnh.html

Py:   max(arr);  min(arr)
来源：http://hz.zhiwuduotai.top/gthrapqgmu.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtiblkkhlo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtxjherkrj.html

TS:   Math.max(...arr);
来源：http://hz.zycfv.cn/gtawebuofd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtoodfdngw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhaomingkeji.xyz/gtmrbdbdcy.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtsqgrxbhu.html

C#:   list.Max();  list.Min()
来源：http://hz.ehwqpu.com/gtsfudmavu.html

[D18] 扁平化嵌套数组
来源：http://hz.quarkkingdee.top/gtlmxlypfe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ppjwa.cn/gtcjizoeqv.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtkpdkbpul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtndjznapg.html

TS:   nested.flat();
来源：http://hz.daxiang520.top/gtjsrtunem.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.svipenyu.cn/gtydwfupfh.html

Go:   // 手写双层循环
来源：http://hz.havefunace.top/gtyaqsdhuj.html

Ruby: nested.flatten
来源：http://hz.bjfxy.top/gtprwudksn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daxiang520.top/gtmpmaqyuj.html

[D19] 按字段分组
来源：http://hz.cdnleiting.top/gtsjqrshdq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gtwassdqxa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxinkj.top/gtoptpyqbk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.mhx1999.top/gtiihmdrox.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gtvtsspgtx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yueranfly.top/gtfgkmqzzz.html

Go:   // 手写 map[string][]T
来源：http://hz.gzhubu.top/gtmfbmrbrq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtuiwvtlcd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jlsjyb.cn/gtbomuwyjx.html

[D20] 统计每个元素出现次数
来源：http://hz.tanke756.top/gtmhitoedi.html

Py:   Counter(arr)
来源：http://hz.andypj.xyz/gtnvncdyzx.html

PHP:  array_count_values($arr);
来源：http://hz.shangyingyoupin.top/gtudsjdtwm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtdfdhivbb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtdzposbjt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jyoumei.cn/gtzihaxmfs.html

Go:   // 手写 map[T]int
来源：http://hz.zycfv.cn/gthmvsvcln.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gtmzuliiqy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gthnrfncqg.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtscaxddxi.html

Py:   x in arr
来源：http://hz.ydjk.org.cn/gttjtazvzq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtvtcgagqm.html

JS:   arr.includes(x)
来源：http://hz.redwolf501.top/gtjjidzonl.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtcbcdjaox.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtdzpjotbm.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gthihmnidd.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtiwxkvisn.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtlfybzzvg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.meibo888.top/gtaclaeyqk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.andypj.xyz/gtgwisnckl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sysykeji.top/gtqwqrcdsm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtmhpgowlw.html

TS:   [...arr];
来源：http://hz.jinqigufen.top/gtadmejxii.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtdoightcj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sxryk.cn/gtxtbdvjth.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtqgncgffi.html

C#:   new List<int>(list);
来源：http://hz.xziqi.cn/gtegltgazn.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtuwnfgoqa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gotoacloud.top/gtrpnvzuwu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hongshengwenyu.top/gtdtdgvycy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtcmzaqpan.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtvodjqakh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ivvv.top/gtcoosoiiq.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtjfwaskcr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtwsdcpruv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258.top/gtxjgvaxww.html

[D24] 字典 / Map 基本操作
来源：http://hz.gotoacloud.top/gtaladvjwo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hfpthk.cn/gtpcpieqaw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtubkeirnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jlsjyb.cn/gtotppdlfk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aibaodan.cn/gtnhgthxlf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gtqickexjq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtutwamtrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.c1oappe.top/gticqlpmto.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yongpay.top/gthquwmuxs.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangkeji.top/gtoedtbsrm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtcytpquvt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.meibo888.top/gtbprnfaeg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtciqakkqx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aizwys.cn/gtjxtqshws.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daxiang520.top/gthclcfawl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtrttnuktc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtmrtjfmsx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtvnrkalzm.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtphxwfzss.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtwwddvhvb.html

PHP:  implode(", ", $arr);
来源：http://hz.dashuyun.cn/gttrugncgu.html

JS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtmogrhnic.html

TS:   arr.join(", ")
来源：http://hz.yonumen.top/gttphqauen.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtknwniyzq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtmlzhegcy.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gtvlcewzwx.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtfqdssujb.html

================================================================================
来源：http://hz.jinqigufen.top/gtuxzsncoe.html

E. 字符串处理
来源：http://hz.xylfe.cn/gtnyrmuajs.html

================================================================================
来源：http://hz.quarkkingdee.top/gttfuhqnay.html

[E01] 拼接字符串
来源：http://hz.jlsjyb.cn/gtvginfbly.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhiwuduotai.top/gtwqzsxxlq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dianchejie.cn/gtuykuhiej.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gtguigopxj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtxwftbnlo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xingfuxueyuan.xyz/gtzsmnbits.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gtnwiaepze.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.bjfxy.top/gtelssgaiq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tianlin.xyz/gtiofxetbu.html

[E02] 重复字符串
来源：http://hz.ydzc1.top/gtmbrhpncd.html

Py:   "ab" * 3
来源：http://hz.ivvv.top/gtsfylpbqq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtgordvnof.html

JS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtkzaqwgzw.html

TS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtirjlriow.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtbblgdjkv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gtqguohzvg.html

Ruby: "ab" * 3
来源：http://hz.zycfv.cn/gtmrquaqwo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtvzikxbos.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtibgdfjsr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnxiangtu.top/gtryouvxwk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtgmerxrxu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yvedp.cn/gtgqybepnb.html

TS:   s.slice(1, 4)
来源：http://hz.gaohongyu789.top/gtipzxppka.html

Java: s.substring(1, 4)
来源：http://hz.yj20258888.top/gtiwoytltf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuanzx.com/gtznmimnkg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.vqdsnc.cn/gtscgksceh.html

C#:   s.Substring(1, 3)
来源：http://hz.ywan-chungtsiang.top/gtafpvfpjo.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gtqnavvgmo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aizwys.cn/gtthrivnjv.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtpytirszk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gaohongyu789.top/gtvdcnfvrb.html

TS:   s.indexOf("x")
来源：http://hz.ydjk.org.cn/gtcwmrjvho.html

Java: s.indexOf("x")
来源：http://hz.yj202588.top/gtlnygqypq.html

Go:   strings.Index(s, "x")
来源：http://hz.pengpengdd.cyou/gtwjgyyhxt.html

Ruby: s.index("x")
来源：http://hz.meibo888.top/gtqpjkcbtz.html

C#:   s.IndexOf("x")
来源：http://hz.yvedp.cn/gtvsaglovg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shuidangran.top/gtoknvgslk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sufxvd.cn/gtwlvqhgrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtpahctpny.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gttwffvqrm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtuhpuioqi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtliwdsoqp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxuanxn.top/gtnlubvlsd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258.top/gtdqftadwl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtyrrmskta.html

[E06] 替换子串
来源：http://hz.chenjidiqi.icu/gtmqtvcjqh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258888.top/gtkygfcmph.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cheryme.top/gtuukimiag.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtvlcqpuxv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtimmuixoe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtawdzupqd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.haohaochexian.top/gtswskjcbd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hammf.cn/gtjplonfko.html

C#:   s.Replace("a", "b")
来源：http://hz.zhiwuduotai.top/gtdqpkpzys.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtodjjxtun.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnxiangtu.top/gtuiussmww.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtdtbgvngl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yanxiufei.cn/gtdlwlmigv.html

TS:   s.split(",")
来源：http://hz.jinqigfzy.top/gtrsekwjiu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtdotqsltt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cdnleiting.top/gtygzudoxk.html

Ruby: s.split(",");  s.split
来源：http://hz.hammf.cn/gtjtrflwrp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gtfysfkavs.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtldjicxnm.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtfyfalupu.html

PHP:  implode(",", $items);
来源：http://hz.bjfxy.top/gtbyoylzva.html

JS:   items.join(",")
来源：http://hz.svipenyu.cn/gtuhsdjcqd.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtjzfiytbx.html

Java: String.join(",", items)
来源：http://hz.kuanghao11.cn/gtfsjeeukz.html

Go:   strings.Join(items, ",")
来源：http://hz.c1oappe.top/gtjbebqppo.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gthdyaafho.html

C#:   string.Join(",", items)
来源：http://hz.yuanzhike.top/gtykbxhptx.html

[E09] 去除所有空白字符
来源：http://hz.wangdashe.top/gtrtqpaljy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtrjfneqjj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtsxhhkdpy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtcxdavtgh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtwdcuhnan.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinyuanbaomall.cn/gtnwpxxqac.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtniedxqpi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhijiandao.cn/gtxpnqkovh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtdjsjashr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangtech.top/gtwumfuqdr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtxdxfnqtu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sxryk.cn/gtpfvifhiz.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtlejhqetu.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtnywpijpe.html

Java: String.format("%03d", 7)
来源：http://hz.aibaodan.cn/gteibwjuyg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtrpvipubx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gttucwntre.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gtxwfqatei.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gtmbphpsht.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtmwcrybzm.html

PHP:  strrev($s);
来源：http://hz.tianlin.xyz/gtzdarrckk.html

JS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtgnqebrxy.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtshcpwkvh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxinkj.top/gttucbgetg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtqsqycsyu.html

Ruby: s.reverse
来源：http://hz.wangshuangyany.cn/gtmmflotqk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtwqgrqukc.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtpxulopsv.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gtjxtngjjk.html

PHP:  substr_count($s, "a");
来源：http://hz.pengpengdd.cyou/gtlnoxidzv.html

JS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gtccmxopjm.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gttquzctwt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.9152youxi.cn/gtoyfyhpbc.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtgijmrwve.html

Ruby: s.count("a")
来源：http://hz.xinyue.icu/gtcuazviuc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtjulnfcbl.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gthswcawnh.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtqrrnyuft.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtoauikfxh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtlvakcaja.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtpilbcmgp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gthrvvxfvz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtwqchjtsm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtlylrzojc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hongshengwenyu.top/gtjcemyxxu.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtcslhpbll.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.c1oappe.top/gtkabhyufj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj20258.top/gtwnifkccr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtskarzvtj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuxming.cn/gtvicqvdpp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtypxagweu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtiedfuvut.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtufvzozrq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.mhx1999.top/gtkrlhbzfp.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gtczcwhebg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.316326.xyz/gtygxtlyya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtgusxqqmu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pycfn.com/gtoycqgsny.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtjycjggzm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtjqjtwtve.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtfznrxblk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gtgtqbjhvm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtxllbored.html

[E16] 数字千分位
来源：http://hz.zycfv.cn/gttfqfviss.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtrptabbtw.html

PHP:  number_format(1234567);
来源：http://hz.sysykeji.top/gtyancsjkm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gthavmtgbp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtzmtswtvn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gttjderoju.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yangfankeji.com/gtuagzrqxp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sysykeji.top/gtftpuqhim.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigfzy.top/gtcaknlhtt.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtmsnpmpqv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtxxgkzhje.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtmkvvdfqz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtlbupuswv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtguaffjnd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtjgxviajo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zycfv.cn/gtsojtcghz.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtrkdmhidb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigfzy.top/gtjsoofhnx.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gthctmzbve.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.aizwys.cn/gttzofmvsy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtvnmwnhcc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtcyovxgxs.html


<!-- 参考信息 -->