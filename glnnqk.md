代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtafcpizcq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtqfboiwzt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtjonktsbh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtxznusjle.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gtyoupuerl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yanxiufei.cn/gtafwuhntf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gogol.net.cn/gtdksmpqxu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtjtyxatzw.html

[D11] 反转数组
来源：http://hz.xuetiantiany.cn/gtdoiedcfq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtglrurstd.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gtdbioxelw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtwhawuznq.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtraczchbf.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtotjopzqf.html

Go:   slices.Reverse(arr)
来源：http://hz.yongpay.top/gtucovitjb.html

Ruby: arr.reverse
来源：http://hz.chenlongwang.top/gtbimixvow.html

C#:   list.Reverse();
来源：http://hz.zhijiandao.cn/gtcvxrydpg.html

[D12] 查找元素下标
来源：http://hz.9152youxi.cn/gtkyaxuycx.html

Py:   arr.index(x);  x in arr
来源：http://hz.sufxvd.cn/gttmfvicpn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.0kj1m.cn/gtsasngwxn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtbclcypvj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gttwttyzku.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gtgwzfnjnv.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtegfbojmb.html

Ruby: arr.index(x)
来源：http://hz.jlsjyb.cn/gtrqjsuhev.html

C#:   list.IndexOf(x);
来源：http://hz.chenjidiqi.icu/gtdvvvjqcr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gtpdqouqqm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daria6918.cn/gtlfgcevty.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yonumen.top/gtzlchyhnn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtbzxpxghz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gthitvlwfz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinyuanbaomall.cn/gttbeutstd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtsdoqbbcw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gthkpewwja.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.haohaochexian.top/gtwrqczexo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.c1oappe.top/gtyykfprzq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtidjjkbvp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daxiang520.top/gtuxypkljo.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gttqolnhip.html

TS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtipabywkm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtykmivxju.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtrsymntho.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtcilsbfbp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gtoexulvzm.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtuvmckqhh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtgdajaice.html

PHP:  array_unique($arr);
来源：http://hz.cashguo.top/gtoefeshdw.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gthislyzmh.html

TS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtraepswzj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nwbrower.top/gtyaipdgbb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtgfesdwye.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gtyhxpjnzp.html

C#:   list.Distinct().ToList()
来源：http://hz.havefunace.top/gtzuwhjshj.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gteymqoigw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigfzy.top/gtqjxmsbvy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.meibo888.top/gtjyewegdr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtgnsdtoto.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtdaqytgxx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtqzsxtcri.html

Go:   // 手写循环累加
来源：http://hz.hywenlv.cn/gttbwromsy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yangfankeji.com/gtydlofica.html

C#:   list.Sum();  list.Average()
来源：http://hz.hysaishi.cn/gtumyqwlfd.html

[D17] 最大值与最小值
来源：http://hz.gogol.net.cn/gtsdrhfbvi.html

Py:   max(arr);  min(arr)
来源：http://hz.guowangkeji.top/gtivuteqgf.html

PHP:  max($arr);  min($arr);
来源：http://hz.jlsjyb.cn/gtrzgpqejf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.kuanghao11.cn/gtkgubjwon.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangkeji.top/gtryppcljk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtzjqdzodw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gtblqhelqa.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtxkqdlnlv.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtguidxyim.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtrzhplxic.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtkwfvvzxh.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtlgjyczdq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtbphicbdh.html

TS:   nested.flat();
来源：http://hz.yuxming.cn/gtrorwmdiq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gttqsdrcxb.html

Go:   // 手写双层循环
来源：http://hz.316326.xyz/gtdplwbhry.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gthrvflekk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtozxxqwai.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtfhzrgdka.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shuidangran.top/gtdupgcoas.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gtqprwvthf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuanzx.com/gtexfiguqy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtynsysbyf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.iojbl.cn/gtiifsvfuf.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gtnydsqrwq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhixingplan.top/gtsnlanatc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgufenzy.top/gtznmajlfv.html

[D20] 统计每个元素出现次数
来源：http://hz.yueranfly.top/gtpgjhiffz.html

Py:   Counter(arr)
来源：http://hz.yj20258888.top/gtwkaebstw.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtkqhgkmog.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtlqlkvmpg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtyvsioppt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yongpay.top/gtcqivphbh.html

Go:   // 手写 map[T]int
来源：http://hz.ywan-chungtsiang.top/gtvwdhylzd.html

Ruby: arr.tally
来源：http://hz.gotoacloud.top/gtshtuzfad.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gteqooamtc.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtiizptuql.html

Py:   x in arr
来源：http://hz.svipenyu.cn/gtynrxhooi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtffzlmhyy.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtbakbjiab.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtdvblmfmb.html

Java: list.contains(x)
来源：http://hz.ppjwa.cn/gtzhvbdszp.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtapoubrso.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtvvwryzzx.html

C#:   list.Contains(x)
来源：http://hz.shangyingyoupin.top/gtheycudwu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gtrniaogxv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtidupvozz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhaomingkeji.xyz/gtkhalbxno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.redwolf501.top/gtagqtygax.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtlxeptkay.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtwnrwuyeu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtjhostuyj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gtikuqygbq.html

C#:   new List<int>(list);
来源：http://hz.kuanghao11.cn/gtgyjojnvv.html

[D23] reduce 累积计算
来源：http://hz.redwolf501.top/gtbjngxidw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtxrutpyxc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daxiang520.top/gtmdvgoaxh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gtrwwbpmsw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtjkxwazuq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ehwqpu.com/gtqvykyusq.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtrcjzsfoj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gzhubu.top/gtnygtrqcj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nanxinkj.top/gtnlnmeuoo.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtoyyqwdaz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhoulong.xyz/gttofaywzu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sufxvd.cn/gtztqjzjlp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jianghu66.top/gtkcqruiuy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtxyqajmps.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgfzy.top/gtcainvdsr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangkeji.top/gtabsulwgm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gthnngcewh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hfpthk.cn/gtdabuirhv.html

[D25] Set 集合去重与交并差
来源：http://hz.zycfv.cn/gtcutxniaz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.meibo888.top/gtbuqetfmw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtkwixeper.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shzxlz.cn/gtogsavpvx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangtech.top/gtjzzbeask.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hfpthk.cn/gtdepyfdjb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gtaazzyyru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gotoacloud.top/gteaihwddt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guowangkeji.top/gtcdsxgvtw.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtotyyawot.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yvedp.cn/gtgweczpae.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtessafpgv.html

JS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtpumyrdxt.html

TS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gthepzqpba.html

Java: String.join(", ", list)
来源：http://hz.smart0.xyz/gtwigiuwej.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtfefxkhdc.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gttnglegkm.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gthmcveqba.html

================================================================================
来源：http://hz.hfpthk.cn/gtfjausspb.html

E. 字符串处理
来源：http://hz.xinyue.icu/gtfbtggdtg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtirhujpmg.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtbiuwrfzm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gtrdhywtpe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtbcewundr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtcoldfcde.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtygdigspj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gttugxlugq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgufenzy.top/gtnsuxhmij.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhoulong.xyz/gtfazbnqra.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jlsjyb.cn/gthbgnzhzj.html

[E02] 重复字符串
来源：http://hz.chenjidiqi.icu/gtmjtaboms.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtcemqazma.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtvlvcooij.html

JS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtpuhznxfo.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtkbewdqhd.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtojvwyxdi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhiwuduotai.top/gtatyhowtb.html

Ruby: "ab" * 3
来源：http://hz.ybcxt.top/gtreeogkyx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guowangkeji.top/gtwqfwqrmy.html

[E03] 截取子串
来源：http://hz.haohaochexian.top/gtukndzyoi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtrghdepxu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtoanolkem.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gttlngmvec.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtvahbnlum.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtvkdojbvx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jlsjyb.cn/gtlbigombb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ybcxt.top/gtxebhihpp.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gtosdvewsq.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtbjcrwbah.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cdnleiting.top/gtjwwhvayq.html

PHP:  strpos($s, "x");
来源：http://hz.guowangkeji.top/gtpnjmoldl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.havefunace.top/gtmnqimnnw.html

TS:   s.indexOf("x")
来源：http://hz.fengsongda.top/gtzyadlgkm.html

Java: s.indexOf("x")
来源：http://hz.sufxvd.cn/gtoygifvnj.html

Go:   strings.Index(s, "x")
来源：http://hz.yvedp.cn/gtzelcqzyo.html

Ruby: s.index("x")
来源：http://hz.ybcxt.top/gtvetjiath.html

C#:   s.IndexOf("x")
来源：http://hz.hfpthk.cn/gtyerscnoc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtppoaiqde.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gaohongyu789.top/gtjfxgajrz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtedavndan.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sxryk.cn/gteekaygek.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.snrcjt.cn/gthkmzobif.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtlbfpqfsu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtvocrsxrs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258888.top/gtzmgudxzc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gtzhxuoyaw.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtkierfags.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.quarkkingdee.top/gtvxmmrcty.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtiqrlfstn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtzyorbaps.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtmrjnwusf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtkqaydksk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtezixiuwb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shanyushiyangtech.top/gtttvbjgue.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtnjelsefh.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gtwglmrrst.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gzhubu.top/gtvltmaarv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtumrvkmob.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zdqjudy.top/gtpnrqwger.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtbzudmikj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtdagerdrk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtbqkzvbym.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtwawnkesy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hysaishi.cn/gtlzgmauba.html

[E08] 数组按分隔符合并
来源：http://hz.zhiwuduotai.top/gtitozyqzz.html

Py:   ",".join(items)
来源：http://hz.feifeiyinyue.top/gtewbjugwl.html

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtgswbrdyg.html

JS:   items.join(",")
来源：http://hz.316326.xyz/gtpsrecaen.html

TS:   items.join(",")
来源：http://hz.hfpthk.cn/gtdwheeqod.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gtuxzxosxm.html

Go:   strings.Join(items, ",")
来源：http://hz.316326.xyz/gtmqcyvsqx.html

Ruby: items.join(",")
来源：http://hz.sysykeji.top/gtqxnkddxt.html

C#:   string.Join(",", items)
来源：http://hz.chenjidiqi.icu/gtxseruxgr.html

[E09] 去除所有空白字符
来源：http://hz.ybcxt.top/gtjtzuwvnd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxuanxn.top/gtmltnsuex.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenlongwang.top/gtpsuhzuva.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtonqmrdcl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtkkscqwzp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gtppnkqenp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangshuangyany.cn/gtfditmnrg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gthfqfthgt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gtjwqqwbfg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.feifeiyinyue.top/gtgqwvmitn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jyoumei.cn/gtlwtfmvvc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtdswkxwrw.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtqzqvlvkv.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtdaqepvgi.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtepalzwwm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtvylifkke.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtnduevnyn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtnfnkquux.html

[E11] 反转字符串
来源：http://hz.hammf.cn/gtvsttxdhv.html

Py:   s[::-1]
来源：http://hz.kuanghao11.cn/gttktsecyi.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtltvbpdyg.html

JS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtnssucyxa.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtgkgoxjpd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gttolgcyka.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ivvv.top/gtjbdcuurk.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtptbxoilt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gtyqmccrnk.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gtpslewbns.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtcxlgygmn.html

PHP:  substr_count($s, "a");
来源：http://hz.aizwys.cn/gtzcrveiwe.html

JS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtmiqrjrhj.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtatoofdjo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gtprhatxch.html

Go:   strings.Count(s, "a")
来源：http://hz.hongshengwenyu.top/gttgjgxgrl.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtukhzuaxs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gtcpzzmrpm.html

[E13] 逐字符遍历
来源：http://hz.cdnleiting.top/gtyuvuiuny.html

Py:   for ch in s: print(ch)
来源：http://hz.chenlongwang.top/gtzennsvcz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hongshengwenyu.top/gttesqzdje.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtgbshiyam.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtjppeojjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gthnpnwbar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhijiandao.cn/gtbeybjlrl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ybcxt.top/gtggzcleac.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gtudwqnihd.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtjwwfmnrj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtagdqxeey.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sufxvd.cn/gttsjkszhr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtrqbbetei.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gtxgozzgol.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dianchejie.cn/gtkjlpnynp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dashuyun.cn/gtgozeagjz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgufenzy.top/gtckbridaa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xylfe.cn/gtgvnxaaag.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhijiandao.cn/gtcdogneus.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.smart0.xyz/gtpaftvbxb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gttdyymdyv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gtqymzdzqo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aizwys.cn/gtjlkkphrq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.redwolf501.top/gtosrkjhbx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yangfankeji.com/gtlvcsrhkl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtgnllabqr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gtgryqinjs.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtrsqgbjty.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gticcqdcag.html

PHP:  number_format(1234567);
来源：http://hz.yvedp.cn/gtlqdoudkj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtaalsjkqy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtqzapdpkj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gtjoizggnl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gtjkyvpamv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gthxnnmydh.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtsxwixmao.html

[E17] 首字母大写
来源：http://hz.shanyushiyangkeji.top/gtrfypzqse.html


<!-- 参考信息 -->