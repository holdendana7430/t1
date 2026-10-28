代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtmomksfji.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gthhkrdatz.html

C#:   list.Sort();
来源：http://hz.xuanzx.com/gtkogaqpnc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.bjfxy.top/gtqdbxuuus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuanzx.com/gtbugxfzsq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuetiantiany.cn/gtxeqbfqkp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtuvawakeb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtmmripjrk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ywan-chungtsiang.top/gtofmcgcfh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtkkxabmev.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fengsongda.top/gtexfhaesd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jiagoushi.top/gtixextauv.html

[D11] 反转数组
来源：http://hz.jyoumei.cn/gtsiktjjsm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.redwolf501.top/gtlgasmqpj.html

PHP:  array_reverse($arr);
来源：http://hz.52xcode.cn/gtmislomlk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtffsanzyf.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtumdlbqnm.html

Java: Collections.reverse(list);
来源：http://hz.pengpengdd.cyou/gtucxtsyxc.html

Go:   slices.Reverse(arr)
来源：http://hz.52xcode.cn/gttjhihsou.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtaxcirrqg.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtognqpwyt.html

[D12] 查找元素下标
来源：http://hz.ybcxt.top/gtqcxfmknb.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gtjbjbdgea.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.vqdsnc.cn/gtyyuckfgi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtpkksavrh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtbqxdwofa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtezvokpiu.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtlwugrzwk.html

Ruby: arr.index(x)
来源：http://hz.ybcxt.top/gtovlukadb.html

C#:   list.IndexOf(x);
来源：http://hz.yonumen.top/gtyboesfkj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtimhlcmau.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yanxiufei.cn/gtvuazrsjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cashguo.top/gtoorhybfc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gtdrejersu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtnsdpgfhe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtjmyhigbm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtssubezhp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gzhubu.top/gthfbzxzeg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtccjgzsrt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtnordgjtp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hammf.cn/gtafovbnrf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ybcxt.top/gtkfchhuru.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtptllbixd.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gttzymfgch.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuanzx.com/gtxmicvwey.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtqivnmodc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhixingplan.top/gtzxtgbsqu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtvlqwzscw.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtnhmcfyxi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtgdyrdmnt.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtnghvrndb.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtoexxdnta.html

TS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtwjkgervq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sxryk.cn/gtabfqzmby.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtperpedlc.html

Ruby: arr.uniq
来源：http://hz.ppjwa.cn/gtjoytpjmc.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtfdasiymg.html

[D16] 求和与平均值
来源：http://hz.ehwqpu.com/gtezdqjgvg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtdryazupj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtvsyikody.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtcmstdhdu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtkrkndpxr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.vqdsnc.cn/gttnwugcgo.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtpxrslpdj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtmrntybbe.html

C#:   list.Sum();  list.Average()
来源：http://hz.cashguo.top/gtsqdigqgi.html

[D17] 最大值与最小值
来源：http://hz.xylfe.cn/gtperuopaq.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtsmkwypfm.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhiwuduotai.top/gtcnqywuvf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxinkj.top/gtfjjhdqhp.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtnpxgvqnz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aizwys.cn/gtjokbiptn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xziqi.cn/gttyhybcra.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtsbdputhi.html

C#:   list.Max();  list.Min()
来源：http://hz.gaohongyu789.top/gtuyulazue.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtiamycwdu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sweek.top/gtcowlpkec.html

PHP:  array_merge(...$nested);
来源：http://hz.zhijiandao.cn/gtssnyebln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gtjazmufnq.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gtvuxzldaa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.smart0.xyz/gtweowehof.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtkqjcxqwa.html

Ruby: nested.flatten
来源：http://hz.zdqjudy.top/gtnvimoham.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jlsjyb.cn/gtwwefevsk.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gthxianiqw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtkojsbags.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.9152youxi.cn/gtxpbqvhnd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guannengcc.top/gtymhltuoq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuetiantiany.cn/gtclgydyud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gtivngvdca.html

Go:   // 手写 map[string][]T
来源：http://hz.zhiwuduotai.top/gtbmswxoeq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtcslrcxoe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtihwgjxot.html

[D20] 统计每个元素出现次数
来源：http://hz.cdnleiting.top/gtwiwgajig.html

Py:   Counter(arr)
来源：http://hz.ywan-chungtsiang.top/gtrhmrzvpg.html

PHP:  array_count_values($arr);
来源：http://hz.andypj.xyz/gtebfybaej.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gthqeodrse.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtwncffaas.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gthcbvzyzi.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gtzteltbxc.html

Ruby: arr.tally
来源：http://hz.zhijiandao.cn/gtrifzgews.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtxtluepqo.html

[D21] 判断是否包含某元素
来源：http://hz.cdnleiting.top/gtdikbjxly.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtlswacelw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shanyushiyangkeji.top/gtuxeidnnj.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtgxgladqh.html

TS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gthlocicvh.html

Java: list.contains(x)
来源：http://hz.zhoulong.xyz/gtaqmhbibl.html

Go:   slices.Contains(arr, x)
来源：http://hz.cqqwz.cn/gtrkklqktb.html

Ruby: arr.include?(x)
来源：http://hz.andypj.xyz/gtrvczmcsl.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtyfkfsvhk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.iojbl.cn/gtitdfjmqr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gtjmxhisey.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.smart0.xyz/gtfzkhxuyh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangshuangyany.cn/gtxryxkxqb.html

TS:   [...arr];
来源：http://hz.nanxinkj.top/gtslauoysd.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtafdqkwfl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.feifeiyinyue.top/gtwmjrssot.html

Ruby: arr.dup;  arr.clone
来源：http://hz.feifeiyinyue.top/gtvqyfwcxl.html

C#:   new List<int>(list);
来源：http://hz.cqqwz.cn/gtlpgffgtx.html

[D23] reduce 累积计算
来源：http://hz.zhixingplan.top/gtvqfkcney.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gttkyvtdwr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dashuyun.cn/gtsvdrgqwz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtqpmnqxox.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtpdtooknx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenlongwang.top/gtwvgpwekz.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtprqitbnd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yueranfly.top/gtmntrjxwa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtagzecaez.html

[D24] 字典 / Map 基本操作
来源：http://hz.gzhubu.top/gtcxjujpao.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ppjwa.cn/gtnmzwqsiy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtfyzgottl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtdryizwmg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yueranfly.top/gtvlonxjsu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.svipenyu.cn/gtqmtbyxvn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinqigufen.top/gtkgqmdsly.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtolyeoywm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.haohaochexian.top/gtbbqmmmll.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtyyigayel.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cqqwz.cn/gtwmgxfujq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtfdnowqig.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.0kj1m.cn/gtguastzyn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuanzhike.top/gtjickvsow.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.9152youxi.cn/gthvgpweia.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fengsongda.top/gtcmqbapvv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtqhsrezeq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtpfnkeltz.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtdmdzouvz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtnyfjhvdw.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtyhxesanv.html

JS:   arr.join(", ")
来源：http://hz.havefunace.top/gtgqiypqtm.html

TS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtktvtunzi.html

Java: String.join(", ", list)
来源：http://hz.ydjk.org.cn/gtkyvkzwee.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhengqikj.top/gtnjqderlt.html

Ruby: arr.join(", ")
来源：http://hz.chenlongwang.top/gtmvwntwho.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtnqqsrxfs.html

================================================================================
来源：http://hz.cucudq.cn/gtldsdjvpt.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gtvgrxmnql.html

================================================================================
来源：http://hz.birdmap.top/gtdtfwnihp.html

[E01] 拼接字符串
来源：http://hz.sweek.top/gtnnphxlmf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.andypj.xyz/gtggmajhhl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtguzmrwcm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtuzbwlpzm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtfgrozvqt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shzxlz.cn/gtntdfdskr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtwcjghuyo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtanumjhta.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxinkj.top/gtioqwafua.html

[E02] 重复字符串
来源：http://hz.jiagoushi.top/gtklludusw.html

Py:   "ab" * 3
来源：http://hz.gzhubu.top/gtoutwmvcm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtefihinsy.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtzpnnhihy.html

TS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtphlbkykr.html

Java: "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gthkhauazs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtgivsoutl.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtekiqweqr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.bjfxy.top/gtnrluchst.html

[E03] 截取子串
来源：http://hz.xziqi.cn/gtcwlixahx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.feifeiyinyue.top/gtfbppquik.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fzhhl.top/gtidtrcwuy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuxming.cn/gtssleunmw.html

TS:   s.slice(1, 4)
来源：http://hz.zhiwuduotai.top/gtaiywhwsw.html

Java: s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtqvcfrabk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xinyue.icu/gtajexfhxx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtvyryobiz.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtnjxvobnz.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gteqbkqxeq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtkdbwufvy.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigfzy.top/gtypgofwud.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haohaochexian.top/gtpvwzwncy.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtutxugqpd.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtkxhyyhtf.html

Go:   strings.Index(s, "x")
来源：http://hz.aizwys.cn/gteoffcrmz.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gtergxlxvw.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gtagsdkunp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhaomingkeji.xyz/gtvimcafmr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gtjatnolfl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cashguo.top/gtapebuaqx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gthufrsfxb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtabellyrg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtxdvodeuc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gttlbluhaw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.kuanghao11.cn/gtydpsdjmh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtimmtfuxm.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtqvsmpmvw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daria6918.cn/gtddlyjsar.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtxivtgzzw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtywlsduhn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gttpnszyef.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtwfkephbe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fengsongda.top/gtwxbladbu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtxqixtere.html

C#:   s.Replace("a", "b")
来源：http://hz.dashuyun.cn/gtwgzbfjqj.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gttrwfujnl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhoulong.xyz/gtzwjfnxds.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sysykeji.top/gtepoyvgkc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtaxpafrog.html

TS:   s.split(",")
来源：http://hz.mhx1999.top/gtjdswkrqm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigfzy.top/gtkrsjegcm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jqgufenzy.top/gtyxyozdtd.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtmnqxlytk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtzdfghylr.html

[E08] 数组按分隔符合并
来源：http://hz.xuanzx.com/gtfocnplfm.html

Py:   ",".join(items)
来源：http://hz.jlsjyb.cn/gtkripeunw.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtnplahesh.html

JS:   items.join(",")
来源：http://hz.dashuyun.cn/gtpduzpxtr.html

TS:   items.join(",")
来源：http://hz.nwbrower.top/gtnahnxgnl.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtuhpdqkbo.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtgmphvwtp.html

Ruby: items.join(",")
来源：http://hz.wangdashe.top/gtoylhhxhe.html

C#:   string.Join(",", items)
来源：http://hz.aizwys.cn/gtblwcsvkx.html

[E09] 去除所有空白字符
来源：http://hz.yvedp.cn/gtimknlhvj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ywan-chungtsiang.top/gtydtiagbx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtocwhjrqs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtdrxzqoxu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtcfjbpujl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangtech.top/gtejuapmla.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtbkkhzviw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yongpay.top/gtcmrtpvnw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtfqasifiq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtnvdmvyfm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhijiandao.cn/gttzudioyl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtaksndyum.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtiwdogoub.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtamudjbeb.html

Java: String.format("%03d", 7)
来源：http://hz.tianlin.xyz/gtzgjzczzb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtblpdlbcm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ybcxt.top/gtrepqnqee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtnzcrywsg.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtpwbbthwk.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtdohobyud.html

PHP:  strrev($s);
来源：http://hz.jinqigufen.top/gtrjssyzih.html

JS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtvlfqazgd.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtfcuziqwb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ppjwa.cn/gtpzpabyew.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtnaabutqd.html

Ruby: s.reverse
来源：http://hz.yj202588.top/gtvjklteyy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtajlyvzvm.html

[E12] 统计某字符出现次数
来源：http://hz.gaohongyu789.top/gtittxdequ.html

Py:   s.count("a")
来源：http://hz.yj20258.top/gtuxtlfesu.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtltffdjxx.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtwrvqjbui.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtxfwquyfx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gtfxvuildy.html

Go:   strings.Count(s, "a")
来源：http://hz.chenjidiqi.icu/gtfsxwnmjs.html

Ruby: s.count("a")
来源：http://hz.ydjk.org.cn/gtmvguxyej.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhiwuduotai.top/gtahabjufl.html

[E13] 逐字符遍历
来源：http://hz.bjfxy.top/gtsvsjajfk.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gthclzstkd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtapmlzdxk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtfnuwwcdx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fzhhl.top/gtnbnydadg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.snrcjt.cn/gtulxzhohp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtmdsopwhw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxinkj.top/gtjdndhiib.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxuanxn.top/gtjjmfopjl.html

[E14] URL 编码与 Base64
来源：http://hz.xinyue.icu/gtzngdmubz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xinyue.icu/gtumbreiqr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtuqzbrpty.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtpqwpttrx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gtzcmfnlge.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtlvzonrwc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zycfv.cn/gtlmvnnswu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtpnepboea.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sxryk.cn/gtkxwizkbi.html

[E15] HTML 转义 / 反转义
来源：http://hz.yanxiufei.cn/gtzqzyurcd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtvvrwopvo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yongpay.top/gtognqsnrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xziqi.cn/gtkyfvriwa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydjk.org.cn/gtdcqoooia.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258.top/gtkqiiorlb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.vqdsnc.cn/gtcczpjuqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hfpthk.cn/gttovfcssv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhoulong.xyz/gtjjqxwelk.html

[E16] 数字千分位
来源：http://hz.xuanzx.com/gtdqpajipg.html

Py:   f"{1234567:,}"
来源：http://hz.sufxvd.cn/gtetjuwuwf.html

PHP:  number_format(1234567);
来源：http://hz.xylfe.cn/gtbcidjjty.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtaepfbkrn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtjtpevzzb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gtxcocphja.html


<!-- 参考信息 -->