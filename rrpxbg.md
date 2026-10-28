代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtikhprvmj.html

Java: list.subList(1, 4);
来源：http://hz.hywenlv.cn/gtgqymxzcm.html

Go:   arr[1:4]
来源：http://hz.jinqigfzy.top/gtrfcapppb.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gtbmmewlye.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gttdepjskg.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gtbbayazif.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtazxprpmv.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtplloiibz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxuanxn.top/gtcuwlidmh.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gthctgpuvu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtexoauawz.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtpfooyfme.html

Ruby: a + b;  a.concat(b)
来源：http://hz.vqdsnc.cn/gtfolomyfw.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtnayfbpvx.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtbqqihwye.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtsjmwhilj.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gturjdfvbh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yanxiufei.cn/gtpkeotpbw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtznknxkne.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtqfluznst.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sweek.top/gtcqixljfx.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtpdyspdbg.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtdvhuzdcb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtyqsxmobc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fzhhl.top/gthzwrzsfl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtrojybfdb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtiizsysku.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtsyxkbusr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daxiang520.top/gttjfvzvwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtuipupgwk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gogol.net.cn/gtpecxmnlb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangshuangyany.cn/gthjejmzlg.html

[D11] 反转数组
来源：http://hz.sweek.top/gtckyibstm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtibgwbkcm.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtrimccfos.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.haohaochexian.top/gtqcfsswdr.html

TS:   [...arr].reverse();
来源：http://hz.xuanzx.com/gtjllkozbi.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtgbvessgz.html

Go:   slices.Reverse(arr)
来源：http://hz.sufxvd.cn/gtyorqjntu.html

Ruby: arr.reverse
来源：http://hz.yvedp.cn/gtrvjohfpn.html

C#:   list.Reverse();
来源：http://hz.aizwys.cn/gtrdusirbc.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gtgmvblgvh.html

Py:   arr.index(x);  x in arr
来源：http://hz.ybcxt.top/gtcmqjpqnl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtebabhqkj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtysxfzxwn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gthxgzyrzz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtwfefmlns.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtmwgculue.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtcawcddaq.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtfwebslyb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ppjwa.cn/gtsdhuezad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daria6918.cn/gtuychdvkf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.havefunace.top/gtvehbqceq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtggcjcgtp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtwybebhaw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ehwqpu.com/gtyqoulair.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cucudq.cn/gtilhivcjn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangdashe.top/gtmqeawepl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuetiantiany.cn/gtklbsqykm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gteceuddmh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258.top/gtkqbdjpiy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gttbbafauz.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtkyjmkuyn.html

TS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtplgupqni.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gtoyaovvrn.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtdvjdqfqq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhiwuduotai.top/gtrxwhaaoq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxinkj.top/gtudvxqazx.html

[D15] 去重
来源：http://hz.cdnleiting.top/gtafhrvxjy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtwnlirovl.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtganecent.html

JS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtymspsdhw.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtcucxeiji.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fengsongda.top/gtkvqttxjb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.smart0.xyz/gtoptwddxd.html

Ruby: arr.uniq
来源：http://hz.9152youxi.cn/gtvurxbcff.html

C#:   list.Distinct().ToList()
来源：http://hz.tian-w.cn/gthmacjfaw.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtibbwyfsk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.havefunace.top/gthlupuiqo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.iojbl.cn/gtkyjjaugx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtwwfdnxku.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtnruhnlcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.fzhhl.top/gtyrtmbyxa.html

Go:   // 手写循环累加
来源：http://hz.ppjwa.cn/gtluawnojo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtavistyws.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtyhntgjvw.html

[D17] 最大值与最小值
来源：http://hz.hongshengwenyu.top/gtrumyihhv.html

Py:   max(arr);  min(arr)
来源：http://hz.gaohongyu789.top/gtdztyjndr.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuanzhike.top/gtlytrcsmf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtcygasnxh.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gtogucbygp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtirrbmkjy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtozyeznqd.html

Ruby: arr.max;  arr.min
来源：http://hz.aizwys.cn/gtqpasumov.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gtsnsasdrs.html

[D18] 扁平化嵌套数组
来源：http://hz.xylfe.cn/gtqywrznwh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuxming.cn/gttpmapani.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgufenzy.top/gtqybktnls.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yueranfly.top/gtrlumkhqd.html

TS:   nested.flat();
来源：http://hz.wangdashe.top/gtihsvfedd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hywenlv.cn/gtyrhoaput.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtfndvcokv.html

Ruby: nested.flatten
来源：http://hz.xylfe.cn/gtjnpeqphj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtpsidtzje.html

[D19] 按字段分组
来源：http://hz.hysaishi.cn/gtuyplakpi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.bjfxy.top/gteckelwyu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.snrcjt.cn/gtsnwzsigk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xinyue.icu/gtdtdafvrw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gteyoskeby.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtbumxzvxc.html

Go:   // 手写 map[string][]T
来源：http://hz.jlsjyb.cn/gtubzbyfoy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gthtumbcjb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtvjbgbmde.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtoysomatt.html

Py:   Counter(arr)
来源：http://hz.xylfe.cn/gtpjycfkvy.html

PHP:  array_count_values($arr);
来源：http://hz.ivvv.top/gtikbnuawn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtrlnqucil.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtosmuzaoh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtbnfombxo.html

Go:   // 手写 map[T]int
来源：http://hz.cheryme.top/gtkwdsquer.html

Ruby: arr.tally
来源：http://hz.shzxlz.cn/gtslfvkzpf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ybcxt.top/gtzepcalon.html

[D21] 判断是否包含某元素
来源：http://hz.tanke756.top/gtszjjhygt.html

Py:   x in arr
来源：http://hz.cucudq.cn/gtnaltwlau.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtjbxrdfkm.html

JS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtjsfyjexg.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gttchyrfbx.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtrgmenasy.html

Go:   slices.Contains(arr, x)
来源：http://hz.shangyingyoupin.top/gtvbzvxhhs.html

Ruby: arr.include?(x)
来源：http://hz.jyoumei.cn/gtvfoclumm.html

C#:   list.Contains(x)
来源：http://hz.yj202588.top/gtgkuvfxft.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuanzhike.top/gtxkbcdsnr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtbqmbjrbc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jyoumei.cn/gtmmobvqbb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yueranfly.top/gtytmsqhug.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtitefvzmo.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtyhjqupbe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.kuanghao11.cn/gtqvnyrehg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtnbfyvkyn.html

C#:   new List<int>(list);
来源：http://hz.hywenlv.cn/gttdvvjazu.html

[D23] reduce 累积计算
来源：http://hz.smart0.xyz/gtiblxlbij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtesappina.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtcmmfvnue.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtrgsjshqb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtlepzajzy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sxryk.cn/gtmlihhsfm.html

Go:   // 手写循环
来源：http://hz.quarkkingdee.top/gtorsfcfoq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtjffgxsll.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jlsjyb.cn/gtciyjpuyp.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnqzz.top/gtoxsoidce.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gzhubu.top/gthdxwyixb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gteietjaby.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.redwolf501.top/gtgsrdpylk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtbuirbdhr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sysykeji.top/gtjkoklixs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinghuilouyu.cn/gtorihgpli.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtxziocogu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtutfvnbjg.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gteelcwqnb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sysykeji.top/gtdvgldvvq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtcdolfzbx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgufenzy.top/gtroxmpgpi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ivvv.top/gtnoswhdsk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xingfuxueyuan.xyz/gtikjkdnzf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shuidangran.top/gtlvpxyegr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtverpqnjr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jiagoushi.top/gtlnicjgti.html

[D26] 数组转字符串
来源：http://hz.nanxinkj.top/gtuvbxgbsy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ivvv.top/gtfyxfnjmy.html

PHP:  implode(", ", $arr);
来源：http://hz.ydzc1.top/gtzbeorgog.html

JS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtzmrqmxdu.html

TS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtdubjttjq.html

Java: String.join(", ", list)
来源：http://hz.jyoumei.cn/gtssfyiyle.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtmlopbomx.html

Ruby: arr.join(", ")
来源：http://hz.cashguo.top/gtqgmvgtca.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtukpwmlmv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtllucymcw.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtdjiwxsnu.html

================================================================================
来源：http://hz.jinqigfzy.top/gtanysifgp.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtvbkqtleo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtbcsnrclp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nwbrower.top/gtulfatsfg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtykpewlkr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtoldolhld.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtfaemaamp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pycfn.com/gtngqpuwbg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhaomingkeji.xyz/gtodjkawmj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtwbrwzetr.html

[E02] 重复字符串
来源：http://hz.yvedp.cn/gtsktracxi.html

Py:   "ab" * 3
来源：http://hz.xinyue.icu/gtikricvdp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258888.top/gtfadwweme.html

JS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gthigrbuib.html

TS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtanxchfkn.html

Java: "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtyxaxisao.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gtlcrafeed.html

Ruby: "ab" * 3
来源：http://hz.shuidangran.top/gtpauwieak.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258888.top/gtdyfmxvrb.html

[E03] 截取子串
来源：http://hz.tanke756.top/gttxfrkzbi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gogol.net.cn/gtonvzupoh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtpaostiys.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xinyue.icu/gttqfekcfh.html

TS:   s.slice(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtlhvhkizi.html

Java: s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtfhexaxbz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zycfv.cn/gtapnugfyz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tian-w.cn/gtufonoksv.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtmbvbfmcx.html

[E04] 查找子串位置
来源：http://hz.zycfv.cn/gtzkrieurd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shuidangran.top/gtlkipxgwb.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gtgsxazbwl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtkmohtddh.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtigwmhbrg.html

Java: s.indexOf("x")
来源：http://hz.yonumen.top/gtkkuhyxuj.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtqgmqaxfz.html

Ruby: s.index("x")
来源：http://hz.cdnleiting.top/gtbunarcmq.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gteicwromu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtjvcngrre.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.bjfxy.top/gtyzfzvvgj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhiwuduotai.top/gtieqetfwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yongpay.top/gtkpkrzauf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gtxsrfvirm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtxjlqyeud.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yangfankeji.com/gttftuoqmx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yangfankeji.com/gtpvwvlqyz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenzaomai.com/gtvunrotjb.html

[E06] 替换子串
来源：http://hz.tanke756.top/gtatoeotya.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.birdmap.top/gtazbsahzn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtyjsaotaf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtfhlgbqop.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtzljqxfmz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtreissptw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtznvvqnjn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gttdvvatwf.html

C#:   s.Replace("a", "b")
来源：http://hz.jlsjyb.cn/gtghnkpnac.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangkeji.top/gtaccyvszb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yangfankeji.com/gtmnzivvph.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gtbzzbaszt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xingfuxueyuan.xyz/gthstwdxfl.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtfbussmqh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtrwqucauq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinghuilouyu.cn/gtmqzwskgp.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gtgqokyhft.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuanzx.com/gtlnwxervk.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtdbxzgplv.html

Py:   ",".join(items)
来源：http://hz.zhengqikj.top/gtpifraoga.html

PHP:  implode(",", $items);
来源：http://hz.vqdsnc.cn/gtdkycruot.html

JS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtyyesygwo.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gtsdeviqyv.html

Java: String.join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtenofwwlx.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigfzy.top/gteszwpipy.html

Ruby: items.join(",")
来源：http://hz.zhijiandao.cn/gtmfzxbhey.html

C#:   string.Join(",", items)
来源：http://hz.nanxuanxn.top/gtohnzxpxh.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtiixfobcf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sxryk.cn/gtcccbsaib.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtptelkcxm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtohnjyxln.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtboiyxtnz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258.top/gtvgbduapu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gtfsvenptl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gaohongyu789.top/gtfffrvfmc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gtbbmzarrg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tian-w.cn/gtczggstkc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtkvgjpfxe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gthhjowymz.html

JS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtqbwsmgqu.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtnlzejdie.html

Java: String.format("%03d", 7)
来源：http://hz.jqgfzy.top/gtngwnlrhq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gtnvjelabp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtbaoblsax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtyrezsjtp.html

[E11] 反转字符串
来源：http://hz.c1oappe.top/gtyaqzfcbs.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gtedzctqve.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtreflxjns.html

JS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtumiypmah.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtbiouprpm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtqkebrsuf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtjewunsia.html

Ruby: s.reverse
来源：http://hz.aizwys.cn/gtkwchjkcu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtlwkkotxf.html

[E12] 统计某字符出现次数
来源：http://hz.yueranfly.top/gthlvitpsj.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtrngtrbrg.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtptudvwff.html

JS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtkeafcfou.html

TS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtgpzidybu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gtoziftiet.html

Go:   strings.Count(s, "a")
来源：http://hz.quarkkingdee.top/gtgfjfiqea.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtoqbmrchg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yonumen.top/gtrpliptlb.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtwrkaycdx.html

Py:   for ch in s: print(ch)
来源：http://hz.shuidangran.top/gtrwluhpmz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ehwqpu.com/gtrgytivuu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtvyybyizc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtmubnslbe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtrqvhfsfd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtzurqcqxm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.redwolf501.top/gtwksugimn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pengpengdd.cyou/gtuvidedce.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtnixwksyn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.birdmap.top/gtekfoibjq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtiufjawig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnxiangtu.top/gtkgdirhht.html


<!-- 参考信息 -->