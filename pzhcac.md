代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.cqqwz.cn/gtejjoijja.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtgjpqfdld.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtumwuidxk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtmgddepvp.html

PHP:  sort($arr);
来源：http://hz.316326.xyz/gtkbnkrlcu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtxefitazl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.feifeiyinyue.top/gtteocgqoy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtsgtnylqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtyfctecxg.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtzyegbxxr.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtwnglfubz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aizwys.cn/gtkzlxbudl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj202588.top/gtxfozpnnz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtgdvlmwvg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtiobzbjew.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtescarnxc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tianlin.xyz/gtlsvoycfg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtqhktaycb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nwbrower.top/gtkclgdqla.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yonumen.top/gtdvlybctv.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtqtodtnfk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zdqjudy.top/gteepaojps.html

PHP:  array_reverse($arr);
来源：http://hz.tian-w.cn/gtklmonhlb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtduivydjz.html

TS:   [...arr].reverse();
来源：http://hz.zdqjudy.top/gtvwnyzlrg.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtsgzrvpwl.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtigrhmkcl.html

Ruby: arr.reverse
来源：http://hz.ydzc1.top/gtobbugyoj.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtkzxlpumj.html

[D12] 查找元素下标
来源：http://hz.chenlongwang.top/gtmlkcrmuz.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtobyjhfgo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtbsbwdgiu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtpvtqiacq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtpomaccch.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenjidiqi.icu/gttwgwltdl.html

Go:   slices.Index(arr, x)
来源：http://hz.zhijiandao.cn/gtzqehqzms.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtlwcyeoyb.html

C#:   list.IndexOf(x);
来源：http://hz.zhongyouzk.top/gteggzyqao.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cucudq.cn/gtbyfoehya.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtbvgruwgn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtlbclsmpr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtfobdxcds.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtgcuxtqht.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dianchejie.cn/gtcdifrrkc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gaohongyu789.top/gtrawwrfay.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cucudq.cn/gtxgxiownr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.52xcode.cn/gtlzsharmi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtctkpjufc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gtfllxtqat.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtfzmfkoyh.html

JS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtxhtplelg.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gthakkufrr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.redwolf501.top/gtdpvcttob.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtwcvcjjpv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sweek.top/gtbjbuplea.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtzkrwvimg.html

[D15] 去重
来源：http://hz.jiagoushi.top/gttghywjya.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tian-w.cn/gtmrccdjph.html

PHP:  array_unique($arr);
来源：http://hz.jlsjyb.cn/gtopesoyrg.html

JS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtmayynelt.html

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtbjymuodx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hfpthk.cn/gtqpfjbhpu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenzaomai.com/gtqeemphjv.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtwibkdhbx.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gtwskogzfa.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gthhbuchou.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhongyouzk.top/gthwollzrw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenjidiqi.icu/gtfvgjgmdx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtdsliontn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gthwbdljrg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtlrspkeqw.html

Go:   // 手写循环累加
来源：http://hz.ywan-chungtsiang.top/gtcucivbfq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gtzhlizieq.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydzc1.top/gtfnnjluir.html

[D17] 最大值与最小值
来源：http://hz.yuxming.cn/gtwlhynjkt.html

Py:   max(arr);  min(arr)
来源：http://hz.havefunace.top/gtlfftxqlg.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtcuhwrxkm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gtaezewjfs.html

TS:   Math.max(...arr);
来源：http://hz.yongpay.top/gtdkwsebrp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xinyue.icu/gtdvvsbruh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.andypj.xyz/gtehxlanbe.html

Ruby: arr.max;  arr.min
来源：http://hz.guowangkeji.top/gtkbosonis.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtwqgtoqzq.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtorgyiiui.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cucudq.cn/gtrwavomoy.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gthljjmoin.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtnzuylfbn.html

TS:   nested.flat();
来源：http://hz.bjfxy.top/gtbfqulioj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xinyue.icu/gtkdyjjdhc.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtlglvslwu.html

Ruby: nested.flatten
来源：http://hz.wangshuangyany.cn/gtmxvjbilt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigufen.top/gtaewtaigj.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtsvmoxfqa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.0kj1m.cn/gtvdbxxkdh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ehwqpu.com/gtgfjaormm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pengpengdd.cyou/gtnnlshtyy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.meibo888.top/gtxeajezyc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangshuangyany.cn/gtwoxvdlcb.html

Go:   // 手写 map[string][]T
来源：http://hz.ehwqpu.com/gtjurlunjt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtacrufapr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhaomingkeji.xyz/gtqshmdihk.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gteyeikmks.html

Py:   Counter(arr)
来源：http://hz.yuanzhike.top/gtswckefxa.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtibrqappm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtqlowddvc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtmovgkpik.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gthcrfigjk.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gtxaqfxifk.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtrnxbvvun.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dianchejie.cn/gtufukkori.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gtbymbaplg.html

Py:   x in arr
来源：http://hz.guowangkeji.top/gtczbheyeg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtdotugona.html

JS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtgfmtwtti.html

TS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtewrtylko.html

Java: list.contains(x)
来源：http://hz.meibo888.top/gtntvsbcxr.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuanzx.com/gttrwdrrym.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gtpgrutoxk.html

C#:   list.Contains(x)
来源：http://hz.tianlin.xyz/gtaejutivj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhixingplan.top/gtgspyzlfb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shuidangran.top/gtmkqraydl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shangyingyoupin.top/gtsszmduqf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tian-w.cn/gtqyrqjyin.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gtdafcytat.html

Java: new ArrayList<>(list);
来源：http://hz.ivvv.top/gticjalqef.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtymeuwpgg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gotoacloud.top/gtqesvkgjh.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtikwncqiz.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtpzyqgtlu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtdzzgkiox.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nwbrower.top/gtpcrxspdl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtezrtswzf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgufenzy.top/gtvotghqbf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtuiltzuef.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtnqigvkik.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtumxifhao.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.9152youxi.cn/gtcfyjvzkx.html

[D24] 字典 / Map 基本操作
来源：http://hz.gogol.net.cn/gtjggwbozt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nwbrower.top/gtkybdgygq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtowlumtjm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ivvv.top/gttnfswaue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtuhmpwffy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtvmpuxtup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gteuqnlfvo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nwbrower.top/gtvvjqvhnq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj20258888.top/gtnskbijiv.html

[D25] Set 集合去重与交并差
来源：http://hz.jyoumei.cn/gtxsyahtga.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtyjvyjbag.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtayxtwovu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtkqystscx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258888.top/gtguqfttfe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj202588.top/gtltfdohhd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shuidangran.top/gtgonupjqm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj202588.top/gtiwkwdzjc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtxboeetzu.html

[D26] 数组转字符串
来源：http://hz.nanxuanxn.top/gtgeptnkvm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ywan-chungtsiang.top/gthaghxleh.html

PHP:  implode(", ", $arr);
来源：http://hz.nwbrower.top/gtmnmavtsc.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtlapjphpw.html

TS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtqspcvcko.html

Java: String.join(", ", list)
来源：http://hz.yj20258.top/gtwspormry.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtqqvmcrhc.html

Ruby: arr.join(", ")
来源：http://hz.9152youxi.cn/gtoakrzjxt.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtxiexgtkw.html

================================================================================
来源：http://hz.jiagoushi.top/gtrqgvftkj.html

E. 字符串处理
来源：http://hz.shanyushiyangtech.top/gtbsmpowqm.html

================================================================================
来源：http://hz.gotoacloud.top/gtuuiimusm.html

[E01] 拼接字符串
来源：http://hz.yonumen.top/gtcepbplyu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinyuanbaomall.cn/gtscrqdozg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.redwolf501.top/gthbtojzup.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtsjjbfwyn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtgupmjaca.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtpiikeowa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.9152youxi.cn/gtzcnizlsb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ppjwa.cn/gtyddxwodw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhijiandao.cn/gtklsopaut.html

[E02] 重复字符串
来源：http://hz.zhengqikj.top/gtaiyoqznr.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtpvhfmadp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gthvgctwkk.html

JS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtuwaaaddm.html

TS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtqfxoncjn.html

Java: "ab".repeat(3)
来源：http://hz.316326.xyz/gtruzsbmvc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtlcvfwrkz.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gteydjcsew.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuxming.cn/gtyoaurmoh.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtmhoryizn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangshuangyany.cn/gtavvuuhhy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nwbrower.top/gtfclmjmwi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtyzlodgif.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtriedlknh.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtzrnivojz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhijiandao.cn/gttlncskse.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtpmxltudf.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtqazaliqn.html

[E04] 查找子串位置
来源：http://hz.chenzaomai.com/gtgdposixu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shangyingyoupin.top/gttbammcyw.html

PHP:  strpos($s, "x");
来源：http://hz.gogol.net.cn/gthqzzvfhw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gthuortkyy.html

TS:   s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtqhxnbqdr.html

Java: s.indexOf("x")
来源：http://hz.dianchejie.cn/gtoulffobu.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258888.top/gtuxsoyrey.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtmhvvirww.html

C#:   s.IndexOf("x")
来源：http://hz.0kj1m.cn/gtymtelnmx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258888.top/gtnzlghpts.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtsjfcmeok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.9152youxi.cn/gtwluznmwm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gttcyrklqr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sufxvd.cn/gtqfzqeofg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gticbagbbx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shzxlz.cn/gtssungzrt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtuxykvzyv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.9152youxi.cn/gtyvbgoibc.html

[E06] 替换子串
来源：http://hz.meibo888.top/gtlfalaaes.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tian-w.cn/gtndokhimi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhengqikj.top/gtfarzomac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtmevgifkt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtjzagxlpr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtcxueyyiq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jlsjyb.cn/gtgcdhzlle.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.svipenyu.cn/gtezafahdw.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtjuuwfsem.html

[E07] 按分隔符拆分
来源：http://hz.zycfv.cn/gtmkbripgo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangshuangyany.cn/gtyyuclcph.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gtekqqdyes.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtdthjjvfi.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtozhuofzf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.mhx1999.top/gtxdhagfvi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigufen.top/gtsbdiswcz.html

Ruby: s.split(",");  s.split
来源：http://hz.chenzaomai.com/gtnfevazdn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gtlkzoejig.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtegqmvzge.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gtisjhtfnu.html

PHP:  implode(",", $items);
来源：http://hz.jianghu66.top/gtbsgczicz.html

JS:   items.join(",")
来源：http://hz.dianchejie.cn/gtiarktqun.html

TS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtswppevvx.html

Java: String.join(",", items)
来源：http://hz.bjfxy.top/gthzvdukrx.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxuanxn.top/gtvpkmxnpm.html

Ruby: items.join(",")
来源：http://hz.nwbrower.top/gtttjpmdno.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtofwmbloc.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gtmrigxxqn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtrrjtctph.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.birdmap.top/gtpeloaqko.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtjdrziylv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtucytjngq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangtech.top/gtrtvrjgcm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtleosojdq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yueranfly.top/gtamwyteps.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtwlypshuz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tanke756.top/gtmsxlynhw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yanxiufei.cn/gtehvoahcw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gthqefpbrh.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtmcagmefr.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtwucsznbf.html

Java: String.format("%03d", 7)
来源：http://hz.zhengqikj.top/gtavjskhzk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ehwqpu.com/gtmnlskyff.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtufkhcgnw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xinyue.icu/gtxhlpluhg.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gtetdmotpr.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtqzdosweg.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtjcihtidm.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtgkpjmmdi.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtgjppjcmq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tian-w.cn/gtsopawbdg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtlxirauwp.html

Ruby: s.reverse
来源：http://hz.zhijiandao.cn/gtcntrnbho.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtblqfqwqq.html

[E12] 统计某字符出现次数
来源：http://hz.yueranfly.top/gtejdlpbqt.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gtmrknjfog.html

PHP:  substr_count($s, "a");
来源：http://hz.xuanzx.com/gtcrhyjebf.html

JS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gttdeneslq.html

TS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gtjmsjzpal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtnoxwxrli.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gtmwglofpv.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtjmpludyx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gogol.net.cn/gtrwpquzrw.html

[E13] 逐字符遍历
来源：http://hz.yuxming.cn/gtkifwdgen.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtazmblnaw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangshuangyany.cn/gtbxcuzhfl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtedpjyrjb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gttyatwnzy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtdnjovfxv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtxkwiuzev.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhaomingkeji.xyz/gtodvmbatk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtdzasycbq.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtjflubjrl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuanzx.com/gtinitsndo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.9152youxi.cn/gtwzmfmjeq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtpekacmtj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydjk.org.cn/gtndxtffdz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtyxwsxlyv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgfzy.top/gtusqsvtrh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgfzy.top/gtfvjbyzav.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtipedodbo.html

[E15] HTML 转义 / 反转义
来源：http://hz.svipenyu.cn/gtznxtwbap.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhiwuduotai.top/gthxgemniv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtwytfqekv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.kuanghao11.cn/gteekyormi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtvgtpocuc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.9152youxi.cn/gtgvpsiaiz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhaomingkeji.xyz/gtujfwoicq.html


<!-- 参考信息 -->