代发 wailian999

[D11] 反转数组
来源：http://hz.hysaishi.cn/gtclrwbzrh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shzxlz.cn/gtvqatmbym.html

PHP:  array_reverse($arr);
来源：http://hz.vqdsnc.cn/gtuwmdcjrk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnxiangtu.top/gtbwdtcsgx.html

TS:   [...arr].reverse();
来源：http://hz.cheryme.top/gtcibsirwe.html

Java: Collections.reverse(list);
来源：http://hz.redwolf501.top/gtvhaxklnc.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtnzxjjjjs.html

Ruby: arr.reverse
来源：http://hz.hfpthk.cn/gtuytiyycb.html

C#:   list.Reverse();
来源：http://hz.jqgufenzy.top/gteqyhulfm.html

[D12] 查找元素下标
来源：http://hz.52xcode.cn/gtfutxpqmk.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenlongwang.top/gtgqxtcjzd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.havefunace.top/gtshlfdghn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtjsybhnrj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtljqlncal.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gtqnheejxw.html

Go:   slices.Index(arr, x)
来源：http://hz.yangfankeji.com/gteigacdwn.html

Ruby: arr.index(x)
来源：http://hz.jinqigufen.top/gtvweneilp.html

C#:   list.IndexOf(x);
来源：http://hz.cdnleiting.top/gtwfjmcwon.html

[D13] 过滤（保留满足条件的）
来源：http://hz.aibaodan.cn/gthsksjikr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ywan-chungtsiang.top/gtbdsnhext.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gtatjduvvm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtllfbxxwg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gtqgtjssnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.feifeiyinyue.top/gtxapsrahx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtcxtyypvi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtitetsilo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtjcvvulwb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.redwolf501.top/gtcofnlmtv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yongpay.top/gtdxedbigx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtjvpilsuy.html

JS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtzebyxelb.html

TS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtvepvnzmy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtqhofdlep.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtouoaquah.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aibaodan.cn/gtkcunpybj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cdnleiting.top/gttbmdxvwr.html

[D15] 去重
来源：http://hz.shanyushiyangtech.top/gtpjfcdmar.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gttwkxdqtm.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtunsibvuq.html

JS:   [...new Set(arr)]
来源：http://hz.andypj.xyz/gtgopwyqru.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtnadfydvc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtqdceioti.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgfzy.top/gtgeikalkh.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtffdwzhfn.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtrxwuaefp.html

[D16] 求和与平均值
来源：http://hz.bjfxy.top/gttpsilqlf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtbqrefwou.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sweek.top/gtfinsvuia.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtzxknwcye.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gttaajytes.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtutjuacxy.html

Go:   // 手写循环累加
来源：http://hz.aizwys.cn/gtasbbgxzw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtyxohsjlb.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigfzy.top/gtojwtricl.html

[D17] 最大值与最小值
来源：http://hz.dashuyun.cn/gtzadfssau.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtyipkvofj.html

PHP:  max($arr);  min($arr);
来源：http://hz.cdnleiting.top/gtbnnrjmer.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtvbfeegzd.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtboukfnbk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtajgzptpg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtxkpzcood.html

Ruby: arr.max;  arr.min
来源：http://hz.hammf.cn/gtbjczkwvs.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtdhmwcpjh.html

[D18] 扁平化嵌套数组
来源：http://hz.wangdashe.top/gtrueialii.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guowangkeji.top/gtrxmifwpw.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtxtpbyhyt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jiagoushi.top/gtaomvtsiz.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtgbhzldyk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.svipenyu.cn/gtyxawduge.html

Go:   // 手写双层循环
来源：http://hz.tianlin.xyz/gthewhcovt.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtjvqtqngs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dianchejie.cn/gtitchbdxf.html

[D19] 按字段分组
来源：http://hz.zdqjudy.top/gteutqnrpb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhengqikj.top/gttmdvgnez.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtadlwhrmn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhijiandao.cn/gtnzuscwmx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtpdrdtwkw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhiwuduotai.top/gtuackygis.html

Go:   // 手写 map[string][]T
来源：http://hz.ybcxt.top/gtzufgukot.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gticzltbrz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtjitpqqqe.html

[D20] 统计每个元素出现次数
来源：http://hz.gogol.net.cn/gtzehmaonz.html

Py:   Counter(arr)
来源：http://hz.ydzc1.top/gtuirwvztv.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtkbtkvdop.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gthlaofiut.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtnysgxqki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.bjfxy.top/gtqdemlgxz.html

Go:   // 手写 map[T]int
来源：http://hz.aibaodan.cn/gtznimumgl.html

Ruby: arr.tally
来源：http://hz.gotoacloud.top/gtmspjzlru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yanxiufei.cn/gtbtvpmgna.html

[D21] 判断是否包含某元素
来源：http://hz.tanke756.top/gtagzocvss.html

Py:   x in arr
来源：http://hz.daria6918.cn/gtditlxrvq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtuxxwkxgp.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtdrcmzucp.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtqopubwlv.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtmdeaclow.html

Go:   slices.Contains(arr, x)
来源：http://hz.nwbrower.top/gtyvhfmzfo.html

Ruby: arr.include?(x)
来源：http://hz.birdmap.top/gtgapilikk.html

C#:   list.Contains(x)
来源：http://hz.zhoulong.xyz/gtoigayvcr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guannengcc.top/gthqojbwaz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ybcxt.top/gtwftrmccx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.birdmap.top/gtvudtwqyr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dianchejie.cn/gteejjmfid.html

TS:   [...arr];
来源：http://hz.ydjk.org.cn/gtavhtxinm.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtpbwirdjg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tanke756.top/gtkdoeizwc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ybcxt.top/gtthujwepd.html

C#:   new List<int>(list);
来源：http://hz.xziqi.cn/gtzvhwndom.html

[D23] reduce 累积计算
来源：http://hz.zhijiandao.cn/gtqebpwuvr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yanxiufei.cn/gtwrwfhqaj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cashguo.top/gtdaesyrag.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtwuaxgnve.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtublidpea.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yangfankeji.com/gtalouvzxn.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtcwlxbtei.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.9152youxi.cn/gtcertxnax.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtvwpxrwmx.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtydrnirqv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.birdmap.top/gtghjolmdq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgfzy.top/gtqbhfnnxk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.mhx1999.top/gtrnuzmvly.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gtqlwuilnt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.svipenyu.cn/gtwxmwnlqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtdzlwbvzq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yanxiufei.cn/gtrlqitvpv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gthxmioxpz.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gtzxxokdcs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gtszthkoid.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guowangkeji.top/gtlxcgpgzw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sxryk.cn/gtitltrxcl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenjidiqi.icu/gtytrauisf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtfwrncevw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gtevdkecaw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shzxlz.cn/gtroohjkkm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtvkfgwhjt.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtrmttmmrc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cucudq.cn/gttkttiavc.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gtclnelnqx.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtxxndnlrj.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtargmztvk.html

Java: String.join(", ", list)
来源：http://hz.jinqigfzy.top/gtwbubmxnl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtmrubmtqo.html

Ruby: arr.join(", ")
来源：http://hz.mhx1999.top/gtrchcjgqg.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtjpjkqrof.html

================================================================================
来源：http://hz.haohaochexian.top/gtkurqucol.html

E. 字符串处理
来源：http://hz.yuanzhike.top/gtxugxeoau.html

================================================================================
来源：http://hz.316326.xyz/gtbfcrlmei.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtdvtgyxpg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydjk.org.cn/gtwyigrpvc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.redwolf501.top/gtfiuvwngz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gtjkcpayen.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtwtcgikez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guowangkeji.top/gtycpafzql.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtnpldtiev.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.bjfxy.top/gtagbrrzbo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtdnrolkkp.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtbrcvyxsn.html

Py:   "ab" * 3
来源：http://hz.jqgfzy.top/gtogaxxlyh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zycfv.cn/gteewvirtf.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gttrmolojm.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtpdupuxre.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gtlhbsqndv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtkylynrsc.html

Ruby: "ab" * 3
来源：http://hz.chenzaomai.com/gtclmbatbm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtydbuaral.html

[E03] 截取子串
来源：http://hz.jinghuilouyu.cn/gtlfoshund.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtelbcxvui.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.meibo888.top/gtmqfehtks.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtjoxnymxn.html

TS:   s.slice(1, 4)
来源：http://hz.chenjidiqi.icu/gtzywdriwt.html

Java: s.substring(1, 4)
来源：http://hz.zycfv.cn/gtcakmvtbv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jlsjyb.cn/gtzoftdibf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sxryk.cn/gtfrfwagej.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gtcmamnkrx.html

[E04] 查找子串位置
来源：http://hz.cqqwz.cn/gtajqjeipp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhiwuduotai.top/gtpnzxkaoj.html

PHP:  strpos($s, "x");
来源：http://hz.cashguo.top/gtzhihxtyl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnqzz.top/gtpzbtqmwc.html

TS:   s.indexOf("x")
来源：http://hz.tian-w.cn/gtytlebmxg.html

Java: s.indexOf("x")
来源：http://hz.ybcxt.top/gtswogsoeh.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtxtalhzde.html

Ruby: s.index("x")
来源：http://hz.xinyue.icu/gtksojqdsl.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gthsmcdjut.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fzhhl.top/gtivlrwuyj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gtaliugiat.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.9152youxi.cn/gtudmsxoyi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtguvnofyv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtyegtitvr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtlafwwifm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gtbjpuydvs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigfzy.top/gtuoawqgvl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gzhubu.top/gtmiddlpuf.html

[E06] 替换子串
来源：http://hz.xziqi.cn/gtouhhnisr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ydjk.org.cn/gtrjttnnkm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtfwkrsikm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtzxagqwxu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtzzhsekgi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtdxufxqgn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guannengcc.top/gtkjfeqrnf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtmgtqgxbm.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtexnqfrbw.html

[E07] 按分隔符拆分
来源：http://hz.yuanzhike.top/gtsqstvysy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cqqwz.cn/gtjnwqfohf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtgodhfxtv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtzxxvkhib.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtqgyjhcdp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gtaibddpew.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gtmmhzvxul.html

Ruby: s.split(",");  s.split
来源：http://hz.ydzc1.top/gtiukkabrn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhengqikj.top/gtvyacajeg.html

[E08] 数组按分隔符合并
来源：http://hz.ehwqpu.com/gtqaespgpp.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtxpzujstw.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gtthabkjkd.html

JS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtonnjpltb.html

TS:   items.join(",")
来源：http://hz.0kj1m.cn/gtcycoqzqf.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gttrnnshhj.html

Go:   strings.Join(items, ",")
来源：http://hz.zdqjudy.top/gtxsxtzcgr.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtdeaqlqqc.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtvzdvnrci.html

[E09] 去除所有空白字符
来源：http://hz.yvedp.cn/gtgnggdjke.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tanke756.top/gtlybipuiq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtzjlxkiqr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtphqwzslz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtbnbbujic.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxinkj.top/gtopezcylb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.svipenyu.cn/gtwldhberm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gtqygjvlva.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gteaegupys.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtkgiahycq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jyoumei.cn/gtbaaiqbeb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.0kj1m.cn/gtgrdeazkk.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtdcwtphtv.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtrsqpgfet.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtcoqezhdd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhijiandao.cn/gtgreshiwn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtjvylnpjc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigfzy.top/gthzkxvyqm.html

[E11] 反转字符串
来源：http://hz.chenjidiqi.icu/gtipnguryu.html

Py:   s[::-1]
来源：http://hz.wangshuangyany.cn/gtmdpogqbg.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gtmhpzviqp.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtdazoyiye.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtglgbsozt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.9152youxi.cn/gtpxjajkid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cucudq.cn/gtffwvzsdr.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtnjxnyaol.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gthftsbroa.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtbmekcmwt.html

Py:   s.count("a")
来源：http://hz.jyoumei.cn/gtzjgauahc.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gtowbvvqjd.html

JS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtzilszjgw.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtbdehylyv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtoxljtolj.html

Go:   strings.Count(s, "a")
来源：http://hz.hammf.cn/gttdqlomlx.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gtwsrahdef.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtncfqlath.html

[E13] 逐字符遍历
来源：http://hz.andypj.xyz/gtsbiuyxnb.html

Py:   for ch in s: print(ch)
来源：http://hz.gaohongyu789.top/gtorgbqpdv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sufxvd.cn/gtuzxwdkix.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtqfabkuqy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtgfcbkpht.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtgaguvutl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhixingplan.top/gtzpamxmet.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gtrzctiynr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jlsjyb.cn/gtcsqyywvf.html

[E14] URL 编码与 Base64
来源：http://hz.xuetiantiany.cn/gtnrrjikaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.52xcode.cn/gtqtpmnymk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pycfn.com/gtanineyyu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinghuilouyu.cn/gttcieqyxo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtnypkyvbq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dianchejie.cn/gttkdzipgi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtfmhgyuwn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pengpengdd.cyou/gtwgdsrupk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fengsongda.top/gtttlhrdhc.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gtzyhjgiqo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.svipenyu.cn/gtbrdoaksu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.dianchejie.cn/gtteiemmbr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtccqtjgnt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtkwfbphcw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hywenlv.cn/gtmflilysx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxinkj.top/gtchfxqnuj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigfzy.top/gttppreqwp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shangyingyoupin.top/gtzhqdemzk.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtllzcduyq.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtxbhcfwry.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtfgjxties.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.316326.xyz/gtoxwwuntw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtnzzpxbzs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xylfe.cn/gthrgzxzph.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shzxlz.cn/gtbjbbcjtg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.mhx1999.top/gtvufkonco.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtibisjhkf.html

[E17] 首字母大写
来源：http://hz.xziqi.cn/gthllrbwxm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtzeoqtade.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tianlin.xyz/gtbreabdxl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtzxxpmcpd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtpuodlaga.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jlsjyb.cn/gtvnnayija.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinyuanbaomall.cn/gtpouoqsoo.html

Ruby: s.capitalize
来源：http://hz.dashuyun.cn/gtawlxnnof.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daria6918.cn/gtbkdfjgla.html


<!-- 参考信息 -->