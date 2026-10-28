代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cashguo.top/gttjxywuxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gtjibkdlqe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtjljrendt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtaqghnlep.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtodtedice.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gtptzxxlrk.html

JS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtqdlauzqt.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtyzoehhox.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtmjdxmaye.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtaxltdxom.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtnbuzycwx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydjk.org.cn/gtpctvfmey.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtbnhphvnk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtkbpgzdam.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtdcztqbfc.html

JS:   [...new Set(arr)]
来源：http://hz.yangfankeji.com/gthttscubo.html

TS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtbhxwfrve.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtnbrknegm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtzfoywiqw.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtgaphwarx.html

C#:   list.Distinct().ToList()
来源：http://hz.yueranfly.top/gtqyxsasil.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtywvjjsrk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.9152youxi.cn/gtzyytgzyi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinqigfzy.top/gtslxzvepp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtvdkmzjvi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtecidbpdo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtcoxkcswv.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtctiqiaza.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtpotdnbnr.html

C#:   list.Sum();  list.Average()
来源：http://hz.yangfankeji.com/gtyvbeurfe.html

[D17] 最大值与最小值
来源：http://hz.yongpay.top/gtddugbsbr.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtmqjdtpai.html

PHP:  max($arr);  min($arr);
来源：http://hz.aibaodan.cn/gtkkbboeod.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtwfddmnrg.html

TS:   Math.max(...arr);
来源：http://hz.ybcxt.top/gtmgqnhaat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtulrrqxeh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.birdmap.top/gtwoushzlw.html

Ruby: arr.max;  arr.min
来源：http://hz.wangdashe.top/gttnvpxauk.html

C#:   list.Max();  list.Min()
来源：http://hz.hnqzz.top/gtvyesqnxf.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtwveypfmw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtfticdwxb.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtmagjtffd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258888.top/gttuomgwjj.html

TS:   nested.flat();
来源：http://hz.jqgufenzy.top/gtwczlebpd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtebempbii.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gtqyqvkamd.html

Ruby: nested.flatten
来源：http://hz.yj202588.top/gtlazfxioa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuanzhike.top/gtkyddbsrm.html

[D19] 按字段分组
来源：http://hz.redwolf501.top/gtkjhqoasd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtjborlokg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtuwsqbgfd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtaccfpawf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtpbxkypja.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenzaomai.com/gtygxnxawl.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtkwicyens.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shzxlz.cn/gtkdabqtxx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.52xcode.cn/gtfpdyapxp.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtvgaansxf.html

Py:   Counter(arr)
来源：http://hz.yuxming.cn/gtkxtxvuyw.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtnuhxegdr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtqwawbzef.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtxddswrgh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.meibo888.top/gtsfpcwhux.html

Go:   // 手写 map[T]int
来源：http://hz.shuidangran.top/gtxghyafbv.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtsvfapdqu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtvynwghbs.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtqcrqzkzm.html

Py:   x in arr
来源：http://hz.yuxming.cn/gtnydsvxhe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtvbrgjmsy.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gthniattsz.html

TS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtvhyotfxe.html

Java: list.contains(x)
来源：http://hz.ppjwa.cn/gtnbnbvkdf.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtocannicl.html

Ruby: arr.include?(x)
来源：http://hz.tianlin.xyz/gtasmzyxtc.html

C#:   list.Contains(x)
来源：http://hz.yj20258.top/gtxrvngsyz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtqfsafebw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hammf.cn/gtnmhaooyh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtybufquye.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhoulong.xyz/gtkdhwzmos.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtdxvnyaiq.html

Java: new ArrayList<>(list);
来源：http://hz.hysaishi.cn/gtorilussd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hfpthk.cn/gtuqjrhrnv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj202588.top/gtgzehwwao.html

C#:   new List<int>(list);
来源：http://hz.smart0.xyz/gtjbqvgzhg.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtufkehvwv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtdazkodry.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtshdorohh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtcxckiyxn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gttzwzvvgx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydzc1.top/gtwpnvsfcz.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtxrrrtixq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnqzz.top/gtqrifenbd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtwppcueud.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuxming.cn/gthddzyxaa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.kuanghao11.cn/gtxjozvxsm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxuanxn.top/gtfcipkwoy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cdnleiting.top/gtbinpupmb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtrywctivp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhixingplan.top/gtsnjgthch.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangkeji.top/gtnulfzunx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gteshfbtsm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtubuqepzj.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtznfqrhjk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenzaomai.com/gtzratnxae.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtlztgcvrz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtzwyirete.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fengsongda.top/gtzvivehbb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhongyouzk.top/gtuxuzchvj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtbnoiupbv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pengpengdd.cyou/gtlyfmmayn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtkxycddek.html

[D26] 数组转字符串
来源：http://hz.yvedp.cn/gtcglfkmkm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hongshengwenyu.top/gtiqrypqrf.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtwteuiwud.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtommkkhbt.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtqeqadjck.html

Java: String.join(", ", list)
来源：http://hz.wangshuangyany.cn/gtxzfexwdm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhengqikj.top/gtillnzoum.html

Ruby: arr.join(", ")
来源：http://hz.jiagoushi.top/gtkvvrecqw.html

C#:   string.Join(", ", list)
来源：http://hz.cdnleiting.top/gtmdmtolhg.html

================================================================================
来源：http://hz.yj20258888.top/gtattrnciy.html

E. 字符串处理
来源：http://hz.pengpengdd.cyou/gtpnqdzyco.html

================================================================================
来源：http://hz.hnqzz.top/gtdntextxh.html

[E01] 拼接字符串
来源：http://hz.shzxlz.cn/gtxfzwfzuv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aizwys.cn/gtzreroexu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shzxlz.cn/gtmukrqtak.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtofepcejl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtijpquhud.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shuidangran.top/gtavgstwes.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gttwmiftdh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jlsjyb.cn/gtoqmvhuoj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hfpthk.cn/gtyenpmgey.html

[E02] 重复字符串
来源：http://hz.hnxiangtu.top/gtodamgzde.html

Py:   "ab" * 3
来源：http://hz.nanxuanxn.top/gtrikumulp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sufxvd.cn/gtozjlthrq.html

JS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtlmgynzlp.html

TS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtqbwbcaia.html

Java: "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtuuyqeprg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtypwmbeaf.html

Ruby: "ab" * 3
来源：http://hz.ppjwa.cn/gtzgmdqtei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtleftzhkp.html

[E03] 截取子串
来源：http://hz.sysykeji.top/gtyazredub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhiwuduotai.top/gteeklrzdz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtfhhztrxb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtvuiifkkz.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtwkzqxnde.html

Java: s.substring(1, 4)
来源：http://hz.yuxming.cn/gtstuphwuj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.0kj1m.cn/gtcrxzgvum.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sufxvd.cn/gtpbwovauf.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtzggqnqcu.html

[E04] 查找子串位置
来源：http://hz.kuanghao11.cn/gtwpkpzowt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.bjfxy.top/gtpqihdeqg.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gtkxmvvuhq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nwbrower.top/gtrwjcaoon.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtnxkaxsas.html

Java: s.indexOf("x")
来源：http://hz.birdmap.top/gtvouuqjci.html

Go:   strings.Index(s, "x")
来源：http://hz.gogol.net.cn/gtaeunjnhh.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtwotepiwg.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gttmxlijla.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jianghu66.top/gtswpaywtv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hfpthk.cn/gtcebfefmm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.vqdsnc.cn/gtkfbaofxd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gthwmkrnea.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xingfuxueyuan.xyz/gtbjebmsfm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtsbgrpgtv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtgquvykmj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.haohaochexian.top/gtpwdgggrt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fengsongda.top/gtqhjsflcr.html

[E06] 替换子串
来源：http://hz.gotoacloud.top/gteofyaxsj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtznocujnw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.birdmap.top/gtnzhzdkgk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtvlkfejdu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtwrerlxdy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtiicqhjxj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yongpay.top/gtsimpnvze.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ehwqpu.com/gttdxqgein.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtfivywjet.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangkeji.top/gtrxcnqebd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtqcdabwng.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenzaomai.com/gtllurxuqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnqzz.top/gtpfzybjbp.html

TS:   s.split(",")
来源：http://hz.pengpengdd.cyou/gtpmbgycag.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtxszozpod.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.meibo888.top/gtfmdtjtsm.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtbnxziwrr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ehwqpu.com/gtpoonnkte.html

[E08] 数组按分隔符合并
来源：http://hz.vqdsnc.cn/gtvjkupbap.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtvlocjdjy.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtsaesghdw.html

JS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtgqzdasls.html

TS:   items.join(",")
来源：http://hz.xuetiantiany.cn/gttggskbcl.html

Java: String.join(",", items)
来源：http://hz.ehwqpu.com/gtxcqxjgml.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtvzpwmeaw.html

Ruby: items.join(",")
来源：http://hz.gotoacloud.top/gtygiuidbc.html

C#:   string.Join(",", items)
来源：http://hz.yanxiufei.cn/gtusfsibkq.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtujwaozdr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtqgppqutr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yuxming.cn/gtjgmtuvgl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtrvhqhtrr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtedgivquk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtgvdmzdbx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jianghu66.top/gtenxuwauu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yangfankeji.com/gtelvikbab.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gtewrurnwq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenjidiqi.icu/gtiyraqatj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtkhuaupfl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zdqjudy.top/gtjfcehcgn.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtlhhcrpgn.html

TS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtimhupogy.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtzwwiofbf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jyoumei.cn/gtkbfnrmcq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydzc1.top/gtcuzmhcal.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gthethwtzy.html

[E11] 反转字符串
来源：http://hz.jinghuilouyu.cn/gtmtsmqcdt.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtsrszhggn.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtkroaorve.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtapdckenz.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtqzkdyfsd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sufxvd.cn/gteqchqiwa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtzruampid.html

Ruby: s.reverse
来源：http://hz.ppjwa.cn/gtxkqupdfb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtcelnyomi.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gtllajpwdr.html

Py:   s.count("a")
来源：http://hz.vqdsnc.cn/gtgrsyuyvi.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtwvdbdmsr.html

JS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtqienxafp.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtifbxgzcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtscmtmqtp.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtvqubmmxc.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gtykwdfzlx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtjupwvbjs.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gtgpruvqsz.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtxrcelqrv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hongshengwenyu.top/gtoashiunc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtpathmjlx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtypvfzpif.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hywenlv.cn/gtjnziniig.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tian-w.cn/gtyclmaqri.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gtbjsdphek.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtqeozsryi.html

[E14] URL 编码与 Base64
来源：http://hz.zhaomingkeji.xyz/gthjeumisj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtdilpllrf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shzxlz.cn/gtqprxkeqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tian-w.cn/gttlfigeqx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtzwtllgak.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gtxaqkhlzv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.bjfxy.top/gtmeqxqpgv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hongshengwenyu.top/gtejhlwoth.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gtkdxjucjm.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtmrghwyip.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xylfe.cn/gtskqmzqyz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtleuwchln.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gzhubu.top/gtshvqtcrs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aibaodan.cn/gtvyheyvqm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtfohpfrnd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtteaihcua.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dianchejie.cn/gtjjmmcgdx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtnsznhleu.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtswefsvvq.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gtlageohqh.html

PHP:  number_format(1234567);
来源：http://hz.yongpay.top/gtuediyuna.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtzmtgurss.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtbhqqooqv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigfzy.top/gtyjiegqow.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sxryk.cn/gtwhccnbjq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtimwtlnpx.html

C#:   1234567.ToString("N0")
来源：http://hz.316326.xyz/gtwcbikweu.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtdzxngeby.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xinyue.icu/gtuyawgnzc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zycfv.cn/gtgcrgxwro.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtqipcjnri.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gteroernfj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhongyouzk.top/gtnbirneso.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hysaishi.cn/gtmvkzbbkw.html

Ruby: s.capitalize
来源：http://hz.jinyuanbaomall.cn/gtqwqjanjg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtpspuiiyq.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtjgqnduee.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tian-w.cn/gtnmztkudq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gtcjzkgcnm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtgmkihfjb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtpwaejvqd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtvlnxtfak.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gtormrpzwh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtpokfpwfx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtmkihacpx.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtaftahiyd.html

Py:   s.splitlines()
来源：http://hz.xylfe.cn/gttbtaulut.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sufxvd.cn/gtbdcwwdhe.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtbljljkqw.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtxsnpgclo.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtxfkazuvc.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinqigfzy.top/gtkikvpgbt.html

Ruby: s.lines
来源：http://hz.tianlin.xyz/gtegziwnfh.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtmfovktem.html

[E20] 判断字符串是否为空
来源：http://hz.jyoumei.cn/gtvhrxpbdm.html

Py:   if not s:
来源：http://hz.cheryme.top/gttnvqxghk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gttgppkifv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnqzz.top/gtjrakoyep.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gtgcmbijjx.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtsjjmoyna.html


<!-- 参考信息 -->