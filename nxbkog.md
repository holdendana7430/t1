代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.kuanghao11.cn/gtcmtzmqja.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tianlin.xyz/gtgagjxucc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnxiangtu.top/gtjxtrgcun.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sufxvd.cn/gtnpvvuirk.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtgersytwd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydzc1.top/gtoxxeqkwb.html

PHP:  array_reverse($arr);
来源：http://hz.0kj1m.cn/gtctqylttk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtinyirbrj.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gtohlygrff.html

Java: Collections.reverse(list);
来源：http://hz.gzhubu.top/gtpxrldisc.html

Go:   slices.Reverse(arr)
来源：http://hz.ivvv.top/gtalybibfq.html

Ruby: arr.reverse
来源：http://hz.redwolf501.top/gtrhxetztc.html

C#:   list.Reverse();
来源：http://hz.tanke756.top/gtofvwhadu.html

[D12] 查找元素下标
来源：http://hz.hfpthk.cn/gtkdsqbddu.html

Py:   arr.index(x);  x in arr
来源：http://hz.shuidangran.top/gtmontltus.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sweek.top/gthjgxtcyi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtfguzzxij.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtdljzrntl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gtppaeuwts.html

Go:   slices.Index(arr, x)
来源：http://hz.shanyushiyangtech.top/gtdnlgcped.html

Ruby: arr.index(x)
来源：http://hz.havefunace.top/gtqopnzqgb.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gttssnemqv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhiwuduotai.top/gtqbbfddsq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jiagoushi.top/gtdollqgxv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinghuilouyu.cn/gtaskdytyk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtjagorjmm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtaokodqqn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.redwolf501.top/gtsqchrjdm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtxngbibuw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigufen.top/gtfdwrgepi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gtuticrgju.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtkpwnyjwz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gttninvqrq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.snrcjt.cn/gttirelenb.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtddwssdhm.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtvlxrqtkw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.52xcode.cn/gtotncmyjo.html

Go:   // 手写循环
来源：http://hz.zdqjudy.top/gtejzuulqd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.bjfxy.top/gthlqnwxle.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtelaktwmz.html

[D15] 去重
来源：http://hz.gogol.net.cn/gttdbekgvb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtdtokwpfj.html

PHP:  array_unique($arr);
来源：http://hz.gotoacloud.top/gtpsbfqatj.html

JS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtxhcizurv.html

TS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gttrbywjxp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtlzweklhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtjdftsylb.html

Ruby: arr.uniq
来源：http://hz.cucudq.cn/gtxcwmlxjf.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtmuzvkkfd.html

[D16] 求和与平均值
来源：http://hz.nanxuanxn.top/gtrzkntiyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtgpaxotjb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtaqmcvhem.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtjtenlyfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtlflvavcq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtxbdqptzp.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtsbqzymom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xinyue.icu/gtikfowcgu.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtnwsmnjrc.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtwhtpsyni.html

Py:   max(arr);  min(arr)
来源：http://hz.fzhhl.top/gthwztcyyc.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gtvyyxarys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtkxwpsayb.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gtctyprizv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtvhtlzbte.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nanxinkj.top/gtrxbkdgur.html

Ruby: arr.max;  arr.min
来源：http://hz.aibaodan.cn/gtwrrullke.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtmawujzwe.html

[D18] 扁平化嵌套数组
来源：http://hz.sufxvd.cn/gteulimygx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtpkxinnhm.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtnrojxgmu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.andypj.xyz/gteciuphzb.html

TS:   nested.flat();
来源：http://hz.jiagoushi.top/gtooayvjud.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinyuanbaomall.cn/gthhwnjxfy.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtscqdzkwj.html

Ruby: nested.flatten
来源：http://hz.hnxiangtu.top/gtumejslac.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daria6918.cn/gtpcexzgrm.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtlgaosibh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtydikrkdc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtngyxwqvh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtfdpktacb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtvvdrjqip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtupkvoqvy.html

Go:   // 手写 map[string][]T
来源：http://hz.yj202588.top/gtsmdobbsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fengsongda.top/gtohspdxuo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tian-w.cn/gtscpavcow.html

[D20] 统计每个元素出现次数
来源：http://hz.xuanzx.com/gteqmttkwq.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtbrnfcyvb.html

PHP:  array_count_values($arr);
来源：http://hz.chenlongwang.top/gtlfgvsamw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtfizojins.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtuhnqlzpg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shuidangran.top/gtqvcurwie.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtltvmwcrl.html

Ruby: arr.tally
来源：http://hz.yanxiufei.cn/gttvlolfru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gttnmrymtj.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtdeumrrcz.html

Py:   x in arr
来源：http://hz.shangyingyoupin.top/gtmtbdovij.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ybcxt.top/gtfrrtlbnd.html

JS:   arr.includes(x)
来源：http://hz.mhx1999.top/gtyshplpdh.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gttcebyaww.html

Java: list.contains(x)
来源：http://hz.ydzc1.top/gtjmfhegvm.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtlpcampjj.html

Ruby: arr.include?(x)
来源：http://hz.daxiang520.top/gtostpakvg.html

C#:   list.Contains(x)
来源：http://hz.iojbl.cn/gttzepkmfp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gtknohflqw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haohaochexian.top/gtexgfesvt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtripvkkxn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgufenzy.top/gtkqbaqypl.html

TS:   [...arr];
来源：http://hz.gzhubu.top/gtvxuncfst.html

Java: new ArrayList<>(list);
来源：http://hz.jiagoushi.top/gtstpkyttz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtyfafylhd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtikvqhweg.html

C#:   new List<int>(list);
来源：http://hz.xinyue.icu/gtuoaflblh.html

[D23] reduce 累积计算
来源：http://hz.hnqzz.top/gtkmefbsxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hongshengwenyu.top/gtmmhokqzi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtcktphbrk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtxcpdynay.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtnwxtsjne.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ybcxt.top/gtyqlxjmxk.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtcmysdfgi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtsnmwvcta.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtjoxuuqxk.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangkeji.top/gtheobsrrn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtjmgovjij.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtwtawclof.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.52xcode.cn/gtrspybuqx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ppjwa.cn/gtncbyjnuv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gtmawgnlma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.quarkkingdee.top/gthspqodhy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gtyvnuedpa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtakgyvqcn.html

[D25] Set 集合去重与交并差
来源：http://hz.dashuyun.cn/gtjutydegr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtojgigkiu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtabtghjcm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinyuanbaomall.cn/gtvraumgeo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.c1oappe.top/gtbxonasbv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ehwqpu.com/gtuktlamhz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtzdyaampi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangtech.top/gtbkimvcym.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daxiang520.top/gtwjhsvbhm.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtuhwwwrfz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yangfankeji.com/gtdlpeycfj.html

PHP:  implode(", ", $arr);
来源：http://hz.cucudq.cn/gtvxcynlfj.html

JS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtktwkfdzq.html

TS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtbmaczjva.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gtlywijngd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.0kj1m.cn/gtvvgzysel.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtdlbzjpij.html

C#:   string.Join(", ", list)
来源：http://hz.dashuyun.cn/gtxflmrjvb.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvvzbjzsx.html

E. 字符串处理
来源：http://hz.redwolf501.top/gtylftqpgu.html

================================================================================
来源：http://hz.52xcode.cn/gtuksepmvi.html

[E01] 拼接字符串
来源：http://hz.quarkkingdee.top/gtsbgcwjyu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hongshengwenyu.top/gtwdamjbjl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangtech.top/gtveevqfmq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtdzdunnjh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtlgsqainh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtkpeiwczp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gttzfmecqz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gtyerliohr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fengsongda.top/gtswmchwwo.html

[E02] 重复字符串
来源：http://hz.xuetiantiany.cn/gtcckpoymr.html

Py:   "ab" * 3
来源：http://hz.yj20258.top/gtcnpmsdav.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258888.top/gtlfpbiwgz.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtmlmbkuyg.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtcqidoaxg.html

Java: "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtboinuvby.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.dianchejie.cn/gtxlwadxfp.html

Ruby: "ab" * 3
来源：http://hz.bjfxy.top/gtinjnifhy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258.top/gtjkbduhmk.html

[E03] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtvsqwnrgf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gttsfwzhgb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cheryme.top/gtsuphtfkf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtvykepkgr.html

TS:   s.slice(1, 4)
来源：http://hz.gotoacloud.top/gtxtmhlklj.html

Java: s.substring(1, 4)
来源：http://hz.zycfv.cn/gtyabywuca.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daxiang520.top/gtcajggzom.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sxryk.cn/gtwezxrrzt.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtbhuzmkql.html

[E04] 查找子串位置
来源：http://hz.chenlongwang.top/gtknvmufwq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtarflxkpr.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtxrijphex.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yongpay.top/gtiahajefr.html

TS:   s.indexOf("x")
来源：http://hz.sufxvd.cn/gtufakgywi.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtpjxtdtwf.html

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gtoebrwimq.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtgbfbbced.html

C#:   s.IndexOf("x")
来源：http://hz.redwolf501.top/gthihzenwp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tanke756.top/gtcltrrmsw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fzhhl.top/gtybailxru.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.nanxuanxn.top/gttmpipqwa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtddvstset.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hfpthk.cn/gtidvzchqd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtcxfyaojt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtfujxingh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.bjfxy.top/gtrjbxeowt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.svipenyu.cn/gtyxtqgbjs.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtjsxpmpxd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtcltsgdrl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.fengsongda.top/gtcbkrssml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gthwgxmyih.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtdiweeqqg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtozlvbdnm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnxiangtu.top/gtyavymvkp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gteaboamtc.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtellxthpb.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gtdhhkprzm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ybcxt.top/gtiuylfzlj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtkafgmzcq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhoulong.xyz/gtqdqxfjed.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gtljwjhhbu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sxryk.cn/gtblcxizef.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cdnleiting.top/gtvyneddab.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtqhlnzfyp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dashuyun.cn/gtqmxhyywe.html

[E08] 数组按分隔符合并
来源：http://hz.gotoacloud.top/gtjgmdzlpr.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtjfpphctu.html

PHP:  implode(",", $items);
来源：http://hz.cucudq.cn/gtleuzbaya.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gthihktkbm.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtamxehxwl.html

Java: String.join(",", items)
来源：http://hz.zhengqikj.top/gtkxhwtsdu.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtgvqzsswm.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gttwqzjncr.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtrovgrfei.html

[E09] 去除所有空白字符
来源：http://hz.jianghu66.top/gtwmbemdar.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gaohongyu789.top/gtjijuhxji.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.vqdsnc.cn/gtuntjvaww.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtvmrcfwyy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtvzmrrabj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtdrwxdpqc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangdashe.top/gtjorvxvlv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtigeydynn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtyhczfqap.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gtqyxcfqge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shangyingyoupin.top/gtipwuqjcw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtvsabdfch.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gttroqykbd.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gthkiccotd.html

Java: String.format("%03d", 7)
来源：http://hz.xinyue.icu/gtjaioipso.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj202588.top/gtwtkjyieb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtgvbbmqgr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pengpengdd.cyou/gtksugburw.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtnqllpovp.html

Py:   s[::-1]
来源：http://hz.zycfv.cn/gtqpqzggai.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtqwophniv.html

JS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtvakfleud.html

TS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gthtainkoi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtirntseap.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtnghnafbt.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gttexbgqla.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtrgpcajto.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtknbnrfbk.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gtilwmxxoi.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gttnkpbhkx.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtsruuekeu.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtdokesifq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daxiang520.top/gtijjwmics.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtnhjvihkw.html

Ruby: s.count("a")
来源：http://hz.hammf.cn/gtzjqdvemq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtlynlfhre.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtglsmozlg.html

Py:   for ch in s: print(ch)
来源：http://hz.c1oappe.top/gteyaomedl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nwbrower.top/gtrjbduuyg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtgcllpyfi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtybyqahtj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydzc1.top/gtlzpqmvzp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgufenzy.top/gtlznrfott.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gthyhoohsg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gogol.net.cn/gtcavctpeh.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtwjmedgag.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhixingplan.top/gtgdcmkbtt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtjumyomoi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtwwdgvnhe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtswczhjwb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258.top/gtelgoqhwq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtcbivnmsc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.iojbl.cn/gtheqtlxnh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gtlrmqxihd.html

[E15] HTML 转义 / 反转义
来源：http://hz.cqqwz.cn/gtclxqukxd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtejvjzpfx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tianlin.xyz/gtvntuoyng.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gtatorznqj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhengqikj.top/gtxuljheui.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shzxlz.cn/gtrrctbcfr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydjk.org.cn/gthxdaxceg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydjk.org.cn/gtlmwodxok.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtdhrxvzck.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtlozfrskz.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtiegkammq.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtjpzuxjsu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtjumhilzu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtyiksazxx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gttykluirc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.iojbl.cn/gtzkzhsckh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.0kj1m.cn/gtoxjrwlit.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtjoiiudtu.html

[E17] 首字母大写
来源：http://hz.havefunace.top/gtotrtuufh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtrlwakekk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigfzy.top/gtvporafjj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtxdgkzkbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtnwahvyxq.html


<!-- 参考信息 -->