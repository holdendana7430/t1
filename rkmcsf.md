代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.snrcjt.cn/gthaiphmcm.html

C#:   a.Concat(b).ToList()
来源：http://hz.yvedp.cn/gtumxegopl.html

[D09] 排序（升序）
来源：http://hz.xziqi.cn/gticivrbci.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gthfbzunji.html

PHP:  sort($arr);
来源：http://hz.gaohongyu789.top/gtcctzhutw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuxming.cn/gtoemvlxix.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hongshengwenyu.top/gtnauojagx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnxiangtu.top/gtlvgbwvry.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtdctyqfzs.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtguviphwg.html

C#:   list.Sort();
来源：http://hz.sxryk.cn/gtfznudxvh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xziqi.cn/gttfmunihs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtpzwkrhbq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtdrqenahs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gtkifrdrdl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtlavzxdcs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ivvv.top/gtqmuukxqe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtutcyadpa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xingfuxueyuan.xyz/gtmjgtncif.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cheryme.top/gtzejqkzyj.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtpvkhfpge.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtakcypyop.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtxifkzdaw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zdqjudy.top/gthfcqwawz.html

TS:   [...arr].reverse();
来源：http://hz.nanxinkj.top/gtfnxbbfpi.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gtvawnndbq.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtybirvjxr.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtpmuowuqc.html

C#:   list.Reverse();
来源：http://hz.ywan-chungtsiang.top/gtrpxhxdlb.html

[D12] 查找元素下标
来源：http://hz.jinyuanbaomall.cn/gtaeqxlkyj.html

Py:   arr.index(x);  x in arr
来源：http://hz.cheryme.top/gtbujqklqx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sysykeji.top/gtvdxbiwjm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtvyviijaa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.0kj1m.cn/gtmugqjoka.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtofjcntvu.html

Go:   slices.Index(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtcrciggxh.html

Ruby: arr.index(x)
来源：http://hz.xuetiantiany.cn/gthehzawwq.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtjvtchhnz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuanzx.com/gtpmkmywat.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangtech.top/gtiuczjpca.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtwdjggchy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtjcakzaag.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nwbrower.top/gtfjrniaxr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtjfgcqyzr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtiqcgxhji.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtypzfcisx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zycfv.cn/gtijlfvdwe.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtsgdlyaoi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtrennajdp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtslrmsjlz.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtlhfaqvad.html

TS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gticxpukxf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.vqdsnc.cn/gtortxazhq.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtfhvlulps.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tanke756.top/gtubofnphv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtbdwrzkdc.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtokfkbovs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gogol.net.cn/gtvszvobiw.html

PHP:  array_unique($arr);
来源：http://hz.zycfv.cn/gtqztnvrto.html

JS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gtdptgskom.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtqnzbqqre.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtkjppempp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daria6918.cn/gtvdtzqgaq.html

Ruby: arr.uniq
来源：http://hz.andypj.xyz/gtpdaehiyu.html

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtcrqbocwf.html

[D16] 求和与平均值
来源：http://hz.yuxming.cn/gtswjzsqfe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.316326.xyz/gttpluumho.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hywenlv.cn/gtroonxsjv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtotqrwmvz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtjheztnws.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.redwolf501.top/gtzrblvzen.html

Go:   // 手写循环累加
来源：http://hz.shangyingyoupin.top/gtqlxnejtf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gtmxwavlnz.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gtsdlfaghw.html

[D17] 最大值与最小值
来源：http://hz.jyoumei.cn/gttvufopyu.html

Py:   max(arr);  min(arr)
来源：http://hz.shzxlz.cn/gtadyzxxur.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtcasowcsc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gogol.net.cn/gtksnmoziv.html

TS:   Math.max(...arr);
来源：http://hz.cqqwz.cn/gthbakqfty.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yueranfly.top/gtgybzdwpc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtaxhffjkk.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtiiuphvqb.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtqmcnkesm.html

[D18] 扁平化嵌套数组
来源：http://hz.tanke756.top/gtotmwetkv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gthqvddlah.html

PHP:  array_merge(...$nested);
来源：http://hz.jlsjyb.cn/gtefnnbamf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtkxtxjrta.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtmxqdigsk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhixingplan.top/gtwdzudcca.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtzvnafqyt.html

Ruby: nested.flatten
来源：http://hz.tanke756.top/gtdeavaowf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtinykjvgf.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtpjrgqmjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtyqxqhpxh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtsrmwfnww.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuanzx.com/gtahjijcit.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gtqgmtbljx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnqzz.top/gtcigctabh.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtmdmygqcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.vqdsnc.cn/gtyubxmtza.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.meibo888.top/gtpgncmhrl.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gtninxqbxl.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtesnuulkv.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtwiapayps.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtvulnrqaf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtbdsoqtcd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtbmdphxkg.html

Go:   // 手写 map[T]int
来源：http://hz.ppjwa.cn/gtucfwneum.html

Ruby: arr.tally
来源：http://hz.quarkkingdee.top/gtblewtnew.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtgsdccjeu.html

[D21] 判断是否包含某元素
来源：http://hz.chenjidiqi.icu/gtozlqkepl.html

Py:   x in arr
来源：http://hz.jinqigfzy.top/gttnvnuuqo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.fengsongda.top/gtyfybbkzr.html

JS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtatnlshly.html

TS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtjuinqgtm.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtkfdxfeca.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtnkqruuyx.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtswmpxqwf.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtlptuivnu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ybcxt.top/gtwccdhahm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtqajpeumx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gtuwavgwxx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtkqaxkqcu.html

TS:   [...arr];
来源：http://hz.sweek.top/gtqriedzki.html

Java: new ArrayList<>(list);
来源：http://hz.nwbrower.top/gtacpodxbv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sweek.top/gtateszfkj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hfpthk.cn/gtrqerltyq.html

C#:   new List<int>(list);
来源：http://hz.hnqzz.top/gtltrzavmk.html

[D23] reduce 累积计算
来源：http://hz.zhengqikj.top/gtfdxqrsme.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangkeji.top/gtuwixuhkt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gtoxvqftka.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtpzvdkwom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtpnyopmcy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gtothyuzjd.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtzrxpyxmi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.feifeiyinyue.top/gtahjqmgyv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gttplnjrwv.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangdashe.top/gtvrplsiwv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tian-w.cn/gtbtbgxzez.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtfbsoyqnm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aibaodan.cn/gtjzrqkhko.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gthhvpydir.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gaohongyu789.top/gtwxiqldvn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gtqwhyydkq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.kuanghao11.cn/gtfsiviqpv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtlbzjqrwa.html

[D25] Set 集合去重与交并差
来源：http://hz.xuetiantiany.cn/gtsgkvyrkx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtguecpytd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuanzx.com/gtzakfmhjq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangdashe.top/gtslpexdjk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.svipenyu.cn/gtpizvsbsb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ywan-chungtsiang.top/gtcvttiaoe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtgvxeeuqt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtcnmicsrz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtqtusyyqo.html

[D26] 数组转字符串
来源：http://hz.xingfuxueyuan.xyz/gttpawrmeq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtooyuqaxt.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtcfrgrych.html

JS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtyamtfear.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtiogvikbk.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtdumewiqt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtfbvqskep.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtdwlaxhao.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtxfwhyrlt.html

================================================================================
来源：http://hz.ivvv.top/gtseklicas.html

E. 字符串处理
来源：http://hz.ehwqpu.com/gtgtxzmvzg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtztvcwauz.html

[E01] 拼接字符串
来源：http://hz.yonumen.top/gtelgctmrn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.c1oappe.top/gtpafujimr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhoulong.xyz/gtyqxywnsh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtscjsbolp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtrylohhzr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ivvv.top/gtdrysafgz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhijiandao.cn/gtuqxllyws.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtbkcltcpi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.316326.xyz/gtqjxwffzq.html

[E02] 重复字符串
来源：http://hz.jinqigufen.top/gtvonqkstm.html

Py:   "ab" * 3
来源：http://hz.shzxlz.cn/gtsqgfsznc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtvwcujswb.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtieifmxak.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gttraszefm.html

Java: "ab".repeat(3)
来源：http://hz.havefunace.top/gtxxqktvdr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnxiangtu.top/gtojvtpmdg.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtdbjzmtoq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ppjwa.cn/gtzgnpomoe.html

[E03] 截取子串
来源：http://hz.hnqzz.top/gtieydjrpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yongpay.top/gtgpjhvryf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gtkyrbghlr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtsvrbrsqg.html

TS:   s.slice(1, 4)
来源：http://hz.aizwys.cn/gtbnqskjgx.html

Java: s.substring(1, 4)
来源：http://hz.xylfe.cn/gtyffebauf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhengqikj.top/gtapmwtonp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.0kj1m.cn/gtiodkaauz.html

C#:   s.Substring(1, 3)
来源：http://hz.wangshuangyany.cn/gtrjlfnizb.html

[E04] 查找子串位置
来源：http://hz.smart0.xyz/gtmaujzzue.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sweek.top/gtwnqxroiz.html

PHP:  strpos($s, "x");
来源：http://hz.pengpengdd.cyou/gtigmgvwiu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtanvpsfwi.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtttvzfnii.html

Java: s.indexOf("x")
来源：http://hz.nwbrower.top/gtouadmuzz.html

Go:   strings.Index(s, "x")
来源：http://hz.svipenyu.cn/gtsjhrsnjm.html

Ruby: s.index("x")
来源：http://hz.c1oappe.top/gtzhlkfcin.html

C#:   s.IndexOf("x")
来源：http://hz.dashuyun.cn/gtipgqaqyp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yueranfly.top/gteqebwsdk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtsblqwurh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtqpejgnga.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtjxpklhwd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hammf.cn/gtwjilgaoz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gthezkhyxp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtvriwoixl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenjidiqi.icu/gtelbhxeoz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yvedp.cn/gtsbiebbcs.html

[E06] 替换子串
来源：http://hz.hywenlv.cn/gtdxshzzee.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gthuyqyrtj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sysykeji.top/gtppvyunlv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtvjooxyzk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtgfyefmsw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gttyojjiiu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtvfsxwciy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtwdliqhwr.html

C#:   s.Replace("a", "b")
来源：http://hz.yj20258.top/gtgrnyfter.html

[E07] 按分隔符拆分
来源：http://hz.zhoulong.xyz/gtxkupyrme.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xinyue.icu/gtaqnuhvli.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtiriivqtf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gtlejiyabl.html

TS:   s.split(",")
来源：http://hz.jqgufenzy.top/gtldynlnca.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yuxming.cn/gtmhfcsrzq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.havefunace.top/gtksiuevpu.html

Ruby: s.split(",");  s.split
来源：http://hz.nwbrower.top/gtkcmtxput.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gogol.net.cn/gteifvmcvs.html

[E08] 数组按分隔符合并
来源：http://hz.fengsongda.top/gtvgtptbtm.html

Py:   ",".join(items)
来源：http://hz.haohaochexian.top/gtfungtfuf.html

PHP:  implode(",", $items);
来源：http://hz.ybcxt.top/gtnghbflwd.html

JS:   items.join(",")
来源：http://hz.tanke756.top/gtqdtjrioj.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtpzkgbnju.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gtepidhbud.html

Go:   strings.Join(items, ",")
来源：http://hz.xuanzx.com/gtmeghiaeb.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtvdtwrugs.html

C#:   string.Join(",", items)
来源：http://hz.dianchejie.cn/gtuwopogmq.html

[E09] 去除所有空白字符
来源：http://hz.birdmap.top/gtxrsgscbp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtypcufjve.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gtghnechdx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtlukhuquo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtgyjxtefp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtwzuphrct.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.quarkkingdee.top/gtbrryyetu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daria6918.cn/gtkloeenep.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.svipenyu.cn/gtyexibamg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtiwdalwuc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guannengcc.top/gtjmptwjlb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gtfkpalrue.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtdwhnzpbn.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtitsqzbqp.html

Java: String.format("%03d", 7)
来源：http://hz.jqgfzy.top/gttbmqtyag.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gttvlbkdym.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jyoumei.cn/gtdgkeflvr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtpkyheuio.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtuqrgqpvb.html

Py:   s[::-1]
来源：http://hz.pycfn.com/gtvtozepgm.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtvkswvimn.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gttftbrdev.html

TS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtgvsztpiw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtiilrdrlp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhaomingkeji.xyz/gtgsgzrabz.html

Ruby: s.reverse
来源：http://hz.chenlongwang.top/gtqtvsvzkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtyvdxjloa.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gthnoabtmq.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtfciumnkd.html

PHP:  substr_count($s, "a");
来源：http://hz.daria6918.cn/gtmkcimpnb.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtpsldpjqc.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtcavopkyc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yangfankeji.com/gtypvbcixj.html

Go:   strings.Count(s, "a")
来源：http://hz.ywan-chungtsiang.top/gtcnuznxhs.html

Ruby: s.count("a")
来源：http://hz.xylfe.cn/gtwjotcxcj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtkxmpflbe.html

[E13] 逐字符遍历
来源：http://hz.fzhhl.top/gtgycorzjb.html

Py:   for ch in s: print(ch)
来源：http://hz.dianchejie.cn/gttufpkfld.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fengsongda.top/gtejonsfmw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gteaczpkml.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gttavwzofh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gtwsuomeuf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fengsongda.top/gtfshlqtmr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gteeppfjql.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtvsxxvshy.html

[E14] URL 编码与 Base64
来源：http://hz.sxryk.cn/gtgqwpdckl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.redwolf501.top/gtotwtghbd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xinyue.icu/gtqzyhmghq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tanke756.top/gtdxyihkew.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gtyavnnqxu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hfpthk.cn/gtuhrxihjz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtfcavouzi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jiagoushi.top/gtizpzvfmd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtdsbgsejm.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtifdzxgnb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sweek.top/gtnncyjhyj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gthcztjatq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.316326.xyz/gtfzxeqotx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gthkhvxthe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuxming.cn/gtwxgxmcit.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhengqikj.top/gtiwvbxsti.html


<!-- 参考信息 -->