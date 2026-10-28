代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtpsexqgdx.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtadnksoxm.html

C#:   list.Sort();
来源：http://hz.andypj.xyz/gtpjdunvux.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daxiang520.top/gtyzvhsbed.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxinkj.top/gtusqkifzm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtjzgtnvto.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtsmpvjvgc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gtxdnildfq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gterezlajh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuanzx.com/gtibqefvwi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtgbxokknu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtfsbvcpcy.html

[D11] 反转数组
来源：http://hz.xziqi.cn/gtexzadnze.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xuanzx.com/gtyfaxncjt.html

PHP:  array_reverse($arr);
来源：http://hz.yangfankeji.com/gtrkucyvft.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.kuanghao11.cn/gtrwhqxgtz.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtgpxxwgnx.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtacheyewf.html

Go:   slices.Reverse(arr)
来源：http://hz.tanke756.top/gthrwqdetw.html

Ruby: arr.reverse
来源：http://hz.yuanzhike.top/gtfqlqzgir.html

C#:   list.Reverse();
来源：http://hz.dianchejie.cn/gtugkyqpww.html

[D12] 查找元素下标
来源：http://hz.nwbrower.top/gtgabolejm.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtpieiggxg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtinsqoeny.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtosgwzbnl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gtonoybabt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.c1oappe.top/gtyjcubkuh.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtuavifsko.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtiitikxvz.html

C#:   list.IndexOf(x);
来源：http://hz.shzxlz.cn/gtpmzaochs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtikhvlmgs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shuidangran.top/gtlurftkww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.snrcjt.cn/gtsmwtphja.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtmafxffle.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtfkjkggsy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yvedp.cn/gtbjstcawv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ybcxt.top/gtsqxjxwue.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtngrpmkjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuxming.cn/gtdvdlbgxn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangdashe.top/gtdlfrmvsx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtqtgpfjmc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuanzx.com/gtqekxuizh.html

JS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtfysdkfaa.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtertalfor.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gtmjrzqtzz.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtnoxsbxks.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gtxucyrbro.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cqqwz.cn/gtsmgpyjok.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtevfougnk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtplpabiyy.html

PHP:  array_unique($arr);
来源：http://hz.chenjidiqi.icu/gtstvnastx.html

JS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtntxcaulf.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtecnqnjwy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgufenzy.top/gtswnphfxo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtscvvjyor.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtcpbhzwli.html

C#:   list.Distinct().ToList()
来源：http://hz.pengpengdd.cyou/gtlbtwptsv.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtssilepat.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gtdsflulcj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtdobzazee.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gttbdnwqwd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtsihfjcgl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtmnpyjqxw.html

Go:   // 手写循环累加
来源：http://hz.ywan-chungtsiang.top/gtjfonxpqp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shanyushiyangkeji.top/gtjbhoiudm.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gtqqqvdyhi.html

[D17] 最大值与最小值
来源：http://hz.gotoacloud.top/gtkxhlbihy.html

Py:   max(arr);  min(arr)
来源：http://hz.yuanzhike.top/gtnkqaydue.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gtdzndkmpe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtyngxivir.html

TS:   Math.max(...arr);
来源：http://hz.yj202588.top/gtlevazkmg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hysaishi.cn/gtdvpcqotu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gtesjpakbo.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtarejybui.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtwcsgyxek.html

[D18] 扁平化嵌套数组
来源：http://hz.shangyingyoupin.top/gtjjlrziba.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daxiang520.top/gtgdeohakr.html

PHP:  array_merge(...$nested);
来源：http://hz.aibaodan.cn/gtzlvtnoxv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gttkbiwifr.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtgiuvptwt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hammf.cn/gtwqfmuovy.html

Go:   // 手写双层循环
来源：http://hz.yonumen.top/gtrkwwcruk.html

Ruby: nested.flatten
来源：http://hz.feifeiyinyue.top/gtafpkhmyh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258.top/gtqyxmfmkz.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtwhukwggw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtutjduplw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtcfnwnctx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xziqi.cn/gtmjpnlztp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xylfe.cn/gtzidvgqxm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gogol.net.cn/gtjcroeddr.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangkeji.top/gtrexmupar.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dashuyun.cn/gtotrldoxz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jiagoushi.top/gtqawgoqsq.html

[D20] 统计每个元素出现次数
来源：http://hz.hammf.cn/gtbrryrpbk.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtvyhwkzzl.html

PHP:  array_count_values($arr);
来源：http://hz.shangyingyoupin.top/gtomqyndrz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtgjscixrd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtxygbcswe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtifqxphxv.html

Go:   // 手写 map[T]int
来源：http://hz.zhaomingkeji.xyz/gthketxscs.html

Ruby: arr.tally
来源：http://hz.zhongyouzk.top/gtvraojgkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daria6918.cn/gtpqguuxpt.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtzwexuedi.html

Py:   x in arr
来源：http://hz.cqqwz.cn/gtnzrqmkjb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.smart0.xyz/gtvdqvrtse.html

JS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtfhwguigi.html

TS:   arr.includes(x)
来源：http://hz.sxryk.cn/gtmpugcqgp.html

Java: list.contains(x)
来源：http://hz.xziqi.cn/gtinebeyrq.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangshuangyany.cn/gtojcrtmjj.html

Ruby: arr.include?(x)
来源：http://hz.xuetiantiany.cn/gtyilsbnlp.html

C#:   list.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtscgefbja.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xingfuxueyuan.xyz/gtvvdmlmrc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj202588.top/gtxlrrpnzx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.pengpengdd.cyou/gtmjvzwnnu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shangyingyoupin.top/gtefmfxouh.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gthtsghvkr.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtmybjpbsn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xinyue.icu/gtyubzarkg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtqhkwcwci.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtaosdbbhu.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gtnvunqxzt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gogol.net.cn/gtqvprcgwr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ehwqpu.com/gtaxrkhmuy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtoadxrczp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtlxgdbjfh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtwtglxnzy.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtfveacmor.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jiagoushi.top/gtsumlrzod.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtfrkeeoow.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtbvspauxd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gttbhqaeon.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gthpybmeeg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtpakjeuhi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gotoacloud.top/gtnzrdpkzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj202588.top/gtykvujhui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhiwuduotai.top/gtnhufiufi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gaohongyu789.top/gthbzdczkl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtgxvmxvgu.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtnglaiaam.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtitntvazx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtzdxfcrdq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hammf.cn/gtlqwujolr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.quarkkingdee.top/gtinpagwox.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj202588.top/gtzcqndcir.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.meibo888.top/gtkihlvaiy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.kuanghao11.cn/gthyanecnh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtotzqhpvo.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtjgzntyzu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuetiantiany.cn/gtmoxpgkga.html

PHP:  implode(", ", $arr);
来源：http://hz.kuanghao11.cn/gtcyjtyhsm.html

JS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtjxhiplrh.html

TS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtwcvsrmie.html

Java: String.join(", ", list)
来源：http://hz.kuanghao11.cn/gtdkfjjtpf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtccqqskmb.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtxjtywjak.html

C#:   string.Join(", ", list)
来源：http://hz.smart0.xyz/gtgzkedgcs.html

================================================================================
来源：http://hz.nwbrower.top/gtgmkggubf.html

E. 字符串处理
来源：http://hz.ivvv.top/gtgnogkwjs.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkffbctra.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtzilohzjb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yanxiufei.cn/gtsclnuuvk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydzc1.top/gtzmxoglju.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtdlssbcai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtptafziwi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gtqshjisnn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtdiqoxust.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gthvhnusrz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gthajrhejd.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gtwfjrfwel.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gtgjxdrats.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gtyttrkqpr.html

JS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtogiqezdj.html

TS:   "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtbinimusv.html

Java: "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtzptzefrb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cashguo.top/gtdttscuyj.html

Ruby: "ab" * 3
来源：http://hz.iojbl.cn/gtxwqichau.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gteehnltvu.html

[E03] 截取子串
来源：http://hz.jiagoushi.top/gtiugrbite.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhongyouzk.top/gtuprfxhxm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtroylkgbg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtznnekkvf.html

TS:   s.slice(1, 4)
来源：http://hz.gogol.net.cn/gtsahkuqul.html

Java: s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtysawkhhe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yvedp.cn/gtlsxhdsps.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj202588.top/gtyyeggxzi.html

C#:   s.Substring(1, 3)
来源：http://hz.chenlongwang.top/gtkiissgef.html

[E04] 查找子串位置
来源：http://hz.jinqigfzy.top/gtakozgbnn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.316326.xyz/gtfqlczvil.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtdeisfkux.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.52xcode.cn/gtvrpjvubm.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtzonxhrnh.html

Java: s.indexOf("x")
来源：http://hz.jinghuilouyu.cn/gtnqhfzldr.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gtkvljsjlq.html

Ruby: s.index("x")
来源：http://hz.52xcode.cn/gtoutqaofg.html

C#:   s.IndexOf("x")
来源：http://hz.quarkkingdee.top/gtzagzkwux.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gtrlgkbwlz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jiagoushi.top/gtixxhftax.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgufenzy.top/gtnwrxkvjv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gthwvhhggk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtaiestyze.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtewtnfcxm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtdtpwaudl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gthupjqrnn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgfzy.top/gtrdnzaeix.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtwpfktivz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtvulceztb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigufen.top/gtmtuqdcte.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtlpnjowrc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtyjcpaqkx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtrmisdznu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nwbrower.top/gteskenejd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.feifeiyinyue.top/gtuwhnqmyf.html

C#:   s.Replace("a", "b")
来源：http://hz.ybcxt.top/gtricqmsds.html

[E07] 按分隔符拆分
来源：http://hz.redwolf501.top/gttzpnphbi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtfijudqzo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.vqdsnc.cn/gtrqxdbmxl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuxming.cn/gtbegkkuam.html

TS:   s.split(",")
来源：http://hz.snrcjt.cn/gtxdywuojb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gtbmbgqikb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nwbrower.top/gtwjffbpaz.html

Ruby: s.split(",");  s.split
来源：http://hz.sweek.top/gtpiixewmz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tianlin.xyz/gtvqnawjcq.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtiyvdfvcd.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtkmgwghqk.html

PHP:  implode(",", $items);
来源：http://hz.ppjwa.cn/gtpuikphwo.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtcjlejdca.html

TS:   items.join(",")
来源：http://hz.shzxlz.cn/gtwdcpnvbt.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtahnptzxb.html

Go:   strings.Join(items, ",")
来源：http://hz.zhoulong.xyz/gtqfqckvsz.html

Ruby: items.join(",")
来源：http://hz.jinghuilouyu.cn/gthcgtqfxa.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtekqifyzf.html

[E09] 去除所有空白字符
来源：http://hz.yvedp.cn/gtmxojjotx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtyjgkzeuu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtxqqxcorr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gthmcskdpk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtklrhmfsy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hywenlv.cn/gtpgltlqbq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtyxnixziv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangdashe.top/gtgptnxdok.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnxiangtu.top/gtodofeico.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgfzy.top/gtsczsblbe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yanxiufei.cn/gtjvsnqenn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.birdmap.top/gtuqnhdrey.html

JS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtmcnjifyl.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtpbaqubhl.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigufen.top/gtbidkjbnm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtiazlwcsi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtvfqujheh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtdemislwj.html

[E11] 反转字符串
来源：http://hz.daxiang520.top/gtwxgzqdaf.html

Py:   s[::-1]
来源：http://hz.jinqigfzy.top/gtmdkxlxhm.html

PHP:  strrev($s);
来源：http://hz.jqgfzy.top/gtqeqstfyn.html

JS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtckjnoyhq.html

TS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtlmnlvqwm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.snrcjt.cn/gtxnhsfoup.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cashguo.top/gteowywvvy.html

Ruby: s.reverse
来源：http://hz.jqgfzy.top/gtolyxxwyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtfqrizyub.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtcvpfkxaj.html

Py:   s.count("a")
来源：http://hz.jinqigufen.top/gtftkajjfu.html

PHP:  substr_count($s, "a");
来源：http://hz.shuidangran.top/gtdsjtmrih.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gthnsegozt.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtljazywes.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtekhwjjku.html

Go:   strings.Count(s, "a")
来源：http://hz.andypj.xyz/gtgkieuyzf.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtatqrmcaa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yongpay.top/gtkbjzfuwt.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtatrixqfa.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtarfkjqiq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shzxlz.cn/gtuecnenjf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtwrjibxpy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gturqmebic.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtkyppnhzy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.havefunace.top/gttbtnnaar.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cucudq.cn/gtfhutchvn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtwmnofdco.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gtytxiicxq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtzawbexgw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtewwxljpg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ybcxt.top/gtvmkjrlfy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.meibo888.top/gtcklojbiq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnxiangtu.top/gtiandlfii.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtkwmqwiya.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gtwnwkrqfy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.quarkkingdee.top/gtqwthmviw.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhengqikj.top/gtcckshxis.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xinyue.icu/gtdpjwhtbo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ybcxt.top/gtlapcmwcd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtjzvuquqj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinghuilouyu.cn/gtqmfnhsfi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gtnjukexso.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtutkltytk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.quarkkingdee.top/gtewtppxql.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daria6918.cn/gtmcscvptc.html

[E16] 数字千分位
来源：http://hz.yj20258.top/gtauubhyxx.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gtegylrvhr.html

PHP:  number_format(1234567);
来源：http://hz.zhongyouzk.top/gtknivlkjs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gttthdgvre.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtlsdyazjm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuxming.cn/gtxmgojzga.html


<!-- 参考信息 -->