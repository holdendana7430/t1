代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.ydjk.org.cn/gtqtckbkxl.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtmwisthta.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gtpozcaprc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtfvakhljj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtuhodgcxu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jlsjyb.cn/gttzwesbcx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenzaomai.com/gtkzehhqdj.html

Go:   // 手写循环累加
来源：http://hz.nanxinkj.top/gtdqefutxd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtfaekffyb.html

C#:   list.Sum();  list.Average()
来源：http://hz.cheryme.top/gtenhdhriz.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gttdhatowz.html

Py:   max(arr);  min(arr)
来源：http://hz.havefunace.top/gtxggorpjm.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtdettjgsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtkwvtcsip.html

TS:   Math.max(...arr);
来源：http://hz.zhaomingkeji.xyz/gtrtrexike.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtlvafcrqz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.9152youxi.cn/gtszppfivw.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gtawnphhqt.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtganzmquu.html

[D18] 扁平化嵌套数组
来源：http://hz.hywenlv.cn/gtjjqjjqov.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.52xcode.cn/gtdrbisjiw.html

PHP:  array_merge(...$nested);
来源：http://hz.quarkkingdee.top/gtrrqlwqfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yanxiufei.cn/gtubgwfbtg.html

TS:   nested.flat();
来源：http://hz.zdqjudy.top/gtmwcbrlpz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtsfgpdvpb.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangkeji.top/gtksprmkzh.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtemjaeuui.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guannengcc.top/gteflwevmo.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtyeghtrtk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pengpengdd.cyou/gtjxyndeuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtfktnqpgx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangshuangyany.cn/gtxmozybuz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtwzizecky.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gzhubu.top/gtiwgpgket.html

Go:   // 手写 map[string][]T
来源：http://hz.jiagoushi.top/gthplhxgyp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtewdreoyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.0kj1m.cn/gteixdikuh.html

[D20] 统计每个元素出现次数
来源：http://hz.52xcode.cn/gtnjbksoxc.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtzbmkubhh.html

PHP:  array_count_values($arr);
来源：http://hz.haohaochexian.top/gtlxudonoj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtpjmwgkdr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtwpsztgyi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gtwidbssem.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtgwezwcqu.html

Ruby: arr.tally
来源：http://hz.shuidangran.top/gtcqndqqkp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtmeeubdsq.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtcdqoaaxu.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gtlbiibvlt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zdqjudy.top/gtuorvfsfm.html

JS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtmtrcdygw.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtygvpzbia.html

Java: list.contains(x)
来源：http://hz.hywenlv.cn/gtljbiuwau.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydjk.org.cn/gtaglmlrai.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtlefmrcrl.html

C#:   list.Contains(x)
来源：http://hz.cheryme.top/gtljqfkhhb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinghuilouyu.cn/gtptbzkqhy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtquaubaww.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtbrekoxph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jianghu66.top/gtgrtdgrhe.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtocqjwanw.html

Java: new ArrayList<>(list);
来源：http://hz.pycfn.com/gtxlwbywgr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yanxiufei.cn/gtosllrdcc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtxgklovjt.html

C#:   new List<int>(list);
来源：http://hz.andypj.xyz/gtupmjrhvt.html

[D23] reduce 累积计算
来源：http://hz.zdqjudy.top/gtwddxqxpn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtzwwhxysm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtbqspvwud.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtdlxrzkaf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gttruzjzch.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gttnqwqivj.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtmfycqest.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.0kj1m.cn/gtsqxcazme.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtdyukneeb.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtwqhgppky.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtwyxbknvr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sysykeji.top/gtmxhzaogr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sysykeji.top/gtlcwaqsgw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dashuyun.cn/gtwrmmpqhy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtxqqwbcob.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sysykeji.top/gtuhbqnkyk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shangyingyoupin.top/gtqzxvfqpi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtsxjfgeqi.html

[D25] Set 集合去重与交并差
来源：http://hz.gaohongyu789.top/gtrmgsykjv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gthwsegoap.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cashguo.top/gtxlqbxjlg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtkmimyxxi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtmesxtlrf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gtgaizcgfo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gthzuxxggs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtfaybhrhj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ppjwa.cn/gtqqosbbau.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtzfgtazyy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guannengcc.top/gtadczspxh.html

PHP:  implode(", ", $arr);
来源：http://hz.vqdsnc.cn/gtnkxyemta.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtrolpocvw.html

TS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtnqprwycm.html

Java: String.join(", ", list)
来源：http://hz.bjfxy.top/gtqdbhdctc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.9152youxi.cn/gttaqllnlv.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtdlykexrz.html

C#:   string.Join(", ", list)
来源：http://hz.zycfv.cn/gtiorodooc.html

================================================================================
来源：http://hz.daria6918.cn/gtdqdbizan.html

E. 字符串处理
来源：http://hz.jianghu66.top/gtyqtagcne.html

================================================================================
来源：http://hz.gzhubu.top/gtcxpoxgjg.html

[E01] 拼接字符串
来源：http://hz.redwolf501.top/gtoiuqsnzz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtartnqayx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ehwqpu.com/gtkjemzrwe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtulkxheac.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtqhnhhwip.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gtosjvazlx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtgqwopurv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtznmyyqff.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtzsyzzwon.html

[E02] 重复字符串
来源：http://hz.havefunace.top/gtaozvstrj.html

Py:   "ab" * 3
来源：http://hz.nanxinkj.top/gtnescfrte.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gtnwsmpipe.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtwnduecxf.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gticwjbrpp.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtnkitfavq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangdashe.top/gtfnbxcawl.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtqfavihqs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sufxvd.cn/gtggohfjdf.html

[E03] 截取子串
来源：http://hz.hnqzz.top/gtcgmxgowr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tanke756.top/gtbclmtpgk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtqwfixnax.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtegehpbtf.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtxzkmfqlz.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtfomukxaa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtuvmtaimh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yonumen.top/gtbqlglprc.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtodzmtojx.html

[E04] 查找子串位置
来源：http://hz.tian-w.cn/gtmqliomks.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aizwys.cn/gtpidtzmyp.html

PHP:  strpos($s, "x");
来源：http://hz.nanxuanxn.top/gtgxycutcp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtmdkpiagm.html

TS:   s.indexOf("x")
来源：http://hz.cucudq.cn/gtajiyssbn.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtfjccyrpa.html

Go:   strings.Index(s, "x")
来源：http://hz.fzhhl.top/gtqozjfrpu.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtjumrxaeo.html

C#:   s.IndexOf("x")
来源：http://hz.sweek.top/gtuenveukv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtselwvtlf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zdqjudy.top/gtdibsykoj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hammf.cn/gtilumdmnp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtyjbnsypg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sweek.top/gtwaltnghd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtiwmeyjbh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtplzvjgji.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gtcmsfzmfr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cqqwz.cn/gtkawzjmel.html

[E06] 替换子串
来源：http://hz.ehwqpu.com/gthykdxaxy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhixingplan.top/gtklsjlpzw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangtech.top/gtztotzvct.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtlkfwqyxo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtrawjjuvz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtlqtxxmxt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gtblfaqgxf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.quarkkingdee.top/gtdjziuvro.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtrhcnpefz.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtxupxkehe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pycfn.com/gtblunkrjm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.haohaochexian.top/gttymcqquz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ivvv.top/gtcvkiahwi.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtlrohiisy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.dianchejie.cn/gtsjehjaen.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gtvjnynzuj.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gttmoexpet.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgufenzy.top/gtaqccrupx.html

[E08] 数组按分隔符合并
来源：http://hz.hnxiangtu.top/gtngehixdw.html

Py:   ",".join(items)
来源：http://hz.wangdashe.top/gtwmuuxkiw.html

PHP:  implode(",", $items);
来源：http://hz.yanxiufei.cn/gtnmrddngi.html

JS:   items.join(",")
来源：http://hz.cheryme.top/gthvhmsqxm.html

TS:   items.join(",")
来源：http://hz.jianghu66.top/gtewoistjf.html

Java: String.join(",", items)
来源：http://hz.yvedp.cn/gtljnjsyly.html

Go:   strings.Join(items, ",")
来源：http://hz.jlsjyb.cn/gtwykxkabw.html

Ruby: items.join(",")
来源：http://hz.ybcxt.top/gtkcdfwcou.html

C#:   string.Join(",", items)
来源：http://hz.jyoumei.cn/gtbdbbuhmk.html

[E09] 去除所有空白字符
来源：http://hz.zhijiandao.cn/gtxncxtbxs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tianlin.xyz/gtydueglyy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zycfv.cn/gtmtsgbtrp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtjwuawgne.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtdlkrjpxg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtnhefyewp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gteccotnph.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtkuxwfcex.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigfzy.top/gtvgvctaww.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtezvwhytj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cucudq.cn/gtqvtqkkdj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hongshengwenyu.top/gtmzvgwoij.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtdwzhkktv.html

TS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtvooqmoxy.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtayxgjiln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtqzinjpec.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtrmuqbtto.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daria6918.cn/gtnqaxddxr.html

[E11] 反转字符串
来源：http://hz.shangyingyoupin.top/gtssnsfbrt.html

Py:   s[::-1]
来源：http://hz.xuetiantiany.cn/gtdbvktsgz.html

PHP:  strrev($s);
来源：http://hz.zycfv.cn/gtmxqhwwyi.html

JS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtsorpklwk.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtizhowqvn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yanxiufei.cn/gtxsupodpt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnqzz.top/gtndduvzwt.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtwhsclcho.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtrsfdaiom.html

[E12] 统计某字符出现次数
来源：http://hz.hammf.cn/gtafqkbjel.html

Py:   s.count("a")
来源：http://hz.sweek.top/gtbctadxjw.html

PHP:  substr_count($s, "a");
来源：http://hz.0kj1m.cn/gtqqgtkvob.html

JS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtdinwjoql.html

TS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gttqgwjxls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gthujuhicn.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtkqivjyoc.html

Ruby: s.count("a")
来源：http://hz.nanxinkj.top/gtnrhxrdab.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zdqjudy.top/gtkvrmbunc.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtihoqdlpa.html

Py:   for ch in s: print(ch)
来源：http://hz.cucudq.cn/gtdbnjfctk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtcetavooo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gthzimtuzn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtjxetdjkz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtmfqfixxr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.kuanghao11.cn/gtlubxwajt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtxspuzwmc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtefrptblp.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gtlqvcxbrg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xylfe.cn/gtbseoikgo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gtdurkxgrv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sxryk.cn/gtvkeurzyc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtgqmekjlq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yvedp.cn/gtaakbgrpx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.316326.xyz/gtjthnulfe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtujnppgyz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yvedp.cn/gtkfuqyhgj.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtetzkznnk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtawrvpcnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yvedp.cn/gtfkhrqphs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtmyphqjlx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtdzflaneu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gtskkpgtnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cqqwz.cn/gtxypemewt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hywenlv.cn/gtfwemczvw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtauikyrdp.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtwgidgaes.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gthdihxtue.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtlzkxfgru.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cdnleiting.top/gtffygsufw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gthiwvxlei.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinyuanbaomall.cn/gtymyfblpj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.kuanghao11.cn/gtdhnesdsx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtagiyoqjc.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtkkksmhwi.html

[E17] 首字母大写
来源：http://hz.kuanghao11.cn/gtmdyfhdqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.9152youxi.cn/gtgguxtjoc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtchjyvjek.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtkwmlodss.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtcgwdmdks.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yonumen.top/gtbqdrpiqp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ywan-chungtsiang.top/gtcfohxvdc.html

Ruby: s.capitalize
来源：http://hz.hfpthk.cn/gtisnicyah.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtwnibyheq.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtggygdmeu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tanke756.top/gtssjvkruf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuxming.cn/gtsnmqinlt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtgmwduscu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtfpbfjtjq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtmpwrvwpp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtjkszgyqy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gtvsnuaqnj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sysykeji.top/gtmpsaglcy.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtvejlpnne.html

Py:   s.splitlines()
来源：http://hz.yuanzhike.top/gtloaspcsh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhongyouzk.top/gtrpyznljl.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtyvcwnqiw.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtmauyvswn.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtxigmjbjw.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gttohnwiuj.html

Ruby: s.lines
来源：http://hz.wangdashe.top/gtsmbnkjdn.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtcueyqwju.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gtclpkquls.html

Py:   if not s:
来源：http://hz.0kj1m.cn/gtjyjimpfl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tianlin.xyz/gtfodriuxu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtrzzudvej.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangkeji.top/gtnelbcqxa.html

Java: if (s.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtvqpicusg.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gthbpkatjq.html

Ruby: if s.empty?
来源：http://hz.yj202588.top/gtbhrjdmbg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtasorgalk.html

[E21] 超长截断加省略号
来源：http://hz.52xcode.cn/gtomijgcyo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gtwansygfi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shzxlz.cn/gthewdnnwf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtyqqccudp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtgpvmvioj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtgdciyisk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gthnkaoehl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hammf.cn/gtebzlynhi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jlsjyb.cn/gtvugimxnw.html

[E22] 字节长度与字符长度
来源：http://hz.jyoumei.cn/gtwdmingtf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxuanxn.top/gtbuqvkhqq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtkkglngqg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtzhfonkwb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtamdduwke.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.feifeiyinyue.top/gtzlxdrzkx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhengqikj.top/gthvlkwumh.html

Ruby: s.bytesize;  s.length
来源：http://hz.ehwqpu.com/gtjvmxmptv.html


<!-- 参考信息 -->