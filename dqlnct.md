代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtpvuldsae.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtnpvopthw.html

C#:   list.Sort();
来源：http://hz.yj20258888.top/gtyarebleb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cqqwz.cn/gtjbckdayi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtjfruxcxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gthpuonimn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtjqolqnni.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtrlgpvrdl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtrliobhxn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtktnayopo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtlezzaogs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtvpiigdik.html

[D11] 反转数组
来源：http://hz.bjfxy.top/gtwapzungs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhongyouzk.top/gtcxgjnllf.html

PHP:  array_reverse($arr);
来源：http://hz.chenjidiqi.icu/gtedromuto.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtwcdyecgz.html

TS:   [...arr].reverse();
来源：http://hz.pengpengdd.cyou/gthfezciim.html

Java: Collections.reverse(list);
来源：http://hz.ydzc1.top/gtpctblbkj.html

Go:   slices.Reverse(arr)
来源：http://hz.haohaochexian.top/gtomnlablm.html

Ruby: arr.reverse
来源：http://hz.andypj.xyz/gtmcvlxshf.html

C#:   list.Reverse();
来源：http://hz.ehwqpu.com/gtdutmrswd.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangtech.top/gtpcfnhlok.html

Py:   arr.index(x);  x in arr
来源：http://hz.shzxlz.cn/gtsguaffjr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gtfwlmbhvo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gteeakvszl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.vqdsnc.cn/gtqiykmyke.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.smart0.xyz/gtgpatpydj.html

Go:   slices.Index(arr, x)
来源：http://hz.daria6918.cn/gtwhhjzpqe.html

Ruby: arr.index(x)
来源：http://hz.nanxinkj.top/gtzonlnbld.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtoqaduxin.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydjk.org.cn/gtyuhleavt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gtsdllgtcg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gtjdswfukn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtywgoiail.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtrgslnidi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ehwqpu.com/gtksyuzzqr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cheryme.top/gtvqkqzuuk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtxtgbryjc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtygatgzzr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgufenzy.top/gtfigdgkat.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jlsjyb.cn/gtntbgywlj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtotfwopii.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gterdmqlml.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtigpqadqg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtwhxuqlre.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtzitrhpov.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydzc1.top/gtszdgsxog.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yangfankeji.com/gtqdovyyxs.html

[D15] 去重
来源：http://hz.daxiang520.top/gtpmvyycwy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.redwolf501.top/gtnaydblbf.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtrhajfbmm.html

JS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtiufynjnt.html

TS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtpxjqkofe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gteohqjunm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dashuyun.cn/gtljytyxrc.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gtuhctctde.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtpizrkbfj.html

[D16] 求和与平均值
来源：http://hz.kuanghao11.cn/gtscwqpuzp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigfzy.top/gtbygzrsru.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtkgxhtkbk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.feifeiyinyue.top/gtfyuiknkh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtirfdkwfh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnxiangtu.top/gtingawcgc.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtflugzcio.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtwpkjjdiv.html

C#:   list.Sum();  list.Average()
来源：http://hz.nwbrower.top/gtsinsuzbz.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gtfcpuguwi.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtlznuyefz.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtctylfeda.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtaynvsqug.html

TS:   Math.max(...arr);
来源：http://hz.jianghu66.top/gtsjmmtxqu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgufenzy.top/gtfcpuzkht.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnqzz.top/gtbveqollw.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gttnekboph.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtdfgrcoch.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtysryitpw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pycfn.com/gtkpjfjnqz.html

PHP:  array_merge(...$nested);
来源：http://hz.sweek.top/gtkrwbqmyh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnqzz.top/gtgcjmwebg.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtvrfcqcqr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtahmlrrco.html

Go:   // 手写双层循环
来源：http://hz.hysaishi.cn/gtyrddnxii.html

Ruby: nested.flatten
来源：http://hz.yanxiufei.cn/gtpsgwyplh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtscktzcgl.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gteemrxzki.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gaohongyu789.top/gtrntzetlb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtogodecvf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydjk.org.cn/gtnjmrxwir.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shuidangran.top/gtupssirij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258.top/gtuvbbqran.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtbhzrahjc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ywan-chungtsiang.top/gtlgepuzie.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtvbruaxmj.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gtsvgzzwgx.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtescmimaf.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtibshlbdv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtexqtggvr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtruniqkke.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gtwjiuiyfz.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtoauxlfqk.html

Ruby: arr.tally
来源：http://hz.feifeiyinyue.top/gtnpmkzily.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhaomingkeji.xyz/gtfthhkfqo.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gtxqvuxord.html

Py:   x in arr
来源：http://hz.meibo888.top/gtzjyehbks.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtjkgjbinv.html

JS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtgofhurht.html

TS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtcnybjbrw.html

Java: list.contains(x)
来源：http://hz.sxryk.cn/gtaahybrfs.html

Go:   slices.Contains(arr, x)
来源：http://hz.jlsjyb.cn/gtuzggnptn.html

Ruby: arr.include?(x)
来源：http://hz.hongshengwenyu.top/gtcphtvpuy.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtexoeklbk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gtrlaimarc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenjidiqi.icu/gtchvhznux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gttvvcskcv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gzhubu.top/gtlynuhmds.html

TS:   [...arr];
来源：http://hz.pycfn.com/gtjnbmmxrg.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtclbdgqpn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtpyitxlyi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sufxvd.cn/gtbonkzzbz.html

C#:   new List<int>(list);
来源：http://hz.ppjwa.cn/gtbvjgcszs.html

[D23] reduce 累积计算
来源：http://hz.hysaishi.cn/gtfgajyjed.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhongyouzk.top/gtqtsfhlor.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhiwuduotai.top/gtkrzaolfk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtbbznpvmy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtirfjqiwa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtknbdpdlz.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtioomupcb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydzc1.top/gtlhyygbgc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtcsfthzuv.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gtqojxpicx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guowangkeji.top/gtlrtlutkv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.birdmap.top/gtsyfodmag.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gtxumbmqyy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtewowcbfz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtoxaxtmif.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.316326.xyz/gtrrokiiag.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtswmbzvpm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtdqbrxmte.html

[D25] Set 集合去重与交并差
来源：http://hz.yueranfly.top/gttxmrytgj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gthrrtyfma.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtklvhnbfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtvhlgmdjr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hfpthk.cn/gthxzppomc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtyynojvei.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.mhx1999.top/gtpamtlwho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhoulong.xyz/gtbjbehysn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtkeqazsou.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtogyfllgs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cheryme.top/gtgnuntduw.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtdutafzxh.html

JS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtxjouwgbw.html

TS:   arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtbbqzbsfw.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtipdfibgj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtegsustwt.html

Ruby: arr.join(", ")
来源：http://hz.yongpay.top/gtjdbhumpp.html

C#:   string.Join(", ", list)
来源：http://hz.nanxuanxn.top/gtxivceddn.html

================================================================================
来源：http://hz.cdnleiting.top/gtbriukylr.html

E. 字符串处理
来源：http://hz.zdqjudy.top/gtozwtmflf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgdspjlsq.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtjsanlzch.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hysaishi.cn/gtzrmqrppt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuetiantiany.cn/gtawsdqmwy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtvrygmkkq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtgdcwmqwn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtpgddqgvr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shangyingyoupin.top/gtzodrtynr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtgcakpzvx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtsvxevcyu.html

[E02] 重复字符串
来源：http://hz.hnxiangtu.top/gtayftesxn.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gthsggldub.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtlpzusbok.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtotewubno.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtcofrwsed.html

Java: "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtcguojymh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigfzy.top/gtumiohjha.html

Ruby: "ab" * 3
来源：http://hz.pycfn.com/gtbwcecjcm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtmexidwsz.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtdfsikhxr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtmrhwtkjc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtpgsujeiy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtpraecpqc.html

TS:   s.slice(1, 4)
来源：http://hz.hongshengwenyu.top/gtqcnhapsk.html

Java: s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtylkpvhbw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj202588.top/gttsjktjrs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtgyopfuzc.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtfxgvjprk.html

[E04] 查找子串位置
来源：http://hz.guowangkeji.top/gtlvcsfevz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangshuangyany.cn/gtmmcboutl.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtyrtpicvc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.snrcjt.cn/gtbunvgvfe.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gthrylahte.html

Java: s.indexOf("x")
来源：http://hz.xziqi.cn/gtgsnvqhrn.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtngyhzded.html

Ruby: s.index("x")
来源：http://hz.feifeiyinyue.top/gtuejisspd.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtzcabiarf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gttgbbiibg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhixingplan.top/gtstxyuklu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yongpay.top/gtjjvtuzif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtacphfqbc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hfpthk.cn/gtrmyxgknv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtjvzyaxdl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.feifeiyinyue.top/gtfblwspak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.0kj1m.cn/gtunwqnjgn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtpeljuekx.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtxjhguvlg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.smart0.xyz/gtohqigcme.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.havefunace.top/gtzhwboazz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtwlhputxa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtcfjelsqu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtgurhbdud.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtplvwvdma.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guannengcc.top/gtruxpjvvq.html

C#:   s.Replace("a", "b")
来源：http://hz.sxryk.cn/gtgbwaednj.html

[E07] 按分隔符拆分
来源：http://hz.ehwqpu.com/gteajfrwdp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yanxiufei.cn/gtsyvdkwbq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fzhhl.top/gtizumolnf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gtlwahxkyn.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gtforhlocv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtfnrmrtjj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gtlwpwyskd.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigfzy.top/gtjurpbsgs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gtezmobwkw.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtfwtsrcdj.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtlgqaibda.html

PHP:  implode(",", $items);
来源：http://hz.fengsongda.top/gtdhzrvhnh.html

JS:   items.join(",")
来源：http://hz.smart0.xyz/gtydpnpryl.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gthvyihimd.html

Java: String.join(",", items)
来源：http://hz.yuanzhike.top/gtczujrwap.html

Go:   strings.Join(items, ",")
来源：http://hz.52xcode.cn/gtmujmkhjh.html

Ruby: items.join(",")
来源：http://hz.hammf.cn/gtbtrbqztp.html

C#:   string.Join(",", items)
来源：http://hz.tanke756.top/gtwfbjfcim.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtlkulnexr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtmvfpkklq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gtkxuszcog.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtdxttgapj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtuylvwpdl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gtxlvpghsg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangtech.top/gtodrbkosi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtqauriucx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yanxiufei.cn/gtwrtcnvfq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nwbrower.top/gttdifafgc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtnsqwmwhw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtkojqwapm.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtjrbtztru.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtdxsnpwno.html

Java: String.format("%03d", 7)
来源：http://hz.iojbl.cn/gtmcynfdhn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangdashe.top/gtrbivxsdh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtxifhrkna.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtkbtubbhf.html

[E11] 反转字符串
来源：http://hz.chenjidiqi.icu/gtfpbnnzlo.html

Py:   s[::-1]
来源：http://hz.zhengqikj.top/gtwcwycfgc.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtafznvrkv.html

JS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtakcvnbrf.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtvmshznja.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.vqdsnc.cn/gtpibnearu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.snrcjt.cn/gtglezblhk.html

Ruby: s.reverse
来源：http://hz.sufxvd.cn/gtqrhibpeq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtsmwnxzny.html

[E12] 统计某字符出现次数
来源：http://hz.sufxvd.cn/gtsvepitxa.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtffzowhtc.html

PHP:  substr_count($s, "a");
来源：http://hz.ybcxt.top/gtmivoltog.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtvwcpooyc.html

TS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtslycvhec.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gteettpqym.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gthiqwnake.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gtpsapgxpn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtfnavcqcz.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtjmtsrmlu.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtcnegvmzs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jlsjyb.cn/gtewlnfvaz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtbcvctdcy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtgksabbtb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtashqlrbd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fzhhl.top/gtfmcgbbto.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtezlnwlsb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ywan-chungtsiang.top/gtwacumpnj.html

[E14] URL 编码与 Base64
来源：http://hz.hysaishi.cn/gtisnzvelk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtqzgbrdrf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj20258.top/gtwzqauiqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xylfe.cn/gtthyxilbn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydjk.org.cn/gtzfxqkacr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jlsjyb.cn/gtjoxixoty.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tianlin.xyz/gttzaarhwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cheryme.top/gtzqbnqlot.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtnpmeutnd.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtiuiliqhy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuanzhike.top/gtddatztrx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xinyue.icu/gtgpfdnggm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gttzwnslia.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gterqvrpxm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gttcwdasvu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.quarkkingdee.top/gtyehkcuep.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtqxwztimr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.kuanghao11.cn/gthtmdgdgc.html

[E16] 数字千分位
来源：http://hz.hnqzz.top/gtthufoagb.html

Py:   f"{1234567:,}"
来源：http://hz.yuanzhike.top/gtqsfcwtmc.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtxggspdio.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtzbbcikxt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtjqeghrwt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtrjdfhrdo.html


<!-- 参考信息 -->