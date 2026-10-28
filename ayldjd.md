代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.birdmap.top/gtzodwfnhy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yonumen.top/gtzqhfetme.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gtmotwozwd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cucudq.cn/gtixfzczwx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtqxtonqry.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgufenzy.top/gtsqeugisd.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258888.top/gtlgribbhe.html

[D18] 扁平化嵌套数组
来源：http://hz.ydjk.org.cn/gtlsqmpaev.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj202588.top/gtwbxrbxzo.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gteomoebds.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ywan-chungtsiang.top/gtwtlyiurt.html

TS:   nested.flat();
来源：http://hz.zhixingplan.top/gtgdvgzglp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtcrmgbtmc.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtpshjgxkc.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtfkzhjchc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtsljcxnkq.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtxcjvggkg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhongyouzk.top/gtdjiiqbzp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xziqi.cn/gtjsvansmc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuanzx.com/gtsvyohupp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtrwzhbhxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangshuangyany.cn/gtvmgfquso.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtvcdmiyoz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hywenlv.cn/gtqephecsn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cucudq.cn/gtzkopluoe.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gtwaustowm.html

Py:   Counter(arr)
来源：http://hz.cdnleiting.top/gtwfcsdgrh.html

PHP:  array_count_values($arr);
来源：http://hz.xuanzx.com/gttiiykktp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtbmdqowsn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtvcrlawov.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtgngicftv.html

Go:   // 手写 map[T]int
来源：http://hz.yvedp.cn/gtepulzqss.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtmwrdubmj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtweyqplmz.html

[D21] 判断是否包含某元素
来源：http://hz.zhongyouzk.top/gtpdyzzjgm.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gtiudtpppx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtfxriasnu.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtskrxgvyp.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtjompptnb.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtqlcdaidq.html

Go:   slices.Contains(arr, x)
来源：http://hz.birdmap.top/gtjvhuhocy.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtpsayjsvc.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gthbscrekj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtwgkijcof.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtiaybhmht.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtvithffxg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigufen.top/gtceprstny.html

TS:   [...arr];
来源：http://hz.tianlin.xyz/gtjybgyvqi.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtgolnnhbq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tanke756.top/gtelovpten.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tanke756.top/gtzwqpygsp.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gtnhkgutom.html

[D23] reduce 累积计算
来源：http://hz.daxiang520.top/gtjhfxiunb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtmexuqqej.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxuanxn.top/gtyzzxnxug.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtlrgjnvcp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtyaowvtsd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tianlin.xyz/gtvzueugjy.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtheybzeth.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hammf.cn/gtcibuvesx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zdqjudy.top/gtoqantejy.html

[D24] 字典 / Map 基本操作
来源：http://hz.yanxiufei.cn/gtxyhrazqi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gtenhsyykz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtqeitgcvs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtfzhxuulc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtpjwgtpkl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtpowjmxxi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shuidangran.top/gtgkzmxfoj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtlyqafqrs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jiagoushi.top/gtkakfexbb.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtftxsywqk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gthshrpaad.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuanzx.com/gtgvavtcht.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gtphqjtrmq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xingfuxueyuan.xyz/gtsbsxwjon.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj202588.top/gtxoaqciox.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gtnhhxxjlc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtmmckdmyw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtffhqxhul.html

[D26] 数组转字符串
来源：http://hz.pycfn.com/gtypxzqjuq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydjk.org.cn/gtlpqcnzpc.html

PHP:  implode(", ", $arr);
来源：http://hz.tanke756.top/gtgsvlxpsm.html

JS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtlkprvmbh.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gthbhhpnue.html

Java: String.join(", ", list)
来源：http://hz.0kj1m.cn/gtqavjfftw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtgcttdvow.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtqzcnmhww.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtrygkhcub.html

================================================================================
来源：http://hz.snrcjt.cn/gtfoguqfxc.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtgqilucwv.html

================================================================================
来源：http://hz.sweek.top/gtumyfgibh.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangtech.top/gtagswynpw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nwbrower.top/gtubmabtjo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xinyue.icu/gtyhvtjvvj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtsbkeygaq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtebalioyb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuxming.cn/gtlxfwzwzu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtdevyqiza.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.0kj1m.cn/gtlufbjgxm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tianlin.xyz/gtnhzzfhpx.html

[E02] 重复字符串
来源：http://hz.xuetiantiany.cn/gtfjvrcctj.html

Py:   "ab" * 3
来源：http://hz.chenlongwang.top/gtiatffbhk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtrnnybisg.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtbmhkxfeg.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtxsmywtyc.html

Java: "ab".repeat(3)
来源：http://hz.52xcode.cn/gtycuyewrq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangkeji.top/gtrgkoyzdd.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtoevwtgiq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sweek.top/gtuopmghqj.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtjkhhzpab.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.316326.xyz/gtinruxjuh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gttogcyypx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtjbgbcjjp.html

TS:   s.slice(1, 4)
来源：http://hz.yongpay.top/gtfseyuzkz.html

Java: s.substring(1, 4)
来源：http://hz.havefunace.top/gtrgdifgoc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtkdumhqjj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ehwqpu.com/gtqzfydask.html

C#:   s.Substring(1, 3)
来源：http://hz.shuidangran.top/gtbrmrdual.html

[E04] 查找子串位置
来源：http://hz.hnqzz.top/gtvwcvbkjc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtlonkqvxs.html

PHP:  strpos($s, "x");
来源：http://hz.gotoacloud.top/gtannjxouo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xziqi.cn/gtrawgzrbk.html

TS:   s.indexOf("x")
来源：http://hz.kuanghao11.cn/gtkkiighha.html

Java: s.indexOf("x")
来源：http://hz.fengsongda.top/gtaqtnhfez.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtzbyptrkr.html

Ruby: s.index("x")
来源：http://hz.yongpay.top/gtaitdjxbf.html

C#:   s.IndexOf("x")
来源：http://hz.nwbrower.top/gtdgdrptqq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gtaxchsppp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gthzndskiz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.0kj1m.cn/gtxpseuquv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtxgbabcxs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtwynkaiyd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gteanjmmpn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigfzy.top/gtqqqgmosl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.316326.xyz/gtibhudklz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinghuilouyu.cn/gtkkissrxw.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtybvytxgf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gtkubxuiuq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ehwqpu.com/gtdjbqloom.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtiauwkxvu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtyjzyiyhi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtktqqqzlf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtbjqjjxun.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtjbsgeajm.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gttoqwnyzx.html

[E07] 按分隔符拆分
来源：http://hz.mhx1999.top/gtanmaswkm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yangfankeji.com/gtnvzklupk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xziqi.cn/gtnuyzmjca.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhijiandao.cn/gtyiptemsp.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtbozufhop.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtocpowfzw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtotukdwsy.html

Ruby: s.split(",");  s.split
来源：http://hz.hysaishi.cn/gtoxhcctyc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtdzabzojr.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtelwimlnx.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtxqdiaojn.html

PHP:  implode(",", $items);
来源：http://hz.jiagoushi.top/gttkgekzmu.html

JS:   items.join(",")
来源：http://hz.ehwqpu.com/gtavmzckkq.html

TS:   items.join(",")
来源：http://hz.sufxvd.cn/gtwressrhe.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gtyzurlokq.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtdcdgzcan.html

Ruby: items.join(",")
来源：http://hz.pengpengdd.cyou/gtmetfodzu.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtpubgjvze.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtwuepklvu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtsderpfvw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtbuvubabq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtynpghmag.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtcrfnoccn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtztpzhsdf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hongshengwenyu.top/gtyjxebphv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgfzy.top/gtmnvqcmts.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtzqyjnjzn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gzhubu.top/gtrtbcymxk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtxbprysrk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gtxshyhzgc.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtnvtrxrpd.html

TS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtmwwbfvmj.html

Java: String.format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtptxgrqvq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtummlsdxn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtwgqmlnnr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ydzc1.top/gtmgtnripa.html

[E11] 反转字符串
来源：http://hz.redwolf501.top/gtalsanuzv.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtcaqhkeec.html

PHP:  strrev($s);
来源：http://hz.cqqwz.cn/gtfbhznqbu.html

JS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtamuvjtmq.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtiwredisy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtnkrliris.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hammf.cn/gtocqjgniu.html

Ruby: s.reverse
来源：http://hz.aizwys.cn/gtrmvnqkxo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtkaysdxab.html

[E12] 统计某字符出现次数
来源：http://hz.fengsongda.top/gtldotjvjs.html

Py:   s.count("a")
来源：http://hz.fzhhl.top/gtlgjydrye.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gtmqnfwkxu.html

JS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtcvgtfgdz.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtazxunfgj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pycfn.com/gtomhiqbru.html

Go:   strings.Count(s, "a")
来源：http://hz.hongshengwenyu.top/gtrvbdwbqh.html

Ruby: s.count("a")
来源：http://hz.ivvv.top/gtuulngkuf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigfzy.top/gtjnghhldy.html

[E13] 逐字符遍历
来源：http://hz.nanxinkj.top/gtoprwgcbr.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigufen.top/gtuastgjvm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.0kj1m.cn/gtfwlszdwp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtwxkxalet.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtteesnmuw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtsemrqztk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hywenlv.cn/gtigjtdlrm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangshuangyany.cn/gtdwreprza.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxinkj.top/gtzaqgekea.html

[E14] URL 编码与 Base64
来源：http://hz.9152youxi.cn/gtjjmuqgja.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jianghu66.top/gtgqkqcmpq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pengpengdd.cyou/gtiurldqsf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtfihplkjp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pycfn.com/gtvuulnjsv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtfrwkfzcs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cdnleiting.top/gtzirbyxvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenlongwang.top/gteqstmbfz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.haohaochexian.top/gtvwnhzvib.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtbbilknrh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtltzefvdi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtzyjgcuno.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtzdtqqrvu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jianghu66.top/gtewcxznjp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gzhubu.top/gthpqiadxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.feifeiyinyue.top/gthgepmxve.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnxiangtu.top/gtbqlhygoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxinkj.top/gtpypgfxpw.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtgfcxgrhi.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtxkgqyqzf.html

PHP:  number_format(1234567);
来源：http://hz.yonumen.top/gtgukkhcpt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtbjeadhty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtuydrsvby.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gtbwuzijdl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.smart0.xyz/gtqlgdmcev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fengsongda.top/gtsbfswptc.html

C#:   1234567.ToString("N0")
来源：http://hz.yueranfly.top/gtykltulgi.html

[E17] 首字母大写
来源：http://hz.sufxvd.cn/gtnwzbpadz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtlddnbijp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shanyushiyangtech.top/gtyiyedgbd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtvzkfisao.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtoajasnqv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj20258888.top/gthsabxrqm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hongshengwenyu.top/gtzoguoxhx.html

Ruby: s.capitalize
来源：http://hz.sxryk.cn/gtscfklnvy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xziqi.cn/gtsacjlpcj.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtoonwnrya.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtmpxzqmbe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhongyouzk.top/gtevlagfix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtdglpoxqa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtnaqvwjnr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhengqikj.top/gtiennrkxw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sweek.top/gtwsxpqhzi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guowangkeji.top/gtnbznasyt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gtlmroktlx.html

[E19] 多行文本按行拆分
来源：http://hz.feifeiyinyue.top/gtbcaflmwp.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtwgorvsqe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtorjkvlzq.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtfqwznsix.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtyrbatvyn.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtfityvbvw.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnqzz.top/gtyacjczel.html

Ruby: s.lines
来源：http://hz.meibo888.top/gtuvnjeopx.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtqufygkhc.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtfhpdplcd.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtrefncibt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtzwoouona.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhoulong.xyz/gtyecgdznc.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtesbuiztm.html

Java: if (s.isEmpty()) {}
来源：http://hz.guannengcc.top/gtpvjpmngj.html

Go:   if s == "" {}
来源：http://hz.ydjk.org.cn/gtytiphirc.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gttimvzotl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtmjlouwra.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtckaoqorn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtauckslnl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtxelyoski.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtdmoohlmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtkdlducvr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtmftwslux.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxuanxn.top/gtatzzyfkx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtkzwcuwtp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtdtupwfsk.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtpvevxlgs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtgwkaovqf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtkoxyvogm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gteibpyclb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtowwlmeob.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aizwys.cn/gtouqxntjx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zdqjudy.top/gtxidwttdy.html

Ruby: s.bytesize;  s.length
来源：http://hz.gotoacloud.top/gtkumknsag.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtbwjfnnzl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpijfvjnj.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtzkimdjda.html

================================================================================
来源：http://hz.nanxuanxn.top/gtolptbjvt.html

[F01] 读取整个文件
来源：http://hz.yuanzhike.top/gtzoxyafgq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ppjwa.cn/gtacdfcxvd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gogol.net.cn/gtdbtjtjjb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtxsgoqssn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gtxejxttha.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gttrmeleik.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtsrhwfesj.html

Ruby: File.read("a.txt")
来源：http://hz.ivvv.top/gtgdsjdwcc.html


<!-- 参考信息 -->