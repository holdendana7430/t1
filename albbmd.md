代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtwwmpsvut.html

Go:   // 手写循环
来源：http://hz.shanyushiyangtech.top/gtrbqsuwdh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtmbyryesu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtvoomrmqt.html

[D15] 去重
来源：http://hz.jinqigfzy.top/gtysubfzfy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtmadryuxo.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtcihbdbqi.html

JS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gttrklysrq.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtfiufcmiu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtymglygxm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhiwuduotai.top/gtwbymtzne.html

Ruby: arr.uniq
来源：http://hz.hysaishi.cn/gtfuaueoyo.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtfutrzbxp.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtnffvform.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtnddlfltl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.c1oappe.top/gtddwejjfw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gttxpmtqyf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtqmgwuqqv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gtionqexfz.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtwaygszoe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gzhubu.top/gtlllvbsfw.html

C#:   list.Sum();  list.Average()
来源：http://hz.yonumen.top/gtyrlegbyw.html

[D17] 最大值与最小值
来源：http://hz.quarkkingdee.top/gtnrhyvzss.html

Py:   max(arr);  min(arr)
来源：http://hz.yj202588.top/gtuafirsaq.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtbnuvogsm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtxtkzdsls.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtmelxxyzv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtqlvtxace.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtjwjvqfmb.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtpmmtgvkr.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtjaqkivyz.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtfvzgtyrz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtkddfcwbe.html

PHP:  array_merge(...$nested);
来源：http://hz.gogol.net.cn/gtescixjkh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cdnleiting.top/gtpbfuurkh.html

TS:   nested.flat();
来源：http://hz.smart0.xyz/gtatalfrbn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.mhx1999.top/gtlxwtlpwe.html

Go:   // 手写双层循环
来源：http://hz.hongshengwenyu.top/gtwmkfomqf.html

Ruby: nested.flatten
来源：http://hz.gzhubu.top/gtxwzcikbv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtubopjxtd.html

[D19] 按字段分组
来源：http://hz.jlsjyb.cn/gtbvdyvfri.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtmhbpgtfw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gtcupihems.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtossatkmk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ppjwa.cn/gtvlgjutmw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gtjtxebgub.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtwvwzpzqk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinyuanbaomall.cn/gtvlpaddoe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fengsongda.top/gtcjhjmneg.html

[D20] 统计每个元素出现次数
来源：http://hz.chenzaomai.com/gtzbkbflfn.html

Py:   Counter(arr)
来源：http://hz.ydjk.org.cn/gtxrxdxwii.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtnvaihpmw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtwmobfxrs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtnijpmhkh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtnlekrejh.html

Go:   // 手写 map[T]int
来源：http://hz.316326.xyz/gtgpijzvph.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gttyldysge.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zdqjudy.top/gtxbdvjaak.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtnrozrmdk.html

Py:   x in arr
来源：http://hz.cashguo.top/gtykzmreyn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtvbqevzcy.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtdttkjyko.html

TS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtbdtxhqmz.html

Java: list.contains(x)
来源：http://hz.52xcode.cn/gtithmkmhm.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtnbqzebta.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtpwifqhwf.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtkuxbkctu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtjxmodtoq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtzmmntusp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigufen.top/gtnwfefbcq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtmrotgcmc.html

TS:   [...arr];
来源：http://hz.jlsjyb.cn/gtqopesasi.html

Java: new ArrayList<>(list);
来源：http://hz.zhongyouzk.top/gtvxrhowjk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtineprpxf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydzc1.top/gtkncclgax.html

C#:   new List<int>(list);
来源：http://hz.hongshengwenyu.top/gtwrioduqm.html

[D23] reduce 累积计算
来源：http://hz.0kj1m.cn/gtusirvhzu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtnbdwonkb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxuanxn.top/gtwvxhcphb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtgstxreua.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtxbimcekm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtlcxpavwf.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtlpbwukwm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtfyfhrkzk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shzxlz.cn/gthoyvzzsa.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gtjzznswdu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhaomingkeji.xyz/gteuezranh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuetiantiany.cn/gtrjqoodhe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yonumen.top/gtfkmfwpcb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gthbrrpejm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gogol.net.cn/gtdudneyhi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gttdeyocni.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gttrxxokyq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ehwqpu.com/gtjvfxujnr.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtrlqmsgyk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ybcxt.top/gtcluljctz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gtswwzhpmv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shuidangran.top/gtcjcxjqsq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtdkpfeqvg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xingfuxueyuan.xyz/gtfaykoacf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtitpwsjbz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cheryme.top/gtlsexmaut.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtznawxkzd.html

[D26] 数组转字符串
来源：http://hz.bjfxy.top/gtxnubcuqz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtkeyvrkqa.html

PHP:  implode(", ", $arr);
来源：http://hz.ydzc1.top/gtdlgektqq.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtaqbtaylo.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtvghmnlol.html

Java: String.join(", ", list)
来源：http://hz.gaohongyu789.top/gtoyzmgtgy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangkeji.top/gtxntrvhzy.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtzhlrpffs.html

C#:   string.Join(", ", list)
来源：http://hz.hnqzz.top/gtxkwoslow.html

================================================================================
来源：http://hz.jqgufenzy.top/gtapjscawt.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtctrjlsdz.html

================================================================================
来源：http://hz.yj20258888.top/gtqcshkxns.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtdojwixmb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gtoupbkpim.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xinyue.icu/gtjkzybyvw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hfpthk.cn/gtlkivufpz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gttbdyucke.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.wangdashe.top/gtpobdyred.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ppjwa.cn/gtvzmpfzyi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.kuanghao11.cn/gtromrxvgg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gthrasopwf.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtdrorvtxk.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtgczmcxsy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtbpxjamvn.html

JS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gttdpoamfg.html

TS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtgoqjdekg.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtpupmehub.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtjuodjabs.html

Ruby: "ab" * 3
来源：http://hz.mhx1999.top/gtntrldncj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhongyouzk.top/gtviiykuin.html

[E03] 截取子串
来源：http://hz.jqgfzy.top/gteehgnsoj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sxryk.cn/gtkuaexlxc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shzxlz.cn/gttlyaeinn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtqesubica.html

TS:   s.slice(1, 4)
来源：http://hz.yanxiufei.cn/gtwjtabglc.html

Java: s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtotwwfjnw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.52xcode.cn/gtxawthbwf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigfzy.top/gtcwkxcour.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtswykffyn.html

[E04] 查找子串位置
来源：http://hz.aibaodan.cn/gtqgpdpejq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aizwys.cn/gtqwdtmsir.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtjkdjpwrw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtivqugbjz.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtavfllmew.html

Java: s.indexOf("x")
来源：http://hz.guowangkeji.top/gtdchrjkcj.html

Go:   strings.Index(s, "x")
来源：http://hz.9152youxi.cn/gtameiwxnd.html

Ruby: s.index("x")
来源：http://hz.jinyuanbaomall.cn/gtxdxnmogw.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtluuxbwfu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtujhgdolg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhiwuduotai.top/gturpffabb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtaevmhghd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtcqiuyowf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgufenzy.top/gtqdluhemc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtexmipfjh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtnooxsdlj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ywan-chungtsiang.top/gtzndryuoj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gtophnwbtx.html

[E06] 替换子串
来源：http://hz.cqqwz.cn/gttlrdzhjv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtquoemmmq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.smart0.xyz/gtimylcfak.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtmtqkrokj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtffxxnqvn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gthtlugaha.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.havefunace.top/gtjboqadng.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigufen.top/gtyifofyfe.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtbhvhxllt.html

[E07] 按分隔符拆分
来源：http://hz.hywenlv.cn/gtfhrhuzpv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gaohongyu789.top/gtbkffvamw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.mhx1999.top/gtpffiipsf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtfhhmofkz.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gtqvsmyjgq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fzhhl.top/gtanghajby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtcxmqhsav.html

Ruby: s.split(",");  s.split
来源：http://hz.yangfankeji.com/gtkpuhsqtt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinqigufen.top/gtqcaavubd.html

[E08] 数组按分隔符合并
来源：http://hz.tian-w.cn/gtpglhoqxa.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtwcwwsgct.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gthijojwup.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gttmxixoyj.html

TS:   items.join(",")
来源：http://hz.cheryme.top/gtzcohdvwi.html

Java: String.join(",", items)
来源：http://hz.hfpthk.cn/gtdtxnfncb.html

Go:   strings.Join(items, ",")
来源：http://hz.52xcode.cn/gtbbmkwyob.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gtduamfiit.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gtdbjemnpk.html

[E09] 去除所有空白字符
来源：http://hz.shzxlz.cn/gthqusybes.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gtdxmirmte.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gaohongyu789.top/gthielfopp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gthispeeme.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtxnxdvlbi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtrgqmsrun.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sysykeji.top/gtnfjfeuch.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aizwys.cn/gttkevqcac.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zdqjudy.top/gtreaybpkf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtqpfzjzqh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtzglmfoal.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258.top/gtofjedbjw.html

JS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtyfdpfvdc.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtevpboooz.html

Java: String.format("%03d", 7)
来源：http://hz.yueranfly.top/gtwcpchbpe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtfqqfliaw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtyiaekslu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fengsongda.top/gtercbqcuw.html

[E11] 反转字符串
来源：http://hz.jinqigufen.top/gtmimuguge.html

Py:   s[::-1]
来源：http://hz.aibaodan.cn/gtsjrtzkug.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtbffuyuom.html

JS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtkktwzszm.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtqahpwbxi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shzxlz.cn/gtzceleirr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtmvzoonhd.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtdujdputc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtksdvhcxi.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtnhbwuymj.html

Py:   s.count("a")
来源：http://hz.sweek.top/gtqkcaxbnv.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtzeqgjhwf.html

JS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gtglvaouyk.html

TS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtywzkgmov.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtxogaifyc.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtoeosbqnq.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtocrvxvkv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtoubajbsm.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtkplicxhf.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gticvcltwy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gzhubu.top/gtccohsrgj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtgpufkhzn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtxfmjvqzk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtiqbvrhkf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtmcoiohty.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtfqkforfc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtqezabxsa.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtgzshpdrj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gtunjnghld.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuanzx.com/gtarqumbpn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gttrztrrlb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.andypj.xyz/gthqytpulv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ehwqpu.com/gteurdbdif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.bjfxy.top/gtjbyeltxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cashguo.top/gthtpvzljf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zdqjudy.top/gtqoajhqyk.html

[E15] HTML 转义 / 反转义
来源：http://hz.aizwys.cn/gtvbvdpqby.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.9152youxi.cn/gtfhvavhks.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtkngnlgkv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtsptepnne.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.iojbl.cn/gtdahbvyfm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtfszmceje.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtlebzxjyd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258.top/gtusbtuaaj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhongyouzk.top/gtmdarfmar.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtqilyrvqq.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtmfypetue.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtaahbruoi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtrcniqhzq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtelsisqdd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuxming.cn/gtusladkws.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtbholfeky.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.meibo888.top/gtycqxlsgg.html

C#:   1234567.ToString("N0")
来源：http://hz.shzxlz.cn/gtyixblbbp.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtsasbkdzz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtjkufirxw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gaohongyu789.top/gtfsdfenzu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtifrayvck.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtmlkmrvnt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtlifzxykk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtmvdjruyq.html

Ruby: s.capitalize
来源：http://hz.cdnleiting.top/gtxbihakcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtxtzakwcd.html

[E18] 模板占位符替换
来源：http://hz.nanxinkj.top/gtvywlgemu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gtuhpvpott.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ywan-chungtsiang.top/gtrxolrpfk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtppylmuuz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtyytisvjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtrkpjeahf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gaohongyu789.top/gtsmgsqhza.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yvedp.cn/gtwbwwbftb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhixingplan.top/gtkcczwvyc.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtleusordb.html

Py:   s.splitlines()
来源：http://hz.zhixingplan.top/gtwaoehsgv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtwnbvgsbh.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtjuogckgn.html

TS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtvsifyuzb.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtuoiqkjvz.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxuanxn.top/gtqrxoiqgd.html

Ruby: s.lines
来源：http://hz.ywan-chungtsiang.top/gtsacvuevy.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtodbzpuug.html

[E20] 判断字符串是否为空
来源：http://hz.vqdsnc.cn/gtnlgfjlkd.html

Py:   if not s:
来源：http://hz.shangyingyoupin.top/gtljophqvr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gtjzhbvxtc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgfzy.top/gtbzpersvb.html

TS:   if (s === "") {}
来源：http://hz.52xcode.cn/gtucpuvuhx.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gthqddatxd.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtbenqhzcp.html

Ruby: if s.empty?
来源：http://hz.sweek.top/gtxfqcfhvg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtboinccxc.html

[E21] 超长截断加省略号
来源：http://hz.haohaochexian.top/gtnqfcwiih.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gtcnvofpbd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jianghu66.top/gtxoktlggk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtuqjbndzt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtriabmwzw.html


<!-- 参考信息 -->