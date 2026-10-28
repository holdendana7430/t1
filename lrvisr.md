代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtcrmiruxg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtuqvmsevw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gthhhjpnci.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtpzayhbmc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtnsdfnplx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xziqi.cn/gtckvoccbi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhongyouzk.top/gtkwejepia.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtsripdflx.html

[D11] 反转数组
来源：http://hz.0kj1m.cn/gtlmknizlj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtyytcbazt.html

PHP:  array_reverse($arr);
来源：http://hz.ydjk.org.cn/gtitrxrtfl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtjdyohlde.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtesvamhya.html

Java: Collections.reverse(list);
来源：http://hz.shzxlz.cn/gtpyceufpb.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258888.top/gtrugvcutc.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gtfbhunykj.html

C#:   list.Reverse();
来源：http://hz.cheryme.top/gtuwfokzcc.html

[D12] 查找元素下标
来源：http://hz.ivvv.top/gtntelzzyu.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgufenzy.top/gtoayeoesi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtymbkuvli.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtctojucfd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtvwixggsg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.iojbl.cn/gthsdpznkm.html

Go:   slices.Index(arr, x)
来源：http://hz.yonumen.top/gtbdstmzbv.html

Ruby: arr.index(x)
来源：http://hz.ppjwa.cn/gtnmzrecpy.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtpxwhbcjp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xylfe.cn/gtktouigjc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtwrbouswk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fengsongda.top/gtdlxpsyxt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtlwvfqnfu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtvhewanfp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtudwoydgi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtufnwceub.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yongpay.top/gtdbuovkup.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtqmgssvga.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gtrbgvtovx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj202588.top/gtpjjnxbyu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tian-w.cn/gtbbibecwd.html

JS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtehydzrzr.html

TS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtdgthklhd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj202588.top/gtuwlpyfpj.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtjvcigprr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtrptqsghm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aizwys.cn/gtxqdgokpj.html

[D15] 去重
来源：http://hz.yj20258888.top/gtglxcpgxc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhengqikj.top/gtodbmjfbx.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtrqvctgoa.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gthzbwdtkv.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtwnfgtscx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtxalubymd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtjfmssthg.html

Ruby: arr.uniq
来源：http://hz.gzhubu.top/gthojmhxha.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gtxppbgxxo.html

[D16] 求和与平均值
来源：http://hz.hysaishi.cn/gtrjatxgjt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.svipenyu.cn/gtensezoib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuanzx.com/gtccqmmbbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtiwdlhlqn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtcjpoxzsl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtsziivbao.html

Go:   // 手写循环累加
来源：http://hz.xuetiantiany.cn/gtkugutmpb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtsykqqeyw.html

C#:   list.Sum();  list.Average()
来源：http://hz.sysykeji.top/gtsmdjyqsp.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtbqnyjwuw.html

Py:   max(arr);  min(arr)
来源：http://hz.sxryk.cn/gtoaozvxar.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtbamzdqnz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sufxvd.cn/gtxkhsvvsa.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtxvrabyjl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtryurjswm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ybcxt.top/gtxlenxbwt.html

Ruby: arr.max;  arr.min
来源：http://hz.ppjwa.cn/gtaiwypldu.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtvymwtpcs.html

[D18] 扁平化嵌套数组
来源：http://hz.gaohongyu789.top/gtnymguaql.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pengpengdd.cyou/gtzdsumybf.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gtvqhbtbfq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nanxinkj.top/gtudgxkelk.html

TS:   nested.flat();
来源：http://hz.9152youxi.cn/gtnxjpwxut.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.c1oappe.top/gtddofvjpi.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtsfezehgl.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtihsjwmqv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnxiangtu.top/gtscnbvuzp.html

[D19] 按字段分组
来源：http://hz.sxryk.cn/gtfbughlmv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtnuwrozpw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtiomblxzj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yvedp.cn/gtxvfhmwce.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtexlmjqvl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guowangkeji.top/gthijaafkh.html

Go:   // 手写 map[string][]T
来源：http://hz.ywan-chungtsiang.top/gtjtqgneeo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangkeji.top/gteeecngwk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtruqrfpcm.html

[D20] 统计每个元素出现次数
来源：http://hz.zhongyouzk.top/gtszmloyux.html

Py:   Counter(arr)
来源：http://hz.zhixingplan.top/gtlzootkib.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtaxnwdzmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtieveuhks.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtkutkkozv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.smart0.xyz/gtxruurmwv.html

Go:   // 手写 map[T]int
来源：http://hz.zhaomingkeji.xyz/gtkgmaaqxt.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gthiacvboe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtgtksnltt.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtwqozwwas.html

Py:   x in arr
来源：http://hz.snrcjt.cn/gtbrcdplap.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zycfv.cn/gtuixwkqxz.html

JS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtbbhpeepm.html

TS:   arr.includes(x)
来源：http://hz.yonumen.top/gtefvnkqgm.html

Java: list.contains(x)
来源：http://hz.jiagoushi.top/gtimothjmv.html

Go:   slices.Contains(arr, x)
来源：http://hz.guannengcc.top/gtjivvtxah.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gteqghjqil.html

C#:   list.Contains(x)
来源：http://hz.zhiwuduotai.top/gtagalbbhs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yueranfly.top/gtteplypdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtvoahfxgj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtoektbhxr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigfzy.top/gtmbqxlvsw.html

TS:   [...arr];
来源：http://hz.0kj1m.cn/gtattinzcw.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtgiqrgjps.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtlzohscuk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtjsrcurtp.html

C#:   new List<int>(list);
来源：http://hz.cqqwz.cn/gtymsgymlr.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtjvogzagv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhengqikj.top/gtevemcqzf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtszjzyuvh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gogol.net.cn/gtyabsddlz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtwanrekkd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenlongwang.top/gtliqirurh.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtcftpzfjf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtmqnwwtwv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gthcpsuxms.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtfqzfsjjd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.havefunace.top/gthmwlvtuj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinghuilouyu.cn/gtnjqwnhkr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigufen.top/gtsvphijpf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fzhhl.top/gtyjqzbmfm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xziqi.cn/gttbzemiul.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtwxvpuwwd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gthexjbomn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gthzowqmqe.html

[D25] Set 集合去重与交并差
来源：http://hz.hammf.cn/gtoylcyfhk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtkmmkeupo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daria6918.cn/gtxzktrsgr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.meibo888.top/gtdrqcpjap.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shuidangran.top/gtorcjnurf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ehwqpu.com/gtgqzuiheg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtbnpiumzo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtxubdqqbo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shuidangran.top/gtzvqeoope.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtkhuxaybn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yongpay.top/gtjsjpgrbq.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtmijrapgd.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtgjabcsjp.html

TS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gthavnpyxq.html

Java: String.join(", ", list)
来源：http://hz.zhengqikj.top/gttasfpibo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sufxvd.cn/gtlmfgqihp.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtkcltjsib.html

C#:   string.Join(", ", list)
来源：http://hz.yj202588.top/gttaxeqahn.html

================================================================================
来源：http://hz.gogol.net.cn/gtghmelnss.html

E. 字符串处理
来源：http://hz.chenjidiqi.icu/gtnqwzqugh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtnyfjobuj.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtqwwsqigw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cqqwz.cn/gterplqvoe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtrqjpuosa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtthsciwcb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtasqevdpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tanke756.top/gtuiefwaql.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangdashe.top/gtwsqczamg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yongpay.top/gtsiqohhep.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtecplgptw.html

[E02] 重复字符串
来源：http://hz.shuidangran.top/gthkbuxiug.html

Py:   "ab" * 3
来源：http://hz.cdnleiting.top/gtbxcnfuyi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgufenzy.top/gtpcoebxur.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtopdpivgw.html

TS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gteurxkxrk.html

Java: "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtgjossdky.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gogol.net.cn/gthaxdzwuk.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gtqvademwa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtxwjzjngs.html

[E03] 截取子串
来源：http://hz.havefunace.top/gtjwmldwdd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtpmothopp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ybcxt.top/gttviszhzy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtjjsyoleh.html

TS:   s.slice(1, 4)
来源：http://hz.sysykeji.top/gtzbflcujm.html

Java: s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtbhrngqjo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cashguo.top/gtxzcdcbuo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtafnofewg.html

C#:   s.Substring(1, 3)
来源：http://hz.yvedp.cn/gtbunylgdm.html

[E04] 查找子串位置
来源：http://hz.cheryme.top/gtrganqjoq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtfskuzvtb.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gtcxvmetqk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinyuanbaomall.cn/gtzxahbrod.html

TS:   s.indexOf("x")
来源：http://hz.wangdashe.top/gtwnvbwmxa.html

Java: s.indexOf("x")
来源：http://hz.xuanzx.com/gtospedyoq.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtdyzuresf.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtpqendtmi.html

C#:   s.IndexOf("x")
来源：http://hz.yueranfly.top/gtpibrexkr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtmscqhjbl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtvawbjbal.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258.top/gtcwzafsal.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtyxjhcghw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gtgydjrrqa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtcqjzqwme.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtcmsoaoeb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtrpgnvekf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yanxiufei.cn/gteoxfrihn.html

[E06] 替换子串
来源：http://hz.ehwqpu.com/gtwodpoxvh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.vqdsnc.cn/gtdksntdih.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nwbrower.top/gtibysshdm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtffdlnhec.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtigxrcvhd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtphigjqdu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gtcteipudt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinghuilouyu.cn/gtcahpvmwv.html

C#:   s.Replace("a", "b")
来源：http://hz.yueranfly.top/gtrfbuhpvo.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtkhyrntrc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxinkj.top/gthrnnsemm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pengpengdd.cyou/gtrakdhzcf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hfpthk.cn/gtrcrwaiof.html

TS:   s.split(",")
来源：http://hz.feifeiyinyue.top/gtdxfylusg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gttrrdwjrd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtlipvqviw.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtffdxrpif.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj202588.top/gtmuigyzsi.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gthhndpzxk.html

Py:   ",".join(items)
来源：http://hz.yonumen.top/gthmiajcwp.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtaifowube.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gtcoondnrc.html

TS:   items.join(",")
来源：http://hz.yueranfly.top/gtredlbvnz.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtrrvyavnc.html

Go:   strings.Join(items, ",")
来源：http://hz.feifeiyinyue.top/gtkjlclsgq.html

Ruby: items.join(",")
来源：http://hz.yvedp.cn/gtioghippt.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtylaknnkt.html

[E09] 去除所有空白字符
来源：http://hz.yongpay.top/gtyiytjkyc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtvljrblwh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sysykeji.top/gtgwfwgnic.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtpmoppjom.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtmzzjadcx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gtvdfghabk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangtech.top/gthgrlptpp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtzxbncqll.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daria6918.cn/gtixtjicsv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtpjkidbgv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.svipenyu.cn/gtigijlldj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtrqcsfvar.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtwelgkkqo.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtmhxetsem.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtcxfqlwfi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtbnyewzao.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtccdawvbp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtocpcaykm.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtdqeiocwu.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtfqpzbmwb.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtnudkdsbs.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gthjpnodds.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtxayhtnoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.haohaochexian.top/gtmamejgta.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cheryme.top/gtqwurdycf.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtyzrpqbkg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtoxuqxzhd.html

[E12] 统计某字符出现次数
来源：http://hz.ehwqpu.com/gtutxxxgzn.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtyduvmqnw.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gttudnvcjz.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtlpbqwfbe.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtzkgpbens.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.guannengcc.top/gteyqkgwnr.html

Go:   strings.Count(s, "a")
来源：http://hz.9152youxi.cn/gtqbpskljr.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtrguauncp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtrltlpeuk.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtkcmypjqg.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgufenzy.top/gtktpftioh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gthrsfsdra.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtxsepfagy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtabuppgbe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuetiantiany.cn/gthuzhxocf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtyvubnbrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtjayxmmxr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtuvaagpyo.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtgjfdeaio.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gaohongyu789.top/gtdypguljg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gotoacloud.top/gtdqowgxus.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtcsmoocom.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.c1oappe.top/gtbgzywzrt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jlsjyb.cn/gtanotpxid.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtpxmvguwi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtdotcqruo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cdnleiting.top/gtxguxwpet.html

[E15] HTML 转义 / 反转义
来源：http://hz.guannengcc.top/gtsrbdcptt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hfpthk.cn/gtjvigclhz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sufxvd.cn/gtotqozqsf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtahuqsczf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ywan-chungtsiang.top/gtvcotvzot.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuetiantiany.cn/gtbzpkuizm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtcagrprop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gteonknmpl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxuanxn.top/gtzckzdrxf.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gttuhnrbsr.html

Py:   f"{1234567:,}"
来源：http://hz.zdqjudy.top/gthiyyarjb.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gtepfmtobr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtvlofwtbc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtzapqgukr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhoulong.xyz/gtummyhnka.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtnakbhtkx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtmnrtuyoi.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gtrxkzcoop.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gtoixquwcw.html


<!-- 参考信息 -->