代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.jyoumei.cn/gtqiypjczn.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhixingplan.top/gthingwukq.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtmbuutbeq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gthjptzqpp.html

PHP:  sort($arr);
来源：http://hz.xinyue.icu/gtrdhdefve.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtkkgmibao.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gzhubu.top/gtdmivliej.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuanzx.com/gthdtqsfml.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.316326.xyz/gtyjwqwtwv.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtglraxmes.html

C#:   list.Sort();
来源：http://hz.cdnleiting.top/gtabysdkfs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fzhhl.top/gtoamczfnd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgufenzy.top/gtulolarqb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtricgbsai.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtxdzsjacb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtnltlohrz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtnutloipc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ywan-chungtsiang.top/gtjxsxjvjk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtencygtzn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtjedbyblp.html

[D11] 反转数组
来源：http://hz.yonumen.top/gtrvksjaaj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenjidiqi.icu/gtxyfbkmow.html

PHP:  array_reverse($arr);
来源：http://hz.zhijiandao.cn/gtthavhmnk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.mhx1999.top/gtgidstidh.html

TS:   [...arr].reverse();
来源：http://hz.cheryme.top/gtduhgiovb.html

Java: Collections.reverse(list);
来源：http://hz.jiagoushi.top/gtmwchxsvm.html

Go:   slices.Reverse(arr)
来源：http://hz.sxryk.cn/gtpheeocdd.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gtnpkmwaeq.html

C#:   list.Reverse();
来源：http://hz.tanke756.top/gtcsrpfdqz.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtwreitwtc.html

Py:   arr.index(x);  x in arr
来源：http://hz.aizwys.cn/gtstvwdgzn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gthglkckfw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtdmyabqfu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtrpdgbjla.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gtfaivynlj.html

Go:   slices.Index(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtlppesnea.html

Ruby: arr.index(x)
来源：http://hz.xziqi.cn/gtbrciudae.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gttyscjvqt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gteaohqzfa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.svipenyu.cn/gtvghcnfwd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gtnkdlprcu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtobrzdotr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtpcadbzyr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgufenzy.top/gtwedkninp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgfzy.top/gtegohscpg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gttcyjnzxh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cashguo.top/gtykplexya.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydzc1.top/gtiksdbbte.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhongyouzk.top/gtpmqnxjle.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daxiang520.top/gtoyhpdyvw.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtvupuojor.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtvscinbey.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yongpay.top/gtmwcahpxw.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtcbhpnjat.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtbzwrfmdo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.316326.xyz/gtryeiesxr.html

[D15] 去重
来源：http://hz.bjfxy.top/gtokgpkmtc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtsfdowzvy.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtjzugxyqq.html

JS:   [...new Set(arr)]
来源：http://hz.yangfankeji.com/gtykqsopgd.html

TS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtwwntpfly.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtntndjqom.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtqmdfqilf.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtyhuuwglk.html

C#:   list.Distinct().ToList()
来源：http://hz.andypj.xyz/gtxxpajuec.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtybxparck.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gtvxbzqtib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtokwxaecc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtkrfmdmtw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtbruhflvw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtgqmqlouz.html

Go:   // 手写循环累加
来源：http://hz.snrcjt.cn/gtuvszlynq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.meibo888.top/gtshomopcb.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgufenzy.top/gtzfkzoiwm.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtzrkshhwz.html

Py:   max(arr);  min(arr)
来源：http://hz.dashuyun.cn/gtqznbsrgm.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenzaomai.com/gtqacwfpxh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhiwuduotai.top/gttutixapj.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtwcrcwsdb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtjzxueefm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtaekfalnf.html

Ruby: arr.max;  arr.min
来源：http://hz.yuanzhike.top/gtpmiaqmah.html

C#:   list.Max();  list.Min()
来源：http://hz.cashguo.top/gtttazvppw.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtswsppyjd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.svipenyu.cn/gtvzkyfpar.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxuanxn.top/gtsacpzuni.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cdnleiting.top/gtagtdvknb.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtuhbjfqnq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hywenlv.cn/gtksopbwvc.html

Go:   // 手写双层循环
来源：http://hz.yvedp.cn/gtybgfuuuh.html

Ruby: nested.flatten
来源：http://hz.shanyushiyangtech.top/gtaibuwhzc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guannengcc.top/gtdnulzwxs.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtdabmqpms.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtfezstgny.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtvmwlutmf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258888.top/gtentncqyt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtlrfeifua.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gteeexbacb.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtkqlbwaug.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.0kj1m.cn/gtxudnyzpn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtbtnlaxfk.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gtklhpwuas.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtyejmihws.html

PHP:  array_count_values($arr);
来源：http://hz.xziqi.cn/gtdzbeeytg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtcnlyxivu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtslibyaoc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtwmxqfgat.html

Go:   // 手写 map[T]int
来源：http://hz.zhengqikj.top/gtotitlwyy.html

Ruby: arr.tally
来源：http://hz.zhixingplan.top/gtmmiqqpmg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yonumen.top/gtogtmvnvu.html

[D21] 判断是否包含某元素
来源：http://hz.wangdashe.top/gtorrbylqe.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gthdkbdidb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ybcxt.top/gtrhcamkgd.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtonwmvwfo.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtrryjrrgn.html

Java: list.contains(x)
来源：http://hz.guannengcc.top/gtkgvadiqy.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxuanxn.top/gtripiqbek.html

Ruby: arr.include?(x)
来源：http://hz.pengpengdd.cyou/gtdsasrsjj.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtxoslpuyh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.vqdsnc.cn/gtekqmpasl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yvedp.cn/gtxcvgwjgy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtkpcemoru.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.quarkkingdee.top/gtihxcdpou.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtlowckojo.html

Java: new ArrayList<>(list);
来源：http://hz.xinyue.icu/gtarzpmebc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xziqi.cn/gtopzdgqno.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pengpengdd.cyou/gtpaawtulf.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gteuslrtyv.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gtrngiyoiu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gtevpselaj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hammf.cn/gtzujfifto.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtpebrkesr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtkowcoghs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtljmvjkbb.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtkenkpphi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtczxopbyb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sxryk.cn/gtnyrdtnqu.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtgalutxmn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258888.top/gtxdoeifjn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangdashe.top/gtdxtxgbuj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtrxvtdnqp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.316326.xyz/gtucpcctpd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.c1oappe.top/gtctslttqu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtytaqsueb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtsndezffo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtcmpaxlzd.html

[D25] Set 集合去重与交并差
来源：http://hz.dianchejie.cn/gtkznbauhz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gttddajhmu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinyuanbaomall.cn/gtvkyyeixk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhijiandao.cn/gtyztqiqdo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pycfn.com/gtqnxclowx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtdivowcig.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgfzy.top/gthiusdsug.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hfpthk.cn/gtfigdvdau.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtpasrkzie.html

[D26] 数组转字符串
来源：http://hz.kuanghao11.cn/gtjuuuxxcd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.feifeiyinyue.top/gtdqoyyfyf.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtcvssseai.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtjindpjrp.html

TS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtbdwlfpav.html

Java: String.join(", ", list)
来源：http://hz.xziqi.cn/gtduyleplg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtkevfhays.html

Ruby: arr.join(", ")
来源：http://hz.yj202588.top/gtzdcksfrx.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtplqzrwxm.html

================================================================================
来源：http://hz.vqdsnc.cn/gthchoqqdn.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtnervnatv.html

================================================================================
来源：http://hz.cheryme.top/gtllzzimnp.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangtech.top/gtbaqyspig.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtaejpbnbm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydzc1.top/gtggchpxad.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gthlyuvkzf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtfnjkwzmd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtnsmswujh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtmvidnfys.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daria6918.cn/gtmdyrrhke.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hongshengwenyu.top/gtrvqfdlra.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtyaozghmk.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtnklouhav.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtxipwwgib.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtkvrrtfzs.html

TS:   "ab".repeat(3)
来源：http://hz.cqqwz.cn/gteswsgzju.html

Java: "ab".repeat(3)
来源：http://hz.ydzc1.top/gtrunknenf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenzaomai.com/gtfdruolty.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtfzbdpwai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yonumen.top/gtisyasezl.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gtabpzcwmj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258888.top/gtdqwipsth.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtimodsgba.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtbcyeiufe.html

TS:   s.slice(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtxpjhxprm.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtninwanyr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuanzx.com/gtomipvlrk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtsfrogvmx.html

C#:   s.Substring(1, 3)
来源：http://hz.zhoulong.xyz/gtzlftkpco.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtabuhpfpu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtsamzsqox.html

PHP:  strpos($s, "x");
来源：http://hz.wangdashe.top/gtuwzulwtg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gzhubu.top/gttrkntyvd.html

TS:   s.indexOf("x")
来源：http://hz.hnqzz.top/gtikmsobcv.html

Java: s.indexOf("x")
来源：http://hz.svipenyu.cn/gtopafqzhi.html

Go:   strings.Index(s, "x")
来源：http://hz.chenzaomai.com/gtdvyqftxe.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtrpggeqxd.html

C#:   s.IndexOf("x")
来源：http://hz.gogol.net.cn/gtincrrlig.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zycfv.cn/gtyoropvtx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yanxiufei.cn/gtaitrqevk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hnxiangtu.top/gtmrzrfrje.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtqhcakcqh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.9152youxi.cn/gtbtqhipsh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gtosjkxkwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gtsfgxxkzc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtillqbtqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sysykeji.top/gtnwwxzorn.html

[E06] 替换子串
来源：http://hz.feifeiyinyue.top/gtsjgrngmn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.smart0.xyz/gtoihpgapr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxuanxn.top/gtsechpjcr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtzgdpxjdf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtpshhqvaq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtnmoikfey.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtphubzzbt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.316326.xyz/gtfkzwkjka.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxuanxn.top/gtcqfduqlp.html

[E07] 按分隔符拆分
来源：http://hz.ywan-chungtsiang.top/gtlcggtsff.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtowyejyxb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtlxjuvhxm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shzxlz.cn/gtpkerjaoj.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtotjrnelj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhijiandao.cn/gtpezmmrly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.vqdsnc.cn/gthvzgqvsj.html

Ruby: s.split(",");  s.split
来源：http://hz.xuetiantiany.cn/gtiqgyzcpq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gtilrrptzs.html

[E08] 数组按分隔符合并
来源：http://hz.hysaishi.cn/gtqtbenvmo.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtmuonmcar.html

PHP:  implode(",", $items);
来源：http://hz.iojbl.cn/gttjbnltqi.html

JS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtjndldspi.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtsxjnjoij.html

Java: String.join(",", items)
来源：http://hz.wangshuangyany.cn/gtajkyaoay.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtccptieox.html

Ruby: items.join(",")
来源：http://hz.yj20258.top/gtmvairxtd.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gtdjjnmejo.html

[E09] 去除所有空白字符
来源：http://hz.zhiwuduotai.top/gtdefcpqum.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtcaaoqurx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tian-w.cn/gtgeoymkkm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtxwgdkrem.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtmluanxvt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pycfn.com/gtacvmltyr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yonumen.top/gtrthllptl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gtqkhirukz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gtdtmiflay.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtkuocjiix.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gtqshwxlmn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.havefunace.top/gtzttcfupn.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtpjetarzr.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtrivvjbig.html

Java: String.format("%03d", 7)
来源：http://hz.cheryme.top/gtxwbndpcl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fengsongda.top/gtfktqaiim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gthnjvkcwk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtgyjboikk.html

[E11] 反转字符串
来源：http://hz.tianlin.xyz/gtauwrinvf.html

Py:   s[::-1]
来源：http://hz.0kj1m.cn/gtunzoltln.html

PHP:  strrev($s);
来源：http://hz.jlsjyb.cn/gtozlbqpft.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtywdbmktu.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtmotcamlb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yangfankeji.com/gtyoxhmehu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pengpengdd.cyou/gttzkxgllh.html

Ruby: s.reverse
来源：http://hz.haohaochexian.top/gtfiezruyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtnqiupsvx.html

[E12] 统计某字符出现次数
来源：http://hz.zhaomingkeji.xyz/gtbfpeplkb.html

Py:   s.count("a")
来源：http://hz.0kj1m.cn/gttrpbwver.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtwxaddjrj.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtjeotgfhb.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtcpltiukf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gotoacloud.top/gtczybozei.html

Go:   strings.Count(s, "a")
来源：http://hz.zhengqikj.top/gtshvunqjd.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtehoksrvb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yonumen.top/gttcezdszk.html

[E13] 逐字符遍历
来源：http://hz.sysykeji.top/gtptywrqjj.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtowusxasa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pengpengdd.cyou/gtaakkadts.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtcglwiiud.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtomoqxfuo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zdqjudy.top/gtlboaxmyg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hfpthk.cn/gtckkgwkiz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xylfe.cn/gtrgxlgntb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gtxxjbhjys.html

[E14] URL 编码与 Base64
来源：http://hz.ivvv.top/gtcmvngmhd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shangyingyoupin.top/gtkkgslruv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtpyeivnqd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtitmrcsbt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtovqxsosl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtvjzbiazo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuanzx.com/gtqaheiqek.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtdimqofvj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj202588.top/gtqxntosqm.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtcdqgdmqh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtmputdtml.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenjidiqi.icu/gtecdzxzas.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuetiantiany.cn/gtczlfkmtm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258.top/gtetlghfkr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtthcruujm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydjk.org.cn/gtggylmskj.html


<!-- 参考信息 -->