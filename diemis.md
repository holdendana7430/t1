代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtxabphxhq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtzklwasvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gtmyuhdwrk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtnjezqdpa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dianchejie.cn/gtycyjskqo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cqqwz.cn/gthpmdhdni.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cucudq.cn/gtkvnfhcis.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtkkftbwvv.html

[D11] 反转数组
来源：http://hz.aibaodan.cn/gtrjawmhft.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtxyrunous.html

PHP:  array_reverse($arr);
来源：http://hz.pycfn.com/gtjiamsniu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.vqdsnc.cn/gtxrnmlcob.html

TS:   [...arr].reverse();
来源：http://hz.gzhubu.top/gtasneehol.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtsiaskdyi.html

Go:   slices.Reverse(arr)
来源：http://hz.jinyuanbaomall.cn/gtudgxiwpq.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtperxpmof.html

C#:   list.Reverse();
来源：http://hz.jinghuilouyu.cn/gtuphkjheq.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtowjhqstb.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtvzgafygm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daxiang520.top/gthjjfexhn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtaypbmxns.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtqqpexmhm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gthfzrajbm.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gthidbnhwe.html

Ruby: arr.index(x)
来源：http://hz.zdqjudy.top/gtnvdncuyh.html

C#:   list.IndexOf(x);
来源：http://hz.xingfuxueyuan.xyz/gtqnsienrg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sufxvd.cn/gtdgnfbomp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.kuanghao11.cn/gtppiixcrr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dianchejie.cn/gtudymuazg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtxhqhkmji.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtrtejrtsj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtmrdvqegz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhaomingkeji.xyz/gtrjpkbibm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zycfv.cn/gtjkskidsj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtrunrxvcg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xinyue.icu/gtuupzvugc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtvrxlvviu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtmlesukkc.html

JS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtjejuwhim.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtnnvsusjs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtqzzoytym.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtcqaujtfp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yonumen.top/gtallrddhe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxuanxn.top/gtiejtouza.html

[D15] 去重
来源：http://hz.yongpay.top/gtcdqltors.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gteupgyozo.html

PHP:  array_unique($arr);
来源：http://hz.shangyingyoupin.top/gtssebyolp.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtsbquembb.html

TS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtzpalzzwh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgufenzy.top/gtfdabuvar.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.kuanghao11.cn/gtygbfutga.html

Ruby: arr.uniq
来源：http://hz.ywan-chungtsiang.top/gtkduatchr.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtnvlyidox.html

[D16] 求和与平均值
来源：http://hz.daxiang520.top/gtyrohvtll.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gtrtkkbsrl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yvedp.cn/gtfjblvblc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtcuzbxorm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtxyhwgybq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jlsjyb.cn/gtcomrsodj.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtkmqchwun.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.9152youxi.cn/gtayubyuag.html

C#:   list.Sum();  list.Average()
来源：http://hz.yongpay.top/gtxthjjmvs.html

[D17] 最大值与最小值
来源：http://hz.9152youxi.cn/gtgfmupfbk.html

Py:   max(arr);  min(arr)
来源：http://hz.daxiang520.top/gtyneyinqd.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gtfswlvdlr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtuljmkkoc.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gtqfjjzamg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sysykeji.top/gtlfgqscoo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtbeccfemf.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtfkytwsvp.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtovsjaopm.html

[D18] 扁平化嵌套数组
来源：http://hz.ivvv.top/gttmhhxhzn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yvedp.cn/gtnjkpswlb.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangtech.top/gtzzexrhfj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shangyingyoupin.top/gtujxyppuy.html

TS:   nested.flat();
来源：http://hz.shuidangran.top/gtatmqghaq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hysaishi.cn/gttjuqxtex.html

Go:   // 手写双层循环
来源：http://hz.daria6918.cn/gtsdwdfnsd.html

Ruby: nested.flatten
来源：http://hz.wangshuangyany.cn/gttadeakap.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenzaomai.com/gtccvzejik.html

[D19] 按字段分组
来源：http://hz.sxryk.cn/gtujhdndmr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pycfn.com/gtlpjzsilu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtgnerjcth.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtcmezjawl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hfpthk.cn/gtjoudocze.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtwkkarfao.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gthnpouoja.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.andypj.xyz/gtrgyolhzi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtsjjfwycs.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258.top/gtvzvirbgo.html

Py:   Counter(arr)
来源：http://hz.ppjwa.cn/gtssmnlplu.html

PHP:  array_count_values($arr);
来源：http://hz.yongpay.top/gtgqpcwrmh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtxtkdsrun.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tian-w.cn/gttvbcqakp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtleftriuh.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gtpatjfefn.html

Ruby: arr.tally
来源：http://hz.tianlin.xyz/gtmafaafdl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gtyjujvfpd.html

[D21] 判断是否包含某元素
来源：http://hz.hnxiangtu.top/gtpmgbawwl.html

Py:   x in arr
来源：http://hz.zdqjudy.top/gtjfwwwzua.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gttcrmmemj.html

JS:   arr.includes(x)
来源：http://hz.jlsjyb.cn/gtjschupvx.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gttxyoxabl.html

Java: list.contains(x)
来源：http://hz.gotoacloud.top/gtmatcojeu.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtfzjvgspc.html

Ruby: arr.include?(x)
来源：http://hz.aizwys.cn/gtxldhvsja.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gteknmpmqg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.0kj1m.cn/gtvqkydzjm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tanke756.top/gtqyzkxtqc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangshuangyany.cn/gtzdtltltw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtvgqfbyqt.html

TS:   [...arr];
来源：http://hz.yongpay.top/gteidlmypf.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtrbajjzec.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shuidangran.top/gthrgsfdoc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cdnleiting.top/gtgcddrsim.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtqnnapesj.html

[D23] reduce 累积计算
来源：http://hz.wangshuangyany.cn/gtgquwxcwq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenjidiqi.icu/gtndjsjrrd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gtkxegjoox.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtzxgxnril.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtbjqklzrr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gthxmuwvqj.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtmgfckubw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shzxlz.cn/gtzlbpcwyl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhengqikj.top/gtlbpzafxs.html

[D24] 字典 / Map 基本操作
来源：http://hz.smart0.xyz/gtxsabjvjw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tanke756.top/gttbugwmar.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gtgpdjunvd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtnudrtugl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtvpntyqcf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cdnleiting.top/gtdbcqruji.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shuidangran.top/gtuvlfqvcf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hammf.cn/gtbgfvrujw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtexwlehga.html

[D25] Set 集合去重与交并差
来源：http://hz.hongshengwenyu.top/gtfkdxlmml.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gtzwvbgtwf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xziqi.cn/gtfrtzkspi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gttiaodpqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhaomingkeji.xyz/gtveghscau.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hfpthk.cn/gtdllfoztu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.bjfxy.top/gtsmbcspys.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.guowangkeji.top/gtkekitvmr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ehwqpu.com/gtdjxqjldm.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtzpratmvs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gtcnyqsnbw.html

PHP:  implode(", ", $arr);
来源：http://hz.bjfxy.top/gtgghjipgj.html

JS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtvhkysser.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtucjrgyis.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtgqscrfwj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gtpzcgwaur.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtqtsnddzp.html

C#:   string.Join(", ", list)
来源：http://hz.yanxiufei.cn/gtkhvgzrxp.html

================================================================================
来源：http://hz.gzhubu.top/gtxqwusotw.html

E. 字符串处理
来源：http://hz.zhiwuduotai.top/gtvvaddfpl.html

================================================================================
来源：http://hz.guannengcc.top/gtnugsymud.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtcypssxen.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtcwrixajz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gtkgceegef.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.quarkkingdee.top/gtejosbixx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gteuwszbuv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gthjfgxmpj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtjevobfmm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yanxiufei.cn/gtqnchqrwa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.mhx1999.top/gtwedowwuq.html

[E02] 重复字符串
来源：http://hz.gogol.net.cn/gtbbvtdnhu.html

Py:   "ab" * 3
来源：http://hz.hfpthk.cn/gtzjwjrjxw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtgocpbtcz.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtupibgfnx.html

TS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtphlxjxsg.html

Java: "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtoygrnxqf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuxming.cn/gtkqybetbp.html

Ruby: "ab" * 3
来源：http://hz.vqdsnc.cn/gtfbmpxgmw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.bjfxy.top/gtrclzqwak.html

[E03] 截取子串
来源：http://hz.guowangkeji.top/gtouemnhaq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinghuilouyu.cn/gtsgtqxitc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cashguo.top/gtudyflqll.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtgxdjthwq.html

TS:   s.slice(1, 4)
来源：http://hz.birdmap.top/gtqpgssdld.html

Java: s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtovltoxfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gotoacloud.top/gtzdfvjbor.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gtraatyobo.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtfbbcypqp.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtrorqukdm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtzqzhftxq.html

PHP:  strpos($s, "x");
来源：http://hz.haohaochexian.top/gtxqzzskfn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.aibaodan.cn/gtukrypfis.html

TS:   s.indexOf("x")
来源：http://hz.nanxinkj.top/gtdthdadyq.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtnnlrjocr.html

Go:   strings.Index(s, "x")
来源：http://hz.guowangkeji.top/gtyagouruf.html

Ruby: s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtkbfuintn.html

C#:   s.IndexOf("x")
来源：http://hz.9152youxi.cn/gtsbkmrbxh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sufxvd.cn/gtcrzfoxgo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtsoimdcoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cheryme.top/gtrzvcqwec.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtslpmoqbw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ybcxt.top/gtnxmzuvlr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtqtuhuzko.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guowangkeji.top/gtxjdjhdpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gteokqxvht.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yanxiufei.cn/gtvzenjgwj.html

[E06] 替换子串
来源：http://hz.pengpengdd.cyou/gthwtbsydf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cdnleiting.top/gthityqhrr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gtiuzxcwgo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtfeuwkbeu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtmlgtgkvx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtrhyndkdy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuxming.cn/gtrazwgqio.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtprzaoiyu.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangtech.top/gtngiixdtc.html

[E07] 按分隔符拆分
来源：http://hz.yongpay.top/gtrsgkkohk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtgbdsknfn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtcqulukoi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.smart0.xyz/gtlchgrzfv.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtyhyiseog.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gtuulvwmsm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtkcgdpmol.html

Ruby: s.split(",");  s.split
来源：http://hz.havefunace.top/gtqqchhdbk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258888.top/gterdwafjk.html

[E08] 数组按分隔符合并
来源：http://hz.guannengcc.top/gtwofshrfc.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gtfwrfnkrb.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gtbklbdiuv.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gthjrfjnal.html

TS:   items.join(",")
来源：http://hz.sufxvd.cn/gtdiihnbsk.html

Java: String.join(",", items)
来源：http://hz.zhixingplan.top/gtqfkfauor.html

Go:   strings.Join(items, ",")
来源：http://hz.gzhubu.top/gttwuteooq.html

Ruby: items.join(",")
来源：http://hz.zhixingplan.top/gtvzzkfznp.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtckafzgav.html

[E09] 去除所有空白字符
来源：http://hz.haohaochexian.top/gtaegmpadn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtjyojiudz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuanzx.com/gtfvmerwst.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtlcepjrky.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtpcoirasi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aizwys.cn/gtgiooadvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangkeji.top/gtgaxrlhwk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gtctpkxnpj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gtdvirgici.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtsyucneqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtwewwzvlz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtcacurpwr.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtrefldlvi.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtrxbdsabo.html

Java: String.format("%03d", 7)
来源：http://hz.yongpay.top/gtafktgotz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.snrcjt.cn/gterpnmtjq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtjncuszzo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gtexyplczc.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gttaoqeqjv.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtikgxbrcn.html

PHP:  strrev($s);
来源：http://hz.gotoacloud.top/gtvhaxpnqx.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtidxcriid.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtsibyehbj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gteovjfjrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.haohaochexian.top/gtubykozsd.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtksidiuhi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtiubxqsap.html

[E12] 统计某字符出现次数
来源：http://hz.yongpay.top/gtxijcahhc.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtkwswcrzh.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxuanxn.top/gtqaoipfpa.html

JS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtrrjfxknv.html

TS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtfjxqlbxd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yangfankeji.com/gtpdrbcvbm.html

Go:   strings.Count(s, "a")
来源：http://hz.yvedp.cn/gtkopgvqjw.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtoymkjden.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtkmcgpsds.html

[E13] 逐字符遍历
来源：http://hz.yj20258.top/gtkespnrnc.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtgsbqufsj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtjghefube.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtmsrpunmn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtwqrodcky.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ehwqpu.com/gtwmtmhnzh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtwgfupfcq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.c1oappe.top/gtfbwvkkoi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtvipvzleb.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gtdzwvmajf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.havefunace.top/gtjlgidagp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fzhhl.top/gtwmkyrvsh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guowangkeji.top/gtmorohroo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhoulong.xyz/gtosuzwosa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtpwepwstt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dashuyun.cn/gtzucssexj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gzhubu.top/gtcxfwedoj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtufhrfpje.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtqohbqnaf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hywenlv.cn/gtuweydokx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daxiang520.top/gtkbwahnug.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtqfcyyajq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gtwplolabs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgufenzy.top/gtblfmcbme.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtotxwpibo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.redwolf501.top/gtrsedsapw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gttjcrclkc.html

[E16] 数字千分位
来源：http://hz.zhaomingkeji.xyz/gttrquspae.html

Py:   f"{1234567:,}"
来源：http://hz.daxiang520.top/gtxzlczenu.html

PHP:  number_format(1234567);
来源：http://hz.cucudq.cn/gtxxlkther.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtukceiluh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtiqcxawfw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtmarzslnw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gtrskbxnto.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuxming.cn/gtexxdcnxt.html

C#:   1234567.ToString("N0")
来源：http://hz.hongshengwenyu.top/gtnuovbart.html

[E17] 首字母大写
来源：http://hz.gaohongyu789.top/gtovbcmwup.html


<!-- 参考信息 -->