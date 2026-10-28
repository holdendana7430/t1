代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgfzy.top/gtlylebrgf.html

Go:   // 手写双层循环
来源：http://hz.nwbrower.top/gtnchukupn.html

Ruby: nested.flatten
来源：http://hz.nwbrower.top/gtufvkrzfb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtrpcecgpj.html

[D19] 按字段分组
来源：http://hz.yj20258888.top/gtgbxtahkb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtnaomgapc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.birdmap.top/gtskqfvihg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtyrqavyxu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.52xcode.cn/gtnschoslr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cucudq.cn/gtxwvkwmxu.html

Go:   // 手写 map[string][]T
来源：http://hz.zhixingplan.top/gtxcdtbslb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.feifeiyinyue.top/gtlkbhleal.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtkhvplrcf.html

[D20] 统计每个元素出现次数
来源：http://hz.yuxming.cn/gtujydmizj.html

Py:   Counter(arr)
来源：http://hz.tian-w.cn/gtllumonix.html

PHP:  array_count_values($arr);
来源：http://hz.birdmap.top/gtkdyvabjd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtbcucljig.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtaasgogte.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtsfirfzly.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtfhmjsjxy.html

Ruby: arr.tally
来源：http://hz.kuanghao11.cn/gtsvxgrcwk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtshckgovs.html

[D21] 判断是否包含某元素
来源：http://hz.cdnleiting.top/gtqgzujpkz.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtlpfvvngf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtjnqrxvih.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtdcgpgeqn.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtvdwklumb.html

Java: list.contains(x)
来源：http://hz.xinyue.icu/gttdjsgray.html

Go:   slices.Contains(arr, x)
来源：http://hz.hfpthk.cn/gtagvzumpn.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangkeji.top/gtycnyxewu.html

C#:   list.Contains(x)
来源：http://hz.dashuyun.cn/gtyhqcquca.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gtkyjapqge.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtpyfruyat.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigfzy.top/gtoqoudctn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtckpxndcg.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gtacaraohj.html

Java: new ArrayList<>(list);
来源：http://hz.9152youxi.cn/gtbfevuumf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jlsjyb.cn/gtjlxmulno.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydzc1.top/gtgbzlungu.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtygddainb.html

[D23] reduce 累积计算
来源：http://hz.gogol.net.cn/gtsvzvpaun.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtzrwqnwch.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gaohongyu789.top/gtvjanqgzn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtywqujjuy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gthpookjct.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shuidangran.top/gtpusmklfn.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtzfkezfeo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zdqjudy.top/gtwdmhnjah.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gtjmqljmng.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtcizpqrsv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gtztykwslt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtxwwjlcnq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxuanxn.top/gtbamnglrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gthfzrwpjy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtfppgkecp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hammf.cn/gtnyjuqzhc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtfjixulng.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtfkutwcim.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtjfntrkzg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zycfv.cn/gtrkujpijf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtezauqmsp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtarhlydhr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.svipenyu.cn/gtoyjyusos.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gtdvtkaobt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtbadadbbm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shzxlz.cn/gtyiimobfy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhoulong.xyz/gtcqslpruj.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtidyekjhf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtchtutgcm.html

PHP:  implode(", ", $arr);
来源：http://hz.pengpengdd.cyou/gtzqmdjydn.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtgthqesxx.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtfrndjlvi.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtsfcvtxql.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtuoctzxtl.html

Ruby: arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtskklrdex.html

C#:   string.Join(", ", list)
来源：http://hz.nanxuanxn.top/gtcigggnep.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkunbsuzv.html

E. 字符串处理
来源：http://hz.iojbl.cn/gtgveguplx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcubczhqi.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtjzircgbj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangdashe.top/gtyawxlzql.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.kuanghao11.cn/gtirttqpfk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtphukgthk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtpcvdggoe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhengqikj.top/gtjsidrufo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhijiandao.cn/gtgbtlhzjm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinyuanbaomall.cn/gtvgmoxkvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtojhyvmjz.html

[E02] 重复字符串
来源：http://hz.svipenyu.cn/gtzrbecvle.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gtsbtexkjk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.smart0.xyz/gtssbculmb.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtcmcogleg.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtbpvjytoq.html

Java: "ab".repeat(3)
来源：http://hz.daria6918.cn/gtoyrrhnwv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtdmiveysa.html

Ruby: "ab" * 3
来源：http://hz.shzxlz.cn/gtfskyebpx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gtuexrtaqz.html

[E03] 截取子串
来源：http://hz.jqgufenzy.top/gthwmnpkyo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtpoepkdhp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.mhx1999.top/gtpvelzlpk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.iojbl.cn/gtqdtpdrmd.html

TS:   s.slice(1, 4)
来源：http://hz.snrcjt.cn/gtzbdctlig.html

Java: s.substring(1, 4)
来源：http://hz.andypj.xyz/gtpigrvepd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtdhtkrslj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtzutcshxw.html

C#:   s.Substring(1, 3)
来源：http://hz.zhijiandao.cn/gtiqxddjrr.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gtrkjtvgmx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtahruukck.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtmtiyordx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gtohyxmqsk.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtxxeaskdw.html

Java: s.indexOf("x")
来源：http://hz.sufxvd.cn/gtuxkxbdmb.html

Go:   strings.Index(s, "x")
来源：http://hz.gzhubu.top/gtttvqxudc.html

Ruby: s.index("x")
来源：http://hz.hongshengwenyu.top/gtlmjqzgfr.html

C#:   s.IndexOf("x")
来源：http://hz.pycfn.com/gtodznqjyd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tianlin.xyz/gtdkutmosc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenlongwang.top/gtnwiwcptn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhengqikj.top/gtfedzpyjx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gteobsrsfi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtxfxmbbuf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtlwbapwzb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gtujjmhtag.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guannengcc.top/gtzpghgflz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtbhecpryh.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtxzemvyap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtrgkcrhdn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.52xcode.cn/gtywfqkcmg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtrjnlfoaw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtyhaxcrzv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtyoqjykfg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nwbrower.top/gtgduqzacp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.birdmap.top/gtjpmdziwq.html

C#:   s.Replace("a", "b")
来源：http://hz.52xcode.cn/gtkaldbhro.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtfdixhzme.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gzhubu.top/gtwrvfnbev.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gtrvxpbgls.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gtqnrcygrn.html

TS:   s.split(",")
来源：http://hz.dashuyun.cn/gtfteysztj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fzhhl.top/gtpkkgmpdp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cdnleiting.top/gtiftjanqt.html

Ruby: s.split(",");  s.split
来源：http://hz.ehwqpu.com/gtmcclwrbx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtwgyhlwgc.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtyfxyfvms.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gteuiwvhpw.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtrgxgedjf.html

JS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtomxthkwx.html

TS:   items.join(",")
来源：http://hz.daxiang520.top/gtbvponvao.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtcfkenhwi.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gtzfipuzxf.html

Ruby: items.join(",")
来源：http://hz.ybcxt.top/gtdwpqqnfu.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtdzutosxg.html

[E09] 去除所有空白字符
来源：http://hz.cdnleiting.top/gtvsdfisll.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydzc1.top/gtgyvnwmgl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hfpthk.cn/gtfehcxglt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtcyinhwpe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtiztrxovy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gtksbbkjum.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ybcxt.top/gtopzazdbx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gtlnhfmncq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gtcktrsnvq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hongshengwenyu.top/gtnqksfiwf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.9152youxi.cn/gtsllyonlt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtkjexnryd.html

JS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtkjjuhlms.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtyejjmewu.html

Java: String.format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtanxcabvq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtwqudixwp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhoulong.xyz/gttpnytpqh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtlolbmpwu.html

[E11] 反转字符串
来源：http://hz.xziqi.cn/gtxaxpjavs.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtvmgoayfk.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtrnrxsydc.html

JS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtamizjahx.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtwyxkmnmr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtpclwflij.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gtqqfnbjzk.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtudrkhlqa.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gthhqgvvlu.html

[E12] 统计某字符出现次数
来源：http://hz.316326.xyz/gtjrdflsdj.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gtykofmary.html

PHP:  substr_count($s, "a");
来源：http://hz.sysykeji.top/gtionxggxm.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtkbnmwivk.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtxeokotxk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jyoumei.cn/gtrptcvxri.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtsbjaptll.html

Ruby: s.count("a")
来源：http://hz.hysaishi.cn/gtgegpymmy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtjssczqfp.html

[E13] 逐字符遍历
来源：http://hz.daxiang520.top/gtzaehylzr.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtyfzezlkj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gtgdezsnge.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtdkobtcyv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtxdztbckm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gtlrlzsldr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtafmlbwef.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtnrycqnvo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtlnpsdqap.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtiaahgblq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.316326.xyz/gtmsjpwhyr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ehwqpu.com/gthkqcgfnv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinghuilouyu.cn/gthlzlhdet.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigufen.top/gttwonnkru.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhengqikj.top/gteegpirun.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhoulong.xyz/gtpbrncuka.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtetgcjhhv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtiucflpvj.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinyuanbaomall.cn/gtuqnzlxeb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.316326.xyz/gtjkggxuem.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yanxiufei.cn/gtbjcwtfry.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gtwyuuoiko.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ppjwa.cn/gtwslaxtrx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.smart0.xyz/gtrylkgfcw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gteuwunlmr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangtech.top/gtlfhwpnfy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dashuyun.cn/gtsshgplbr.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtzytwypjh.html

Py:   f"{1234567:,}"
来源：http://hz.quarkkingdee.top/gtkiuleeqh.html

PHP:  number_format(1234567);
来源：http://hz.fzhhl.top/gtdisajylu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gthsazucig.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtzbmtxvuj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtrzvifzpy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hysaishi.cn/gtqixmmdui.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258888.top/gtxsdvdvvm.html

C#:   1234567.ToString("N0")
来源：http://hz.xuetiantiany.cn/gtcaxevwxm.html

[E17] 首字母大写
来源：http://hz.gzhubu.top/gtziwfduzq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yueranfly.top/gtzmhxhwnf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nwbrower.top/gttbjolwyq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gthnrhxqvf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtyjaicgvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtdzgroeho.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtgjodpvmv.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtcmbhcori.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hfpthk.cn/gtcydrogpm.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtmufqryyo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtcidtpydk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gtvpmwsngb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtirlmrczs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtnpvsilfw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtjktekmka.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtxeeroljc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gotoacloud.top/gtjboefyln.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtgksrerty.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtsubtknzk.html

Py:   s.splitlines()
来源：http://hz.yonumen.top/gtvscbfnwc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.kuanghao11.cn/gtysvixsyy.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxuanxn.top/gtknnblzvi.html

TS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtuuwkonks.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtjqivyxhz.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangkeji.top/gtmqmpdlvd.html

Ruby: s.lines
来源：http://hz.nwbrower.top/gthyxycpht.html

C#:   s.Split('\n')
来源：http://hz.sweek.top/gtlkrfwmry.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtwwedfktv.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtvrmyfjiq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dashuyun.cn/gtlksgkzhc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yongpay.top/gtifvbnwrw.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtblabkbru.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtqhbtthxi.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtdklmxddl.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtjcgzaezt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangshuangyany.cn/gtralcayvg.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtglxlqcnv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gthlrzefhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtbydbfiyp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtylnwrskf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtotpcfbct.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtxoyrrmbk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtwbmeijpl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtivjnxwie.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.svipenyu.cn/gtggynfbeh.html

[E22] 字节长度与字符长度
来源：http://hz.zhijiandao.cn/gtbztzwetg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtaskhcerc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtqoptaxfh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ivvv.top/gtqsgfftmp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtoekxxdoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gtmppoabcj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shzxlz.cn/gtmhujrrhq.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhongyouzk.top/gtlenkkelu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtfamqmazy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxxjlpiaz.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gtasgpclbg.html

================================================================================
来源：http://hz.havefunace.top/gthmkhwmwd.html

[F01] 读取整个文件
来源：http://hz.nanxuanxn.top/gtmenizwok.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtishlzair.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtffdoawty.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.havefunace.top/gtidulvgna.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtttpelnqe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtborwfenq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhixingplan.top/gtsppaimid.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtjnwvfxme.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtqbfwtnnz.html

[F02] 逐行读取文件
来源：http://hz.zhijiandao.cn/gtxuohzjfr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gtcxudmxxb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gzhubu.top/gtqioesxsy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gtbpeblinr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtlrjopulw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtaryyvmuu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xinyue.icu/gthqfwmpon.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guowangkeji.top/gttzvcwixq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtnvaoewan.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtreznqdib.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtnyikvgfb.html


<!-- 参考信息 -->