代发 wailian999

Ruby: arr.index(x)
来源：http://hz.hnxiangtu.top/gtrvlrkluk.html

C#:   list.IndexOf(x);
来源：http://hz.daxiang520.top/gtoybhrhrf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtrbkmvtig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jyoumei.cn/gtzbiypqsm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258.top/gtjjtqhoin.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gttlwyspeo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gthmnrsslx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtkstgfxnx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtxuaiiddg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gtxemdyxca.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.52xcode.cn/gtjwcybxbo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xylfe.cn/gtwbiyoxxu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pengpengdd.cyou/gtjarxlmsc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtdldiwkdb.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtueukxhrs.html

TS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtyhvmlnhq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtxobytwdv.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtrqtazuwa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuetiantiany.cn/gtsixdfxeo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtvxxrbbyq.html

[D15] 去重
来源：http://hz.yuanzhike.top/gtgtbvbcom.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gtzipqhgyq.html

PHP:  array_unique($arr);
来源：http://hz.cheryme.top/gtqgqglogb.html

JS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtldpffinc.html

TS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtyeqbwkns.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtyrsvoppq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtmowurzhm.html

Ruby: arr.uniq
来源：http://hz.yj202588.top/gtsgkhuyim.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gtxgxewxec.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtljawlhtw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gtpythppqq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtnzupzdfd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtwoepwmnt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtfmxkpgrt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtayskintk.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtrxfbjiqd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jianghu66.top/gtiuzwuwex.html

C#:   list.Sum();  list.Average()
来源：http://hz.gotoacloud.top/gtsqaggild.html

[D17] 最大值与最小值
来源：http://hz.zdqjudy.top/gtxvfmwdtc.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gtkdpwmosa.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gtjkzogjny.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtryeavyhl.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtzbhhuxzy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jyoumei.cn/gtjcjcznde.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtgexzlkkm.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gttvwhfqbw.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtfhoebgma.html

[D18] 扁平化嵌套数组
来源：http://hz.chenjidiqi.icu/gttkzmrxos.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtxxsfqadi.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtrwkgbcbs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sysykeji.top/gtwbmkygwl.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtsfoztctq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gtmwdhezks.html

Go:   // 手写双层循环
来源：http://hz.xziqi.cn/gtudqmztcu.html

Ruby: nested.flatten
来源：http://hz.iojbl.cn/gtnaqiyhen.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtlmudfswt.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gtkymfxccj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.0kj1m.cn/gtutcyybhc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtiizxrjhf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sufxvd.cn/gtcyeztdqy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtlbyfwpnx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtftdkdylf.html

Go:   // 手写 map[string][]T
来源：http://hz.nwbrower.top/gteeuuejnm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.redwolf501.top/gtsllaiidx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sweek.top/gtvwllbptf.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtsmntxsny.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangkeji.top/gtsemtpper.html

PHP:  array_count_values($arr);
来源：http://hz.cashguo.top/gtvefbkxff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtydjrwynj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtkgytgltd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtsurzqncx.html

Go:   // 手写 map[T]int
来源：http://hz.yuxming.cn/gtwryxmlxl.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtfreflyqq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtvnanjmsc.html

[D21] 判断是否包含某元素
来源：http://hz.andypj.xyz/gtbfwojbdj.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtwbyiqhau.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgfzy.top/gtpabhtcoc.html

JS:   arr.includes(x)
来源：http://hz.cheryme.top/gtyeeprooa.html

TS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtdoomkmpl.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtbvpquhka.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenzaomai.com/gtecihedjb.html

Ruby: arr.include?(x)
来源：http://hz.haohaochexian.top/gtsuftgfex.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtdqavrqwd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtxobmzpwr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dashuyun.cn/gtwxtitkgj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guannengcc.top/gtcaxbshgi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangdashe.top/gtxagvdazc.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtucphqdsf.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtvgctwbjf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cucudq.cn/gtqhhmacdh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigufen.top/gtvzvckusy.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtwnfuhter.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtsplqeytc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtkktrsbfa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guowangkeji.top/gtilspxvtk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtnmciueth.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtfrfothiu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtcmbmrhgq.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtaqxvopvi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.mhx1999.top/gtyksvjryk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtqydnllqg.html

[D24] 字典 / Map 基本操作
来源：http://hz.xziqi.cn/gtoqcsefcu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtqorehqgh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jlsjyb.cn/gttqqekifd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gteisqefoj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtairiibci.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtgwyprqrm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ybcxt.top/gtmissiglz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuxming.cn/gtrrasymau.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigufen.top/gtxwbxlxuz.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtdqorghrf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtqykzszha.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtinhklkbo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtpbrtmneb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gaohongyu789.top/gtrysbigmi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.bjfxy.top/gtingfkwuo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sufxvd.cn/gtwnvukcnw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtchrponjd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtniucosww.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtczmmyomw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtcnjdvddd.html

PHP:  implode(", ", $arr);
来源：http://hz.snrcjt.cn/gtekkitqcp.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtaiappzlx.html

TS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtwchrdpnn.html

Java: String.join(", ", list)
来源：http://hz.smart0.xyz/gtmparkkwb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhixingplan.top/gteoirylzg.html

Ruby: arr.join(", ")
来源：http://hz.meibo888.top/gthtnafozb.html

C#:   string.Join(", ", list)
来源：http://hz.c1oappe.top/gtppazdicu.html

================================================================================
来源：http://hz.xylfe.cn/gtbsxljwhk.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtiurtpgco.html

================================================================================
来源：http://hz.yj202588.top/gtulkirmkg.html

[E01] 拼接字符串
来源：http://hz.smart0.xyz/gtwdcdvvac.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.guowangkeji.top/gtwioicamt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuxming.cn/gtlcuhunsm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtsnfvgafp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtzphzolha.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gtrokeaeuq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtfhxyatnx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtoserheui.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sxryk.cn/gtvkgrziwo.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtyjwfxnbq.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtnrlhdhga.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtdtvqptpf.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtaumchmvu.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gttnqfxwei.html

Java: "ab".repeat(3)
来源：http://hz.yonumen.top/gtravaacbz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jianghu66.top/gtsjjpqeiv.html

Ruby: "ab" * 3
来源：http://hz.yanxiufei.cn/gtqivkfpbx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shuidangran.top/gtqdlzhkme.html

[E03] 截取子串
来源：http://hz.jlsjyb.cn/gtfvulcmrg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gogol.net.cn/gttdblyyth.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangdashe.top/gtjhmuesbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtrqewtccw.html

TS:   s.slice(1, 4)
来源：http://hz.xinyue.icu/gtrvausnvt.html

Java: s.substring(1, 4)
来源：http://hz.0kj1m.cn/gterrqvxqz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtondtzvkv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenjidiqi.icu/gtvyjeoaqv.html

C#:   s.Substring(1, 3)
来源：http://hz.xuetiantiany.cn/gtnsxzncgw.html

[E04] 查找子串位置
来源：http://hz.tianlin.xyz/gtesphpsst.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangdashe.top/gtqygjvydf.html

PHP:  strpos($s, "x");
来源：http://hz.mhx1999.top/gtsajvwabd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hongshengwenyu.top/gtqvetrkdm.html

TS:   s.indexOf("x")
来源：http://hz.meibo888.top/gthrnwzfoz.html

Java: s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtwfoulbbu.html

Go:   strings.Index(s, "x")
来源：http://hz.9152youxi.cn/gtsozpxaph.html

Ruby: s.index("x")
来源：http://hz.zdqjudy.top/gtmbwisbxs.html

C#:   s.IndexOf("x")
来源：http://hz.xziqi.cn/gtmpsrqhcm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tianlin.xyz/gtsdyaypbj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydjk.org.cn/gtdyoyykaa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtjgesbdrm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gttbrhhuks.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sufxvd.cn/gtcaiupntq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtemwwmvqn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dianchejie.cn/gtzfmmqtxn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtpshoiyck.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gtivxhmmcy.html

[E06] 替换子串
来源：http://hz.bjfxy.top/gtseskteua.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.vqdsnc.cn/gtzujowxvh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hammf.cn/gtwfptltnw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtebymdmgp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtljntgfxc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtoetptiws.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtqvsecsrc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zdqjudy.top/gtbxrviosp.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxinkj.top/gtdxofrakq.html

[E07] 按分隔符拆分
来源：http://hz.gaohongyu789.top/gtabpkeeqk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtirnxxwnk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yangfankeji.com/gtgwerauaw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sxryk.cn/gttczyidiv.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gttmnfdspf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtmupsrhup.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtahfdjdzt.html

Ruby: s.split(",");  s.split
来源：http://hz.gogol.net.cn/gtrpimnrhf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.kuanghao11.cn/gtiuwbkgrs.html

[E08] 数组按分隔符合并
来源：http://hz.yvedp.cn/gtdqjlxvpr.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtykfmhdlu.html

PHP:  implode(",", $items);
来源：http://hz.dianchejie.cn/gtdtefdzel.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtmkywqxsn.html

TS:   items.join(",")
来源：http://hz.yuanzhike.top/gtulcwsxjh.html

Java: String.join(",", items)
来源：http://hz.yuxming.cn/gtuhikyive.html

Go:   strings.Join(items, ",")
来源：http://hz.hnxiangtu.top/gtlrgrrtts.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtknioqktg.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gthkrzacoe.html

[E09] 去除所有空白字符
来源：http://hz.cheryme.top/gtjzagczau.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtnfmsgola.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.bjfxy.top/gtuwxhbygn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtddlqicoa.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtfvrvujll.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.dianchejie.cn/gtdswsebrp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daria6918.cn/gtbifrfmsc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtkwxuqrub.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.mhx1999.top/gtjaroyaon.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yanxiufei.cn/gtswpiqioo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtxsnrxffr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhijiandao.cn/gtjfxkklaj.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtaapufyrw.html

TS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtkidfryfo.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtpiafymjp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gtzgdykvwc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtmypswowt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gtkuonlksk.html

[E11] 反转字符串
来源：http://hz.xuanzx.com/gtuxvsmfnn.html

Py:   s[::-1]
来源：http://hz.yueranfly.top/gtpqihnoug.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtdrpaheud.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtybapcfug.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtiwomhjin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtgvxmstjq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtssoyvjri.html

Ruby: s.reverse
来源：http://hz.xuetiantiany.cn/gtydxwfinz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtagwqdprr.html

[E12] 统计某字符出现次数
来源：http://hz.tanke756.top/gtofnllzxp.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtdhitrmkl.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtmrhkxneq.html

JS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtejmyiueq.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtvtennkuh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shanyushiyangtech.top/gtyogkboyn.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtqknwiguq.html

Ruby: s.count("a")
来源：http://hz.sysykeji.top/gteyniiqmz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yueranfly.top/gtsnidipla.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtzrnjgezi.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gttjbtvueh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtgrppspto.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtobgvdxnj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtolgyjlgj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gogol.net.cn/gtzwbowwfh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtcrckokfy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtyomatiip.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ehwqpu.com/gtoinrtaff.html

[E14] URL 编码与 Base64
来源：http://hz.yanxiufei.cn/gtyzpqsbry.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gttefjpskf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnqzz.top/gtzxlukhqc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtlwhwqoth.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.svipenyu.cn/gtkaerykha.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtoolctoip.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yueranfly.top/gtrgkphlwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtyofmadhw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.0kj1m.cn/gtuxskayom.html

[E15] HTML 转义 / 反转义
来源：http://hz.daxiang520.top/gtzpgbzliy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.vqdsnc.cn/gtrnclcoob.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhiwuduotai.top/gtqjvwfqir.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtcfptlpfy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gtsggenpkf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtqfguhyom.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtdwwjwzqm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtkpwipswy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gttfwmedhd.html

[E16] 数字千分位
来源：http://hz.cucudq.cn/gtzdliwocs.html

Py:   f"{1234567:,}"
来源：http://hz.hammf.cn/gtfcmaisct.html

PHP:  number_format(1234567);
来源：http://hz.tanke756.top/gtggvajyha.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtlzeednzc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtqtwncwsk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydzc1.top/gtavsqeopi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtazhuyaqp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yongpay.top/gtpndclbms.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtezcethyn.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtqvccafkf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gtgueumlhi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtlwjlmflu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtwljpulza.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtucifakuz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtglpgcfzu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shangyingyoupin.top/gtxhefrmyq.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtjwvsbvxn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtubehssox.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gtiksyfckr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jlsjyb.cn/gttcwcbaot.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtjhmnunhl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtbvptuyhp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtwygqsbqr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtnkypzdcw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.haohaochexian.top/gtsgodunms.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtuwgmbzkg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hongshengwenyu.top/gtacmoggkh.html

[E19] 多行文本按行拆分
来源：http://hz.shangyingyoupin.top/gtarmboxuo.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gtiuxpoogv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj202588.top/gtvnwufgag.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtmjemvwod.html

TS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtnwroargz.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtwecnhaux.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtjhuccwrm.html


<!-- 参考信息 -->