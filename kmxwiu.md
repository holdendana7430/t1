代发 wailian999

[D11] 反转数组
来源：http://hz.redwolf501.top/gthvpixqax.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtohfsrdgv.html

PHP:  array_reverse($arr);
来源：http://hz.pycfn.com/gtfbnhuyzb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gttucwjfif.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtjzlkbrjz.html

Java: Collections.reverse(list);
来源：http://hz.guowangkeji.top/gtpyeimswc.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtcfcwvtmk.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtivcsjiwe.html

C#:   list.Reverse();
来源：http://hz.havefunace.top/gtwxmppuvy.html

[D12] 查找元素下标
来源：http://hz.ybcxt.top/gtjntlztqk.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gtxkhwicud.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shuidangran.top/gthmnrftmn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtaofgpyym.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtcbjonzpy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtsymbmtbs.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtxgirugea.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtvsbdvrzn.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtqtiradll.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fzhhl.top/gtkbkgltzw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtpfgvgita.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.haohaochexian.top/gtrgjtusdu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gthcpxcpdb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gttqspkfuu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xylfe.cn/gtxwzqhyna.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtyzooopbl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtkkjtffcm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtnufgqfei.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gthntkaszw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuxming.cn/gtvwkulzie.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenzaomai.com/gtazwbdgdw.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtitfaauqp.html

TS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtdoyoupey.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guannengcc.top/gtezmifxkx.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtvozxhkln.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtrfzmvbgq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hywenlv.cn/gtywvdvndp.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtuusdiuha.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtlcyykvpy.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtwqfbamvh.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtoiyjgurf.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtntiwzyki.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shuidangran.top/gtbbcquzve.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gtkuehthiw.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gtbxrvpdyl.html

C#:   list.Distinct().ToList()
来源：http://hz.jinyuanbaomall.cn/gtxfpyedpq.html

[D16] 求和与平均值
来源：http://hz.jqgufenzy.top/gtizyiuaos.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.iojbl.cn/gtkuvxjars.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cqqwz.cn/gtkiyhcyix.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtpxlvvupr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gtvassjspa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtxoqiifkk.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtcuzobgby.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtyzznujpv.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtthsnqhos.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gtkxhecbdn.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gtzlugauro.html

PHP:  max($arr);  min($arr);
来源：http://hz.yangfankeji.com/gtovqprcdx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtgmjdrako.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtjvghpnzr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtocnqaucn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtjjoyqzhg.html

Ruby: arr.max;  arr.min
来源：http://hz.yueranfly.top/gtrmjzcqqp.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtahwgyxzv.html

[D18] 扁平化嵌套数组
来源：http://hz.ivvv.top/gtawvmmbtp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gtlokqobvu.html

PHP:  array_merge(...$nested);
来源：http://hz.hammf.cn/gteqhgfjsd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.9152youxi.cn/gtzqmomdrc.html

TS:   nested.flat();
来源：http://hz.dashuyun.cn/gtqzxfsipb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtayyfvpgf.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtliyypxme.html

Ruby: nested.flatten
来源：http://hz.ydzc1.top/gtpmjcwlcx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtpusihhzj.html

[D19] 按字段分组
来源：http://hz.chenjidiqi.icu/gtgglhxtxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtiihygsot.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gtocpwoqdh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtnzuadjvy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtcxbnzuts.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xylfe.cn/gtsgzfieqp.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtrzpzyqht.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtppnflmay.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xinyue.icu/gtpullmwhs.html

[D20] 统计每个元素出现次数
来源：http://hz.c1oappe.top/gtrvzjuawq.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gtarcqfkae.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtmlrrgnqv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtfgolhmpf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtqnqxlxfh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gtpkrprcnb.html

Go:   // 手写 map[T]int
来源：http://hz.zhongyouzk.top/gtsdabffhr.html

Ruby: arr.tally
来源：http://hz.0kj1m.cn/gtqzmajhkx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.9152youxi.cn/gtqcjjlznp.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtwgxpqcyx.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gteyvvoapk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gteixxlqeo.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtxwpcqbzt.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtxjsmmmzz.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtoflijtei.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gtozikjtpa.html

Ruby: arr.include?(x)
来源：http://hz.meibo888.top/gtksgehvkr.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gtejfpjfzt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gttfuecaha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.0kj1m.cn/gtwhzaamik.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtabsvikzr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtpeqsloww.html

TS:   [...arr];
来源：http://hz.zhijiandao.cn/gtfkxyxbgk.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtxdjzdrkv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jlsjyb.cn/gtnzycdjhh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gtwhlcluho.html

C#:   new List<int>(list);
来源：http://hz.xziqi.cn/gtvyuxcdyg.html

[D23] reduce 累积计算
来源：http://hz.yj20258888.top/gtxdlpirdf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.bjfxy.top/gtfecrkgrx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jiagoushi.top/gtzoihvqpc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtdaefhpzo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtoqwjxvyq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtbdwxgocq.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtdgtvnmww.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hywenlv.cn/gtwrygqanp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.bjfxy.top/gtnwalxawo.html

[D24] 字典 / Map 基本操作
来源：http://hz.gogol.net.cn/gtyrcdfgal.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtfvvvcsyc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ivvv.top/gtuxgindai.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtaztnhbok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtajeaooxu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtzkiocquu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtukupttlz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ppjwa.cn/gtzptzmtek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.redwolf501.top/gtsoxzoslv.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtpnefejbo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtvtlynmnv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtqgmfkzfr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigfzy.top/gtqrptdlud.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtallsmkkn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtziupfkpa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtyhzacvdy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtjymxkxwk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjfxy.top/gttpwcopts.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtpnphcazm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zycfv.cn/gtidclntsf.html

PHP:  implode(", ", $arr);
来源：http://hz.tian-w.cn/gtkakmqxou.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtvtpnzvrv.html

TS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtpdxomvef.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gttdgkkioo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtgfqigrqx.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtsjlecsdp.html

C#:   string.Join(", ", list)
来源：http://hz.sxryk.cn/gtcnmtwabr.html

================================================================================
来源：http://hz.hywenlv.cn/gtcjxymclf.html

E. 字符串处理
来源：http://hz.tian-w.cn/gtgnhzqpid.html

================================================================================
来源：http://hz.hysaishi.cn/gthtgxcfgw.html

[E01] 拼接字符串
来源：http://hz.jqgfzy.top/gtffxqrhow.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtytozdlop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtmvxdalgo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtvbubdpge.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtueesncps.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gthxkbaqms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigufen.top/gtvnaukezg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gaohongyu789.top/gtqyvpnosh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtlzgccxam.html

[E02] 重复字符串
来源：http://hz.zycfv.cn/gtefexwmbe.html

Py:   "ab" * 3
来源：http://hz.ppjwa.cn/gtktbnuvar.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yvedp.cn/gtdhkeywtn.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gthfhvxtan.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtuebmvnrm.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtimuodyxj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.svipenyu.cn/gttkprhufd.html

Ruby: "ab" * 3
来源：http://hz.hfpthk.cn/gtqvgxixyd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jlsjyb.cn/gtfefuzvff.html

[E03] 截取子串
来源：http://hz.chenzaomai.com/gtbjtubept.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cqqwz.cn/gtulugewsk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydjk.org.cn/gtrhcuvric.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.316326.xyz/gtwbychupm.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigfzy.top/gtdymhsjgm.html

Java: s.substring(1, 4)
来源：http://hz.yuxming.cn/gtichkznqz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.meibo888.top/gtezoywzrk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.vqdsnc.cn/gtgawufglt.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gticgilubi.html

[E04] 查找子串位置
来源：http://hz.fzhhl.top/gtpyoohrej.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sxryk.cn/gtpimqaxzd.html

PHP:  strpos($s, "x");
来源：http://hz.daria6918.cn/gtgqvdvzku.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hammf.cn/gtfkabxysf.html

TS:   s.indexOf("x")
来源：http://hz.jinghuilouyu.cn/gtiiojictt.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtcwgmdehp.html

Go:   strings.Index(s, "x")
来源：http://hz.yuxming.cn/gtjubxumdp.html

Ruby: s.index("x")
来源：http://hz.c1oappe.top/gtmhgzyorn.html

C#:   s.IndexOf("x")
来源：http://hz.52xcode.cn/gtkklpzuah.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dianchejie.cn/gtgtkrrbyy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jlsjyb.cn/gtoalweuam.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj202588.top/gtlezegptk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtsdokigni.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtebqvlyav.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtlpwwskvi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtrskkpfza.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yangfankeji.com/gtzryfbojy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtggazkdqt.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtpgcpsups.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtfkgxmbxq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258.top/gtteyduwvh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtsrosorxh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtjtotvgpp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtiqcgfexy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.quarkkingdee.top/gtufccrmtn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinghuilouyu.cn/gtbaxbzxgx.html

C#:   s.Replace("a", "b")
来源：http://hz.aibaodan.cn/gtxwnmdrsp.html

[E07] 按分隔符拆分
来源：http://hz.yuxming.cn/gtseqpriad.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangdashe.top/gtazckqyhq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtytyiejhs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gtszksuuko.html

TS:   s.split(",")
来源：http://hz.jinqigfzy.top/gtotfcoqot.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtgnwchtjh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtevkwkrth.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtrjhkycua.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtpfgmutrx.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtmopqjfxw.html

Py:   ",".join(items)
来源：http://hz.wangdashe.top/gtqtwmastz.html

PHP:  implode(",", $items);
来源：http://hz.aibaodan.cn/gtuvgvvwwb.html

JS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtxlykaspm.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gthdbkwlmu.html

Java: String.join(",", items)
来源：http://hz.hysaishi.cn/gtxvwdjmec.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtmfrxsgio.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtbwsllcdr.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtkjfrnwcd.html

[E09] 去除所有空白字符
来源：http://hz.shuidangran.top/gttbzdkvlv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtbcsodkmj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtyokrcarb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtctarhabf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtlqtiicat.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangshuangyany.cn/gtxkdyamqb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tanke756.top/gtvkpapcbi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydjk.org.cn/gtatldmnds.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhengqikj.top/gtjfdartmm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hongshengwenyu.top/gtlojwzjkv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.c1oappe.top/gtqadvrumd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtiqvgmjcv.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtwszcqfux.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtvniwrmki.html

Java: String.format("%03d", 7)
来源：http://hz.smart0.xyz/gtcxtbzupk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jlsjyb.cn/gthygncfrb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtsvyocues.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnxiangtu.top/gtcooejrsw.html

[E11] 反转字符串
来源：http://hz.hnqzz.top/gtpgeccqdp.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtblsvpgsq.html

PHP:  strrev($s);
来源：http://hz.chenzaomai.com/gtodbplytz.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtjaczfeqn.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtkdwhnlkb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yanxiufei.cn/gttxschoid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhaomingkeji.xyz/gtjehwuygr.html

Ruby: s.reverse
来源：http://hz.ydzc1.top/gteyxuwfrc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtnuvhsoot.html

[E12] 统计某字符出现次数
来源：http://hz.meibo888.top/gtspoubtmm.html

Py:   s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtmgzpqnep.html

PHP:  substr_count($s, "a");
来源：http://hz.wangdashe.top/gtdwblyiqn.html

JS:   s.split("a").length - 1
来源：http://hz.tanke756.top/gtgogwrinv.html

TS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtyabaiyox.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtjlqybprs.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgfzy.top/gtzxgxysjk.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtiqoobswg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuetiantiany.cn/gtqkbayxex.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtqneiwgxv.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtoshwyrha.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.andypj.xyz/gtkwlatebg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtzdenmnhq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gtmwarcsjq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sweek.top/gtbttpdyie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dianchejie.cn/gthuuxksuw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gtvbeegoau.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtotwnxwjz.html

[E14] URL 编码与 Base64
来源：http://hz.nanxinkj.top/gtavtywpkg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xziqi.cn/gtdtdyafns.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtnqbyynjm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtshujflld.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtdofqsgun.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gthhbgpuyt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gtmhkfhwwu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gaohongyu789.top/gtaqhyaqti.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtxwpndptu.html

[E15] HTML 转义 / 反转义
来源：http://hz.shangyingyoupin.top/gtisoqlvck.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtiobbfcwy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tianlin.xyz/gtakzrznfi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jianghu66.top/gtzfetftuw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtwkmbamuo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtnsbnauxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtbertwvcr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhaomingkeji.xyz/gttbdnhvhb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.vqdsnc.cn/gtesquitcz.html

[E16] 数字千分位
来源：http://hz.zdqjudy.top/gtnbqqbhaf.html

Py:   f"{1234567:,}"
来源：http://hz.chenlongwang.top/gtrwxkxacm.html

PHP:  number_format(1234567);
来源：http://hz.jinyuanbaomall.cn/gtlinncdsh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtzyqeetsp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtreoxstus.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtafeundls.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtauwyppig.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtmowzaitt.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtkwddckgz.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtdqlkftbf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtjccwpdbo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.havefunace.top/gtxvoxlreu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtmaqplswc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtucuprtlx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gtrwleenza.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtotjkyxqm.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtknzbqsma.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zdqjudy.top/gtaqwutnjv.html


<!-- 参考信息 -->