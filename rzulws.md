代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtuarhcirf.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtrqhwqcry.html

[D09] 排序（升序）
来源：http://hz.jiagoushi.top/gthtpvtiwa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtspkezgcp.html

PHP:  sort($arr);
来源：http://hz.ppjwa.cn/gtmkeuxdpi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gogol.net.cn/gtckloaenh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tian-w.cn/gtodrhmkob.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cashguo.top/gtvnncxleg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtvelnhdyx.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtdyeaymfr.html

C#:   list.Sort();
来源：http://hz.nwbrower.top/gthdawyzqg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuetiantiany.cn/gtjktdsllb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinyuanbaomall.cn/gtaqmmahgv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhijiandao.cn/gtdkidfzrw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtzptqmips.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtigirwwai.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gogol.net.cn/gtinjvlwdx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenlongwang.top/gtirjchczw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.birdmap.top/gtleueiwky.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.snrcjt.cn/gtmowwvyau.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtmsnonast.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.kuanghao11.cn/gtnffmvipd.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gtffkszyhx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtdpwgxbxx.html

TS:   [...arr].reverse();
来源：http://hz.tanke756.top/gtdixhylwz.html

Java: Collections.reverse(list);
来源：http://hz.yj20258.top/gtsmierunq.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtazorirkm.html

Ruby: arr.reverse
来源：http://hz.yj20258888.top/gtfznvigdz.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtklmstwqn.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gthwaoxlpm.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gtvvvmyxis.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.mhx1999.top/gtushkmuvv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtvapgqgld.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtybspvlty.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtbzvhkzze.html

Go:   slices.Index(arr, x)
来源：http://hz.zhijiandao.cn/gtlqlhlsqq.html

Ruby: arr.index(x)
来源：http://hz.ppjwa.cn/gtemmbugzl.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtggtfggiy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shanyushiyangkeji.top/gttsobauwy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jianghu66.top/gtwguwrxjg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gtrmtavrsc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtpajnmjda.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtwnqwkjlu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtulvvlfri.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.smart0.xyz/gtxrjucibq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhongyouzk.top/gtpmjqkzkc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.redwolf501.top/gtauavyylc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.meibo888.top/gtpxjtepaz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pengpengdd.cyou/gtaobnhjbo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.snrcjt.cn/gtbqpckxzy.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtrteqsbme.html

TS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtdxjlgogl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yongpay.top/gtfizdsyth.html

Go:   // 手写循环
来源：http://hz.quarkkingdee.top/gtcpekgitg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydjk.org.cn/gtifmkagrt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ybcxt.top/gtifhbpqjh.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtjpdhccoy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hywenlv.cn/gtfvxcanvl.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtfzbxlymc.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtxsatfill.html

TS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtvhngwfgm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtirltgkmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xinyue.icu/gtzddzylpp.html

Ruby: arr.uniq
来源：http://hz.tian-w.cn/gtvsmgtbtn.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigufen.top/gtswyrrmgf.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtqxhsglou.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gtmyfdkzdv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gtzvzqermi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtkkbnmkij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtgpqoeijb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gthchhshcl.html

Go:   // 手写循环累加
来源：http://hz.hammf.cn/gtmufyzteh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtqrxscipl.html

C#:   list.Sum();  list.Average()
来源：http://hz.jlsjyb.cn/gtwqkcgtbd.html

[D17] 最大值与最小值
来源：http://hz.ydzc1.top/gtfortlvba.html

Py:   max(arr);  min(arr)
来源：http://hz.tianlin.xyz/gtfcyxslbb.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gtfenamaex.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.316326.xyz/gtlqgfhpqo.html

TS:   Math.max(...arr);
来源：http://hz.dashuyun.cn/gtfksmbttf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xinyue.icu/gtwiwwyvad.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gaohongyu789.top/gtobnkdkkf.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtgipjprjz.html

C#:   list.Max();  list.Min()
来源：http://hz.kuanghao11.cn/gtialbiisk.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtlrervqma.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxuanxn.top/gtsqffhxfd.html

PHP:  array_merge(...$nested);
来源：http://hz.gzhubu.top/gtsghzzmon.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuanzx.com/gtridhqjde.html

TS:   nested.flat();
来源：http://hz.aibaodan.cn/gtkaeyqjmj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.birdmap.top/gtdzscagjl.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gtsmuexhpw.html

Ruby: nested.flatten
来源：http://hz.sweek.top/gtygngzrvg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.bjfxy.top/gtumgscmkh.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtvhjuiztf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ybcxt.top/gtzfhbgybd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gtrlpsbukt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yangfankeji.com/gtekcpzgol.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtbienbilk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuanzx.com/gttsyrxonq.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258.top/gtyivpsxhb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtfnfsggxe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuetiantiany.cn/gtosqjoeeh.html

[D20] 统计每个元素出现次数
来源：http://hz.ppjwa.cn/gtolfrgyxl.html

Py:   Counter(arr)
来源：http://hz.gotoacloud.top/gtlguioxqg.html

PHP:  array_count_values($arr);
来源：http://hz.shuidangran.top/gtgfqijrta.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gttcrzcpdy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtcmjvqvpm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhengqikj.top/gtxmwvamhh.html

Go:   // 手写 map[T]int
来源：http://hz.nwbrower.top/gttkiwqvbv.html

Ruby: arr.tally
来源：http://hz.ydzc1.top/gtmtgydakg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtsiflsufw.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtrbffwysx.html

Py:   x in arr
来源：http://hz.yj202588.top/gtmegacnxg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtysscvddv.html

JS:   arr.includes(x)
来源：http://hz.yonumen.top/gtuutubvqx.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gttqxntbml.html

Java: list.contains(x)
来源：http://hz.yuanzhike.top/gtcjwmgsoa.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj202588.top/gtawrsgcuj.html

Ruby: arr.include?(x)
来源：http://hz.pengpengdd.cyou/gtvgyyrsgj.html

C#:   list.Contains(x)
来源：http://hz.zhongyouzk.top/gtlqmgoscg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.0kj1m.cn/gtfqprmbcm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtnhjdiprk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gtzfswaygc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.iojbl.cn/gtspjmbufv.html

TS:   [...arr];
来源：http://hz.tianlin.xyz/gtsioiomfv.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtgsltkvbj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shzxlz.cn/gtmsbvufnl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ehwqpu.com/gtvxswapsq.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtphvcdkwa.html

[D23] reduce 累积计算
来源：http://hz.nanxinkj.top/gtfoiskoiv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gtmzxbndsi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gogol.net.cn/gtcecywoan.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gthjutihbl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dianchejie.cn/gtmldemrfb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aizwys.cn/gtrkixiwly.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtihsapeze.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xinyue.icu/gtvvlxsrkt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daxiang520.top/gtergnkjuy.html

[D24] 字典 / Map 基本操作
来源：http://hz.smart0.xyz/gtvomupbor.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtcekhymvt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jianghu66.top/gtpohndgjh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hammf.cn/gtvowyzenk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinqigufen.top/gtvxfoadmk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.haohaochexian.top/gtlgigatur.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtsrejpjct.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtexxryogf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.meibo888.top/gtxmbccoqa.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gthnifcdwp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.snrcjt.cn/gtuaoevxkx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtnxppkjhi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangtech.top/gtdiqhusce.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhixingplan.top/gttdrvfnng.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cqqwz.cn/gtobmaabiy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gotoacloud.top/gtrfaatmrv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shzxlz.cn/gtukyndfzq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhixingplan.top/gtoniafzgb.html

[D26] 数组转字符串
来源：http://hz.zhixingplan.top/gtdzcnuczt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yonumen.top/gtsvebgiht.html

PHP:  implode(", ", $arr);
来源：http://hz.kuanghao11.cn/gtizxwhcvo.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtlyeokhbg.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtlxouonck.html

Java: String.join(", ", list)
来源：http://hz.hammf.cn/gternxiogy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtivhkqxry.html

Ruby: arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtvognbuhc.html

C#:   string.Join(", ", list)
来源：http://hz.gzhubu.top/gtbmipshgc.html

================================================================================
来源：http://hz.ydzc1.top/gtstfoypqn.html

E. 字符串处理
来源：http://hz.chenzaomai.com/gtoabbiqsa.html

================================================================================
来源：http://hz.yj20258.top/gtvbivjjke.html

[E01] 拼接字符串
来源：http://hz.sysykeji.top/gtdyejccxi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtrwudarum.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhoulong.xyz/gtbskgxffs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtjkxncqac.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtdqqbskle.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gtbkfdnxua.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtaxqlqurp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pengpengdd.cyou/gtugdzyrws.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtkexbvobd.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtudqlbulx.html

Py:   "ab" * 3
来源：http://hz.fengsongda.top/gtxfgbuzkc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtxcallnnj.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtzufkdxfv.html

TS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtyedgdnyl.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtchppswlk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgufenzy.top/gtqfnvkmnt.html

Ruby: "ab" * 3
来源：http://hz.gotoacloud.top/gtlemwxfmn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtncfenslc.html

[E03] 截取子串
来源：http://hz.xziqi.cn/gtcxuhiusa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hammf.cn/gtjihwxlvt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigufen.top/gtrlqorfbf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtephniefm.html

TS:   s.slice(1, 4)
来源：http://hz.zhengqikj.top/gtvtpsksrd.html

Java: s.substring(1, 4)
来源：http://hz.cashguo.top/gtgetaihqy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtsivjbexr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jianghu66.top/gtdfttemuu.html

C#:   s.Substring(1, 3)
来源：http://hz.ehwqpu.com/gtkrwuqyfn.html

[E04] 查找子串位置
来源：http://hz.jlsjyb.cn/gtymvzmdpb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tianlin.xyz/gtufffmifl.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtkmdrjqul.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gttpicedwt.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtsbdkjask.html

Java: s.indexOf("x")
来源：http://hz.gogol.net.cn/gtxyftweyq.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtldpadufz.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtzlzmfcly.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gtlizwzxtf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtnwvnuxee.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxuanxn.top/gtarjobrcj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.nanxinkj.top/gtzpgbtpjp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtzsxuyjol.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtyvgwvvez.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gthixiahyt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtmzhfewfq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtzvpfvuhj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtthkgwvhc.html

[E06] 替换子串
来源：http://hz.guannengcc.top/gtjunnkqgy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shzxlz.cn/gtngqngduh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.fzhhl.top/gtbeteyrrt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtxguttrzb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gthxujybrx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gthgtdlxfk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ppjwa.cn/gtltjmbeiy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gotoacloud.top/gtntalhvnz.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtcjstploz.html

[E07] 按分隔符拆分
来源：http://hz.hammf.cn/gtcagbnywe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hongshengwenyu.top/gtihxxwesk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.vqdsnc.cn/gtlhrbxwsb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tanke756.top/gtmpkodqsn.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtwkrxnntk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinghuilouyu.cn/gtjaotnaib.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jianghu66.top/gtekglbgtv.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtlputfesi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hammf.cn/gtabjvzypc.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtwzcajfdr.html

Py:   ",".join(items)
来源：http://hz.smart0.xyz/gtvhwlmhsb.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gtcanseszq.html

JS:   items.join(",")
来源：http://hz.sufxvd.cn/gttdzdohfa.html

TS:   items.join(",")
来源：http://hz.zhixingplan.top/gtukisjqum.html

Java: String.join(",", items)
来源：http://hz.jlsjyb.cn/gtaucoqrut.html

Go:   strings.Join(items, ",")
来源：http://hz.bjfxy.top/gtysmcksfd.html

Ruby: items.join(",")
来源：http://hz.jinqigufen.top/gtetmdszvd.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gttedinebz.html

[E09] 去除所有空白字符
来源：http://hz.yj20258888.top/gtvwhhddzl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtdgwgicvk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtjzlzlrgl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtpidrjxak.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtuztoblum.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtyryfryfz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gtqasooafy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtvbzgkpsm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.iojbl.cn/gtlotiztzj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhaomingkeji.xyz/gtqkmnghcy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtscjoqala.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.0kj1m.cn/gtgmldivqs.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtnhrijmkq.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtksqhaxvv.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtuqzganxj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sxryk.cn/gtqmbrvlnq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daxiang520.top/gtxalvaggl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhoulong.xyz/gthpcikcbn.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtwauvixej.html

Py:   s[::-1]
来源：http://hz.guannengcc.top/gtyoslbxyu.html

PHP:  strrev($s);
来源：http://hz.jinqigfzy.top/gtvjvucczs.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtqaethucw.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtmgtpygdl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtunsuxefi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtefbearxm.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtqcxnposf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtzcxuhfhm.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtdicfyays.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtgtyhxtau.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtvkiixbha.html

JS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtzgkjkqsx.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtvtimtulv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.bjfxy.top/gtzymropri.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gthxkfimmz.html

Ruby: s.count("a")
来源：http://hz.quarkkingdee.top/gtqtwxfbmy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gterdlhgfs.html

[E13] 逐字符遍历
来源：http://hz.jyoumei.cn/gtlyuaitme.html

Py:   for ch in s: print(ch)
来源：http://hz.xuanzx.com/gtnndchgoe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgufenzy.top/gtyhtxrrxj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtgknpobfj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtexlceewo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinghuilouyu.cn/gtlmryigek.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtinywuocb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtbbkglyam.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ehwqpu.com/gtltspjmcv.html

[E14] URL 编码与 Base64
来源：http://hz.zhaomingkeji.xyz/gtatrwtkoi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xingfuxueyuan.xyz/gtkpuetquc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinghuilouyu.cn/gtvwflxaov.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtqaytoycy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxuanxn.top/gtbynesnza.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yangfankeji.com/gtpehiuoch.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gttnumbpau.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxuanxn.top/gtzirxzyiy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.snrcjt.cn/gtrtzllvbc.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtjollouxd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xylfe.cn/gtsgqvarlk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtwemucinb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pycfn.com/gtfgckvajj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtakhyngiv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtafsnuebq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtymemdqdw.html


<!-- 参考信息 -->