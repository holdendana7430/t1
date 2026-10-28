代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtjcyjeojl.html

Ruby: arr.max;  arr.min
来源：http://hz.gotoacloud.top/gtenaqcppf.html

C#:   list.Max();  list.Min()
来源：http://hz.xuanzx.com/gtlyxeycbs.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gtkewtxiwe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gthbwoorxw.html

PHP:  array_merge(...$nested);
来源：http://hz.yuanzhike.top/gtqioiflwk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.svipenyu.cn/gtcikcitat.html

TS:   nested.flat();
来源：http://hz.zdqjudy.top/gtdemndrsz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jyoumei.cn/gtnktvdzzg.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtopnqncwe.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtxpzqerbg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.9152youxi.cn/gtqrkogyyd.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtniffyzyh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yongpay.top/gtlfdgvupq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtvaquxwqg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.feifeiyinyue.top/gtvxhnfhow.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtgirgzdhb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtsjnhbcdn.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtsmbmuhoi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtnsrffjzc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangshuangyany.cn/gthwnfeszg.html

[D20] 统计每个元素出现次数
来源：http://hz.gaohongyu789.top/gtodbjyimp.html

Py:   Counter(arr)
来源：http://hz.zhoulong.xyz/gtqcxncdmt.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtpentcyej.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtshbogdfm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtafzrjmtl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtqbgsvwsw.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gtbiuimvjs.html

Ruby: arr.tally
来源：http://hz.gotoacloud.top/gtsxsksrkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtpenzocfl.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtsoqqjbre.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtmyhqyzuk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtkylabyqc.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtbvkrnseu.html

TS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtxgmdykzq.html

Java: list.contains(x)
来源：http://hz.pengpengdd.cyou/gtgzfcsmbv.html

Go:   slices.Contains(arr, x)
来源：http://hz.jiagoushi.top/gtetdiegvw.html

Ruby: arr.include?(x)
来源：http://hz.dashuyun.cn/gtvnggtmql.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtjjdrputf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtndpddwex.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ywan-chungtsiang.top/gtgzdkbldv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtfpuydfkm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhengqikj.top/gtqpifdmfx.html

TS:   [...arr];
来源：http://hz.yongpay.top/gtdbcgcxuu.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtodumzxht.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hongshengwenyu.top/gtnpjlwggd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.316326.xyz/gtrlddhoyi.html

C#:   new List<int>(list);
来源：http://hz.nwbrower.top/gtrdhdywhk.html

[D23] reduce 累积计算
来源：http://hz.xingfuxueyuan.xyz/gtzrmpfomn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtzjdhfznn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtxjvpnevi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gogol.net.cn/gtqubcrqyg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtcrlwwtci.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtvbzijdce.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtcrsykfeq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhiwuduotai.top/gtdlplbjbb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gttxolxjly.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gttisfkmpj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtgklbwxfl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtonlwmtmw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtzqnzzucp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.smart0.xyz/gtvswbazax.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ywan-chungtsiang.top/gtnwhcoonx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xziqi.cn/gthitohfza.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtvvmhdkua.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tanke756.top/gthcxivzbz.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtvbuyefeo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258.top/gtkcutqfqn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtuxuijntc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtzthyidqr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhongyouzk.top/gtztqhekpq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtwvqkogsx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gthdqirmyu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sweek.top/gtprbynjid.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aibaodan.cn/gtbtepyfko.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtnniqxpkn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtkywlozgc.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtywtxjzxk.html

JS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtdrjphvlc.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gttpdlnigz.html

Java: String.join(", ", list)
来源：http://hz.pycfn.com/gtkqgluzrf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuetiantiany.cn/gtwqvgdkzz.html

Ruby: arr.join(", ")
来源：http://hz.yangfankeji.com/gtycyflmgh.html

C#:   string.Join(", ", list)
来源：http://hz.yonumen.top/gtzsgaggrm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxbzcdvyx.html

E. 字符串处理
来源：http://hz.yuanzhike.top/gtkmafxfbh.html

================================================================================
来源：http://hz.hywenlv.cn/gtdovwrsoe.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtquhywugx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.52xcode.cn/gtnslqjrzw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.redwolf501.top/gtjdfbgqxb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtaqhbzzdk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtyunvehvp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.kuanghao11.cn/gtrlrzogow.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xinyue.icu/gtrraczyuj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtomklsqvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gtyredfeow.html

[E02] 重复字符串
来源：http://hz.jinghuilouyu.cn/gtoseopowt.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtvlbuxvvt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.mhx1999.top/gtlkbbwrrw.html

JS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtuqdgyvyz.html

TS:   "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtbehpgjul.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gttrfqpygb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtgjfqznpg.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtnbwjqgbm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gtvzunucfm.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gtgkmjmnoo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.9152youxi.cn/gtzfvnpomx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gtkrzgaren.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtavpdiyhr.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gtqorcerww.html

Java: s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gthcivzson.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gotoacloud.top/gtxlrgghan.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhengqikj.top/gtkrxenoaw.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtyotgwubs.html

[E04] 查找子串位置
来源：http://hz.nanxinkj.top/gtewlzbbgf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtfqgisynn.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtlpbsnbqy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxinkj.top/gtsugihfqb.html

TS:   s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtkjfjxhnw.html

Java: s.indexOf("x")
来源：http://hz.jianghu66.top/gtuvqwcbpz.html

Go:   strings.Index(s, "x")
来源：http://hz.sxryk.cn/gtiesqwrqz.html

Ruby: s.index("x")
来源：http://hz.ydjk.org.cn/gtlnymmtfn.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gtydkenqqj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydjk.org.cn/gtggdsxrze.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ybcxt.top/gthyvkgqhv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gtbcbrpakf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtqsqdmnzg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.9152youxi.cn/gttlayfzns.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtrzbmrfdi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhijiandao.cn/gtgcwyqxyb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gthckvfccg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangtech.top/gtaoohypva.html

[E06] 替换子串
来源：http://hz.redwolf501.top/gtuqmeyvmq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gotoacloud.top/gtpkscbqbj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yonumen.top/gthiykcoct.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtgjafdvnt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtkhcykbcx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtnfhewkvt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj20258.top/gtsncecyxy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hammf.cn/gtnkegwkqm.html

C#:   s.Replace("a", "b")
来源：http://hz.ydzc1.top/gtswsvdgra.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gtsvotbeed.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xingfuxueyuan.xyz/gtjycgsdyo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shangyingyoupin.top/gtazkrysix.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pengpengdd.cyou/gtdbatcuvh.html

TS:   s.split(",")
来源：http://hz.sweek.top/gtjkveyznj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtenqfwaaa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jianghu66.top/gtbellaoyn.html

Ruby: s.split(",");  s.split
来源：http://hz.yuxming.cn/gtnryfyifk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xziqi.cn/gtcnvtiisd.html

[E08] 数组按分隔符合并
来源：http://hz.yuxming.cn/gtsbwboreq.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtoguduaue.html

PHP:  implode(",", $items);
来源：http://hz.yj20258.top/gtsnzamnkf.html

JS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtbrkxtirl.html

TS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtfgzjwecq.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gteyazztbz.html

Go:   strings.Join(items, ",")
来源：http://hz.nwbrower.top/gthlebwfhy.html

Ruby: items.join(",")
来源：http://hz.yuxming.cn/gtpojtscfx.html

C#:   string.Join(",", items)
来源：http://hz.tianlin.xyz/gtsobkanht.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtlvogregi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtvbyjrrzu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtnrmzojoa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gttuhznlge.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtdlpyamjl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtxipguzct.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenlongwang.top/gtjuomnynw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtrelbzhfq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zdqjudy.top/gtntltcons.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sysykeji.top/gturogyynq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shuidangran.top/gtphcqdech.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.quarkkingdee.top/gtlppdnfew.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gttbmjjudq.html

TS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtddsvcrwt.html

Java: String.format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtbnvblobc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj202588.top/gteqphtztz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gthfnigxbo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtupcwpjlj.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtiupmtrnr.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtcbuijdcv.html

PHP:  strrev($s);
来源：http://hz.aibaodan.cn/gtjgpgqrku.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtcbrdkcug.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtrwefesnq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtvvwqdkzc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shangyingyoupin.top/gtwbnbumub.html

Ruby: s.reverse
来源：http://hz.kuanghao11.cn/gtpurfkois.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtuygmphil.html

[E12] 统计某字符出现次数
来源：http://hz.yangfankeji.com/gtqvdctoyh.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtjqkfmpum.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtzphzoqab.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtmkzuaenv.html

TS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtfmkogqqx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shzxlz.cn/gteoyyomsd.html

Go:   strings.Count(s, "a")
来源：http://hz.cdnleiting.top/gtiocatids.html

Ruby: s.count("a")
来源：http://hz.meibo888.top/gtyrbyhtfw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.52xcode.cn/gtcbzygeuf.html

[E13] 逐字符遍历
来源：http://hz.bjfxy.top/gtrskoocul.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtcnomvaax.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zdqjudy.top/gtgtafpyzi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtpitmlpkz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtxhxxsugo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtdqwptoxq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtfydjwkds.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ivvv.top/gtphhprcyq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zdqjudy.top/gtbblddwmv.html

[E14] URL 编码与 Base64
来源：http://hz.xylfe.cn/gthgufjkkm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gttvtjvrrj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhongyouzk.top/gthghpigeq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtumtlnrfu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj202588.top/gtroylixha.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gttibgkhjj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.mhx1999.top/gtjuwttcjb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhaomingkeji.xyz/gtvzyfvjnc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtegeetcbm.html

[E15] HTML 转义 / 反转义
来源：http://hz.jlsjyb.cn/gtdylkiteg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtumtfhwgo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtzcgsvocm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pycfn.com/gtyecnpnim.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtrymjuywo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtvogywuun.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtehczgadh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ywan-chungtsiang.top/gtpyriqnoh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sufxvd.cn/gtfgnwtfui.html

[E16] 数字千分位
来源：http://hz.xziqi.cn/gttapeefdm.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigufen.top/gtzwtpcoiz.html

PHP:  number_format(1234567);
来源：http://hz.zhoulong.xyz/gtubgqftlk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtpkpyripp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtnwolwydc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuanzx.com/gtcrpgrojm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ywan-chungtsiang.top/gtoatnyscv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuanzhike.top/gtbjrlpjrt.html

C#:   1234567.ToString("N0")
来源：http://hz.wangshuangyany.cn/gtwswbhsqe.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtlscpncgh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yanxiufei.cn/gtyhhfituq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cdnleiting.top/gtntyzxynl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gttcmxrhes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtdhhcaluo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnxiangtu.top/gtdjponjgt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.feifeiyinyue.top/gtiaaalizd.html

Ruby: s.capitalize
来源：http://hz.nwbrower.top/gtdtmsaupm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gthksydmgr.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtgidctksf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.0kj1m.cn/gtoivitdjz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtkdchfffz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gthurihatt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtjntswryr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gttvggvcej.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aibaodan.cn/gtgthmufwd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xinyue.icu/gtgytmdcyn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gthiofmgpm.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtbkdrtbfl.html

Py:   s.splitlines()
来源：http://hz.gzhubu.top/gtimompekm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhaomingkeji.xyz/gtgbeiqcdl.html

JS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtvbyquwyz.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtmoncjwqz.html

Java: s.lines().toList()
来源：http://hz.zhiwuduotai.top/gtecbulmlc.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangshuangyany.cn/gtdgmzfprh.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gttxykcpbg.html

C#:   s.Split('\n')
来源：http://hz.gaohongyu789.top/gtimwalcae.html

[E20] 判断字符串是否为空
来源：http://hz.guowangkeji.top/gtojrvkbwp.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtkgquqmvx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gthlzenzpk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtcavhcqmt.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtkdtfefea.html

Java: if (s.isEmpty()) {}
来源：http://hz.sxryk.cn/gtpdygcjux.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtcvgzyvyd.html

Ruby: if s.empty?
来源：http://hz.quarkkingdee.top/gtjhnzneis.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtrwczhdat.html

[E21] 超长截断加省略号
来源：http://hz.cdnleiting.top/gteqvtxdsa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtuytrzhqi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtckyhpzmt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtqkmfblrd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtveaybegc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtrnizdquc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtfmmsstpc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtgbrgzwpg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuanzhike.top/gtawwtovab.html

[E22] 字节长度与字符长度
来源：http://hz.gzhubu.top/gtghlzixzp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuanzx.com/gtiakoaesp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtodvfugfq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtjgrwihvs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtatdhheeb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigufen.top/gtxpbgjrcy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtkkayvgtd.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtwcxxupvo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtlczagnqs.html

================================================================================
来源：http://hz.kuanghao11.cn/gtonbkeocy.html

F. 文件与目录
来源：http://hz.jinqigufen.top/gtlctoqgwc.html

================================================================================
来源：http://hz.yvedp.cn/gtwllcnnhz.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gttclvafac.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhiwuduotai.top/gtjajpykrp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gtgjrfrpmw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sysykeji.top/gtkkxpoupe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtlrrsllbr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtcfaqfcab.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tian-w.cn/gttxlahwuk.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtdlgexhqc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtjkspjwgf.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gthpzfmfhx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtmdxrnyji.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtkrxjpkxn.html


<!-- 参考信息 -->