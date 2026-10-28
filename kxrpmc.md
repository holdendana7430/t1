代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xziqi.cn/gtrzljdygl.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtkvuwxned.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hfpthk.cn/gtyvzwaauv.html

Go:   append(a, b...)
来源：http://hz.meibo888.top/gtbahulggk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yonumen.top/gtyarwmwob.html

C#:   a.Concat(b).ToList()
来源：http://hz.shuidangran.top/gtcvqyselm.html

[D09] 排序（升序）
来源：http://hz.jinqigufen.top/gtgdtxnbyl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtxvamlyqz.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtlwpbvmrn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yvedp.cn/gtxlmulxwj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtltzllfje.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gtwqwdinob.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtksycstdr.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtptcxdvqi.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gteleuqihr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.birdmap.top/gtgurqacis.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgufenzy.top/gtllibvtkh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtuucqyenv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtsrkhlkut.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtyzstozvl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hfpthk.cn/gttevwxxkq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtnwuivpxq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cdnleiting.top/gtwbvtrdov.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtfjtiowlt.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtalyctwna.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guowangkeji.top/gtzhhordyp.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtgdqonmwc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.kuanghao11.cn/gtchwrtqpi.html

TS:   [...arr].reverse();
来源：http://hz.yj20258888.top/gtkrsiljbn.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtakicmakg.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtcaixxbpk.html

Ruby: arr.reverse
来源：http://hz.c1oappe.top/gtcgqbpafx.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtceojepkv.html

[D12] 查找元素下标
来源：http://hz.pengpengdd.cyou/gtnsxumvjf.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinyuanbaomall.cn/gtkfoctqyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.andypj.xyz/gtfryfyinv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtzvxscvtv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtjlblyqvt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jyoumei.cn/gtgnjmmfax.html

Go:   slices.Index(arr, x)
来源：http://hz.haohaochexian.top/gtlvxhckcw.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gtcfkuujsi.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtoyuvuwgg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.redwolf501.top/gtdivrjyfc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gtxbdgryss.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtvoyfexry.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtgwrqcxah.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ybcxt.top/gtktnudcea.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtqywvxnho.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xingfuxueyuan.xyz/gtcvkteojm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xingfuxueyuan.xyz/gtxohxqdha.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gtktqjfvbu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.meibo888.top/gtbsyvdcge.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtotgmeppr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtcjgnqfpa.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtqpggaddi.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gteoctdtvg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtllmjlnwc.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtxvmczwvo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aibaodan.cn/gtfxcuwzos.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangkeji.top/gtqwdxozte.html

[D15] 去重
来源：http://hz.fengsongda.top/gtinquuiyq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dashuyun.cn/gtytokabbc.html

PHP:  array_unique($arr);
来源：http://hz.xuetiantiany.cn/gtrgsjueiw.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtzyqbkoax.html

TS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtotvklaoe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtbedshvkm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yueranfly.top/gtbbxgvinq.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtenekvszn.html

C#:   list.Distinct().ToList()
来源：http://hz.tanke756.top/gtxdtrlrvq.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtjsukwkad.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daxiang520.top/gtibbrjsgd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cucudq.cn/gtsvnujoqm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtejigfudt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtdfbfzlhv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sufxvd.cn/gtlkayuunu.html

Go:   // 手写循环累加
来源：http://hz.sxryk.cn/gtkofidepl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gtefpfwlah.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gthcycdqhw.html

[D17] 最大值与最小值
来源：http://hz.gotoacloud.top/gthshqekom.html

Py:   max(arr);  min(arr)
来源：http://hz.zhoulong.xyz/gtlypasaox.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtuubcogwa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtscnrfhbs.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtkklltact.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shangyingyoupin.top/gtstojkymi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.9152youxi.cn/gtribupvkn.html

Ruby: arr.max;  arr.min
来源：http://hz.kuanghao11.cn/gtjghdbbqo.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtvazmdcdx.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtylrufhkl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtempgtvdi.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtjpqnisdr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hysaishi.cn/gtlgriwulb.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtppiquoaa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sxryk.cn/gtewrrdgfd.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gttfdmonwb.html

Ruby: nested.flatten
来源：http://hz.yj202588.top/gtdufikcbh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtpeonkuwz.html

[D19] 按字段分组
来源：http://hz.chenzaomai.com/gtngrbjzfq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtetfguqpz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydzc1.top/gtthrmrcko.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgufenzy.top/gtaxtrsohf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtioqvrqso.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnxiangtu.top/gtonlbwfce.html

Go:   // 手写 map[string][]T
来源：http://hz.chenlongwang.top/gtwfiyoman.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aizwys.cn/gtejhquour.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gthufyjvqr.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtpcereefe.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gtmbfkqzrj.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtdxygnjya.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtstevyjsw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shuidangran.top/gtxohuqjkl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gteyzltzxk.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258.top/gtzsvrrlre.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtehiznekb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sweek.top/gttvnwjopr.html

[D21] 判断是否包含某元素
来源：http://hz.smart0.xyz/gtuypldbog.html

Py:   x in arr
来源：http://hz.52xcode.cn/gtzmnxnroo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxuanxn.top/gtcyvgusjd.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtbulabptu.html

TS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtvdigttfh.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gtxcvgvxyp.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtedawguwf.html

Ruby: arr.include?(x)
来源：http://hz.hywenlv.cn/gtjloysogg.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtuaymvyyw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtsuiqjyhw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtfeluvkvn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.pycfn.com/gtujlliojs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtbyhveizo.html

TS:   [...arr];
来源：http://hz.c1oappe.top/gtekchibuy.html

Java: new ArrayList<>(list);
来源：http://hz.wangdashe.top/gtjjsvljsf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daria6918.cn/gtqdkwombj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ppjwa.cn/gtejfmrbzy.html

C#:   new List<int>(list);
来源：http://hz.316326.xyz/gtgfmystaz.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtekulslan.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtnulvakny.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.vqdsnc.cn/gtsbuzirwf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtrsfntkgz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtpaenxxmu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtnuadjgoi.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtxszvbvaa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtmnpmewtx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.bjfxy.top/gttsksbvzw.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtwojsxsvs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtpfqoqpsy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtkzxbwvdb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yanxiufei.cn/gtqhaquyey.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtfkkoqcvi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtzlwpjyge.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtivndpyjl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.kuanghao11.cn/gtzwjonrfd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtaclaqrgu.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtqffjtewt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pycfn.com/gtojcnhhba.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtnuhxjbjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xylfe.cn/gtvyvilkkf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtnqozqmgj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtxjibwazg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhengqikj.top/gtxwhuqazw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yvedp.cn/gtnqixrbjw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258888.top/gtjpaudffo.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtmoztmzjy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtkahdoosd.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtlnjsbmfm.html

JS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtamuyqvnm.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtljhmjlmd.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gtfhglfuvv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtcprxptxi.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtsoogragf.html

C#:   string.Join(", ", list)
来源：http://hz.vqdsnc.cn/gtlufkfupb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdjwnyeft.html

E. 字符串处理
来源：http://hz.birdmap.top/gtsceujehh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtavhwdymj.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtueczfpqe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtyzzkzrxd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtklfhhmsd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtdstyapts.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtqlgygark.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.andypj.xyz/gtgmvinhwp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gthtbdsrxh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtshobvfar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gtuqwvglqf.html

[E02] 重复字符串
来源：http://hz.shanyushiyangkeji.top/gtrqofmgiz.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtnzrdvrby.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhijiandao.cn/gtcbyebcwx.html

JS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtpjrhuxhw.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtwbvreibg.html

Java: "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtacsejgci.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jianghu66.top/gtwdajqzhy.html

Ruby: "ab" * 3
来源：http://hz.9152youxi.cn/gtbvkrmswd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gtqsrlngvz.html

[E03] 截取子串
来源：http://hz.tanke756.top/gtaxkdgnyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtdmuavjto.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtfcswqbnp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtjkexabzs.html

TS:   s.slice(1, 4)
来源：http://hz.ehwqpu.com/gtygufwzte.html

Java: s.substring(1, 4)
来源：http://hz.yj20258.top/gtlgnnrvni.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhijiandao.cn/gtbvzzrtrr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenjidiqi.icu/gtuogwfxaw.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtmawanadr.html

[E04] 查找子串位置
来源：http://hz.sufxvd.cn/gtkhglmdpn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtfuiydsec.html

PHP:  strpos($s, "x");
来源：http://hz.zhixingplan.top/gtgnphpflr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gtjfgtjpnh.html

TS:   s.indexOf("x")
来源：http://hz.c1oappe.top/gtcufzzrdc.html

Java: s.indexOf("x")
来源：http://hz.gogol.net.cn/gtcrpksfhj.html

Go:   strings.Index(s, "x")
来源：http://hz.daria6918.cn/gtspbxslym.html

Ruby: s.index("x")
来源：http://hz.sysykeji.top/gtoldveger.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gtqevmrifi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pycfn.com/gtheeahxsy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hongshengwenyu.top/gtwyskdulg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dashuyun.cn/gtbfubunbh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtjmwimhld.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnxiangtu.top/gtjtuolqoq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gtiuhofylj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtebyimofx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258888.top/gtycoxiyqy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxuanxn.top/gtlrnxwdvj.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtplniuhbe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.iojbl.cn/gtpcidwnzx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtelvbkgyn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtmjpbcdsk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtnfcdarov.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtjpbvoekr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zdqjudy.top/gtgsyrmcla.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgufenzy.top/gtwfmdxgjf.html

C#:   s.Replace("a", "b")
来源：http://hz.aizwys.cn/gtmyneezhs.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtshcjolut.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.andypj.xyz/gtishbclyg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtvhbxccts.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuanzx.com/gtuthkdwda.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gtygnczvtn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuetiantiany.cn/gtqybjckaa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.0kj1m.cn/gtfiyprvcs.html

Ruby: s.split(",");  s.split
来源：http://hz.dianchejie.cn/gtdzsnwuef.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtgdpwgmcz.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtvvznpfaf.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtdjwrtwmy.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtmzmnrgnm.html

JS:   items.join(",")
来源：http://hz.guannengcc.top/gtmvmglveb.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gtvgjwbnjr.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtsbbftkuu.html

Go:   strings.Join(items, ",")
来源：http://hz.yj202588.top/gtcuxjtzwl.html

Ruby: items.join(",")
来源：http://hz.birdmap.top/gtchpdljve.html

C#:   string.Join(",", items)
来源：http://hz.haohaochexian.top/gtdyeoukcb.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtmhtpyolk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gtzbmoiwrt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigfzy.top/gtsqmlijpi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtetmtwbkc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtpobhmfvl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cucudq.cn/gtzemgvbzk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.52xcode.cn/gtwadabkki.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtwnplcrmr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yonumen.top/gtefrhehwv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtznqeqxup.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sxryk.cn/gtmnkckthc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhiwuduotai.top/gtqropmquk.html

JS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtmzoyrxkp.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtpgwcecqw.html

Java: String.format("%03d", 7)
来源：http://hz.nwbrower.top/gtwkafxtsh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hammf.cn/gteifmfcrh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtdqryqwxc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gtqjdrncnf.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtilgltexz.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtoeigaoem.html

PHP:  strrev($s);
来源：http://hz.zdqjudy.top/gtxhqswbql.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtxsvwvydp.html

TS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtfyfbepkf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhiwuduotai.top/gtfybakrtv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tanke756.top/gtsufzqhyd.html

Ruby: s.reverse
来源：http://hz.guannengcc.top/gtpznhznqu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtkdyhhpxw.html

[E12] 统计某字符出现次数
来源：http://hz.guowangkeji.top/gtihiloxsr.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gtetnffcru.html

PHP:  substr_count($s, "a");
来源：http://hz.jinghuilouyu.cn/gtpmccwojy.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtnwzjjduc.html

TS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gturvpqxzw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dianchejie.cn/gtxagcpvqg.html

Go:   strings.Count(s, "a")
来源：http://hz.chenjidiqi.icu/gtdnccslay.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtiuzzyrhh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydjk.org.cn/gtmcmbzvmn.html

[E13] 逐字符遍历
来源：http://hz.iojbl.cn/gtzfjhpkvi.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtlfkoyscq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinyuanbaomall.cn/gtpqojogyr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gttuqkvwun.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gtdvsaxblp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gtaeihrnhn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.52xcode.cn/gtmlwoqtit.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtbexwyvvc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cqqwz.cn/gtandovdsv.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gtraoafpel.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtrudsczrt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxinkj.top/gtfnfgsjqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtasdkobdd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtiyckzytd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtqjsxwwlg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xinyue.icu/gtafknfpoo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigfzy.top/gtojbegclp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gtlpzgddta.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhengqikj.top/gtyguyffwi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shangyingyoupin.top/gtqvehvmio.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhixingplan.top/gtjmzzfqmp.html


<!-- 参考信息 -->