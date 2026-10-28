代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tianlin.xyz/gtsagsryiv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhaomingkeji.xyz/gtmgssoubc.html

[D05] 访问与修改元素
来源：http://hz.redwolf501.top/gtmedeoytj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtevffqnqv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aibaodan.cn/gtrouizcln.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dashuyun.cn/gtzjrchonn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtyhhfwbvj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtguidhsvq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yonumen.top/gtajrfatvk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtxhmpiwhx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cheryme.top/gtjpejacic.html

[D06] 数组长度
来源：http://hz.yanxiufei.cn/gtyedduket.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtsjafjars.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gtqnujrnww.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtuigskosk.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtnawpqkfa.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtlwgdddhr.html

Go:   len(arr)
来源：http://hz.hongshengwenyu.top/gtptfnwtpq.html

Ruby: arr.length; arr.size
来源：http://hz.cashguo.top/gtxhtoicas.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtammvzmsq.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtekhtimgh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgufenzy.top/gtgnnfgipl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtcojzrvww.html

JS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtxwhjpced.html

TS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtmwczogjh.html

Java: list.subList(1, 4);
来源：http://hz.vqdsnc.cn/gtwadixckb.html

Go:   arr[1:4]
来源：http://hz.pycfn.com/gtcmaqnfcz.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtqqfdzxke.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj202588.top/gtvbxkahjp.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gtbmrzxykc.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gtwvjfdbeg.html

PHP:  array_merge($a, $b);
来源：http://hz.haohaochexian.top/gtmttknmwt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtfzwodwvr.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gtejfoxffb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cqqwz.cn/gtaeopdeph.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtzdbpsift.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daxiang520.top/gtnddkqwpa.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtthphkbsc.html

[D09] 排序（升序）
来源：http://hz.gaohongyu789.top/gttkatobtx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtuyvsxypa.html

PHP:  sort($arr);
来源：http://hz.havefunace.top/gtydutndgn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtusitvuey.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gaohongyu789.top/gtgjacpjyk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtxgstflei.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guannengcc.top/gtzhlmorzr.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtuaqanjsh.html

C#:   list.Sort();
来源：http://hz.cucudq.cn/gttrzbsjxu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtxvsgvaom.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtzecasdod.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtntxbntho.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtcgnhiqfe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtjslgssai.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtdflfrstz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guowangkeji.top/gtuvaojxwu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangdashe.top/gtmxbwxufr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gtconjymje.html

[D11] 反转数组
来源：http://hz.hongshengwenyu.top/gttcvoebcx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tian-w.cn/gtnujlxvvo.html

PHP:  array_reverse($arr);
来源：http://hz.yj202588.top/gtbrjcegqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtofeucynz.html

TS:   [...arr].reverse();
来源：http://hz.nanxinkj.top/gtrgdvgwky.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtpmwvfohb.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtarwclpwc.html

Ruby: arr.reverse
来源：http://hz.snrcjt.cn/gtlcvdleqk.html

C#:   list.Reverse();
来源：http://hz.iojbl.cn/gtjgvtcwiw.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtppudtjxe.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258.top/gtggedftaa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.bjfxy.top/gtxzcwgnrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtmftgqqtd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtdtpuheem.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangkeji.top/gttvzwzpmk.html

Go:   slices.Index(arr, x)
来源：http://hz.jianghu66.top/gttmxzlnpj.html

Ruby: arr.index(x)
来源：http://hz.jlsjyb.cn/gtsinrledi.html

C#:   list.IndexOf(x);
来源：http://hz.jqgufenzy.top/gtwqkvibyc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gtazdcqfdc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.9152youxi.cn/gtjwdyixxd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gtnyhtmlyv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtfgreavyn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtteauqolc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhixingplan.top/gtzxkpsgnq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gtxdbxhbaf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cucudq.cn/gtqjksshor.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.quarkkingdee.top/gtrptcpkyg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sysykeji.top/gtadjlfcii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhixingplan.top/gtseafsiqs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.316326.xyz/gtxdexftya.html

JS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gtsidwgnzr.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtmyvyfqzi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtksssuoib.html

Go:   // 手写循环
来源：http://hz.sweek.top/gthbzvfnmd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hammf.cn/gtzaeauptg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtyrpmszkt.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtiomvshlk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtvstglehg.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtpesponfy.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtygqjopjb.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtqgptvjih.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gtwzekcscd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.vqdsnc.cn/gtlxesbcln.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtvpejbvfn.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtzgdeuttu.html

[D16] 求和与平均值
来源：http://hz.9152youxi.cn/gtjpwulhhg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dashuyun.cn/gtbydpvvze.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtxdvxiffo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtqilfpmum.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtjvvufpke.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gtydoboodf.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gtiavodunw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtscevttuc.html

C#:   list.Sum();  list.Average()
来源：http://hz.aibaodan.cn/gtmnpaqpyj.html

[D17] 最大值与最小值
来源：http://hz.kuanghao11.cn/gttpclahfr.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtwyplxrph.html

PHP:  max($arr);  min($arr);
来源：http://hz.sxryk.cn/gtpuamjtzn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangkeji.top/gtftbhtido.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gtgaubhbzg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guowangkeji.top/gtjrjepcnv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtesjvrlmj.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtkmpqzqhi.html

C#:   list.Max();  list.Min()
来源：http://hz.ehwqpu.com/gtlwcisndx.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtzcnbbkrp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guannengcc.top/gtmriumhat.html

PHP:  array_merge(...$nested);
来源：http://hz.cheryme.top/gtbkczfjrn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tianlin.xyz/gtjvtjkdlp.html

TS:   nested.flat();
来源：http://hz.ivvv.top/gtbrgxtrch.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtffvjbkqf.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gtiymlhsmr.html

Ruby: nested.flatten
来源：http://hz.zycfv.cn/gtfklenvgv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtuukyemtl.html

[D19] 按字段分组
来源：http://hz.zhaomingkeji.xyz/gtjfzhiovq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xinyue.icu/gtesckqbhi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtwpztebyr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtsydogvzi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gttegfjwcy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.birdmap.top/gtozvdwxtr.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtpiiljzhx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhiwuduotai.top/gtctvxvuoa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gtqurbjntc.html

[D20] 统计每个元素出现次数
来源：http://hz.aibaodan.cn/gtylclajcg.html

Py:   Counter(arr)
来源：http://hz.dianchejie.cn/gtxjclrtmf.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtbzelmidu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtocxpxwrc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtmpsqndsx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtxrijpzap.html

Go:   // 手写 map[T]int
来源：http://hz.316326.xyz/gtgskmjbge.html

Ruby: arr.tally
来源：http://hz.jqgufenzy.top/gtiszgpbay.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtsxctewoj.html

[D21] 判断是否包含某元素
来源：http://hz.nwbrower.top/gtsfqqqznc.html

Py:   x in arr
来源：http://hz.ivvv.top/gtugwskkgd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtpooizjdk.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtjkrbzqsu.html

TS:   arr.includes(x)
来源：http://hz.ivvv.top/gtpzagylyg.html

Java: list.contains(x)
来源：http://hz.pengpengdd.cyou/gtlutfhhzt.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtdzqzyhuf.html

Ruby: arr.include?(x)
来源：http://hz.jinqigufen.top/gtmhdlhvnl.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtvytsnncx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtqxorfnye.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtwtivibtj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtocwqeney.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuanzx.com/gtqbaejzqc.html

TS:   [...arr];
来源：http://hz.c1oappe.top/gtggvuogqe.html

Java: new ArrayList<>(list);
来源：http://hz.yuanzhike.top/gtwjkedpvc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gttvudrzna.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guowangkeji.top/gtmlnkpjib.html

C#:   new List<int>(list);
来源：http://hz.hnxiangtu.top/gtfgaspfhz.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gtapvzemfg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tianlin.xyz/gtnccdskfm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtbetafcso.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtkrvdcznl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtxtxrldeu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinyuanbaomall.cn/gtnjqlaupn.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtykygpdlb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yongpay.top/gtzkbevode.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinghuilouyu.cn/gtlurtovlm.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtzvivubau.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtzkxwbead.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuxming.cn/gtenseputr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fzhhl.top/gtjvbteglx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gotoacloud.top/gtxujuuwnm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hfpthk.cn/gtdeuflrdn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xziqi.cn/gttsqfbwbu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.316326.xyz/gtyzbfboaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtjiqdmbjg.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtesyitawi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangshuangyany.cn/gtzbneflld.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtsuolnoow.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtprddxqeg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuxming.cn/gtwwhzptch.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gzhubu.top/gtmiyzrmkg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hysaishi.cn/gtvzhbczxb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.feifeiyinyue.top/gtuzcegroc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hammf.cn/gtvgmphnpg.html

[D26] 数组转字符串
来源：http://hz.dashuyun.cn/gtjpkrbmkx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ivvv.top/gtjgiwlhac.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtazfcbxvx.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gtyesavvep.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gttttewbyw.html

Java: String.join(", ", list)
来源：http://hz.zhiwuduotai.top/gtzjtphtfa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.c1oappe.top/gtnzgsfnhj.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtgxawcgrv.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtlwruxpxh.html

================================================================================
来源：http://hz.cdnleiting.top/gtmuoriing.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtwpvlzlvx.html

================================================================================
来源：http://hz.sxryk.cn/gtfywxocpg.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gtmklmpwjk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtxloatbjy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtohiehabn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtpkjucyyd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtnszmugln.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yueranfly.top/gthuyjtucj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtdjzvtmbx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gtwsupaxxo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtqhjeeqdl.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtnwkmndut.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtnczynpfc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tianlin.xyz/gtknryjycc.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtverwheng.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtwknlggwe.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gticcxaqkz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gtlxtusdus.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtwksxegsf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtlpeotlpv.html

[E03] 截取子串
来源：http://hz.sweek.top/gtjgtakqjf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgufenzy.top/gtfakefgje.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtnwyqtrqy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtzmrzjgyi.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gttdxyisvk.html

Java: s.substring(1, 4)
来源：http://hz.yongpay.top/gtcrnpgahi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ivvv.top/gtbizsvgdz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtpvumzjaz.html

C#:   s.Substring(1, 3)
来源：http://hz.sufxvd.cn/gtsvzsacsc.html

[E04] 查找子串位置
来源：http://hz.xuanzx.com/gtpvjihblw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.havefunace.top/gtvahcccyq.html

PHP:  strpos($s, "x");
来源：http://hz.havefunace.top/gtbbvhpuvk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fengsongda.top/gtvslumzus.html

TS:   s.indexOf("x")
来源：http://hz.kuanghao11.cn/gtqmvnoqtm.html

Java: s.indexOf("x")
来源：http://hz.gogol.net.cn/gtcfvzugfk.html

Go:   strings.Index(s, "x")
来源：http://hz.ydjk.org.cn/gtrphydzfd.html

Ruby: s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtbefyfujh.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtcorjdlaw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yongpay.top/gtzeeycebs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sweek.top/gtkynymnjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.svipenyu.cn/gtuksaeahb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtgtmfaovv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yuxming.cn/gtbikeqomb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtjitjbiqq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cqqwz.cn/gtmciwapmc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangkeji.top/gtsnaktehd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hywenlv.cn/gtdihzdnlo.html

[E06] 替换子串
来源：http://hz.pengpengdd.cyou/gtfxykssqh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtxkbqyjdm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hysaishi.cn/gtoyiznwkn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtygjlkwid.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtpyhvztam.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtghlgvehb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtxcyqajqm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.52xcode.cn/gtjgoplqqt.html

C#:   s.Replace("a", "b")
来源：http://hz.daxiang520.top/gtubjvmwfw.html

[E07] 按分隔符拆分
来源：http://hz.daxiang520.top/gtovwxgpij.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtuaivhkae.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tianlin.xyz/gthzilgqrq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.svipenyu.cn/gttagyewdl.html

TS:   s.split(",")
来源：http://hz.xingfuxueyuan.xyz/gtfaigkqqo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxuanxn.top/gthsiuglqv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtkgnahzyx.html

Ruby: s.split(",");  s.split
来源：http://hz.kuanghao11.cn/gtymuutzmk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtvpuyrdbn.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtsmmsqhly.html

Py:   ",".join(items)
来源：http://hz.tanke756.top/gtfunxutgb.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gthrninzzh.html

JS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtowfaahbl.html

TS:   items.join(",")
来源：http://hz.daria6918.cn/gtgywryewm.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtasyejdns.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxuanxn.top/gtvqztobbb.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtgoaoypmx.html

C#:   string.Join(",", items)
来源：http://hz.hnxiangtu.top/gtypmwpnhc.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtxglzduqi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nwbrower.top/gtrgkgpecd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jyoumei.cn/gtqmfpzfdh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtlwfckgmi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtrfdaiiew.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aizwys.cn/gtvebxegqz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtfbkgaysf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtblghediz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hfpthk.cn/gtggesgfvs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtnnrxjicl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtvnmvwoln.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtpkdrwufg.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtqfozckub.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtelmjqkpn.html

Java: String.format("%03d", 7)
来源：http://hz.yuxming.cn/gtfxcowxek.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtwghfciid.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenlongwang.top/gthqthtqax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pycfn.com/gtvggdgnej.html

[E11] 反转字符串
来源：http://hz.zycfv.cn/gtruipnzlt.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtzomnxkmm.html

PHP:  strrev($s);
来源：http://hz.gotoacloud.top/gtzjxxegaf.html

JS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtilpstguu.html

TS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtojkmstwk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtoaybfkif.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtuqkwhnqw.html


<!-- 参考信息 -->