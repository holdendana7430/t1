代发 wailian999

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtrgdzgzbp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xinyue.icu/gtgymloeif.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gtcgjhyagq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.feifeiyinyue.top/gttezprnzd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtyufwlsuh.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gthidnxuex.html

C#:   list.Sort();
来源：http://hz.pengpengdd.cyou/gtgfaqduxv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guannengcc.top/gtbjjfcuqy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtbkqiczwa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gtxfypzzal.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.52xcode.cn/gtgnofdguo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtthtvzwps.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gogol.net.cn/gtsirrwtty.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hywenlv.cn/gtpdwdbbjr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtsggsxtjl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gtbgelydpn.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtujzzpqrd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cdnleiting.top/gtwiawdvko.html

PHP:  array_reverse($arr);
来源：http://hz.guannengcc.top/gtszodzmdy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gttufyglah.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtngwwznsk.html

Java: Collections.reverse(list);
来源：http://hz.sufxvd.cn/gtmanufimn.html

Go:   slices.Reverse(arr)
来源：http://hz.svipenyu.cn/gtgqhvjbsp.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtxyktkqgn.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtcnlkttaf.html

[D12] 查找元素下标
来源：http://hz.daria6918.cn/gtmfognwuz.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gtlpzcfcri.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gttwldyfaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gthghlqgyu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtraorjfgi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtunhtyetw.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgufenzy.top/gtkbamfnqr.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtsumklrzr.html

C#:   list.IndexOf(x);
来源：http://hz.sysykeji.top/gtubrpgjop.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtlozydffs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinqigfzy.top/gtrlycokhb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xinyue.icu/gtqjrofayr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtsypzxzoz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtxedcuuef.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhixingplan.top/gtngxmdwfg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tanke756.top/gtwntptfup.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.andypj.xyz/gtmgesjaay.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuanzx.com/gtydyqrvos.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtmhoxsdrt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dashuyun.cn/gtwynvaedp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yvedp.cn/gtfwkefwup.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtochbhyig.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtognxundw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhongyouzk.top/gtxtwliszu.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtxflygzuq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtarfdyhle.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gthxzjfnpq.html

[D15] 去重
来源：http://hz.yonumen.top/gtaucwfcve.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtzbmacofo.html

PHP:  array_unique($arr);
来源：http://hz.havefunace.top/gtkelzwrnf.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gthupwtgeu.html

TS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtodmosepl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtijbmdmww.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shuidangran.top/gthylalami.html

Ruby: arr.uniq
来源：http://hz.yj20258888.top/gtknockmgl.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gthswhiqel.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtyivowcuu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtoqruqydp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtttzyunjc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtqkrhgpzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtxsicwcxq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhixingplan.top/gtdnernndu.html

Go:   // 手写循环累加
来源：http://hz.yangfankeji.com/gtyrzhqzry.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gteipfyvzx.html

C#:   list.Sum();  list.Average()
来源：http://hz.gotoacloud.top/gtttjhgduq.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gtdkjlfyho.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtsjnyieoc.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtjozbfuxz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenjidiqi.icu/gthlditmdl.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gtkoentoxo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtxeabtfem.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.snrcjt.cn/gtsbomvcjg.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtajaijesl.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtfbjcpjbu.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtsuxykvvc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.haohaochexian.top/gtxwmyahzh.html

PHP:  array_merge(...$nested);
来源：http://hz.zhixingplan.top/gtqveqgudp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhixingplan.top/gteoyzvyqn.html

TS:   nested.flat();
来源：http://hz.havefunace.top/gtjkwsrdch.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gotoacloud.top/gttcitjhlr.html

Go:   // 手写双层循环
来源：http://hz.yongpay.top/gtadxfdzys.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtlobwupqf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jianghu66.top/gtiugoyxpv.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtvcrcqwxk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yanxiufei.cn/gtaukbmfah.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gotoacloud.top/gtjreomvwy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tianlin.xyz/gtrrhgnxyo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtbhloauql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtiihmcxvo.html

Go:   // 手写 map[string][]T
来源：http://hz.jianghu66.top/gtrxtqhqcf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnxiangtu.top/gtuumwrtcm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtagptcepm.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtfpvvxttp.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gtpnnwrrij.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtxiauyyok.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtrwkdchyc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtuylfaczc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtzxlftgxf.html

Go:   // 手写 map[T]int
来源：http://hz.gogol.net.cn/gtqlxpnvzg.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gthhgtziqp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dianchejie.cn/gtofdjsssg.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtrbnqctgg.html

Py:   x in arr
来源：http://hz.sufxvd.cn/gtvibksrqz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtjhhocppj.html

JS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gtnwlstzhx.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtvnvqbkue.html

Java: list.contains(x)
来源：http://hz.wangdashe.top/gttuorhoan.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtiufzotmf.html

Ruby: arr.include?(x)
来源：http://hz.hnxiangtu.top/gtngdofxkw.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtdmqlgpiv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jianghu66.top/gtrcyutcgb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gaohongyu789.top/gtevvvkkhi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gthudmtxwg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigufen.top/gtadzertdc.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtfgiimreb.html

Java: new ArrayList<>(list);
来源：http://hz.redwolf501.top/gtjtrwnpvy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ivvv.top/gtffxlbhbb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yongpay.top/gtxfkspqyy.html

C#:   new List<int>(list);
来源：http://hz.shuidangran.top/gtengfbkuk.html

[D23] reduce 累积计算
来源：http://hz.smart0.xyz/gtieiyqrzr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guowangkeji.top/gtcbkpdoes.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtoytukrjj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtudmuzcdj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtmxscdyls.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtbuerxgxo.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtnflsrjwr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.redwolf501.top/gtighkqexh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtdccoeryy.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtbtpfoebe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtsgqohitb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigfzy.top/gtjnfqpdtd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cqqwz.cn/gtkcrkthah.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtqqdrfrvv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hysaishi.cn/gtpccwjppq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guowangkeji.top/gttddyetvq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxuanxn.top/gtpxwvggzs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtzaueenxu.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtzcknadbf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gtfanauvum.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtmkuoxbjd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtyfdkvxuo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtjgtbkrdp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jyoumei.cn/gtkqfffimr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtljxmdvei.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cucudq.cn/gttynxovqi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.316326.xyz/gtmfeotdns.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtzcacwjyn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtpzbzghyv.html

PHP:  implode(", ", $arr);
来源：http://hz.pycfn.com/gtwwziexai.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtjtxizkjf.html

TS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtbfqjlend.html

Java: String.join(", ", list)
来源：http://hz.yj20258888.top/gtaxrerebg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fengsongda.top/gtueuiwqur.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gttefmsmnm.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gtanodqahg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtczpgpgbx.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtvcenohvk.html

================================================================================
来源：http://hz.guowangkeji.top/gtmsodqzdw.html

[E01] 拼接字符串
来源：http://hz.yj202588.top/gtuoscswmm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtzmpvsgpe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fzhhl.top/gtckqbtqfx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtgqperrzy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangkeji.top/gtqpalugcd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtwuuqfaou.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtxzmyhwpo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gtpsnlhspu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxinkj.top/gtgiwidngn.html

[E02] 重复字符串
来源：http://hz.chenzaomai.com/gtbmujardc.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtaeyqbciq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.smart0.xyz/gtqprfdvkw.html

JS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtdxaqmrna.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtenlwuimx.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gtnghnbdid.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtosdqpwhw.html

Ruby: "ab" * 3
来源：http://hz.xylfe.cn/gttsetbhty.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gtooiqdbka.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtjljnclvr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.kuanghao11.cn/gtdaplpxvu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydjk.org.cn/gtgctcpwel.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtmpgfmboj.html

TS:   s.slice(1, 4)
来源：http://hz.svipenyu.cn/gtvbesfopf.html

Java: s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtnimzxiky.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhengqikj.top/gthumwpegf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gttxsvcomr.html

C#:   s.Substring(1, 3)
来源：http://hz.chenlongwang.top/gttlduggrr.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gtrimxtlus.html

Py:   s.find("x");  s.index("x")
来源：http://hz.andypj.xyz/gtsvlijtky.html

PHP:  strpos($s, "x");
来源：http://hz.sufxvd.cn/gtthtycgfr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gttfdfsdtp.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtxwfhurkn.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtmrxstwqj.html

Go:   strings.Index(s, "x")
来源：http://hz.xuetiantiany.cn/gtyjsrxeqd.html

Ruby: s.index("x")
来源：http://hz.nanxinkj.top/gtthcxykoi.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtjryeuuav.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ywan-chungtsiang.top/gtopekummv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhiwuduotai.top/gttooqdfsk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.redwolf501.top/gtqtncdngi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtcuylvqdp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daxiang520.top/gtucfehdzp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtcpamwkhe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yongpay.top/gtjzldciqh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xziqi.cn/gtgplapdvz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgfzy.top/gtufrngdtd.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtsmlklyby.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtkxycdrzh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.redwolf501.top/gtaiojlfse.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gttnqwvrht.html

TS:   s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtyufcjowa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtuznizptp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtxpeayvpw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cashguo.top/gtiyshejkp.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtskiffpgs.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gtwijiybxl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fzhhl.top/gtxkrxivby.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtpftivvwm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtcgrhajvz.html

TS:   s.split(",")
来源：http://hz.daria6918.cn/gthaqpovsg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtheakywjs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yueranfly.top/gtinkiqgdg.html

Ruby: s.split(",");  s.split
来源：http://hz.gotoacloud.top/gtkzkmfbyy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hysaishi.cn/gtlxrfrade.html

[E08] 数组按分隔符合并
来源：http://hz.jqgufenzy.top/gtfbxnjpso.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtxcultpwt.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtxwsypktr.html

JS:   items.join(",")
来源：http://hz.iojbl.cn/gtzqbzzjqn.html

TS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtxayzhzpb.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtnxfkbtfr.html

Go:   strings.Join(items, ",")
来源：http://hz.hnqzz.top/gtyamvqnpz.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtouxburts.html

C#:   string.Join(",", items)
来源：http://hz.ehwqpu.com/gtpnylfque.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtirnlzcwd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtdhvkrhwp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.svipenyu.cn/gtlinnvbmg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gthfpyqrmf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtaexytgsc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ehwqpu.com/gtdioheelh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtkcxubiet.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yvedp.cn/gtntoicugl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxuanxn.top/gtlydjbnuo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtzhkqnpel.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtyjyftdes.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xingfuxueyuan.xyz/gtkibtblbx.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtsmmftfuc.html

TS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gthspwucgd.html

Java: String.format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtcqlajyfi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtzmkeuocn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtefwpnbxa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtojtzabbz.html

[E11] 反转字符串
来源：http://hz.shangyingyoupin.top/gtphmswcjw.html

Py:   s[::-1]
来源：http://hz.jlsjyb.cn/gtsdxfukvo.html

PHP:  strrev($s);
来源：http://hz.ydzc1.top/gtnkumzcci.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtgcoknmto.html

TS:   [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtcbzqzzov.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ywan-chungtsiang.top/gttvqllcdp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtwhhmszdu.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gttwwmalvm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtiewgabna.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gthgbsqinu.html

Py:   s.count("a")
来源：http://hz.fzhhl.top/gtzwrhkacb.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258888.top/gtkguvvseh.html

JS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtqyivhdco.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtojczrlyr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jiagoushi.top/gttpnbknex.html

Go:   strings.Count(s, "a")
来源：http://hz.redwolf501.top/gtxtfbnrrw.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtadxfmqen.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tianlin.xyz/gtxnbflvfg.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtdewxdqie.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtoezhvvwc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gttpxvertx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtfoxmazfa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtlzqunaep.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gtimkosscy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtrjkjitly.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258888.top/gthovgdoks.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtuojpixvb.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtsyfyntru.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gtoeodupya.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtmntixmbr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gtwcapvnfc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhaomingkeji.xyz/gtuqftowmf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sweek.top/gtukaezwws.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtwayluhjl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gturxyscdy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtkicziyms.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtyrwiqift.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgufenzy.top/gtioqpbpaa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtcdkzyhnn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ehwqpu.com/gtfhyrynlh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hfpthk.cn/gtqlhwivbj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gtdqyamjai.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtkweoucnp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fzhhl.top/gtxqnzmwlb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gteavbrcmk.html

[E16] 数字千分位
来源：http://hz.andypj.xyz/gtuhzxjpja.html

Py:   f"{1234567:,}"
来源：http://hz.ppjwa.cn/gtcjttdvic.html


<!-- 参考信息 -->