代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtorohwinp.html

Java: list.subList(1, 4);
来源：http://hz.tian-w.cn/gtosgepeav.html

Go:   arr[1:4]
来源：http://hz.xylfe.cn/gtdnndxkoa.html

Ruby: arr[1, 3]
来源：http://hz.vqdsnc.cn/gthbsnyept.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtrsvtiajf.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gtiyvhnnbb.html

Py:   a + b;  a.extend(b)
来源：http://hz.tian-w.cn/gtbpnjrkhc.html

PHP:  array_merge($a, $b);
来源：http://hz.mhx1999.top/gtsaunyree.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtqfpcjnyf.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gtmyujbyjx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.iojbl.cn/gtcgbpnlsd.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtbjaqhjuq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtzyabxnrz.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtzjvnxhfw.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtofcjikud.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtlhyayumn.html

PHP:  sort($arr);
来源：http://hz.feifeiyinyue.top/gtfmgaveyf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.havefunace.top/gtxoshugpu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gterohtxio.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtkwiqgnle.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtmgcpndvt.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtnjdufcpc.html

C#:   list.Sort();
来源：http://hz.ehwqpu.com/gtrnyhxjfv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtpjlpmoma.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zycfv.cn/gtsjgdtnev.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtvhcjvzom.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtgcoymjpv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydjk.org.cn/gthokaqilk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtdptbkegg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtikutxvab.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zdqjudy.top/gtzshlyqqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtxorewpuo.html

[D11] 反转数组
来源：http://hz.tianlin.xyz/gtgikshtyf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xuetiantiany.cn/gtcoxlmnut.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtolysjdbp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtgrvsbuhx.html

TS:   [...arr].reverse();
来源：http://hz.fzhhl.top/gtslnbdckp.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gttnhidjoi.html

Go:   slices.Reverse(arr)
来源：http://hz.yuxming.cn/gtdeeeivtr.html

Ruby: arr.reverse
来源：http://hz.meibo888.top/gtatmyxfvm.html

C#:   list.Reverse();
来源：http://hz.yueranfly.top/gtcfvkuqjl.html

[D12] 查找元素下标
来源：http://hz.pengpengdd.cyou/gtfgdeppqo.html

Py:   arr.index(x);  x in arr
来源：http://hz.52xcode.cn/gtcawnrprp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhijiandao.cn/gtwaajmlyg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtblltxggw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gtsypxsmok.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sufxvd.cn/gtwhyzfghy.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gtyensidfo.html

Ruby: arr.index(x)
来源：http://hz.fengsongda.top/gtqzhyfcbx.html

C#:   list.IndexOf(x);
来源：http://hz.bjfxy.top/gtzbbkiexe.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtswdkysjg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtanukzwbu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtyqfocmgv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtdgyclwot.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtaxowqrfn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtzqzthsku.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtxyrgphye.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tian-w.cn/gtohcvqdyp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtjpanjdgo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtjpesscxw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.52xcode.cn/gtpjvbytjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.iojbl.cn/gtqzjtslns.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtkvvslvao.html

TS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtpfihykvv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtydywjxeb.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtfqvmjriw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtwocokljh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtcbzvhlei.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtarcfkbel.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtyoebnxkm.html

PHP:  array_unique($arr);
来源：http://hz.yj202588.top/gtybuwojxf.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gteoyufhtp.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gthqedfetd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gotoacloud.top/gtvfsisktk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xingfuxueyuan.xyz/gtbzmhoqyx.html

Ruby: arr.uniq
来源：http://hz.ywan-chungtsiang.top/gtegrkjkrn.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gtzkfpdjog.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtbjwjkwhg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258.top/gtwyqzukfu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangkeji.top/gtwdkzzebj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtylqjtome.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtgmzgdelv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.snrcjt.cn/gtrgadacoe.html

Go:   // 手写循环累加
来源：http://hz.shangyingyoupin.top/gtecdetyjr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtrqnuqabx.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gteaeoqfde.html

[D17] 最大值与最小值
来源：http://hz.c1oappe.top/gttfsqdrur.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtnrdbetza.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtcywqyyoh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtnwvjnhqy.html

TS:   Math.max(...arr);
来源：http://hz.vqdsnc.cn/gtditagcix.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtnbstlivx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gtiakgkdpk.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtyoeahmki.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtixsneora.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtnxdhfuab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.iojbl.cn/gtujxkcdxv.html

PHP:  array_merge(...$nested);
来源：http://hz.gotoacloud.top/gtsztmgqqf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gtypvzmavc.html

TS:   nested.flat();
来源：http://hz.jinqigufen.top/gtaaakcqkv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.c1oappe.top/gtrbtjoqks.html

Go:   // 手写双层循环
来源：http://hz.jqgufenzy.top/gtgkyubxoo.html

Ruby: nested.flatten
来源：http://hz.smart0.xyz/gtkjmznbtt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtpjwsxppl.html

[D19] 按字段分组
来源：http://hz.xuetiantiany.cn/gtaobclqwh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pengpengdd.cyou/gtrvmuwofy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinqigufen.top/gtbxdbbolf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ppjwa.cn/gtsqkphvlh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gthkjcdzhx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.feifeiyinyue.top/gtyvujxpke.html

Go:   // 手写 map[string][]T
来源：http://hz.gotoacloud.top/gtacybvvyt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zdqjudy.top/gtvvhlzcfr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.vqdsnc.cn/gtfdahjofi.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtejafdtzb.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtybnannqo.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtvaqscjgj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtscdjqazf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtnwcplrwj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtqdkpeepv.html

Go:   // 手写 map[T]int
来源：http://hz.ywan-chungtsiang.top/gtscctgjiq.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gtlufodyok.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shuidangran.top/gtedivzzvr.html

[D21] 判断是否包含某元素
来源：http://hz.nanxuanxn.top/gtwoflmmoh.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtcgmrmeas.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yanxiufei.cn/gtquscxykm.html

JS:   arr.includes(x)
来源：http://hz.xziqi.cn/gthqvkgkjr.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gttoezuqns.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gtvonppgrk.html

Go:   slices.Contains(arr, x)
来源：http://hz.yanxiufei.cn/gtqqdqwjti.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gttcjmntsy.html

C#:   list.Contains(x)
来源：http://hz.ehwqpu.com/gtuttuurag.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jlsjyb.cn/gtkjrpydaw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hammf.cn/gthwiahyno.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtkrfppzwu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cdnleiting.top/gtwihqhywh.html

TS:   [...arr];
来源：http://hz.hongshengwenyu.top/gtxigwpesj.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtgonwsuap.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xingfuxueyuan.xyz/gtytmgvtbg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aizwys.cn/gtopxtgwah.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtpwhqkhbk.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtujreepkw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtonohcjsw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258.top/gtuwenzhdi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtlefoigvd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtvwgxljtj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gtbrkppphp.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtglcbggsf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtqmcylkqx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yonumen.top/gttcauqina.html

[D24] 字典 / Map 基本操作
来源：http://hz.sxryk.cn/gtjqkkjpsm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtraihdusi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtrmdcavzv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gtnmloeyxc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgfzy.top/gtvkwfxucl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.mhx1999.top/gtmzfiabta.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.0kj1m.cn/gtxxwiwitc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daxiang520.top/gtyqrskcgr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shuidangran.top/gtfdcgyglp.html

[D25] Set 集合去重与交并差
来源：http://hz.feifeiyinyue.top/gtsltposdr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.vqdsnc.cn/gtxlvpyxph.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtrvovgoin.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtwkibessn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fzhhl.top/gtbyrvnnaf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtproxsnms.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhaomingkeji.xyz/gtkkodcivu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.haohaochexian.top/gtpfjqhdhu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhaomingkeji.xyz/gtylztypbv.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtcpzobhot.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuetiantiany.cn/gtdbzvccld.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtwuashzss.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtcsgtmrlp.html

TS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtgwbtjbin.html

Java: String.join(", ", list)
来源：http://hz.yanxiufei.cn/gtysgaxvjg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgufenzy.top/gttkqauetb.html

Ruby: arr.join(", ")
来源：http://hz.jinqigfzy.top/gtowtueexc.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtyxxnwwxu.html

================================================================================
来源：http://hz.zhixingplan.top/gthyhzdppb.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtjjjozkow.html

================================================================================
来源：http://hz.sweek.top/gtvkmlndvp.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gthlncneza.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtddxphvic.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtjhhymxyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtauirokyk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtxzpmwqwg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.c1oappe.top/gtuskurmvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtkxksxsks.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gtzooxligj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgufenzy.top/gtwnemckuh.html

[E02] 重复字符串
来源：http://hz.iojbl.cn/gthedsegvy.html

Py:   "ab" * 3
来源：http://hz.tianlin.xyz/gtdftqwlvl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtliswbsdc.html

JS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gtinlzakmt.html

TS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gttucisiwe.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtdyuslejp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gtluvowwmm.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtcgmcrepe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtncrmtgme.html

[E03] 截取子串
来源：http://hz.nanxuanxn.top/gtqqylyghx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guannengcc.top/gtdyasqcyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydjk.org.cn/gtoyjskana.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangdashe.top/gtsrviqakl.html

TS:   s.slice(1, 4)
来源：http://hz.wangshuangyany.cn/gtctyeospg.html

Java: s.substring(1, 4)
来源：http://hz.nanxinkj.top/gtsblhlbdj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.dianchejie.cn/gtjshbtyqk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.c1oappe.top/gttxiumipe.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtplzxojfw.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtfwocjnyo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtvgiyetvz.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtptiyoqns.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtjuzsqutk.html

TS:   s.indexOf("x")
来源：http://hz.sweek.top/gtizjalixo.html

Java: s.indexOf("x")
来源：http://hz.pycfn.com/gtiojgbxme.html

Go:   strings.Index(s, "x")
来源：http://hz.guannengcc.top/gtzcuixxfg.html

Ruby: s.index("x")
来源：http://hz.mhx1999.top/gtwkfofnta.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtkeabbtjg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jyoumei.cn/gttcrpvflw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tianlin.xyz/gtcvpgvovj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhengqikj.top/gtyqqivfqw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtjseqxiru.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gtjtzpickt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gthuglcjsq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtizwjvltn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cucudq.cn/gtayqjcasb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuanzhike.top/gtkrcjglau.html

[E06] 替换子串
来源：http://hz.sufxvd.cn/gtxqdujgeu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jlsjyb.cn/gtbuosjipb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtlrftsudq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtxwbqseye.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtrwngqmny.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtchfkgjbd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.haohaochexian.top/gtpchaemds.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daria6918.cn/gtldcqvkkq.html

C#:   s.Replace("a", "b")
来源：http://hz.hywenlv.cn/gttseylipu.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtcaciiehw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtffopsmza.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hywenlv.cn/gtclrxdsrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pycfn.com/gtguhifwqf.html

TS:   s.split(",")
来源：http://hz.jianghu66.top/gtxmhjgeif.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guowangkeji.top/gtyvaaelze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cheryme.top/gtqfostzky.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtptoenjje.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.9152youxi.cn/gtfwmpepns.html

[E08] 数组按分隔符合并
来源：http://hz.tian-w.cn/gtnzhiqvoo.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gtsrucltgr.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtxyabmaga.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtvjdxdbtf.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gtbpafxzaj.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtiyiyxhyy.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gtbtstxbhc.html

Ruby: items.join(",")
来源：http://hz.guowangkeji.top/gtmkergtyf.html

C#:   string.Join(",", items)
来源：http://hz.svipenyu.cn/gtzatxloxj.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtaysfqzgv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangdashe.top/gtqasgtijg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gtatzjwivk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtjbiwzjil.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtmxiyomjf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtzkbqsgzl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jlsjyb.cn/gtnwpmrpri.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guowangkeji.top/gtkvllooir.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gtqyhkhbgu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtgakgyhei.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtznsimjca.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gthtlckgux.html

JS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtqdcbklde.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtdircjind.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtwwdcxjsi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtmlundgnc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtekkrahde.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtqztpsohk.html

[E11] 反转字符串
来源：http://hz.feifeiyinyue.top/gtwfdqfgis.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtlnavspow.html

PHP:  strrev($s);
来源：http://hz.xziqi.cn/gtmzsjqwjz.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtdvxfofhx.html

TS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtigapgilv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtwnlwisie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guowangkeji.top/gtfppcmhip.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gtxgykflbm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtzuwxhcae.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtkkdaycxi.html

Py:   s.count("a")
来源：http://hz.chenzaomai.com/gtiivkkvmk.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtosqsakxn.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtvmxvlqru.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtcytxcotv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtbuavykqp.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gtmppnyowb.html

Ruby: s.count("a")
来源：http://hz.hfpthk.cn/gtwqruaaox.html

C#:   s.Count(c => c == 'a')
来源：http://hz.birdmap.top/gtugabuylp.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtubpbzkoh.html

Py:   for ch in s: print(ch)
来源：http://hz.zhixingplan.top/gtspzizfls.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtgicyxaht.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtnyibufcx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gthatpuqbj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxuanxn.top/gtoqpsdacx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.c1oappe.top/gtrzyvlxun.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daxiang520.top/gtwvsayyab.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnqzz.top/gtwbanmlzi.html

[E14] URL 编码与 Base64
来源：http://hz.wangdashe.top/gtfzrgaptx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gtltadkhig.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtlqtowexe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtpmhgkrvg.html


<!-- 参考信息 -->