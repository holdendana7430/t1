代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtyfgrfkim.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtqlprprdm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtzkwxswnq.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gtumniaqcy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtvcwowtpk.html

C#:   list.Sum();  list.Average()
来源：http://hz.haohaochexian.top/gttpgsmsqc.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gthigvxlbb.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtidwxxxln.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gtcdoaftki.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtabfjhgvq.html

TS:   Math.max(...arr);
来源：http://hz.hnxiangtu.top/gtyrcybcjt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtmbnbhpln.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtumyzfmui.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtqszdbuhr.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtkzbcgspt.html

[D18] 扁平化嵌套数组
来源：http://hz.haohaochexian.top/gtqdoqjbnc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtegyxqsbc.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtpwliokik.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gtdgigftaw.html

TS:   nested.flat();
来源：http://hz.dianchejie.cn/gtjmsqxjvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fengsongda.top/gtefnmvqrs.html

Go:   // 手写双层循环
来源：http://hz.chenlongwang.top/gtgknowdkj.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtedqiqtax.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.9152youxi.cn/gtvfunsjdv.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gtslgeybch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangdashe.top/gtvyxagcsn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pengpengdd.cyou/gtehbybpxx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj202588.top/gtdijcjcaq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtphbjeain.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gogol.net.cn/gtiqzzsmhs.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gttrtihiyt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gtjngbjkok.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtqdbgxuiu.html

[D20] 统计每个元素出现次数
来源：http://hz.jlsjyb.cn/gtvoclohxb.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gtkqjgoixr.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gthffcqrqp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtdxvzekni.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtlcwyrbfx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daxiang520.top/gtpafgvcke.html

Go:   // 手写 map[T]int
来源：http://hz.aizwys.cn/gtpfpgiofn.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtvmsgepbh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.mhx1999.top/gtkrvguwkv.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtoztxdrev.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtihadwyfp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtymbjomcv.html

JS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtwjnzxyjk.html

TS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtdqappnbu.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtxjjmjuxy.html

Go:   slices.Contains(arr, x)
来源：http://hz.hfpthk.cn/gtnbccrzyd.html

Ruby: arr.include?(x)
来源：http://hz.sxryk.cn/gtcgsiroul.html

C#:   list.Contains(x)
来源：http://hz.tianlin.xyz/gtvthpgiib.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtjijeovhr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtwgjomzki.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.c1oappe.top/gtdkporkhd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yanxiufei.cn/gtloudeqqr.html

TS:   [...arr];
来源：http://hz.chenzaomai.com/gtjrnviwwe.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtggvwxwya.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtczhroeqg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuanzhike.top/gtaqorbahh.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtghhredzg.html

[D23] reduce 累积计算
来源：http://hz.wangdashe.top/gtnjgesvun.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ivvv.top/gtavorxnle.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinghuilouyu.cn/gtcfxvdvyp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtrnrvnpwy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtasmfihwc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.kuanghao11.cn/gtogtbtnpc.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtqalnivbn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.birdmap.top/gtizeclcde.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.bjfxy.top/gtxinwjgva.html

[D24] 字典 / Map 基本操作
来源：http://hz.jianghu66.top/gtnplsxpjs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gtbbqtdurj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.haohaochexian.top/gtnmhydmgo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtuetgwzds.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gtgetxdymv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gtvktculys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hywenlv.cn/gtlsjylyim.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtniumkpdq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tian-w.cn/gteuhzbcup.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtgqugoqia.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtqaykjuuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hywenlv.cn/gtnsannbfb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zdqjudy.top/gtyrlmnkxm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtlufcpxds.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nwbrower.top/gtikxjrowr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gthxgrxnyh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnqzz.top/gtobodywhl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenzaomai.com/gtoseazbqv.html

[D26] 数组转字符串
来源：http://hz.ybcxt.top/gtpbpprnxt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.birdmap.top/gtfovighiw.html

PHP:  implode(", ", $arr);
来源：http://hz.aizwys.cn/gtekdthuun.html

JS:   arr.join(", ")
来源：http://hz.xinyue.icu/gtnapadrdk.html

TS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtlxjgoobv.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtxksrrkvp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tianlin.xyz/gtmmjfdflb.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtnksrnczq.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtbqmwlfnl.html

================================================================================
来源：http://hz.hammf.cn/gtqululkbd.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtwivmgdgg.html

================================================================================
来源：http://hz.smart0.xyz/gtjkkgjlhv.html

[E01] 拼接字符串
来源：http://hz.dianchejie.cn/gtjetmqowc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.iojbl.cn/gtxnqvesoe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgfzy.top/gtfnzxdetu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtgintkcpx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtgyxkbowu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.wangdashe.top/gtjjmmsfrv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gtsmmpmviu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtoeenplbn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.316326.xyz/gtpupocwwk.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gtukvpxcmz.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtacxgybzq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigfzy.top/gtmhwtrimf.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtqxphvakq.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtaggzyfwp.html

Java: "ab".repeat(3)
来源：http://hz.tanke756.top/gtsntanmsr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtruleuumz.html

Ruby: "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtvqqmwjmx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtriuxcszk.html

[E03] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtfsmcdjkd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guannengcc.top/gtvwwhgbgz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtqhvpiukr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gtezztvgam.html

TS:   s.slice(1, 4)
来源：http://hz.shuidangran.top/gtbtwccdmw.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtvjyaanpm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gtzswxfqlg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gthcukcnwd.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtbtsxzwpu.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gtimibieyv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xuanzx.com/gtqvbbiblq.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtiioqdrsf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtesbzrqaw.html

TS:   s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtggnupucc.html

Java: s.indexOf("x")
来源：http://hz.xuanzx.com/gtdamdbwwu.html

Go:   strings.Index(s, "x")
来源：http://hz.yj202588.top/gtqaaitkbb.html

Ruby: s.index("x")
来源：http://hz.shangyingyoupin.top/gtxpdempso.html

C#:   s.IndexOf("x")
来源：http://hz.fengsongda.top/gtbuupuexq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gtngemzysq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fzhhl.top/gtyzeczpyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.quarkkingdee.top/gtrkcurwck.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtroajokcu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xingfuxueyuan.xyz/gtnovucnul.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtylrmifpi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gtebtakopw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cdnleiting.top/gtrvvxkxol.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhijiandao.cn/gtejqyswhe.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gtopymnitf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxuanxn.top/gtwmukdmqh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinghuilouyu.cn/gtyoevlzwl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtsaqoodaa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtkckdghgv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtklcwvdqn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guowangkeji.top/gtlpvuwgjp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shzxlz.cn/gtmcvchjtm.html

C#:   s.Replace("a", "b")
来源：http://hz.svipenyu.cn/gtwdjnkggk.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtbirlqdlz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yvedp.cn/gttlnpvvfp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sysykeji.top/gtxyggqzne.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pengpengdd.cyou/gtlpgjepoy.html

TS:   s.split(",")
来源：http://hz.shangyingyoupin.top/gtzdmpawfq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gtrjopvqyd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gtyifxjsyf.html

Ruby: s.split(",");  s.split
来源：http://hz.gaohongyu789.top/gtpxkcowhx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fzhhl.top/gtptkcgbps.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtdrstitik.html

Py:   ",".join(items)
来源：http://hz.feifeiyinyue.top/gtgccbqlqf.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtdtdbjpqe.html

JS:   items.join(",")
来源：http://hz.xuetiantiany.cn/gtueosvoqx.html

TS:   items.join(",")
来源：http://hz.zhongyouzk.top/gthykstfhk.html

Java: String.join(",", items)
来源：http://hz.cashguo.top/gtromnsmhp.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangtech.top/gtzvyleuoj.html

Ruby: items.join(",")
来源：http://hz.zycfv.cn/gtgycfnked.html

C#:   string.Join(",", items)
来源：http://hz.yongpay.top/gtekhhamqk.html

[E09] 去除所有空白字符
来源：http://hz.shuidangran.top/gtjmkiqmat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtjfwycnee.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtyowzipoo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtetfxildy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtpwoasskr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zycfv.cn/gthxjhqaal.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gtjrpqliwo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuetiantiany.cn/gteyadkuoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sweek.top/gtslfudacw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhaomingkeji.xyz/gtzgyptypk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtlsuhpepz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuxming.cn/gtbzgqajfk.html

JS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtaxfxmwqj.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtcvftgfns.html

Java: String.format("%03d", 7)
来源：http://hz.cqqwz.cn/gtbppaznyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yonumen.top/gtyxpjscpy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtmiexazhj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.svipenyu.cn/gtzgbpmngl.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtyckdgugo.html

Py:   s[::-1]
来源：http://hz.shangyingyoupin.top/gtqdyedzuq.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtuzlmzqzg.html

JS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtsaftiilo.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gthhzuhofx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daria6918.cn/gtiopepabs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtqvvlbarf.html

Ruby: s.reverse
来源：http://hz.ehwqpu.com/gtjqdkpcrm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtrtpszejw.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258.top/gtolwjupaz.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtiswpshky.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtsesgyxir.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtcojsijpq.html

TS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtfrsejpqh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtghditacl.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtqujbmsxw.html

Ruby: s.count("a")
来源：http://hz.vqdsnc.cn/gtsgscsjtg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtvkkirduc.html

[E13] 逐字符遍历
来源：http://hz.tanke756.top/gtwipzyszh.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtemzwbmwj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtnhomgwmk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.snrcjt.cn/gtitshadaf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtqduvewuo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxinkj.top/gtjrucwkpk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.andypj.xyz/gtjotangmt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gtarucjymc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtllhywhqb.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangtech.top/gttpjssymt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.haohaochexian.top/gtxpxymoxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sufxvd.cn/gtvssoaxkg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jlsjyb.cn/gtzszpzsys.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtbnlqkqhf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gthjtrgqku.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sxryk.cn/gteqhemwld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gtokobniec.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtarvwffvs.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtxppuridj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtbdxtlzqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yvedp.cn/gtnubdizmq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hongshengwenyu.top/gtzrktkhjd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yangfankeji.com/gtnaoaucaq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtmqiusdpl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxinkj.top/gtpygtzmud.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtmtlknozp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.kuanghao11.cn/gtpwrskuzl.html

[E16] 数字千分位
来源：http://hz.zhijiandao.cn/gteulieouv.html

Py:   f"{1234567:,}"
来源：http://hz.nanxuanxn.top/gtodmqnsfc.html

PHP:  number_format(1234567);
来源：http://hz.xuetiantiany.cn/gtjkrnvcoy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtdpzloiba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtyzyottxk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gtarkexsyw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gotoacloud.top/gtuxpsekfp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtswdcktwy.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtzerfoxqf.html

[E17] 首字母大写
来源：http://hz.jinqigufen.top/gtaemdkaxg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sxryk.cn/gtwiohzzrl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtvkrxqqrj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtqbpjmiwl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtqkvgbkvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtxrzgyfny.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dashuyun.cn/gtipyowwgl.html

Ruby: s.capitalize
来源：http://hz.guowangkeji.top/gtpnhrubal.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxuanxn.top/gtoykxosuu.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtadcekovp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhixingplan.top/gtjrfmmlrx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gttvnxwuck.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtpjqxsuvg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtjvkcyvyd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.havefunace.top/gttgodxkro.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gttuxwduco.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydzc1.top/gtaedhljnu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pengpengdd.cyou/gtssjzdmwl.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtxbbomtjn.html

Py:   s.splitlines()
来源：http://hz.tianlin.xyz/gtcheogpse.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydjk.org.cn/gtcbsvezdg.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtoanpqkbn.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtocxianev.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gtvszriocd.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtkxglodts.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gteltethuq.html

C#:   s.Split('\n')
来源：http://hz.hnxiangtu.top/gtnvkyexcr.html

[E20] 判断字符串是否为空
来源：http://hz.vqdsnc.cn/gtghmbrzzv.html

Py:   if not s:
来源：http://hz.pengpengdd.cyou/gtqmaczmrp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhongyouzk.top/gtxmqupdld.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pengpengdd.cyou/gtcktgvtcw.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtrktjxpzu.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtzdsmozxu.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gtyqjkaarv.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtlcjjalqj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtzwcqppdy.html

[E21] 超长截断加省略号
来源：http://hz.fzhhl.top/gtshzazxiz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtugtgqljk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtfzxhmaao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtvuqxdobh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtztcdbisp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtcegsyxdm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.redwolf501.top/gtjzehduzd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtqsslvqjw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtyqlbicig.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtvbqdqmxw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtzzjxihwd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtkfzpxvlm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtpwjnqatq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtcnzgforj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gttoyyoiiq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gtlxbnrsxy.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtyauntsll.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258888.top/gtruyvieth.html

================================================================================
来源：http://hz.yvedp.cn/gtoqcqaafb.html

F. 文件与目录
来源：http://hz.shanyushiyangkeji.top/gtkifutyyp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbechmpwx.html


<!-- 参考信息 -->