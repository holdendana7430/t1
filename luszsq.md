代发 wailian999

Java: list.size();
来源：http://hz.52xcode.cn/gtowyimdnp.html

Go:   len(arr)
来源：http://hz.0kj1m.cn/gtwnerwguz.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigfzy.top/gtmgcfehpw.html

C#:   list.Count;
来源：http://hz.zhongyouzk.top/gtblwvovgu.html

[D07] 切片 / 取子数组
来源：http://hz.nwbrower.top/gtozvhuezh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cheryme.top/gtjouidgmg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gtvzxqpaaf.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtttycxmni.html

TS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gtyswpguzw.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtkkttktmm.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtihawpfdh.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtlplutzbt.html

C#:   list.GetRange(1, 3);
来源：http://hz.jlsjyb.cn/gtgwlxxyxx.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtrnivkfsw.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gtbskovoex.html

PHP:  array_merge($a, $b);
来源：http://hz.ppjwa.cn/gttalhzdiv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtrmvjrslh.html

TS:   [...a, ...b];
来源：http://hz.yanxiufei.cn/gtpaxcydsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.andypj.xyz/gtpwxdhori.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtcnninvgj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hysaishi.cn/gtmmgecwgp.html

C#:   a.Concat(b).ToList()
来源：http://hz.quarkkingdee.top/gttvaxlctd.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gtxqbbualk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtvoamxpsr.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtflsjveuj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtwqfjucbp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zycfv.cn/gtmqeuljdc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nwbrower.top/gtjmnsytsx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtlvmlmwxm.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gthyfwtnek.html

C#:   list.Sort();
来源：http://hz.jqgufenzy.top/gtsliwoyrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gtmgzrmtcn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yvedp.cn/gttchhqlpv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gthwhgxjzc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtxojlzidn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtjpncmvdu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtmpgkxwzi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ybcxt.top/gtypjauhxr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtalgmrpmg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ehwqpu.com/gtmnwfxoom.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtmzxfzxcz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yongpay.top/gtpfbbcfqe.html

PHP:  array_reverse($arr);
来源：http://hz.yangfankeji.com/gtkfaibvbr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.mhx1999.top/gtxqlnhllc.html

TS:   [...arr].reverse();
来源：http://hz.hywenlv.cn/gtdjbfetyw.html

Java: Collections.reverse(list);
来源：http://hz.aibaodan.cn/gtypooeohw.html

Go:   slices.Reverse(arr)
来源：http://hz.guannengcc.top/gtrtxaiyuw.html

Ruby: arr.reverse
来源：http://hz.fzhhl.top/gtyjnhesfa.html

C#:   list.Reverse();
来源：http://hz.xylfe.cn/gtftdnzjgw.html

[D12] 查找元素下标
来源：http://hz.yangfankeji.com/gtxykciohs.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtexyuptpq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.havefunace.top/gtuboraypo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gthpmjoidy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtzkbvnmbp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.feifeiyinyue.top/gtxaddxzdy.html

Go:   slices.Index(arr, x)
来源：http://hz.fengsongda.top/gtqetwvmno.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtnysevnzh.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtwiyznfmm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtrpsqlext.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhoulong.xyz/gtphegoiyc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.c1oappe.top/gtpuztvkvm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtuljubsch.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtllkvcxbw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtkihisqnm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtoqqhgdec.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hongshengwenyu.top/gtiivtbjsx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258888.top/gtxbfbjzkd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigufen.top/gtdrxmwhwh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daria6918.cn/gtyvxteamd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yonumen.top/gtgmuexygz.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtatctfnmk.html

TS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gthmdbbwtn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenlongwang.top/gtnmxnsfru.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtdafcwmkz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.quarkkingdee.top/gtyojwtebf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xziqi.cn/gtccurzwrt.html

[D15] 去重
来源：http://hz.cucudq.cn/gtrndudplh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtzuiqvdin.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gthzlzcxuo.html

JS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtgyhfewis.html

TS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtyfcanopv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.0kj1m.cn/gticnkukho.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtgxzggfrn.html

Ruby: arr.uniq
来源：http://hz.chenlongwang.top/gtltjmwgfz.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtndyuwjhh.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtnpabjzlm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtsvgrnddg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtgwzctouo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtwdbdazog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtvzxbknle.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtnqolwcsm.html

Go:   // 手写循环累加
来源：http://hz.zhiwuduotai.top/gtisczdjje.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aizwys.cn/gtydsrnfhw.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtcdzqxztw.html

[D17] 最大值与最小值
来源：http://hz.birdmap.top/gtqzjmlgjn.html

Py:   max(arr);  min(arr)
来源：http://hz.yanxiufei.cn/gtjvzvijil.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gteoegzola.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtewjeizuh.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gtrjeptkeq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shangyingyoupin.top/gttstjqcnv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhongyouzk.top/gtwlnjemdu.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtoygiwuiw.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gtbxangkgs.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtoxumsppa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtwfodgbtb.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtfqfqixzw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenlongwang.top/gtbicwsmov.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtoeegjfpl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hysaishi.cn/gtsziapxyu.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gthzpeoeeo.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtwhdlmddi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtbujzojcq.html

[D19] 按字段分组
来源：http://hz.zhiwuduotai.top/gtzggjyfzx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtcdhebhjv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.birdmap.top/gtktoatujh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtrtklsxrq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtuswfxkez.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtsgfhfxjd.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtttmmsltz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtekwfvnyk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zdqjudy.top/gtwgjkyqqd.html

[D20] 统计每个元素出现次数
来源：http://hz.kuanghao11.cn/gteniutmip.html

Py:   Counter(arr)
来源：http://hz.jqgufenzy.top/gtbvnzybsq.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtplmhyjzh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtcokpcmxg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtepxnpvym.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gtdfwdcydw.html

Go:   // 手写 map[T]int
来源：http://hz.jyoumei.cn/gtxocmjlhx.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gtfaylzhis.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtijnvkcng.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtdmiyrojs.html

Py:   x in arr
来源：http://hz.fengsongda.top/gtncazihdv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.bjfxy.top/gtntrujcmd.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtifxcwrmm.html

TS:   arr.includes(x)
来源：http://hz.jianghu66.top/gttaeyjqql.html

Java: list.contains(x)
来源：http://hz.tianlin.xyz/gtwdkywjnv.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtqzbdksdh.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtjmxpxczd.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtxumqonor.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258888.top/gtudryugil.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtbfkycepj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtflshgcff.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtabqzzbly.html

TS:   [...arr];
来源：http://hz.haohaochexian.top/gtfywolyqz.html

Java: new ArrayList<>(list);
来源：http://hz.feifeiyinyue.top/gtwekrbzot.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtjjjzvgeu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtxpckcvyt.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtfjcfuaux.html

[D23] reduce 累积计算
来源：http://hz.yonumen.top/gtrloojkjd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gtixiikqta.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuxming.cn/gtgulylrig.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtjwevbtbw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtapzhcuox.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtyqbpbcyc.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtfitdwnom.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gthswrtxqk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gteqqhlhoq.html

[D24] 字典 / Map 基本操作
来源：http://hz.shzxlz.cn/gtnghnpbjb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gaohongyu789.top/gtugfmnsap.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenjidiqi.icu/gtzjvpcfns.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gthcqrbbau.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhijiandao.cn/gtpsbjkzug.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtevimatju.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydjk.org.cn/gtgstygvrt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtjtzhylbi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtwmxvdejn.html

[D25] Set 集合去重与交并差
来源：http://hz.daria6918.cn/gteamhdqnz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtwzsmtwwh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cheryme.top/gtnhugvkvi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuanzx.com/gtgjjlmtat.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtdhcjilmh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenzaomai.com/gtioqzkduw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gtetbuywku.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtnwysguiq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tian-w.cn/gtnulyvyqs.html

[D26] 数组转字符串
来源：http://hz.zhiwuduotai.top/gtourafszs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gogol.net.cn/gtdfsgzgzx.html

PHP:  implode(", ", $arr);
来源：http://hz.redwolf501.top/gtyoxhpaxs.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtdgkegcqf.html

TS:   arr.join(", ")
来源：http://hz.cheryme.top/gtxjyxbetg.html

Java: String.join(", ", list)
来源：http://hz.jianghu66.top/gtmtwunqmn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtnlepemdh.html

Ruby: arr.join(", ")
来源：http://hz.daxiang520.top/gtjcssxyme.html

C#:   string.Join(", ", list)
来源：http://hz.guowangkeji.top/gtaiwxrjyo.html

================================================================================
来源：http://hz.zhijiandao.cn/gtakufzyll.html

E. 字符串处理
来源：http://hz.yonumen.top/gtvtylipxg.html

================================================================================
来源：http://hz.ivvv.top/gtttfflvhq.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtgfamefza.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.snrcjt.cn/gtbrhvxugg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinghuilouyu.cn/gtrbhvrcar.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtjwyhrxzw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtfarcrrlt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gturwewplf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtcxiohqiv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtbmpjjvdn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtmemsrnkn.html

[E02] 重复字符串
来源：http://hz.hnxiangtu.top/gtigdpicgp.html

Py:   "ab" * 3
来源：http://hz.hfpthk.cn/gtbfeawbfb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangshuangyany.cn/gtqdicufbp.html

JS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtusvbmewc.html

TS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtiuzdtpfc.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtikujuqxc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xinyue.icu/gtkisabrmz.html

Ruby: "ab" * 3
来源：http://hz.cdnleiting.top/gtltbwifdu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gtxqveidke.html

[E03] 截取子串
来源：http://hz.pycfn.com/gtrtecdltm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gtggvixojn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gtwxrqrjgj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gtiyxannge.html

TS:   s.slice(1, 4)
来源：http://hz.fengsongda.top/gteephvpdr.html

Java: s.substring(1, 4)
来源：http://hz.ppjwa.cn/gtpswspsio.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.vqdsnc.cn/gtqmupmjze.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sweek.top/gtpuuzrwut.html

C#:   s.Substring(1, 3)
来源：http://hz.xuanzx.com/gtpezlqlyr.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangtech.top/gtnwcnzxeq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.svipenyu.cn/gtfojvsdjo.html

PHP:  strpos($s, "x");
来源：http://hz.cheryme.top/gtktumoxgh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnqzz.top/gteudnnkli.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtegqqrnfj.html

Java: s.indexOf("x")
来源：http://hz.yj202588.top/gtizbnnscv.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gtrlbgwpof.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtvkeqxvmf.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtxhhdxpln.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tanke756.top/gtxjptfepp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtwdnunbew.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.meibo888.top/gtyvdvwfnc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtohkablbt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtmcqautja.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtnarkglyw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yongpay.top/gtsgvudesx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ehwqpu.com/gtpsjkplli.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtbnoxnmau.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gtvpsizzqz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gttcywptoy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhengqikj.top/gtsuioeeti.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtdbiogyky.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtsvaockis.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtjirojvmd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtcvmznlfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.meibo888.top/gtamyjcnju.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtdheqdqxb.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtzjcrhijb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tian-w.cn/gtnfibgskj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtodgyunpn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jyoumei.cn/gttasylhhy.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtbvdjgakg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gtueqhyyxv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jlsjyb.cn/gtxstshqdn.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtzxvbsysj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtoqbhbmtv.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtoreeaata.html

Py:   ",".join(items)
来源：http://hz.andypj.xyz/gtogverdov.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtdgaocmqr.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtshtquqzz.html

TS:   items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtqxhdhqce.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gtufcfczsn.html

Go:   strings.Join(items, ",")
来源：http://hz.bjfxy.top/gtkcieitaa.html

Ruby: items.join(",")
来源：http://hz.hnqzz.top/gtgnhovvbt.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtvskwyazo.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtoncfdkjd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtmzbuwqge.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtkpiuvamd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtkukmxtup.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtebohyksf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gtpwptaclh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhixingplan.top/gtwznkjjzq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hysaishi.cn/gtozmgttbu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtpbaamtch.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fzhhl.top/gtvmfbmesx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gotoacloud.top/gtqkvhqxqa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gttxgrwzjf.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtjogumeae.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtqpktmlrb.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gtxxjskfzy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtvlrjodsm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtjjprekxm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yongpay.top/gtmuptiaip.html

[E11] 反转字符串
来源：http://hz.hnxiangtu.top/gtwozrbhzu.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtwmemrttd.html

PHP:  strrev($s);
来源：http://hz.xuanzx.com/gtdfteqcyv.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtrivublke.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtrusulnnx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtzzvhiuyd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangdashe.top/gtttirgwod.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gtqmtffyoq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtqtirsszq.html

[E12] 统计某字符出现次数
来源：http://hz.jinyuanbaomall.cn/gtpjzwqiwv.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gtzyrngonr.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gtrlgjkxvm.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gttyvpvipx.html

TS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtzwqywqez.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jyoumei.cn/gtdilfkecl.html

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtmtqmuumd.html

Ruby: s.count("a")
来源：http://hz.cdnleiting.top/gtvlipdcka.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtmfjzeqot.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtcqnukwcs.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gtrklwebsg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.iojbl.cn/gtvscxjnwf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtqukhbqjy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gthgghyixn.html


<!-- 参考信息 -->