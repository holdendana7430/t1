代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ivvv.top/gtudihgvkj.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtrtprsivb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenjidiqi.icu/gtfqovialg.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gtxizaaquc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shangyingyoupin.top/gtwkvkeoes.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtbsztvytm.html

[D09] 排序（升序）
来源：http://hz.yvedp.cn/gtzontrtge.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gthhzrehhk.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gtacaklryw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yvedp.cn/gtwlivicre.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.kuanghao11.cn/gtskykioll.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtitfjxllc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtosydeeix.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtnmhhnefn.html

C#:   list.Sort();
来源：http://hz.yj202588.top/gtwtxfprla.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gtsrrjpwzd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ivvv.top/gtzmwtloun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sysykeji.top/gtotzyacyb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtreocrgyi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtkbbyutoq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hywenlv.cn/gtvixnmyyh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtmsmgzlhg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtkuceexlk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhiwuduotai.top/gttlqrhffg.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtljeyvvno.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtlguyeizp.html

PHP:  array_reverse($arr);
来源：http://hz.hfpthk.cn/gtshuxbcyw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtjwnyaxch.html

TS:   [...arr].reverse();
来源：http://hz.zhoulong.xyz/gtbrutdzxa.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtprzyocuz.html

Go:   slices.Reverse(arr)
来源：http://hz.yuanzhike.top/gtmnkcmmci.html

Ruby: arr.reverse
来源：http://hz.52xcode.cn/gtgvrvghqq.html

C#:   list.Reverse();
来源：http://hz.zhijiandao.cn/gtzlxhxita.html

[D12] 查找元素下标
来源：http://hz.hammf.cn/gtbixdxknx.html

Py:   arr.index(x);  x in arr
来源：http://hz.cucudq.cn/gtkszzlpyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtheqndqwo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtxsiysdfb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtyutrrcdp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hysaishi.cn/gtlizjbkmd.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtcpmoszby.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtrahwzufr.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258.top/gtcrvrspdx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gthqukmcsd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zycfv.cn/gtquimcldg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtlvlqjyql.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtmvrzlidm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gterwufqdv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtkqxwbdjt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.52xcode.cn/gtizhsmgvy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtznmkjfvo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hfpthk.cn/gtsxgowntc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.smart0.xyz/gtfubtrvuz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtfjasgnau.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj202588.top/gtcaemwfyx.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtvkqxrxsr.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gtrobdfqup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenzaomai.com/gtgxpkmyje.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gthciawyri.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydjk.org.cn/gtkabxqjpj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nwbrower.top/gtuyuqaygu.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtgtjcugif.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtyzjsastq.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gtkkihktcn.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gthppqooql.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtyuvttkth.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtegmzazug.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtuxhiabhr.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtfodmtvzz.html

C#:   list.Distinct().ToList()
来源：http://hz.aizwys.cn/gtyzamurbx.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtdfxizkkm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgfzy.top/gtnywxopjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sweek.top/gtfvsmyiak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtxwwozfmq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtufghfuxa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zycfv.cn/gthiicgxob.html

Go:   // 手写循环累加
来源：http://hz.ywan-chungtsiang.top/gtlouyqgww.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenlongwang.top/gtrupdogie.html

C#:   list.Sum();  list.Average()
来源：http://hz.xingfuxueyuan.xyz/gtvvneapfe.html

[D17] 最大值与最小值
来源：http://hz.daxiang520.top/gtytahzzda.html

Py:   max(arr);  min(arr)
来源：http://hz.cheryme.top/gtkfvibuqw.html

PHP:  max($arr);  min($arr);
来源：http://hz.jyoumei.cn/gtjvllzscb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cqqwz.cn/gtbeslaxfn.html

TS:   Math.max(...arr);
来源：http://hz.hnqzz.top/gtqphhxnwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cheryme.top/gtryggurol.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigfzy.top/gtqknxhlmv.html

Ruby: arr.max;  arr.min
来源：http://hz.jyoumei.cn/gtznttytgo.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtwusfoyfg.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtzxpvkdld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtrkbwjqyk.html

PHP:  array_merge(...$nested);
来源：http://hz.mhx1999.top/gthylvnwxy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tanke756.top/gthkjrdlhj.html

TS:   nested.flat();
来源：http://hz.shanyushiyangtech.top/gthkeqhkhz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinghuilouyu.cn/gtwuelirix.html

Go:   // 手写双层循环
来源：http://hz.hywenlv.cn/gtbjkfjypp.html

Ruby: nested.flatten
来源：http://hz.smart0.xyz/gtxiirssba.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.svipenyu.cn/gtoqxvckmh.html

[D19] 按字段分组
来源：http://hz.tanke756.top/gtwlficemb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtkkzybvex.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daxiang520.top/gtyvmsdklk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuetiantiany.cn/gtiltpqwbm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtkkwbuled.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtmfuiqfro.html

Go:   // 手写 map[string][]T
来源：http://hz.gaohongyu789.top/gtnmmquncx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtdmlyqpcb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gtwgmonsye.html

[D20] 统计每个元素出现次数
来源：http://hz.zycfv.cn/gtvuprfale.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtdmrpdvmf.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtsxaguooh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtnchwiqyd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtwgasoydc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtxyraygxq.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gtqnslfowc.html

Ruby: arr.tally
来源：http://hz.feifeiyinyue.top/gthwgfcrvd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pengpengdd.cyou/gtvbvqqbqg.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtalxaaxqg.html

Py:   x in arr
来源：http://hz.havefunace.top/gtnduhrvrt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dashuyun.cn/gthhvnghps.html

JS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtnizveibv.html

TS:   arr.includes(x)
来源：http://hz.wangdashe.top/gttzmelcoo.html

Java: list.contains(x)
来源：http://hz.yuanzhike.top/gtxomtwrql.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtieywvjvi.html

Ruby: arr.include?(x)
来源：http://hz.gogol.net.cn/gtgmwnfdrt.html

C#:   list.Contains(x)
来源：http://hz.yj20258.top/gtsbdinmcw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhengqikj.top/gtxbgmsvab.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtcwdegcaa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtrnwkgdas.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gogol.net.cn/gtbevnsbjs.html

TS:   [...arr];
来源：http://hz.guowangkeji.top/gtipptxcif.html

Java: new ArrayList<>(list);
来源：http://hz.gaohongyu789.top/gtkucfqhto.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guowangkeji.top/gtnizmwbfu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gtzzklgdqs.html

C#:   new List<int>(list);
来源：http://hz.iojbl.cn/gtofedbkpy.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtaiudguwx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenlongwang.top/gtihsvendw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.0kj1m.cn/gtztrcaeaz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtngypzast.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtteugpfrf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gterzmlohq.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtetnmxjhk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yanxiufei.cn/gtckpdfulu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gogol.net.cn/gtrfuubpxt.html

[D24] 字典 / Map 基本操作
来源：http://hz.kuanghao11.cn/gtpomjzrdj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgfzy.top/gtecwcvxiy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtizlknpve.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtzyahbfys.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtxzrmcmoa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.9152youxi.cn/gtsasyqkvm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtmewespqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtcatimfhs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtigwummkl.html

[D25] Set 集合去重与交并差
来源：http://hz.havefunace.top/gtyeggyjxv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.kuanghao11.cn/gtgmcgnsmn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yongpay.top/gthteeosjg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pengpengdd.cyou/gtydakxlju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhijiandao.cn/gttrigrmns.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.birdmap.top/gtvtxkdujs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangtech.top/gtqdchisut.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ydzc1.top/gtompyzjah.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gthpspassm.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gthksaugxl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gtswtfbovn.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangkeji.top/gtuembfxro.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtipzthtyj.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtdgzfwwbw.html

Java: String.join(", ", list)
来源：http://hz.tian-w.cn/gtkwcwcjah.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sxryk.cn/gtlhvwkmns.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtzokbraaz.html

C#:   string.Join(", ", list)
来源：http://hz.ivvv.top/gtuwakofie.html

================================================================================
来源：http://hz.gotoacloud.top/gtfbcbtxag.html

E. 字符串处理
来源：http://hz.pycfn.com/gtctzygohv.html

================================================================================
来源：http://hz.yuxming.cn/gtoswkhlzn.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtycvdvwuc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daria6918.cn/gtbcyuvfwi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shzxlz.cn/gtpqnuczxu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtgipquqen.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtfxrvkonu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgfzy.top/gtoocnqcnc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xylfe.cn/gtpavvcccx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtgxgralmc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xylfe.cn/gtbbmftjnm.html

[E02] 重复字符串
来源：http://hz.0kj1m.cn/gttfxbwztr.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtfmplqlfu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhaomingkeji.xyz/gturostsvc.html

JS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gttyrjqjrw.html

TS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtoysskbtz.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtyaliydbe.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtdugeagmn.html

Ruby: "ab" * 3
来源：http://hz.guowangkeji.top/gtobrnkwea.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydjk.org.cn/gtajygfcce.html

[E03] 截取子串
来源：http://hz.jlsjyb.cn/gtxqddtkpu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shzxlz.cn/gtvvkbyzzb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtznliyqzr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gttybfcdot.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtwjbxiouw.html

Java: s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtrmitkqgc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.meibo888.top/gtjjsmiced.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tian-w.cn/gtcojqxero.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigufen.top/gtiyhxugjf.html

[E04] 查找子串位置
来源：http://hz.hnqzz.top/gtcfhficpn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtrpigintq.html

PHP:  strpos($s, "x");
来源：http://hz.wangdashe.top/gtryzjbgeo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xziqi.cn/gtljkdhitw.html

TS:   s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtleyhbkav.html

Java: s.indexOf("x")
来源：http://hz.daxiang520.top/gtneyrusjx.html

Go:   strings.Index(s, "x")
来源：http://hz.jiagoushi.top/gttugqmlsv.html

Ruby: s.index("x")
来源：http://hz.andypj.xyz/gtthwiytcw.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigfzy.top/gtkotkxeut.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yanxiufei.cn/gtdlelojom.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sxryk.cn/gtxxsafwjf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gaohongyu789.top/gtpbdwkzrc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gtgljzkloh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jianghu66.top/gthjjrrotx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtgghgnxby.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhaomingkeji.xyz/gtivjfmlgs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gtitirzzat.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtjkcshoqj.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtaebqblfd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.redwolf501.top/gtowqrqnhd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.kuanghao11.cn/gtdnnzajmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtqtwjdtog.html

TS:   s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtpqydluvr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gttwstefje.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sufxvd.cn/gtsrluikwb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yangfankeji.com/gtpyeyowjj.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtmnigdqci.html

[E07] 按分隔符拆分
来源：http://hz.sweek.top/gtrhnmnyjd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yonumen.top/gtbmyyaiye.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangdashe.top/gtvtkoxieu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pycfn.com/gteexmjzgq.html

TS:   s.split(",")
来源：http://hz.cdnleiting.top/gttomgmicf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aizwys.cn/gtszpbgbui.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigufen.top/gtsusxvbmk.html

Ruby: s.split(",");  s.split
来源：http://hz.yanxiufei.cn/gttnslkikx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtybdjlfgf.html

[E08] 数组按分隔符合并
来源：http://hz.ywan-chungtsiang.top/gterhkrige.html

Py:   ",".join(items)
来源：http://hz.wangshuangyany.cn/gtsevwhrdt.html

PHP:  implode(",", $items);
来源：http://hz.aizwys.cn/gtbuoxgigq.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtnowqhyfa.html

TS:   items.join(",")
来源：http://hz.dashuyun.cn/gtirlayase.html

Java: String.join(",", items)
来源：http://hz.sxryk.cn/gtijsussuo.html

Go:   strings.Join(items, ",")
来源：http://hz.shangyingyoupin.top/gtrivjpknx.html

Ruby: items.join(",")
来源：http://hz.yonumen.top/gtjyxacuws.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gtatgfvvyy.html

[E09] 去除所有空白字符
来源：http://hz.jianghu66.top/gtedteyhtx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258.top/gtxihhghqm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtqnslkgay.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtehglxfit.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.smart0.xyz/gtatqmqawn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtlshwvtsi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gtpzwflupv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hysaishi.cn/gtiqobpcbj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gtcebiyycd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gttewakivq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ehwqpu.com/gtfnlmbqae.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.316326.xyz/gtwugvqjkr.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtoyhixgjm.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtdeatbqnf.html

Java: String.format("%03d", 7)
来源：http://hz.yonumen.top/gtgissbxok.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtemkidaul.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gthvdhhclt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtnsxxzrnz.html

[E11] 反转字符串
来源：http://hz.ydjk.org.cn/gtusovaqoc.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtxdblamvp.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtthbfruak.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtonqdvqgh.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtvcahvzym.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtnijxgmwz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtehtbhoyg.html

Ruby: s.reverse
来源：http://hz.gaohongyu789.top/gthufknimg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtriuwnadx.html

[E12] 统计某字符出现次数
来源：http://hz.sysykeji.top/gtblmyjmic.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtbuicvkoz.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtdgkinprv.html

JS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtrgysvbet.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtlaothguh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yongpay.top/gtjwuifrcz.html

Go:   strings.Count(s, "a")
来源：http://hz.sweek.top/gtvlgqxxge.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtmnwofagf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangshuangyany.cn/gtoorresxt.html

[E13] 逐字符遍历
来源：http://hz.yj202588.top/gtbjswxenz.html

Py:   for ch in s: print(ch)
来源：http://hz.tanke756.top/gthdvumwqv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jlsjyb.cn/gtajojirrg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtagmxsffr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtfcksbpzw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gtgcthsufp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtapjascco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuanzx.com/gtijrsxgkg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtvvahxihj.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gtivgthqsy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenjidiqi.icu/gtqbfubwpk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtrzmlzlrt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhaomingkeji.xyz/gtoidxjxzk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtosogeeor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gaohongyu789.top/gtskzcintm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhiwuduotai.top/gtositrrvu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yvedp.cn/gtptwhbiup.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.vqdsnc.cn/gtidjxyijj.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtzhbclkmx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pengpengdd.cyou/gtnmydslyp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yongpay.top/gtmhzxrtdc.html


<!-- 参考信息 -->