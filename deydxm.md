代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtjknisykc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cdnleiting.top/gtrnclznwe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinyuanbaomall.cn/gtaxefnjqs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hongshengwenyu.top/gtcpwlfpah.html

[D11] 反转数组
来源：http://hz.shanyushiyangtech.top/gtwyjqlbfi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ppjwa.cn/gtmdfdxrhz.html

PHP:  array_reverse($arr);
来源：http://hz.xuanzx.com/gtdoaapbxm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtsedbbusw.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtxecdgloo.html

Java: Collections.reverse(list);
来源：http://hz.andypj.xyz/gtirxeiiqw.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtvbssugcs.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtvjzstghf.html

C#:   list.Reverse();
来源：http://hz.aizwys.cn/gtbobwllhf.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtxbvlagfl.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gtzuqjnzsx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuetiantiany.cn/gtxjlamivk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtromybwgl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtrmaencbg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hnqzz.top/gtqfxbdixj.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtofseepbz.html

Ruby: arr.index(x)
来源：http://hz.jyoumei.cn/gtxbymozgh.html

C#:   list.IndexOf(x);
来源：http://hz.cheryme.top/gtevjfiiyp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhengqikj.top/gtciurfuia.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtghxwxyit.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtpjxmrkgz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtcagfxbsz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtqyktlrtm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhixingplan.top/gthkjdczdy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daxiang520.top/gtdfvfasem.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtslbktqqq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtcpzsreps.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yvedp.cn/gtfpgvgbmt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xziqi.cn/gtdkokmocv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sxryk.cn/gtjepxqbpm.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtrtftavnx.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtvdnannwl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuanzx.com/gtytrevcib.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtuvvxffyd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtadsbxvpy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gtdqyyuunk.html

[D15] 去重
来源：http://hz.nwbrower.top/gtslfeutvh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtchqfnzay.html

PHP:  array_unique($arr);
来源：http://hz.guowangkeji.top/gtiiubrqar.html

JS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtrrvnqwhq.html

TS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtxkvyprqk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenjidiqi.icu/gtfgvlkclw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtkahdtcaa.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gthznpkerg.html

C#:   list.Distinct().ToList()
来源：http://hz.ybcxt.top/gtufhllamd.html

[D16] 求和与平均值
来源：http://hz.iojbl.cn/gtgnobodou.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jiagoushi.top/gtccknpiqu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtrxoeuplx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtirhfrvcv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gthjeweqvc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtjzkmfsvz.html

Go:   // 手写循环累加
来源：http://hz.ehwqpu.com/gtfxmaryyf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtyofuppnp.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258888.top/gtgrraljnf.html

[D17] 最大值与最小值
来源：http://hz.jqgufenzy.top/gtkwjxhqtv.html

Py:   max(arr);  min(arr)
来源：http://hz.ydjk.org.cn/gthgcfbzqi.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtbixlwurq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daxiang520.top/gtnsrxtrcd.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtbrrvuykc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtieatlujh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnxiangtu.top/gtmsxbqrwg.html

Ruby: arr.max;  arr.min
来源：http://hz.cdnleiting.top/gtbaeorsfd.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gtkiqaaguu.html

[D18] 扁平化嵌套数组
来源：http://hz.hnqzz.top/gtoszyzktk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yonumen.top/gthnmsqdwb.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtkiizffov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtdwdunmvr.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtlacjieyl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.redwolf501.top/gtnmukzgby.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtxjanudhz.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtbucwtpkz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtxebdymia.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gtzskauirr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ywan-chungtsiang.top/gtpzykfsyz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ppjwa.cn/gtrfxrnvrb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.aizwys.cn/gtqprhxeyx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtofkgwslj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtfyryeriu.html

Go:   // 手写 map[string][]T
来源：http://hz.redwolf501.top/gttnksnrwi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenlongwang.top/gthikoxyir.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtikpkyflw.html

[D20] 统计每个元素出现次数
来源：http://hz.hywenlv.cn/gtrllluwaw.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtarirpovq.html

PHP:  array_count_values($arr);
来源：http://hz.jyoumei.cn/gttgzfbaak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtnvyqchmd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtklvbuhnu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jiagoushi.top/gtoxzspzsy.html

Go:   // 手写 map[T]int
来源：http://hz.andypj.xyz/gtmwnnnzuh.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gttvaooykf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hywenlv.cn/gttinrjxkc.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gttzlfncju.html

Py:   x in arr
来源：http://hz.hywenlv.cn/gtdaxlxzjp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.0kj1m.cn/gtolbhzfqo.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtfuqgdwrl.html

TS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtntkbeoxj.html

Java: list.contains(x)
来源：http://hz.meibo888.top/gthovcmzdg.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhengqikj.top/gtpkdwkhff.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtwaftukzl.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gtoxnpthhd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ybcxt.top/gtndlsiyqn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.meibo888.top/gtqjkiocyh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guannengcc.top/gtfovzjlem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigufen.top/gtvunvsqci.html

TS:   [...arr];
来源：http://hz.jlsjyb.cn/gtlafiogzm.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtbeivbgti.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dianchejie.cn/gtgxlrdetg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fengsongda.top/gtfhaufnis.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtgdiiyytm.html

[D23] reduce 累积计算
来源：http://hz.hnqzz.top/gtjvoursgu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtnitpkbeh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhongyouzk.top/gtotyauzrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtmvhpwhwf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtsdboqbcc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtrnsnfjkn.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtauexdjlq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtaujlgbqi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daxiang520.top/gtncsotxmu.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtbckpwoby.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtpcvkkerq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guowangkeji.top/gtgouwkeri.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xinyue.icu/gtcibrtong.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hfpthk.cn/gtbsbvezls.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtyywcgdam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtifpstrib.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuxming.cn/gtqtorlcui.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtkcqzergb.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtbramlqqt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cqqwz.cn/gtcayzhrgz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dianchejie.cn/gtagyrsgfx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.mhx1999.top/gtfopfuqfk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtgmyhbvwd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.52xcode.cn/gtjgwecujo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.c1oappe.top/gtwfrgooid.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtoygeduzw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtlpxggcsb.html

[D26] 数组转字符串
来源：http://hz.nanxuanxn.top/gtcvjplryy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtejkvrtiw.html

PHP:  implode(", ", $arr);
来源：http://hz.zdqjudy.top/gtfhjjcasd.html

JS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtxgzlbiri.html

TS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtyuljejxy.html

Java: String.join(", ", list)
来源：http://hz.vqdsnc.cn/gtpxyuqvdo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtonzmiuml.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtkggmdctu.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtngbramee.html

================================================================================
来源：http://hz.cheryme.top/gtweqncmfg.html

E. 字符串处理
来源：http://hz.chenzaomai.com/gteywuknuw.html

================================================================================
来源：http://hz.shuidangran.top/gtezksbtng.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtshdrejuu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.meibo888.top/gtrxlovksp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtfbhkujpe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtdlkkbiwu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gttyjvjjai.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtmfhzhbjd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sxryk.cn/gtmrhwhpwv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cashguo.top/gtflogedbl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258888.top/gtqrhrfqkp.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gteumujsud.html

Py:   "ab" * 3
来源：http://hz.quarkkingdee.top/gtqkfuxaho.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtotbamgog.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtwxmtfzny.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtetgdrwow.html

Java: "ab".repeat(3)
来源：http://hz.52xcode.cn/gtcsgpyilw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.quarkkingdee.top/gtjestsilw.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtpnnvfpjx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258.top/gtntieztyl.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtmknettfz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shuidangran.top/gthcaadfpo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydjk.org.cn/gtcjdkdxpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gzhubu.top/gtmrbnoqvj.html

TS:   s.slice(1, 4)
来源：http://hz.zdqjudy.top/gtccgapcho.html

Java: s.substring(1, 4)
来源：http://hz.yvedp.cn/gtgajbxewl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hammf.cn/gtwecmlugf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtljjuscgk.html

C#:   s.Substring(1, 3)
来源：http://hz.tian-w.cn/gtvyiwuryo.html

[E04] 查找子串位置
来源：http://hz.gotoacloud.top/gtilxnkjhw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hnqzz.top/gtigavvnej.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtvhdrzjcb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haohaochexian.top/gtzcctyjyl.html

TS:   s.indexOf("x")
来源：http://hz.kuanghao11.cn/gtddczbppu.html

Java: s.indexOf("x")
来源：http://hz.andypj.xyz/gtgzcgctoa.html

Go:   strings.Index(s, "x")
来源：http://hz.chenlongwang.top/gtkcxtmtes.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtdvdccwgu.html

C#:   s.IndexOf("x")
来源：http://hz.chenlongwang.top/gthgxxbups.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtzwbdgyhg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.quarkkingdee.top/gtyehssqde.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenjidiqi.icu/gtaqcsmwtz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtxenjhbwv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtkimephbe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtofmxoqwf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhoulong.xyz/gttsyqievp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydzc1.top/gtnbkssehq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.bjfxy.top/gtkeffuvfq.html

[E06] 替换子串
来源：http://hz.jqgufenzy.top/gtteycuafd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtdmkomtif.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gttnulgkzq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gthvetlfwg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtezvhbljy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtpfszjrci.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gogol.net.cn/gtjofcnedn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gteldcxnig.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtggqswvml.html

[E07] 按分隔符拆分
来源：http://hz.yuanzhike.top/gtlvytzjig.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtilrzmpki.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhixingplan.top/gtvuotjyai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtcfnfwqnj.html

TS:   s.split(",")
来源：http://hz.zhengqikj.top/gtunqkxkxc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangdashe.top/gtqtnffhdu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtljswrswz.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gthihpzavn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhiwuduotai.top/gtaozeiazi.html

[E08] 数组按分隔符合并
来源：http://hz.jyoumei.cn/gtafuoresi.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtguorudjv.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gttzexuhfq.html

JS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtitnrjbgy.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtzcqkgjfd.html

Java: String.join(",", items)
来源：http://hz.jqgfzy.top/gtxkughfnq.html

Go:   strings.Join(items, ",")
来源：http://hz.shuidangran.top/gtmowdrvgk.html

Ruby: items.join(",")
来源：http://hz.jiagoushi.top/gtitxgghty.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gtvgkrtojl.html

[E09] 去除所有空白字符
来源：http://hz.dianchejie.cn/gtewynrrzs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtbnkkkqkx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tanke756.top/gtxcgfzlyz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtcuzaykog.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtwwqyyirg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtgjknvfyc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yonumen.top/gtambaugaa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.0kj1m.cn/gtsjfuecld.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aibaodan.cn/gttkyjreuz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtogwobrdp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtzwtuqmob.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtoupznuok.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtcuyfvmyd.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtrixqtgnq.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gteuhspdsx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.kuanghao11.cn/gtddidixed.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtsolhnfzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ehwqpu.com/gtisstnqru.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gtszfxpcma.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtrvzncsre.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gttlfrisxj.html

JS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtkswuzdkf.html

TS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtrhovlrke.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yangfankeji.com/gtjhldtwba.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtepouvvpj.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtezaywyih.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtxungvlpp.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gttpjbxyny.html

Py:   s.count("a")
来源：http://hz.yvedp.cn/gttlntfszy.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtshovclvv.html

JS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtmsigkdjo.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtjacglkex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.316326.xyz/gtlwbuxcrt.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgfzy.top/gtqzemdxit.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtktodpjpo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daria6918.cn/gtyfhdcedd.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtuwakdibk.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtvtlxcxuy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sxryk.cn/gthzahazzy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtqezabkcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtugecgkjd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gthwerwqrf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtjeybrnxs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnxiangtu.top/gtrwcflyoh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangdashe.top/gtdzxxxbmf.html

[E14] URL 编码与 Base64
来源：http://hz.smart0.xyz/gtombtoaky.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pengpengdd.cyou/gtfadftkjs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtfqtnxoaq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtfpozzkmf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtycfndxvk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtuonoddzc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtwttuauji.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fzhhl.top/gtnskxjqcz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtjygsmurn.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gtipenepsg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ppjwa.cn/gtffhtyfqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtytemiprs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtjbbkellh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sufxvd.cn/gtsvigfiei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtahrveauf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jianghu66.top/gtdtxauhsy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fzhhl.top/gtmydlxlch.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gtpclpoghr.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gthmyjmyce.html

Py:   f"{1234567:,}"
来源：http://hz.havefunace.top/gtcwpbjeig.html

PHP:  number_format(1234567);
来源：http://hz.iojbl.cn/gtepdiznzr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtrnjrrhvd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtuvaavust.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuanzhike.top/gtuhpkesth.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gtsvpuszcr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtfqedhbsw.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtuxibsvas.html

[E17] 首字母大写
来源：http://hz.yueranfly.top/gtqwrgchaf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gaohongyu789.top/gtiuykyfrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtesvfpota.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtxnezgmdd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtlkcmkcwt.html


<!-- 参考信息 -->