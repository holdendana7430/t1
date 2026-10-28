代发 wailian999

[D11] 反转数组
来源：http://hz.xylfe.cn/gtdsjhhygk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gthaewmbga.html

PHP:  array_reverse($arr);
来源：http://hz.yonumen.top/gtfoiwrskx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtnkhveakt.html

TS:   [...arr].reverse();
来源：http://hz.chenlongwang.top/gteuhnhlcc.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtgtbkiqft.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtuciljazu.html

Ruby: arr.reverse
来源：http://hz.hywenlv.cn/gtnnauwkhr.html

C#:   list.Reverse();
来源：http://hz.hysaishi.cn/gtzmvxlxoz.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtydowpwkg.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtyaqtmtxl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xinyue.icu/gtarmicfsy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtgsrjnbkh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtyilxjjpq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtcljbibmb.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gtolzhhbgt.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangkeji.top/gtsbubfgno.html

C#:   list.IndexOf(x);
来源：http://hz.xziqi.cn/gtrxebzkwo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yongpay.top/gtcdhqfjmb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.birdmap.top/gtjenxdwpl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtouenxuaj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtguqwelht.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtdzovepvj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtjdxdaysw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gtzoospums.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtohxesafl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yueranfly.top/gtbcynvogi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigufen.top/gtydltzfia.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gtidldxsqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gtqblklaxz.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gthvdaaosi.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtjddrfnlh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.9152youxi.cn/gtlacidyqq.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtkmpwwupe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtwmwnbhaz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtbopyzvud.html

[D15] 去重
来源：http://hz.yangfankeji.com/gtsjqwxabx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtpjetsfso.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtuqiuando.html

JS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtbfvvqfsn.html

TS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtehefnnlo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhoulong.xyz/gtvmmvqjkx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtwqtfllpl.html

Ruby: arr.uniq
来源：http://hz.wangdashe.top/gtfunechqq.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtqiknohga.html

[D16] 求和与平均值
来源：http://hz.yuanzhike.top/gtgugdzvkr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sysykeji.top/gtilwikruw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ehwqpu.com/gtpjlbglnb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtflcwjdtg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtywatyguu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shzxlz.cn/gtykklrupe.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtiyutsbhy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gtzventotn.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtpgrspstj.html

[D17] 最大值与最小值
来源：http://hz.zhoulong.xyz/gtqrewzbto.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtrbnczekb.html

PHP:  max($arr);  min($arr);
来源：http://hz.xingfuxueyuan.xyz/gtudbfcbuw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cucudq.cn/gtztuznyhf.html

TS:   Math.max(...arr);
来源：http://hz.chenjidiqi.icu/gtzpsuonvh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtfisqazuw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nwbrower.top/gtxigygoom.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtyyurlcqm.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtydoetjko.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtlwwpizwf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtckmqvekk.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtinseqfvt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ppjwa.cn/gtbffjctes.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtmfygcuea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.0kj1m.cn/gtdykjhqpf.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtqwaujvrl.html

Ruby: nested.flatten
来源：http://hz.wangshuangyany.cn/gtxnenikjo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.havefunace.top/gtiitgejzn.html

[D19] 按字段分组
来源：http://hz.cqqwz.cn/gttpldxpnr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gaohongyu789.top/gtsqdrixld.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gotoacloud.top/gtyoewjajf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hysaishi.cn/gtittdkunz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtibwztlav.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.havefunace.top/gthkppanlb.html

Go:   // 手写 map[string][]T
来源：http://hz.chenlongwang.top/gtnpomhfkl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cucudq.cn/gthinydtyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinghuilouyu.cn/gtmghgzzqo.html

[D20] 统计每个元素出现次数
来源：http://hz.tian-w.cn/gtntjwnstt.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gtsostyjvi.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gttmtjfwbo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtbhqibycp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydzc1.top/gtrwhusoxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtnhcvjixd.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtyneectuc.html

Ruby: arr.tally
来源：http://hz.316326.xyz/gtqhjffsvq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtvishwzpc.html

[D21] 判断是否包含某元素
来源：http://hz.chenlongwang.top/gterkxqqlv.html

Py:   x in arr
来源：http://hz.ppjwa.cn/gttebtiwtr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guannengcc.top/gtzbtjrdrb.html

JS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtjpyfzvfl.html

TS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtzkkkfhqk.html

Java: list.contains(x)
来源：http://hz.gaohongyu789.top/gttlgkrgzw.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtnroxjxwl.html

Ruby: arr.include?(x)
来源：http://hz.cashguo.top/gtbgiabjmb.html

C#:   list.Contains(x)
来源：http://hz.sufxvd.cn/gtxjobwrqu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtlygiaasj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenjidiqi.icu/gtjghmukxf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fengsongda.top/gtghyeigxk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtocuurumj.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtevfkhhvf.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangtech.top/gtlcxuhxbf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daria6918.cn/gtfdhkkmgz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ehwqpu.com/gtvehziqpr.html

C#:   new List<int>(list);
来源：http://hz.xylfe.cn/gtmrpzrqul.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtjoyocjwe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtzsorlsrd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pengpengdd.cyou/gtpsiynbuh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtltjzhrqd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gtpeexkcon.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gttbzvudac.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtorvexkpr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.quarkkingdee.top/gtejjsauxs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtvhovnooy.html

[D24] 字典 / Map 基本操作
来源：http://hz.hongshengwenyu.top/gtrxdbqydx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.redwolf501.top/gtsolgplkb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fengsongda.top/gtzpexvvat.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtffxfiqdq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtefptnheq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.kuanghao11.cn/gtaxgkvqxr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtqlyrqddd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tian-w.cn/gtlibxsdyw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtwthkiibw.html

[D25] Set 集合去重与交并差
来源：http://hz.cashguo.top/gtgujpchgv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yvedp.cn/gtwgkqkulk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuanzhike.top/gtbzwzriey.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jlsjyb.cn/gtnlkxdels.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhengqikj.top/gtfkxygqwo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ivvv.top/gtzpgwtiwz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cheryme.top/gtnkrbgpxd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.feifeiyinyue.top/gtpjrtyibe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtquzgxqrb.html

[D26] 数组转字符串
来源：http://hz.sysykeji.top/gtfrjjrzfx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtlvgqnkvc.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtptrhpgpz.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtfocnvpvx.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gttbteegqx.html

Java: String.join(", ", list)
来源：http://hz.birdmap.top/gtifhurtix.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxinkj.top/gtnbruyflj.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gthvgxgrnf.html

C#:   string.Join(", ", list)
来源：http://hz.zycfv.cn/gtrweqjnct.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjkzrpvsn.html

E. 字符串处理
来源：http://hz.wangshuangyany.cn/gtiuvreodv.html

================================================================================
来源：http://hz.smart0.xyz/gtbjkcbfly.html

[E01] 拼接字符串
来源：http://hz.ydzc1.top/gthrrhfbbp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtgwdkbzbw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinghuilouyu.cn/gttsqdowkh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtkxrymqku.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtpalezxsp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinyuanbaomall.cn/gttarnsmpf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtbqnfblll.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtqovwhfbi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gzhubu.top/gtfjjbodnq.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gtfmpalkwv.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtfdstoxrp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tian-w.cn/gtbjirzqcl.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gthqxsdzfw.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtcvjzubiv.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtzxhcxcsp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtbaywakig.html

Ruby: "ab" * 3
来源：http://hz.pycfn.com/gtgehudave.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj202588.top/gtpiummfep.html

[E03] 截取子串
来源：http://hz.zhongyouzk.top/gtgblnbgkx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dashuyun.cn/gtjfgpiejb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuanzhike.top/gtwuahgtzo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtwzvvfyff.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigufen.top/gtpinytoxs.html

Java: s.substring(1, 4)
来源：http://hz.zycfv.cn/gtqupknsnk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zdqjudy.top/gtjmukbehb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtdcbrgfas.html

C#:   s.Substring(1, 3)
来源：http://hz.havefunace.top/gtqayzmhlt.html

[E04] 查找子串位置
来源：http://hz.daria6918.cn/gtekrkazun.html

Py:   s.find("x");  s.index("x")
来源：http://hz.feifeiyinyue.top/gtbrbelhwk.html

PHP:  strpos($s, "x");
来源：http://hz.ybcxt.top/gtqkijafms.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.kuanghao11.cn/gtusthnpsc.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtjixbbuii.html

Java: s.indexOf("x")
来源：http://hz.sufxvd.cn/gtauexvrsf.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gtarjqpblf.html

Ruby: s.index("x")
来源：http://hz.pengpengdd.cyou/gtaofkquzz.html

C#:   s.IndexOf("x")
来源：http://hz.dianchejie.cn/gtvouxlpns.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtxpsbkosj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gtlpkjrtmk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtkdysrgek.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtcsuseggo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xinyue.icu/gtnitmtqju.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtorapqscu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtchdobgzk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shuidangran.top/gtbnvunwar.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tanke756.top/gtpojncacf.html

[E06] 替换子串
来源：http://hz.feifeiyinyue.top/gtkzmpdnqm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtpxncbdju.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shangyingyoupin.top/gtepcfzjas.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtfojvacit.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtwqdmsrta.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtfgntgfiu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gaohongyu789.top/gtrqeucmaw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtvxowlgsc.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtddsrjqkb.html

[E07] 按分隔符拆分
来源：http://hz.xingfuxueyuan.xyz/gtkvirgfkh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gtdoihkthx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gthduqvmmf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtdbmajewz.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtafphcwoa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xylfe.cn/gtuhrdmpvu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.feifeiyinyue.top/gtscxzndnt.html

Ruby: s.split(",");  s.split
来源：http://hz.hysaishi.cn/gtvjhwgtgx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuxming.cn/gthuxjwoyp.html

[E08] 数组按分隔符合并
来源：http://hz.snrcjt.cn/gtjxtsiiio.html

Py:   ",".join(items)
来源：http://hz.redwolf501.top/gtvwdkfiov.html

PHP:  implode(",", $items);
来源：http://hz.bjfxy.top/gtrgzcbdmo.html

JS:   items.join(",")
来源：http://hz.dianchejie.cn/gtkbfriiyq.html

TS:   items.join(",")
来源：http://hz.jianghu66.top/gtlmvvulwz.html

Java: String.join(",", items)
来源：http://hz.chenjidiqi.icu/gtrrbwdimk.html

Go:   strings.Join(items, ",")
来源：http://hz.nwbrower.top/gteebztfis.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtwtybwdjb.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gttrwofuck.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtfbsdamrw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtmaqslxjo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangshuangyany.cn/gtwnhzhppc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtedevheun.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtgczjqxqu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtoyjduyfg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nwbrower.top/gtrcbhwadn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gotoacloud.top/gtfysjznmb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtezjdqtvb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zdqjudy.top/gtykaahaqh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shuidangran.top/gtkhfzcvmp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxinkj.top/gtauctarzx.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtyveobyfj.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtrddreacx.html

Java: String.format("%03d", 7)
来源：http://hz.birdmap.top/gtfasitbmc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fengsongda.top/gtmfmxoait.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shzxlz.cn/gtdvetirys.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.9152youxi.cn/gtimgkdopo.html

[E11] 反转字符串
来源：http://hz.daxiang520.top/gtpngxevfy.html

Py:   s[::-1]
来源：http://hz.meibo888.top/gtuiemockg.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtikkubwsl.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtyuweccjf.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtbalcsgin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtknntejkm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtqyvfvggt.html

Ruby: s.reverse
来源：http://hz.xinyue.icu/gtwtduadbu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtdxioyqpc.html

[E12] 统计某字符出现次数
来源：http://hz.svipenyu.cn/gtfztyxfvr.html

Py:   s.count("a")
来源：http://hz.zhengqikj.top/gtrcqreyof.html

PHP:  substr_count($s, "a");
来源：http://hz.vqdsnc.cn/gtmmrhxilf.html

JS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtaygygbop.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtawecfajq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenzaomai.com/gtdrpjrmcx.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtsrtqfwjd.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gteqkutmxf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.quarkkingdee.top/gtocovscbf.html

[E13] 逐字符遍历
来源：http://hz.nanxinkj.top/gtufizmrvo.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gtvicpztxd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gthtongily.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtxrospelu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtbaizjngx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jianghu66.top/gtupyzmkjr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.9152youxi.cn/gtqajjtibq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gtswbhdhao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gthnzskobe.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gtiamfztru.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.kuanghao11.cn/gtatzhtomj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gtkugmiylp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jlsjyb.cn/gtcmdlirfi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtaowvlkug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tian-w.cn/gticulzupa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.52xcode.cn/gthhbytkbe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtgjhjpqhi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtsvivwuhw.html

[E15] HTML 转义 / 反转义
来源：http://hz.guannengcc.top/gtlyktofra.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hfpthk.cn/gtfsxjsbis.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtajnphgpg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtgjlivpyk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yongpay.top/gtsgataqlk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangtech.top/gtgiejtzsw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gtowtbdtmn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydjk.org.cn/gtnphvevep.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtawgfziai.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtvhvmstfk.html

Py:   f"{1234567:,}"
来源：http://hz.zhoulong.xyz/gtxlxvcobo.html

PHP:  number_format(1234567);
来源：http://hz.fzhhl.top/gtkdrasjyh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtuizoxuyf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtjwtnjqav.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtuwscziuj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guannengcc.top/gtckgrpdij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangtech.top/gtjviorhis.html

C#:   1234567.ToString("N0")
来源：http://hz.guannengcc.top/gtujrgjfht.html

[E17] 首字母大写
来源：http://hz.sufxvd.cn/gtsckokfir.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.snrcjt.cn/gtkufhmtsr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtstoqludi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gtsdjzuwbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtpcdvjbfg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gtahaodzes.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinyuanbaomall.cn/gtkenqiyjn.html

Ruby: s.capitalize
来源：http://hz.daxiang520.top/gtwssazvpe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuxming.cn/gtgguxovse.html


<!-- 参考信息 -->