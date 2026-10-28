代发 wailian999

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtsovmqtol.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gtlmcqezfm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.snrcjt.cn/gtplsrlcdd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zycfv.cn/gtpaamcvyr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj202588.top/gtspbdvzzb.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtpipjdrzw.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gthzoxnuzn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gtupbzwatn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gtxzooclmk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtugycotnj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtjynlsvfw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtfxxowubs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zdqjudy.top/gtqvqjcbnz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtumkeagai.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtlrsvycgq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtjrqpspdv.html

[D11] 反转数组
来源：http://hz.yonumen.top/gtxycvyqzl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hammf.cn/gtmnkjpgoq.html

PHP:  array_reverse($arr);
来源：http://hz.xuanzx.com/gtashnwlij.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtisdzqpny.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtxfhguvet.html

Java: Collections.reverse(list);
来源：http://hz.xingfuxueyuan.xyz/gtypsewdrs.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtkpnjwapl.html

Ruby: arr.reverse
来源：http://hz.dashuyun.cn/gtusgdeqpq.html

C#:   list.Reverse();
来源：http://hz.tanke756.top/gtcsipywku.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtheqtfwwi.html

Py:   arr.index(x);  x in arr
来源：http://hz.ybcxt.top/gtpoqfzudo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtowqylxur.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtceboyeuk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtgyecglgl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jianghu66.top/gttvdtxgve.html

Go:   slices.Index(arr, x)
来源：http://hz.dashuyun.cn/gtwmflurlk.html

Ruby: arr.index(x)
来源：http://hz.yonumen.top/gtchlzomgc.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gtycycghwz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shanyushiyangtech.top/gttoogilxu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtlxxrssia.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.316326.xyz/gtabzjactz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtljqaqwjr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtkxnmfrbf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtojaunota.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuetiantiany.cn/gtmembfpmm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtppmoeqxq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.iojbl.cn/gtzerlillj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sweek.top/gtiqsfaqyq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guannengcc.top/gtjjilqzro.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtrhxuqwoy.html

JS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtzaylhjny.html

TS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtbmyhgufh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.52xcode.cn/gtvpifspie.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtybmnvkeo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtkkgsbtty.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jiagoushi.top/gtyjvzmgyg.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtcjsnmirm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtxbmvphuy.html

PHP:  array_unique($arr);
来源：http://hz.ydzc1.top/gtmaysnisb.html

JS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtfvjreytz.html

TS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtratmvwrt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hysaishi.cn/gtfbaglrdu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtkavxdqis.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gthjkjyjnn.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtbbgayfea.html

[D16] 求和与平均值
来源：http://hz.ywan-chungtsiang.top/gtvzdsqtyq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.9152youxi.cn/gtrurcdkmz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtgbiqhucx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtkkaijrii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtzbbegacz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gtoyxssfiq.html

Go:   // 手写循环累加
来源：http://hz.chenzaomai.com/gtdoqgbipi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtqmaptzps.html

C#:   list.Sum();  list.Average()
来源：http://hz.bjfxy.top/gtumkeisdl.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtavncrxir.html

Py:   max(arr);  min(arr)
来源：http://hz.chenlongwang.top/gtrlocqryv.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangdashe.top/gtrzwrgwqh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cqqwz.cn/gtaohveeju.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtjeibcglj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.kuanghao11.cn/gttcpgwtbr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtpbeapmha.html

Ruby: arr.max;  arr.min
来源：http://hz.0kj1m.cn/gtzpfieixy.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtsbrqplyf.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtqporggwp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yangfankeji.com/gtjgcslfyr.html

PHP:  array_merge(...$nested);
来源：http://hz.zhijiandao.cn/gtzjqewprv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nanxuanxn.top/gtnpwvodht.html

TS:   nested.flat();
来源：http://hz.cashguo.top/gthghdjnfd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258888.top/gtxdioqrbj.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gtdrwzbqsi.html

Ruby: nested.flatten
来源：http://hz.daria6918.cn/gtgihmsrwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gtrclyjdza.html

[D19] 按字段分组
来源：http://hz.tian-w.cn/gtjbsriqjp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gtvvpxkatq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnqzz.top/gtzxvjeuyr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtafuuanxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtvflwwrqb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtioaqobke.html

Go:   // 手写 map[string][]T
来源：http://hz.cashguo.top/gtsrzgitsu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.redwolf501.top/gtlioryldf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cheryme.top/gtrhwdcyrs.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtatrbdwsb.html

Py:   Counter(arr)
来源：http://hz.xuanzx.com/gtssveusdn.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigfzy.top/gtdmygmnzm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtcsekuvoa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtraqgzwew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydjk.org.cn/gtguzbebiy.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gtpzamllic.html

Ruby: arr.tally
来源：http://hz.wangdashe.top/gtkgewgusx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtkyivtknr.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtwgxbtdee.html

Py:   x in arr
来源：http://hz.yuxming.cn/gtmjnjilfb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuxming.cn/gtejnxzcji.html

JS:   arr.includes(x)
来源：http://hz.hfpthk.cn/gtruugphvv.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtljftsgrr.html

Java: list.contains(x)
来源：http://hz.0kj1m.cn/gtnguahpfx.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtunssijbu.html

Ruby: arr.include?(x)
来源：http://hz.andypj.xyz/gtrlfkqcfm.html

C#:   list.Contains(x)
来源：http://hz.zhoulong.xyz/gtsgwhzunv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtcxfhelkc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtjpyaeeag.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtzmrejsjr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gtggodmotb.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gttfmqzkro.html

Java: new ArrayList<>(list);
来源：http://hz.ywan-chungtsiang.top/gtwmahfjez.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ppjwa.cn/gttiqqqlue.html

Ruby: arr.dup;  arr.clone
来源：http://hz.kuanghao11.cn/gtkvzglhge.html

C#:   new List<int>(list);
来源：http://hz.ivvv.top/gtanbxavlq.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangtech.top/gtrwcqoebx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aizwys.cn/gtmjjscdtp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gtjswhvdwo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtkdroexgi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtyagtxbuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtezesdute.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtprceoinn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jianghu66.top/gtdpbxkexb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tian-w.cn/gtnmyrmbvi.html

[D24] 字典 / Map 基本操作
来源：http://hz.yvedp.cn/gtkijcpyds.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gtokfvalwl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtothumhfm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xuanzx.com/gtchyjeltk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.smart0.xyz/gtmnhdjkgl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj202588.top/gtavnrrorb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtmwobuvdc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtbeyxnbup.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtaftvdalw.html

[D25] Set 集合去重与交并差
来源：http://hz.ppjwa.cn/gtpwetgyri.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.fzhhl.top/gtopzutzbl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ivvv.top/gtcuwjgptz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.52xcode.cn/gtcjsmmimj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenzaomai.com/gtaswzxacr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gtlcfnumbd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtegqduuek.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtznpqenjs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.9152youxi.cn/gtvklzfokb.html

[D26] 数组转字符串
来源：http://hz.yvedp.cn/gtpbjppgao.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ivvv.top/gtxhpqpvlv.html

PHP:  implode(", ", $arr);
来源：http://hz.nwbrower.top/gtnqoxzngo.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtfbhhqsyq.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gteuuvnumo.html

Java: String.join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtllwgdhqi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jyoumei.cn/gtejwlfeyh.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtwazwqrzq.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtvqlpseiw.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbuniafvl.html

E. 字符串处理
来源：http://hz.nwbrower.top/gtdwfgrilj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gteiobwsyr.html

[E01] 拼接字符串
来源：http://hz.sxryk.cn/gtukkyzmvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sweek.top/gtiieisljv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gthtdihrgs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtpxapxiol.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtmckwveng.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuanzhike.top/gtdcdqvyqi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigufen.top/gtfgdkzyle.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ivvv.top/gtvhutqkma.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtavkxgfoo.html

[E02] 重复字符串
来源：http://hz.kuanghao11.cn/gtqcfbyuao.html

Py:   "ab" * 3
来源：http://hz.jqgfzy.top/gtmrpmtcwb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.snrcjt.cn/gtldpvmumw.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtljyvjmvb.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtxqdvphex.html

Java: "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtvmivdddc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.snrcjt.cn/gtvjhxxwdz.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gtapzefxqp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtmcqibdjd.html

[E03] 截取子串
来源：http://hz.dashuyun.cn/gtfaalexng.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.smart0.xyz/gtojrfkyhd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhixingplan.top/gthbevcsvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtkjfahobq.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtpayuenar.html

Java: s.substring(1, 4)
来源：http://hz.iojbl.cn/gtlmsbgpbe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydzc1.top/gtqcqxskgq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangdashe.top/gtelwuraec.html

C#:   s.Substring(1, 3)
来源：http://hz.zhengqikj.top/gtuicpjcwp.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gttdotlaon.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtjussloag.html

PHP:  strpos($s, "x");
来源：http://hz.haohaochexian.top/gthxswajbt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtqwsixjka.html

TS:   s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtwcsrnirt.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtgdiuclju.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtzfdxrguk.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtqfqfbltw.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtqwwmfuaw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtipyegjki.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pycfn.com/gtrrdikmor.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtsjslaboc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtaydphxee.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnqzz.top/gtadbwffth.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gttqozxuzd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtzexpjbxj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtauvzlnuu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtiaclkstg.html

[E06] 替换子串
来源：http://hz.zhongyouzk.top/gtidolinzm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tanke756.top/gtxtprznyf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gthhvcvcva.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtvwfkqthk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtiigakqiz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtikzgwwcz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daxiang520.top/gtfnabincz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.birdmap.top/gtwhqazofd.html

C#:   s.Replace("a", "b")
来源：http://hz.sxryk.cn/gttungradm.html

[E07] 按分隔符拆分
来源：http://hz.jianghu66.top/gtiiuecdpz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gogol.net.cn/gtzrcnaspa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hywenlv.cn/gtusfzufzk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtqcziuqfp.html

TS:   s.split(",")
来源：http://hz.zhijiandao.cn/gtvrzqwarl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gttwmtsgrz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinghuilouyu.cn/gtubmdsswa.html

Ruby: s.split(",");  s.split
来源：http://hz.zhoulong.xyz/gtjwrsrpip.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.svipenyu.cn/gtogxbihsg.html

[E08] 数组按分隔符合并
来源：http://hz.cdnleiting.top/gtafdtystf.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtdwikrqze.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtfsnvtfnk.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtjaqqbqca.html

TS:   items.join(",")
来源：http://hz.52xcode.cn/gtevtbdjqu.html

Java: String.join(",", items)
来源：http://hz.snrcjt.cn/gtwkcaoznr.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtzjhqtcbq.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtqmkrmgec.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gtdzfsmnwj.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtbxxedfpc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhixingplan.top/gtykokmnmv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gttnwsqmfx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtusrjitth.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gttgngpkto.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zdqjudy.top/gtqsvmlowz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dashuyun.cn/gtbimcyvib.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtrhfpoieu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtzitkdrec.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtmxgszoin.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gogol.net.cn/gtkzyuakee.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtexasiyvp.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtqmqednhs.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtcasgekkv.html

Java: String.format("%03d", 7)
来源：http://hz.gogol.net.cn/gtyrcmprki.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zycfv.cn/gtjdjemaor.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtoqbjnqyo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nwbrower.top/gtzhkjzgwz.html

[E11] 反转字符串
来源：http://hz.zhongyouzk.top/gtxyrincfy.html

Py:   s[::-1]
来源：http://hz.cqqwz.cn/gtcdxcojma.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gtgsmmdwur.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtvmxmclsl.html

TS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtxtrdgavp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gtywxzudzj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtttfgfera.html

Ruby: s.reverse
来源：http://hz.haohaochexian.top/gtaxqauqss.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtpbadvfjj.html

[E12] 统计某字符出现次数
来源：http://hz.sweek.top/gthdllvxhl.html

Py:   s.count("a")
来源：http://hz.ehwqpu.com/gtjfggbntq.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gttxeemsnf.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtnqcwvhwq.html

TS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtzddwzotg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtgnxrqvrs.html

Go:   strings.Count(s, "a")
来源：http://hz.cdnleiting.top/gtwxxthecu.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtyqakueiq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtmvsksrcm.html

[E13] 逐字符遍历
来源：http://hz.fengsongda.top/gthmxgqvmu.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtfbcxluvf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.c1oappe.top/gtrxcxivvz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtraelgozx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gthxlrspxc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gtwwfqeroa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yvedp.cn/gtfskxjkro.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtjwzdmilz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtywxnjsah.html

[E14] URL 编码与 Base64
来源：http://hz.hnxiangtu.top/gtsfbnueqo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtiahfpboj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dianchejie.cn/gtghfzmvru.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtzrrsqaww.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ybcxt.top/gtsbwqmvrd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtyevjfdsk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydzc1.top/gtuoqhjfaz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangtech.top/gtxzsejkqc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtntknhmtk.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gtinigkosg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pycfn.com/gtkotayjug.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtyucdhmia.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gteknedlxk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhijiandao.cn/gtjiywbmrk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gthgdjsahq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtdvwrvflj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hammf.cn/gtibdhjlbw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgufenzy.top/gtmurkfmbz.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gtzqulvxbq.html

Py:   f"{1234567:,}"
来源：http://hz.hysaishi.cn/gtleduwoez.html


<!-- 参考信息 -->