代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.ivvv.top/gtvqtbdxyf.html

[D08] 合并两个数组
来源：http://hz.yanxiufei.cn/gtkrbxmvxr.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtwhrfpugp.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtptsxgfqd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.kuanghao11.cn/gtckxmyxxx.html

TS:   [...a, ...b];
来源：http://hz.nanxuanxn.top/gtvhwyyhxm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xziqi.cn/gtlqesyyej.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gttzhtrwwo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daxiang520.top/gtcsgxghrd.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gtomubmfdt.html

[D09] 排序（升序）
来源：http://hz.fzhhl.top/gtlwakfrma.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtbpauhymo.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtjvtkwbff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cdnleiting.top/gtwywbkvih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangtech.top/gtegfdbqps.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenlongwang.top/gtwdrxqsbl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtgejdrrfu.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtkywlhqbu.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtjajzvznd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sweek.top/gtpfmgarwi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxuanxn.top/gtuurfkpjf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtcrgearmw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtlphxmvgu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtjxyotzij.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daxiang520.top/gtpwntgdos.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tian-w.cn/gtdgnskzbx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jiagoushi.top/gtdyezglxp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtnirzybwl.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtyvbkogin.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xylfe.cn/gtmlgtukgq.html

PHP:  array_reverse($arr);
来源：http://hz.ydjk.org.cn/gthyjuqxqa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnqzz.top/gtamfjyxgf.html

TS:   [...arr].reverse();
来源：http://hz.tian-w.cn/gtalkppdyb.html

Java: Collections.reverse(list);
来源：http://hz.jyoumei.cn/gtxxlejhvl.html

Go:   slices.Reverse(arr)
来源：http://hz.andypj.xyz/gtmerulqye.html

Ruby: arr.reverse
来源：http://hz.hysaishi.cn/gtddmonarr.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtehgdqpom.html

[D12] 查找元素下标
来源：http://hz.sysykeji.top/gtexqjphui.html

Py:   arr.index(x);  x in arr
来源：http://hz.havefunace.top/gtokhgyode.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gtfqsnilsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtrphjjmod.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtfdrvrttr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yonumen.top/gtzsyeffpf.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigufen.top/gtlvbcnibq.html

Ruby: arr.index(x)
来源：http://hz.dashuyun.cn/gtckqrmers.html

C#:   list.IndexOf(x);
来源：http://hz.shangyingyoupin.top/gtorddiqct.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtwercyejl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtmqhlwtuf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtklyzahgo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtwmczlwqk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtyebapart.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtntlobmxz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtczkgeklj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aibaodan.cn/gtlmeahpnz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangtech.top/gtnwuueebc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.c1oappe.top/gtlzwonnru.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuanzx.com/gtsftxyijh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtlsqyryqt.html

JS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtyvazxqpn.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtpauffwav.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ivvv.top/gtkylffreg.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtcpxlhmcl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gtizepybaf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhiwuduotai.top/gtsgulrwdj.html

[D15] 去重
来源：http://hz.redwolf501.top/gtrbqppsax.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtudyhlukr.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtewklyjlb.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtufpkrmgw.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtoadknhmw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtyfydvzcw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gttqfzjodx.html

Ruby: arr.uniq
来源：http://hz.zycfv.cn/gtlciiyqlw.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtwkafdaex.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtwchktbvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jianghu66.top/gtuykysama.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtbngvmzff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtrkdbgcwg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtgddzsuef.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenzaomai.com/gtycaqmmgs.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtfpomcnkn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gtfobfkaot.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtymhqgwnr.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtkrrjxtwr.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gttortsjvo.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangtech.top/gtkgmjdxiv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgufenzy.top/gtqtyadrfd.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtyzuhhprm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.vqdsnc.cn/gtpqxbrxlh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtdpuymhpr.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtditfyysh.html

C#:   list.Max();  list.Min()
来源：http://hz.cucudq.cn/gtjktjjhop.html

[D18] 扁平化嵌套数组
来源：http://hz.xylfe.cn/gtknudwvzv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.kuanghao11.cn/gtpguyinom.html

PHP:  array_merge(...$nested);
来源：http://hz.sweek.top/gtpzbxcfnc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gzhubu.top/gtjfiazgzb.html

TS:   nested.flat();
来源：http://hz.gogol.net.cn/gtucdxohyu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtmlmrrbzq.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtdfbsxyzx.html

Ruby: nested.flatten
来源：http://hz.ivvv.top/gtbvrjjdzx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtemkwjggl.html

[D19] 按字段分组
来源：http://hz.yj20258.top/gtsiefmcqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shuidangran.top/gtnfpgargu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daria6918.cn/gtbupiokoz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtokioylyi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258888.top/gtvkeookwe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtcruxqtvx.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtuanxtinv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtwzehogrf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gotoacloud.top/gtwvkswlyn.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gteuznvvjd.html

Py:   Counter(arr)
来源：http://hz.dianchejie.cn/gtzucptpvx.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtuhfmopkn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtuscspzwh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtkoxakhli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gthvwiuujv.html

Go:   // 手写 map[T]int
来源：http://hz.zhiwuduotai.top/gtmyagfryp.html

Ruby: arr.tally
来源：http://hz.guannengcc.top/gtfjvimtdw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sweek.top/gtvxeyzbbt.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gtlqlqmlkq.html

Py:   x in arr
来源：http://hz.xinyue.icu/gtrxidybhk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.quarkkingdee.top/gtsovbkrbr.html

JS:   arr.includes(x)
来源：http://hz.birdmap.top/gtunwjlcdn.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gthirswzll.html

Java: list.contains(x)
来源：http://hz.xziqi.cn/gtajmuioem.html

Go:   slices.Contains(arr, x)
来源：http://hz.cashguo.top/gtqilgbpge.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtqrnrxjlm.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtnpqnbbqp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hywenlv.cn/gtbopqlnhu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hammf.cn/gtinbfyfon.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gthorfbtiq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sxryk.cn/gtrwqlgoyh.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtjpddmwnk.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangkeji.top/gtmlhofhie.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtfeojeyob.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtvpbmdyxp.html

C#:   new List<int>(list);
来源：http://hz.fzhhl.top/gtjwljzdas.html

[D23] reduce 累积计算
来源：http://hz.bjfxy.top/gtwsczhzas.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fzhhl.top/gtlqbdyzvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtfdcskinx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtywpjqhsp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtoxcvbafe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtxkvhmzmj.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtujlmkpyq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtcfezmjxz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ivvv.top/gtpjljtgeu.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtpwtygthj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xinyue.icu/gtkrdcwgkz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.haohaochexian.top/gtlfkwgigg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxuanxn.top/gtfsbckgyc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gttstgtwdh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtwcrkuqvj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ybcxt.top/gtqjtxboql.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtklyyckhh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtjgyxzcbg.html

[D25] Set 集合去重与交并差
来源：http://hz.xuetiantiany.cn/gtisguncko.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtkygxfhij.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dianchejie.cn/gtcskwvmqc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gtyzocsnrf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtwmmkanum.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtrtdcmfiw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtozfcnupn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtbcsqhebd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aibaodan.cn/gtpfvhxnds.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtmxffrmwc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangdashe.top/gtsojbzyoo.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtrzxygfwg.html

JS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtyaraqpbi.html

TS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtrynefkhm.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtxfyenkzu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtutdfgjfs.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtbblwnenc.html

C#:   string.Join(", ", list)
来源：http://hz.yj202588.top/gtqxrmsgjg.html

================================================================================
来源：http://hz.shuidangran.top/gtnplqmatg.html

E. 字符串处理
来源：http://hz.tanke756.top/gthhyyojmm.html

================================================================================
来源：http://hz.tianlin.xyz/gtqtpvikai.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangkeji.top/gthywdsemo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinghuilouyu.cn/gtymbrpeqw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtkdezsqch.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.feifeiyinyue.top/gtmaasbyoe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtsfhttold.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtlfgcwdwz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gttbwodvle.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtpztghrgl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtsqqwufgc.html

[E02] 重复字符串
来源：http://hz.cdnleiting.top/gtzlouwrfh.html

Py:   "ab" * 3
来源：http://hz.ydzc1.top/gtabizzraq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtbickwwad.html

JS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gttclhtkkj.html

TS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtxntmskfb.html

Java: "ab".repeat(3)
来源：http://hz.wangdashe.top/gthrjrswhn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gtmflwyccm.html

Ruby: "ab" * 3
来源：http://hz.shzxlz.cn/gtrkackder.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.bjfxy.top/gtgiokhflo.html

[E03] 截取子串
来源：http://hz.tanke756.top/gtvqnfbvdf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtujohjmut.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtycedukfl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtcyaeleyx.html

TS:   s.slice(1, 4)
来源：http://hz.sweek.top/gtsebgfswg.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtxphgutue.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinqigufen.top/gtkpybjgec.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtoebfahvz.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtwpctxdio.html

[E04] 查找子串位置
来源：http://hz.feifeiyinyue.top/gtimbxqtuf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangtech.top/gtnykuzjjl.html

PHP:  strpos($s, "x");
来源：http://hz.daxiang520.top/gtglzavmwo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ehwqpu.com/gtfgcajnhy.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtqotloeau.html

Java: s.indexOf("x")
来源：http://hz.sufxvd.cn/gtfuwrwyjp.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtilavejpg.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtwnzxusna.html

C#:   s.IndexOf("x")
来源：http://hz.316326.xyz/gtjahjpkme.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xinyue.icu/gtrmsnehka.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.kuanghao11.cn/gtantxdtdu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gtndcmmojd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtyqihsndp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gtigcccmah.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gtqbrqxiwk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ywan-chungtsiang.top/gthrvjfqrb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtzkaocxbt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.haohaochexian.top/gtouwewsbr.html

[E06] 替换子串
来源：http://hz.pycfn.com/gtfrakzjkk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tianlin.xyz/gtnnyyjwai.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.vqdsnc.cn/gtbsfpkznv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtitmehypj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtkxbuimhz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtjyowqycu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtjmhuhhkb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jianghu66.top/gtjmyrptfr.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtoalqpayv.html

[E07] 按分隔符拆分
来源：http://hz.bjfxy.top/gturioqtuh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtxmilrabm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gttogltmuq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtntwvnpvh.html

TS:   s.split(",")
来源：http://hz.pycfn.com/gtlodlbopm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yuanzhike.top/gtwmnipglv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.birdmap.top/gtwedoimmd.html

Ruby: s.split(",");  s.split
来源：http://hz.chenlongwang.top/gtebwksflj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shzxlz.cn/gtioeyutwc.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtrkhdjbkd.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gtpjgccbxv.html

PHP:  implode(",", $items);
来源：http://hz.birdmap.top/gtzwmkwgla.html

JS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtxgmzckvf.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtszzrndxn.html

Java: String.join(",", items)
来源：http://hz.feifeiyinyue.top/gtxfxirlov.html

Go:   strings.Join(items, ",")
来源：http://hz.hnxiangtu.top/gtbawfwjlb.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gtmxswhphh.html

C#:   string.Join(",", items)
来源：http://hz.tanke756.top/gtuybosiin.html

[E09] 去除所有空白字符
来源：http://hz.nanxuanxn.top/gtmgoswshw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtmdulcybd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtbtsiwwmi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hnxiangtu.top/gtpglqkomd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtatmkqbev.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtgotyofib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.haohaochexian.top/gtrifvvrpg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.svipenyu.cn/gtcyukmuww.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhengqikj.top/gtniltnplb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtisiiapbe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhijiandao.cn/gtinusiupu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.snrcjt.cn/gtcyrrmjcp.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtuinbgfkb.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtmvtychdl.html

Java: String.format("%03d", 7)
来源：http://hz.aibaodan.cn/gtxemfaksb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtfverwunz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.meibo888.top/gtopfvvaku.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258.top/gtasvvvxea.html

[E11] 反转字符串
来源：http://hz.zhongyouzk.top/gtmrfjdpcv.html

Py:   s[::-1]
来源：http://hz.zhiwuduotai.top/gtnoftdhlb.html

PHP:  strrev($s);
来源：http://hz.yj20258888.top/gtrotcvdsw.html

JS:   [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtqyquidhd.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gthjptvruj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtxtffszzt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gtslhxuwgv.html

Ruby: s.reverse
来源：http://hz.guowangkeji.top/gtrnqejgjw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtahbecxwa.html

[E12] 统计某字符出现次数
来源：http://hz.ywan-chungtsiang.top/gtpsmiwldk.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtcwspixoy.html

PHP:  substr_count($s, "a");
来源：http://hz.fzhhl.top/gtlatzugyi.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtsxqbgtsq.html

TS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gtzxpghnhx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtxaxzzdjz.html

Go:   strings.Count(s, "a")
来源：http://hz.9152youxi.cn/gtpqexhnql.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gtmmcxagwb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gtltfztqtb.html

[E13] 逐字符遍历
来源：http://hz.pengpengdd.cyou/gtburgacsp.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtsjtpjssz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gogol.net.cn/gtlvgmzpcu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtajynpdhp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.meibo888.top/gtrgyjmsne.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydjk.org.cn/gtxodpcmia.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gtoaptzwmg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtbunhqmpk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258888.top/gtyvxsxhrc.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtxivhqrnj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtigtlvkdr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuxming.cn/gtxgquilvs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgufenzy.top/gtfrqcawsx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtaujgqbif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gtsnbcyqqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhixingplan.top/gtdvnzdars.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xziqi.cn/gtvupjctoa.html


<!-- 参考信息 -->