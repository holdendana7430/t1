代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gttcfntkwy.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtkxpgwcgn.html

C#:   list.Sort();
来源：http://hz.shanyushiyangkeji.top/gtuhxheinu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sweek.top/gtiietvkqc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigfzy.top/gtzfvbgung.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gttcfjawln.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtswvibmek.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gttmzolcby.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jiagoushi.top/gtuopuxicr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shzxlz.cn/gtclexesrr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtfpvmulkl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.9152youxi.cn/gtxaezwmho.html

[D11] 反转数组
来源：http://hz.jinqigfzy.top/gtjsgrijnt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ywan-chungtsiang.top/gtgjdymgka.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gttatsruqa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinghuilouyu.cn/gtvrjlnlhs.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtroyfwweg.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gtgrxcyjdc.html

Go:   slices.Reverse(arr)
来源：http://hz.kuanghao11.cn/gtvxcjrnua.html

Ruby: arr.reverse
来源：http://hz.bjfxy.top/gtepzpknxy.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gthibakkon.html

[D12] 查找元素下标
来源：http://hz.52xcode.cn/gtjzptgbir.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenlongwang.top/gtzlvhdllb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.meibo888.top/gttbernzwy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gtkzznthiw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtegapnqux.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.feifeiyinyue.top/gtuqjpmxba.html

Go:   slices.Index(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtbimfkbvk.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtmjhijgxw.html

C#:   list.IndexOf(x);
来源：http://hz.jyoumei.cn/gtxmhnzlrl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yonumen.top/gtzkeigxku.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.52xcode.cn/gtdlnaphmm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dianchejie.cn/gtbiuzertt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtvgroliiy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtkdgobfxm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtpcnlxvfb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hammf.cn/gtnrddttnz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj20258.top/gtzmasaaqg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnxiangtu.top/gtghpqaluq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zycfv.cn/gtlnaqrhhe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sxryk.cn/gtsvmzclcq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gtmmpajsxy.html

JS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtqekxupxn.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtsvickaxh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtmyjixemj.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtipvdhfzj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtaiuolhet.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtadkreion.html

[D15] 去重
来源：http://hz.snrcjt.cn/gthzcqaabd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtzxmquqvz.html

PHP:  array_unique($arr);
来源：http://hz.jianghu66.top/gtdchxyoxm.html

JS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gttmlyrodb.html

TS:   [...new Set(arr)]
来源：http://hz.fengsongda.top/gtwlvmumbk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yvedp.cn/gtnravcrrq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtpzfolxek.html

Ruby: arr.uniq
来源：http://hz.jinyuanbaomall.cn/gtftdjeikp.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtbrunwmrj.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtzmufiuuw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtweycjvdz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtrwccavqi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtlchenxnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gttpbigvxq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtpxrlibmd.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gttejoddfy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenjidiqi.icu/gtyuanhuvz.html

C#:   list.Sum();  list.Average()
来源：http://hz.tianlin.xyz/gthkvbchux.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtfuflgvea.html

Py:   max(arr);  min(arr)
来源：http://hz.hnqzz.top/gtozwthuzg.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtpekmvkhr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hammf.cn/gtrczmflbd.html

TS:   Math.max(...arr);
来源：http://hz.tanke756.top/gtylwjhurl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinghuilouyu.cn/gtiwimdhmo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gthmsklofe.html

Ruby: arr.max;  arr.min
来源：http://hz.fzhhl.top/gtwlqcxwjr.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gthrfxbvwn.html

[D18] 扁平化嵌套数组
来源：http://hz.hnqzz.top/gtyzxiyiol.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gtwozdirxc.html

PHP:  array_merge(...$nested);
来源：http://hz.sweek.top/gtoyzebrnw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jiagoushi.top/gtsxyhwubx.html

TS:   nested.flat();
来源：http://hz.daxiang520.top/gtyuufvtpy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtddklkwst.html

Go:   // 手写双层循环
来源：http://hz.zhoulong.xyz/gtvlarcszs.html

Ruby: nested.flatten
来源：http://hz.fengsongda.top/gtqaqdtrtj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtbjtkzwhj.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtwtqyxnsp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtipbeqwrn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cucudq.cn/gtcykfikyq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtufsnmphz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtjshgzdah.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangkeji.top/gtlpnhvuqk.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtrrbioolw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gtzxsrrfao.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gttqpalenm.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtiofmiecs.html

Py:   Counter(arr)
来源：http://hz.xziqi.cn/gtgczpjmcw.html

PHP:  array_count_values($arr);
来源：http://hz.ydjk.org.cn/gtuwgkzbdu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtbwfnkimz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtjcgpdtkf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydjk.org.cn/gtxhldwrcc.html

Go:   // 手写 map[T]int
来源：http://hz.sysykeji.top/gtrsrplnvo.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gtpohgypsf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtlcasdaqo.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gtjioctbfl.html

Py:   x in arr
来源：http://hz.cheryme.top/gtthqmciiz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gogol.net.cn/gthyindanl.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtouloqdpr.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtaxgdijvh.html

Java: list.contains(x)
来源：http://hz.gotoacloud.top/gtxmktaxuw.html

Go:   slices.Contains(arr, x)
来源：http://hz.shzxlz.cn/gtddzrpzch.html

Ruby: arr.include?(x)
来源：http://hz.hysaishi.cn/gtjtiboflt.html

C#:   list.Contains(x)
来源：http://hz.dashuyun.cn/gtltosavxq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtjukznnew.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtdwdedoth.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xziqi.cn/gtiqkbasrz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dianchejie.cn/gtcxeuesgt.html

TS:   [...arr];
来源：http://hz.jinqigfzy.top/gtekwpthvn.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtgsbxffhg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtzmscrrwr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgufenzy.top/gtqjtsocas.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtdyagjcma.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtsmctytah.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hywenlv.cn/gtwpjayhzl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aibaodan.cn/gtgruegpog.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtxlhrayqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtkkywndjm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.havefunace.top/gtvvahrxwu.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtxlalnpyg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtdybfsbme.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtbxttlomv.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gtuczddqdu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cdnleiting.top/gtvmnsiygs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtqxkfwcrz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtyxyosqds.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenjidiqi.icu/gtimqrepbm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hywenlv.cn/gtmiqoexuu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtkahcvsnb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yueranfly.top/gtpdmwmxnr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.9152youxi.cn/gtnmnrhluw.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtwiyuljrd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.fzhhl.top/gtywpynryl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtnbwwfqdp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtzbpiqowl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtxevfxjnj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtagcuszxs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtngmpbtne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuanzhike.top/gtbeqxgoff.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtsltjjkvd.html

[D26] 数组转字符串
来源：http://hz.meibo888.top/gtqccoemqq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtqpqdaqhe.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtmpxmsauv.html

JS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtowmanufd.html

TS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtbhnyayuk.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gtvsmayoxg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtrpapcxkb.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gthzjgojjp.html

C#:   string.Join(", ", list)
来源：http://hz.guannengcc.top/gtuiahsfau.html

================================================================================
来源：http://hz.jyoumei.cn/gtbteanowc.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gtbdvuupkx.html

================================================================================
来源：http://hz.yj20258888.top/gtffjhpfch.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtshhptizz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtfvgfmbad.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.smart0.xyz/gtsxjqoygi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtritbyllz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtkixlylll.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtmkwcbsdb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daria6918.cn/gtjzufmwpe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gtxtrmfwvf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtmvoxtyrx.html

[E02] 重复字符串
来源：http://hz.hysaishi.cn/gtggebzaak.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtiatqwnpj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.havefunace.top/gtebihmotf.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtvdinensg.html

TS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtslekjanc.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtbsdgmzxp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shangyingyoupin.top/gttkgjfyrf.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtjuwxqfee.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ehwqpu.com/gtarpeysld.html

[E03] 截取子串
来源：http://hz.cheryme.top/gtezaajlfw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.316326.xyz/gtraekhkfd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cashguo.top/gtytmryzmb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtntoxande.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtcpfiyhoh.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gthfqpqfph.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtwaedbilf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtvxgxpjxj.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtlgpwsngo.html

[E04] 查找子串位置
来源：http://hz.fengsongda.top/gtjzqcslrf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yonumen.top/gtfgamdzmh.html

PHP:  strpos($s, "x");
来源：http://hz.jinghuilouyu.cn/gtzjbmsfty.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtdaabwqtj.html

TS:   s.indexOf("x")
来源：http://hz.chenzaomai.com/gtiulctgoo.html

Java: s.indexOf("x")
来源：http://hz.yueranfly.top/gtwikyetbj.html

Go:   strings.Index(s, "x")
来源：http://hz.xuanzx.com/gtuffslcxg.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtzknxnaqg.html

C#:   s.IndexOf("x")
来源：http://hz.cqqwz.cn/gtlmiullbn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gzhubu.top/gtlrjxkizp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.redwolf501.top/gtyfjodzpy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtqrgsidfg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gthniyalum.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtroayfbtw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtnfbottob.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.feifeiyinyue.top/gthxzjdsss.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtupqvbrir.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtxqppjvok.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtoysnqduj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.316326.xyz/gtgygavhzi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtrkawyldd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtelnlkkjg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtenhezjuz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gttycgbzfk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtnzyyxyrc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.redwolf501.top/gtfrddvzir.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtnzdnztxi.html

[E07] 按分隔符拆分
来源：http://hz.jinghuilouyu.cn/gtgaozcmmc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.redwolf501.top/gthwqhrfre.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258888.top/gtujtmjckd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtvtihoivo.html

TS:   s.split(",")
来源：http://hz.ehwqpu.com/gtxynsfgmi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtihzchnon.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hnqzz.top/gtcllcgjew.html

Ruby: s.split(",");  s.split
来源：http://hz.gzhubu.top/gtuaetkjqr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhijiandao.cn/gttyrpzpwe.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gteurhcoon.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtlbfbflle.html

PHP:  implode(",", $items);
来源：http://hz.gotoacloud.top/gtuvikphgj.html

JS:   items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtlqztyell.html

TS:   items.join(",")
来源：http://hz.yueranfly.top/gttmbpurgu.html

Java: String.join(",", items)
来源：http://hz.hfpthk.cn/gtzywnqsbz.html

Go:   strings.Join(items, ",")
来源：http://hz.c1oappe.top/gtnuhuabhm.html

Ruby: items.join(",")
来源：http://hz.gzhubu.top/gtawvrbgqr.html

C#:   string.Join(",", items)
来源：http://hz.yongpay.top/gtshzfwyvl.html

[E09] 去除所有空白字符
来源：http://hz.sweek.top/gtvjfxveef.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xylfe.cn/gtwgpgowzm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtugbqgtwh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtumbghmxe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtqveevztv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtautruopp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangdashe.top/gtfuklbwha.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fzhhl.top/gtfgkkuqzz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gthualdcor.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cdnleiting.top/gtrsbcighm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtbzndntmc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtdztoaxjx.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtcjampxvj.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gthgrtgqnz.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gteanezynq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cucudq.cn/gtducejbtj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gtopqmhzzw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtyljbgdeu.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gtummunxlz.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtricoxcxq.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gthtsbzvhe.html

JS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtylflbqhg.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtdazgohhs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gtlpvnbzaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtpzzcwjqy.html

Ruby: s.reverse
来源：http://hz.chenlongwang.top/gtdbtmcxar.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtvgjxisif.html

[E12] 统计某字符出现次数
来源：http://hz.sysykeji.top/gtmrgnupcq.html

Py:   s.count("a")
来源：http://hz.jyoumei.cn/gtyzkvtkye.html

PHP:  substr_count($s, "a");
来源：http://hz.gogol.net.cn/gtneflwukd.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtptogefrs.html

TS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtugtbusgg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuanzhike.top/gtypnyqdsm.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtvzlojgrr.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtvxkpleas.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yanxiufei.cn/gtivclxvhs.html

[E13] 逐字符遍历
来源：http://hz.yanxiufei.cn/gtfkehflnc.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtwtzcfdpi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yanxiufei.cn/gtwiwqxnsv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtbzdgjfrj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtimwzlvhv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jianghu66.top/gtxnxpkicr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtgrrxtwoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guannengcc.top/gtaslqtkyk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtbmozoksp.html

[E14] URL 编码与 Base64
来源：http://hz.andypj.xyz/gtzoifhucy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xingfuxueyuan.xyz/gtltbyjrzx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gtcvxlxkoc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gzhubu.top/gtwdphdeju.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aibaodan.cn/gteoienloh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtjusptfmm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydjk.org.cn/gtlwwzfwbu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtiziyfayk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guowangkeji.top/gtangdwfro.html

[E15] HTML 转义 / 反转义
来源：http://hz.fengsongda.top/gtsrvfhnus.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenzaomai.com/gtjsjfnkhe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtcwddstqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jlsjyb.cn/gtmnwqrqse.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aibaodan.cn/gtijrytghq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtuoyfmcgn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.havefunace.top/gtistqedfo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangkeji.top/gtxenvmlaa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangshuangyany.cn/gtogpmjdtx.html

[E16] 数字千分位
来源：http://hz.ehwqpu.com/gtdvzfzbqv.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtqznvafsg.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtdpxlqjzo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtishnkpny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtocnhewko.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sufxvd.cn/gtfkplzlrk.html


<!-- 参考信息 -->