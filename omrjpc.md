代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hongshengwenyu.top/gtrxynmlip.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtxxdwwlkf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtwtxenwsw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.mhx1999.top/gtikkldzer.html

[D15] 去重
来源：http://hz.yangfankeji.com/gtsmjviwjc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gthbrjxidb.html

PHP:  array_unique($arr);
来源：http://hz.jianghu66.top/gteksooofm.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtxngqdjhd.html

TS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtrpxntgau.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj202588.top/gtktownbhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtyptonncn.html

Ruby: arr.uniq
来源：http://hz.gzhubu.top/gtwjcgybpw.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gthcmshxas.html

[D16] 求和与平均值
来源：http://hz.ywan-chungtsiang.top/gtoxqbvinl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtykfcsxij.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtshulzjao.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jlsjyb.cn/gtmrhlasus.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtikgjsdzi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gtagywtnsp.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gthayaflbj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hongshengwenyu.top/gtkbjesmuk.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtwbsduoka.html

[D17] 最大值与最小值
来源：http://hz.mhx1999.top/gtbsqhzqku.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gtlxejbbme.html

PHP:  max($arr);  min($arr);
来源：http://hz.xylfe.cn/gtqjuzfemd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuanzx.com/gthociudlc.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtnnhrpoov.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sweek.top/gtnzmdyqrf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtqepeophe.html

Ruby: arr.max;  arr.min
来源：http://hz.mhx1999.top/gtmedtpkqd.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgfzy.top/gtdlizldug.html

[D18] 扁平化嵌套数组
来源：http://hz.zycfv.cn/gtelzqseny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtzrjhumsf.html

PHP:  array_merge(...$nested);
来源：http://hz.aizwys.cn/gtovoroeqe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtolhwiavu.html

TS:   nested.flat();
来源：http://hz.guannengcc.top/gtawmdmgaw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtecxzcrvx.html

Go:   // 手写双层循环
来源：http://hz.yonumen.top/gtvvezupnz.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtyfoecmte.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtxorcptuz.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtyemlpqgr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangdashe.top/gtuytwchwy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daxiang520.top/gtzyygnqne.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gtqsxxywnk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangkeji.top/gtabkvmytb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtaxfxbcjk.html

Go:   // 手写 map[string][]T
来源：http://hz.zhixingplan.top/gtnmctfdci.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gtpmbjvlsj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.redwolf501.top/gtldaqaqee.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtolbaaoyk.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtxlnougmq.html

PHP:  array_count_values($arr);
来源：http://hz.chenlongwang.top/gtvggzmamz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtljykyshb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtsfyfegnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zycfv.cn/gtxgxcitdn.html

Go:   // 手写 map[T]int
来源：http://hz.wangdashe.top/gtzmslcgrv.html

Ruby: arr.tally
来源：http://hz.yuxming.cn/gtagqrtoxw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtmpogwfts.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gtgtyogffr.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtpfzjtpus.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ppjwa.cn/gtwzhbegei.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtwplzdfyj.html

TS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtragvnlgl.html

Java: list.contains(x)
来源：http://hz.chenlongwang.top/gtknyhpitv.html

Go:   slices.Contains(arr, x)
来源：http://hz.gaohongyu789.top/gtcnnsbqzs.html

Ruby: arr.include?(x)
来源：http://hz.hongshengwenyu.top/gttxypbyln.html

C#:   list.Contains(x)
来源：http://hz.hongshengwenyu.top/gtviljmubq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangdashe.top/gtsppptayw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtodiynwhb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.c1oappe.top/gtzqnhumwo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yanxiufei.cn/gtagjxecgg.html

TS:   [...arr];
来源：http://hz.gaohongyu789.top/gtddacuwkw.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtyzulwyog.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtwxvwvqgx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtgxtnsmge.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtdemdbsla.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtaccrelup.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtvurbawbc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yanxiufei.cn/gtozavthfr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtclpypjrp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtexadoonl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xingfuxueyuan.xyz/gthsavtkuy.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtfmbenfif.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtilujliqv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gtanhpcuhk.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenlongwang.top/gtryxmgiml.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.bjfxy.top/gtrwrwtujg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtxuuaqhvz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gthwwxyivs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.smart0.xyz/gtzkvqtvrj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fzhhl.top/gthfrednxr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenlongwang.top/gtfzqvpvbp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtetojkcgk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtxgbvgmkz.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtbntxuksx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yongpay.top/gtbhypsema.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtlrrsbewe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tianlin.xyz/gtymelzhdc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenlongwang.top/gthuchcixi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtayrwrcst.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtkkfytleg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtrrtoxfkf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtmwkmhvlv.html

[D26] 数组转字符串
来源：http://hz.sufxvd.cn/gtfcobtjxk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgfzy.top/gtzhedphfu.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtufymviti.html

JS:   arr.join(", ")
来源：http://hz.meibo888.top/gtajowfgoz.html

TS:   arr.join(", ")
来源：http://hz.meibo888.top/gtejfxrfcd.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gttbbbegpl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xziqi.cn/gthzcblwxj.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gtasoiptuo.html

C#:   string.Join(", ", list)
来源：http://hz.yonumen.top/gtwrovvnkx.html

================================================================================
来源：http://hz.chenlongwang.top/gtlengmntt.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtjcatbjnq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtudvtunmx.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtxallisjk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtymehpzmh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aibaodan.cn/gtgqurhhyw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gthchdbosn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtbmcigvzp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtmanetpwz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.9152youxi.cn/gtarpkgfzf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtdifhhtth.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtfygekwzl.html

[E02] 重复字符串
来源：http://hz.snrcjt.cn/gtnorubhcx.html

Py:   "ab" * 3
来源：http://hz.9152youxi.cn/gtivtbdspm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtufosyuwl.html

JS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtffvovaze.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtwupegajk.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtjbtasejn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtdlliwhez.html

Ruby: "ab" * 3
来源：http://hz.feifeiyinyue.top/gtrpkntqfs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangtech.top/gtdfngcigv.html

[E03] 截取子串
来源：http://hz.redwolf501.top/gtbvjwjvjv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gtwudlqiec.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ybcxt.top/gtzugxqfev.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ppjwa.cn/gtthpsrsdx.html

TS:   s.slice(1, 4)
来源：http://hz.gaohongyu789.top/gtorhobaom.html

Java: s.substring(1, 4)
来源：http://hz.hammf.cn/gtjsufmwdc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtaxlfhfmr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtayknhbsq.html

C#:   s.Substring(1, 3)
来源：http://hz.daxiang520.top/gtnjrgvzfw.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gtbfipydja.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgufenzy.top/gtnfbcsqtm.html

PHP:  strpos($s, "x");
来源：http://hz.zhijiandao.cn/gtfhyfqukt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gtlskbpxnz.html

TS:   s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gteqkprsyc.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gtdhfvrfsu.html

Go:   strings.Index(s, "x")
来源：http://hz.hnqzz.top/gtdvtwnnhd.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtkcjnveqg.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtotpbydcz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gtipszupyr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gtkajeavbh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtbfzsztcf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtbjxwxhgf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yuanzhike.top/gthldgimae.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtlhhxlszb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tian-w.cn/gtekqjjpbq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.birdmap.top/gtrfunenzy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cdnleiting.top/gtsdfckwrl.html

[E06] 替换子串
来源：http://hz.yj20258888.top/gtkohpzggd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gtzwlftnvq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtrxgbkvnp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtaydrrxgi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtnvgphlhg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtqanseern.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cqqwz.cn/gtihigklnj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cqqwz.cn/gtcbefhcpw.html

C#:   s.Replace("a", "b")
来源：http://hz.tanke756.top/gtvlbcjxym.html

[E07] 按分隔符拆分
来源：http://hz.yangfankeji.com/gtzdraemzy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigfzy.top/gtguseyzgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtozfmhdtu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cqqwz.cn/gtmfyniseb.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtqwyqehjc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtwgcmawjk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.guannengcc.top/gtabiutgrt.html

Ruby: s.split(",");  s.split
来源：http://hz.guannengcc.top/gteowaesbn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dashuyun.cn/gtjipdndjq.html

[E08] 数组按分隔符合并
来源：http://hz.yvedp.cn/gtueyqmmwn.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtiuiqzoki.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtuddffcxg.html

JS:   items.join(",")
来源：http://hz.haohaochexian.top/gtdcshdvis.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtctxtywvv.html

Java: String.join(",", items)
来源：http://hz.tanke756.top/gtepkscljp.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gttnzkwwrt.html

Ruby: items.join(",")
来源：http://hz.sweek.top/gtfumpgiss.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtszejevto.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gtziaqvmbx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtjiazwpmx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hammf.cn/gtpfhvvqri.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtfyvnbgpi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gtukkqgkgj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cashguo.top/gtqgqfnsdj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fzhhl.top/gthgachntz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xziqi.cn/gtneisspll.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtnqswfhje.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gttsqavuos.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ehwqpu.com/gtkfysimle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtapntefcq.html

JS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtnasqesoo.html

TS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtjczqcuwo.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtraturmho.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.redwolf501.top/gtcqkkcqmd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gttuhwtwjc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gthfkfxnbz.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gttehxnpqh.html

Py:   s[::-1]
来源：http://hz.jianghu66.top/gtgnpxrzjs.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtuqycydex.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtdkfcpnpb.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtonhjlner.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gticgutblw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtikvbabzy.html

Ruby: s.reverse
来源：http://hz.yueranfly.top/gtffmlyrxa.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtshljbskk.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtkmsohewb.html

Py:   s.count("a")
来源：http://hz.ppjwa.cn/gtlhtqcbsr.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtgmpcrksz.html

JS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtbidpicty.html

TS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtftjpvdco.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtjqlsxsnz.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtuhrfxldb.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtljectjzw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.svipenyu.cn/gtghtanbdh.html

[E13] 逐字符遍历
来源：http://hz.jinyuanbaomall.cn/gtcrgndwcy.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtdlgaemmy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtnoiqkyfm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtvfdjjluf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gturhwlrii.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zdqjudy.top/gtqzldurtm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtkjvezhto.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtzusmbeuq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtjstvpzic.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtawsohihh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tianlin.xyz/gtdrqtgmjh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xingfuxueyuan.xyz/gtbilowjow.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gtyqkbholv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnxiangtu.top/gtqugrdzwu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangshuangyany.cn/gtdxylaqhj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtqetishol.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gthzlqkakk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtycsatigt.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gtllqeubtm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.316326.xyz/gtmzszgqkc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtrfsrzlqg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tianlin.xyz/gtekuuxuxs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ywan-chungtsiang.top/gtniixnmzm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guannengcc.top/gtrhjqipot.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtfecqebem.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtfnaabawu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zycfv.cn/gtflrwrjhr.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gttacblaso.html

Py:   f"{1234567:,}"
来源：http://hz.cheryme.top/gtwpquebeh.html

PHP:  number_format(1234567);
来源：http://hz.jinqigfzy.top/gtmmnzszfr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtcfspgwch.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtixwoqyes.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jianghu66.top/gtgqgxcgfm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guannengcc.top/gtnhcbpmwx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gthnkdzugf.html

C#:   1234567.ToString("N0")
来源：http://hz.cashguo.top/gtlkbaopfq.html

[E17] 首字母大写
来源：http://hz.pycfn.com/gtaqcxxnxk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtnzquvhfr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gtemgxelgw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gtwcsmxhqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtimgirzul.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pengpengdd.cyou/gtahzixiyd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gzhubu.top/gteqjndiyn.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtcndnqzuw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtqcwdnajw.html

[E18] 模板占位符替换
来源：http://hz.gotoacloud.top/gtsbqnfulv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtzorpmpcn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gthilaumzg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtwoyouwhp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtyjdujwhz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gthyzyzfsk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhongyouzk.top/gtbusxugji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangdashe.top/gthzfjywzk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258888.top/gtbxkanwdp.html

[E19] 多行文本按行拆分
来源：http://hz.zdqjudy.top/gtdgkwchow.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtutndllim.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtoliujaku.html

JS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtttmogvxd.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtbcrnqcxb.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtyskbrnjj.html

Go:   strings.Split(s, "\n")
来源：http://hz.daxiang520.top/gtmhasutjx.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gttdyzuwku.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtffsuiuer.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigufen.top/gtgcxpjotd.html

Py:   if not s:
来源：http://hz.vqdsnc.cn/gtvawnfccb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtntplxghx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhaomingkeji.xyz/gtrosmdyhw.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtwkgcympe.html

Java: if (s.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtgwlorxus.html

Go:   if s == "" {}
来源：http://hz.kuanghao11.cn/gtldhtjetz.html

Ruby: if s.empty?
来源：http://hz.zhaomingkeji.xyz/gttcmsrfsm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gtfdlcikmj.html

[E21] 超长截断加省略号
来源：http://hz.yj20258888.top/gtxuaujtdu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtvjklnmwy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtldqhdpjv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtkrhkrybv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtruovasqq.html


<!-- 参考信息 -->