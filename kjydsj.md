代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yanxiufei.cn/gtegljvwco.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtmwewensr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gthzaqttmq.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtlrgtysxa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenjidiqi.icu/gtlzyaqdzv.html

C#:   a.Concat(b).ToList()
来源：http://hz.cashguo.top/gtaeqzwtrt.html

[D09] 排序（升序）
来源：http://hz.gogol.net.cn/gtgojffqyu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtnlikntrw.html

PHP:  sort($arr);
来源：http://hz.sufxvd.cn/gtwcyepgon.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtqkukcasv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daxiang520.top/gteeoziepd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxuanxn.top/gtnpvcwqwp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtmgtladun.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtdesareqv.html

C#:   list.Sort();
来源：http://hz.fzhhl.top/gtkiivfsnq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gtpivbcmej.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtljtjqbtd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtdiywgjgc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtwvxyagvr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtcgpyxllw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.smart0.xyz/gtusgmcjgp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guowangkeji.top/gtjacqioxu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuanzx.com/gtjgxtthes.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtytapwmlf.html

[D11] 反转数组
来源：http://hz.fengsongda.top/gtifrjlcmg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yanxiufei.cn/gtocztluli.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangtech.top/gtgbgiwapu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cheryme.top/gtnzsmndkc.html

TS:   [...arr].reverse();
来源：http://hz.xuetiantiany.cn/gthuprpnkg.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtkscvukph.html

Go:   slices.Reverse(arr)
来源：http://hz.andypj.xyz/gtylhstvag.html

Ruby: arr.reverse
来源：http://hz.gotoacloud.top/gtdgitplfc.html

C#:   list.Reverse();
来源：http://hz.hysaishi.cn/gtypvltruv.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangtech.top/gtkbsgynrl.html

Py:   arr.index(x);  x in arr
来源：http://hz.52xcode.cn/gtekuedjqm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtddwbezyf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtlhzjawnv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtwsutzucb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtvhrfgagd.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gtubtwbbug.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtdkztqmcw.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gtxtmsjrtw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.kuanghao11.cn/gtfrwmtsgr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtgdpheayx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnxiangtu.top/gtczblixwl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtepajnmdf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtuojzzffz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hywenlv.cn/gtyjstefel.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxinkj.top/gtshijafpv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtxecotsui.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtakbkvmhi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guowangkeji.top/gtxigkzheb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenzaomai.com/gtxgeucgni.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtbwqgsaxe.html

JS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtmofbfzjc.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtrbylyrnz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.birdmap.top/gthyraokpq.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtivrbvcaq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gtuvcntpgb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtnyikchkz.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtrahstnxp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtnhmhmono.html

PHP:  array_unique($arr);
来源：http://hz.yuxming.cn/gtigoxjqzb.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtfdzoxdit.html

TS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtyvzccrna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtootyacss.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtrrzzkpzo.html

Ruby: arr.uniq
来源：http://hz.jinqigufen.top/gttsaqylis.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtljnqqlid.html

[D16] 求和与平均值
来源：http://hz.hnxiangtu.top/gtfeqmlfvc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xylfe.cn/gtohtxvgcz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gzhubu.top/gtadjntiab.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtivxxdyld.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yueranfly.top/gtdobxesir.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tian-w.cn/gtqlcxwpak.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gtgczutqec.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtwtjllzwf.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtvvrocguw.html

[D17] 最大值与最小值
来源：http://hz.zhaomingkeji.xyz/gtvlvecbws.html

Py:   max(arr);  min(arr)
来源：http://hz.smart0.xyz/gtszwhgzke.html

PHP:  max($arr);  min($arr);
来源：http://hz.ppjwa.cn/gtvopomkqj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtlwwtgxbs.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gttuwaglue.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtltemxtjq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnqzz.top/gtmrvxjdyq.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtpurchciy.html

C#:   list.Max();  list.Min()
来源：http://hz.wangdashe.top/gthcsesvhh.html

[D18] 扁平化嵌套数组
来源：http://hz.daxiang520.top/gtpldlagun.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.haohaochexian.top/gtfttsoahd.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtvxfebwtl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daria6918.cn/gttmjhswfo.html

TS:   nested.flat();
来源：http://hz.cucudq.cn/gtnbfxdrsh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtnaxoqulk.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtrrzrmahb.html

Ruby: nested.flatten
来源：http://hz.andypj.xyz/gtpduapwdv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtognlbwdx.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtqfkrgqan.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.meibo888.top/gtkcnwvhcs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ybcxt.top/gtjmcabhbu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtzzztmkjr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtywsawnys.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangtech.top/gtiyjhtiic.html

Go:   // 手写 map[string][]T
来源：http://hz.dashuyun.cn/gtrzpszglc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhiwuduotai.top/gtlokpbjlv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.redwolf501.top/gtldqlgtwc.html

[D20] 统计每个元素出现次数
来源：http://hz.yonumen.top/gtfgkuzuyq.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtpqkrkjrd.html

PHP:  array_count_values($arr);
来源：http://hz.yuxming.cn/gtufznbpwq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtxgslgcnl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtfsrqmcjk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhijiandao.cn/gtxtgchomf.html

Go:   // 手写 map[T]int
来源：http://hz.gzhubu.top/gtewzkzgvx.html

Ruby: arr.tally
来源：http://hz.zhixingplan.top/gtimhhwnel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtbbrytpff.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtnkxjbcfm.html

Py:   x in arr
来源：http://hz.xingfuxueyuan.xyz/gtugezralb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtxwmhwgqn.html

JS:   arr.includes(x)
来源：http://hz.yongpay.top/gtpjwcjqlz.html

TS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gthnyvoxgw.html

Java: list.contains(x)
来源：http://hz.sweek.top/gtawqnngch.html

Go:   slices.Contains(arr, x)
来源：http://hz.quarkkingdee.top/gthviuqkpz.html

Ruby: arr.include?(x)
来源：http://hz.yuanzhike.top/gtvxkiqsex.html

C#:   list.Contains(x)
来源：http://hz.xuetiantiany.cn/gtvwssnkob.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hammf.cn/gtbvguzdet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.c1oappe.top/gtgcgyssnr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jlsjyb.cn/gtespiyvng.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtnsgwejsi.html

TS:   [...arr];
来源：http://hz.nanxinkj.top/gtscuhulje.html

Java: new ArrayList<>(list);
来源：http://hz.ydjk.org.cn/gtjiifefys.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pengpengdd.cyou/gttgjyspgi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtlkrgzsro.html

C#:   new List<int>(list);
来源：http://hz.sweek.top/gtsugdjsfw.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtmaboeuyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtwwddeish.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtcmyuokef.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtkouwczyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtxciemong.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.smart0.xyz/gtxsumgydh.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtfjfcbnwc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gzhubu.top/gtgwcjccja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xziqi.cn/gtbgbvkufv.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtcbzjacjg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.bjfxy.top/gttcizgjga.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gtycimsfel.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtctzzpybh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuanzx.com/gtqrxkravd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xinyue.icu/gtntqjdpwz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.bjfxy.top/gteqsmnhns.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtppyjegkb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgfzy.top/gtlwlngixx.html

[D25] Set 集合去重与交并差
来源：http://hz.aizwys.cn/gtygvjddou.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gttdnqcdhr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jianghu66.top/gtcxtwtixy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.havefunace.top/gtpabzdhub.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtozcknryf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jiagoushi.top/gttltophkc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gzhubu.top/gtodmwydwa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sweek.top/gtdlnrsfrh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gtaccxoqyn.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtcdxjemcj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xingfuxueyuan.xyz/gtgqwsjwth.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtzkyqjdjj.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtodafsgkq.html

TS:   arr.join(", ")
来源：http://hz.meibo888.top/gtaodyklhn.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gthumcaqhc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yongpay.top/gtyzexarll.html

Ruby: arr.join(", ")
来源：http://hz.redwolf501.top/gtqtneyoze.html

C#:   string.Join(", ", list)
来源：http://hz.aizwys.cn/gttakjzgxc.html

================================================================================
来源：http://hz.smart0.xyz/gtdfbojsis.html

E. 字符串处理
来源：http://hz.yongpay.top/gtqcnphqkx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrdhbwipc.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gtsnepubkm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yangfankeji.com/gttkuvkkjr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtgljuzeyf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtbftymrbp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtqudzuoam.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtpzdzlzke.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cdnleiting.top/gttczvwfzh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtzemcellx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxinkj.top/gtvfibtnro.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtbscbhxau.html

Py:   "ab" * 3
来源：http://hz.haohaochexian.top/gtkyhfomuc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinghuilouyu.cn/gtdlsdenwr.html

JS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtdrahvwnu.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtnrbkviss.html

Java: "ab".repeat(3)
来源：http://hz.cqqwz.cn/gtivxcklgn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jyoumei.cn/gtrkcmzndw.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gthvhrihfk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gthjfcrhhl.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtmpnwjqlp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtsryhemug.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.mhx1999.top/gtafapykog.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtbhhjxfvn.html

TS:   s.slice(1, 4)
来源：http://hz.xinyue.icu/gtizeaapbj.html

Java: s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtazrhcikc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aizwys.cn/gtdqwlfcud.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gtdcarvffv.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258.top/gtwmfabskn.html

[E04] 查找子串位置
来源：http://hz.zhaomingkeji.xyz/gtfbqqydyu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtdlmtyiry.html

PHP:  strpos($s, "x");
来源：http://hz.cqqwz.cn/gtcdihsjok.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gtxlximmix.html

TS:   s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gttcgwwmjk.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtioboadpg.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtieidswwy.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtvzhrjtli.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtuvnecmdc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtzmyznzxm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.316326.xyz/gtzgsdpmkz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gtrzznjyur.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtpuzxwxgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hammf.cn/gtdxndttjo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtvrnsmuuw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gzhubu.top/gtcmbxsvpy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ywan-chungtsiang.top/gtgtxesige.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhixingplan.top/gtnoxjwvfj.html

[E06] 替换子串
来源：http://hz.ydzc1.top/gtxwyquhon.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gtqngbibuq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gttorlgzdw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtdrqzzfxm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtezqmrpti.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtzqijtkgs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtdyvxlxym.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.52xcode.cn/gtrvhqnkjc.html

C#:   s.Replace("a", "b")
来源：http://hz.pengpengdd.cyou/gtddtkurvu.html

[E07] 按分隔符拆分
来源：http://hz.jinyuanbaomall.cn/gttsvassex.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtwhjkixeo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhixingplan.top/gtekgdsvfa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gaohongyu789.top/gththelrax.html

TS:   s.split(",")
来源：http://hz.jinghuilouyu.cn/gtaerfxecz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jiagoushi.top/gttfalmfoo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhiwuduotai.top/gtdavxhtdo.html

Ruby: s.split(",");  s.split
来源：http://hz.shuidangran.top/gtzpjkixgm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.316326.xyz/gthytlnrcq.html

[E08] 数组按分隔符合并
来源：http://hz.ydzc1.top/gtqbffltjc.html

Py:   ",".join(items)
来源：http://hz.ydjk.org.cn/gtmenmrrhb.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtvrtmqeov.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtlkbrxziv.html

TS:   items.join(",")
来源：http://hz.cdnleiting.top/gtaeiyvvkc.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtwlfinzid.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gtvuzcgkya.html

Ruby: items.join(",")
来源：http://hz.yanxiufei.cn/gtyteefvha.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtocauomlx.html

[E09] 去除所有空白字符
来源：http://hz.nanxuanxn.top/gtqlkokayb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhixingplan.top/gtxcjjipdc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.0kj1m.cn/gtytoewlpu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.mhx1999.top/gtencrycjy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtwlqjnprt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gtpiwwgnjm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenlongwang.top/gtxirlbcuh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sweek.top/gtzybksaem.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tian-w.cn/gtfrzogbwy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yangfankeji.com/gtsebakkpu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fengsongda.top/gtplalnrgs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.smart0.xyz/gtnydzzwan.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtasofwzpm.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtiysivpuo.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtdragbekn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gturddgvtt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gtkoejgrhe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtizqwmcwy.html

[E11] 反转字符串
来源：http://hz.ybcxt.top/gtqdeinxcf.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtrxobzsxu.html

PHP:  strrev($s);
来源：http://hz.quarkkingdee.top/gtyysvttnj.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtsrgaehmy.html

TS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtcxwhnotp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtceywmttg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtriqmjowo.html

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtiqecrulq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtyfgjcefw.html

[E12] 统计某字符出现次数
来源：http://hz.9152youxi.cn/gtixjmfmso.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtzbkyrbbu.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtlefuxbqy.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtdfkcjido.html

TS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtssieikvt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.andypj.xyz/gtljxyzihc.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtbentncke.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtydwwalys.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nwbrower.top/gtmwctkhiz.html

[E13] 逐字符遍历
来源：http://hz.jyoumei.cn/gtzoqrqfzs.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtcfgcpjfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtytqqhpfh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtukgghpug.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hongshengwenyu.top/gtlzxeboen.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.smart0.xyz/gtfwoswpia.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtldegmxym.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtkcynxeyg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.iojbl.cn/gtiytovjzd.html

[E14] URL 编码与 Base64
来源：http://hz.xuanzx.com/gtkctvmxwa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gtmclljsxa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.iojbl.cn/gtrqfmjest.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.havefunace.top/gtfamfrkmj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtkrsbbsru.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtqgfbhgtu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xylfe.cn/gtogwpbwoy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yvedp.cn/gtinhaimsm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtzasfkxdh.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtxxsvmizf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj20258.top/gtkmcomsws.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtepcpmlkx.html


<!-- 参考信息 -->