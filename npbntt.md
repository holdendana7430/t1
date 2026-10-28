代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinghuilouyu.cn/gtybqahqzu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.iojbl.cn/gtitjwpcwc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cashguo.top/gtexpbgzkb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtakxgkrce.html

[D11] 反转数组
来源：http://hz.hammf.cn/gtayebculd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtesgaqqyn.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gtgturphwm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cdnleiting.top/gthgcpmkbg.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtiltvkptr.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtodiaskaz.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtbojzxgji.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtoaefjaog.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtszununef.html

[D12] 查找元素下标
来源：http://hz.smart0.xyz/gtasvgfgjf.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gtzhqojgox.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guowangkeji.top/gtwsandoeg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtyjkobfpf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gttywzcltm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtivbbrisv.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtivlpwuuv.html

Ruby: arr.index(x)
来源：http://hz.tian-w.cn/gtlsqanuif.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtxozfijta.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydzc1.top/gtdwxpqqaz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tianlin.xyz/gtlrilanxa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtjhkjridb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtedxrfuuj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtbyuqdzdi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.havefunace.top/gtlnlgbwqr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtslvmvdub.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cheryme.top/gtynejvcym.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.guannengcc.top/gtclliruhg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gterjyarjf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtsdwtizwv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtppwyhmlo.html

JS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtreecfkse.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtohhplxku.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sweek.top/gtmorjoohs.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtxfafsunn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtydwiylae.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtwktibqhg.html

[D15] 去重
来源：http://hz.52xcode.cn/gtugpcujlx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtnesrholc.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtkgcqphac.html

JS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gttlczpwuf.html

TS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtavsiwtvj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtwhpkdues.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtabqgboak.html

Ruby: arr.uniq
来源：http://hz.svipenyu.cn/gtaynahkkm.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigfzy.top/gtmylteexx.html

[D16] 求和与平均值
来源：http://hz.nanxinkj.top/gtefkfdppo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtzbitonlu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.wangdashe.top/gtztdnrhvv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtqpiunulz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtrdvrctvk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jianghu66.top/gtaysaiqfn.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtzmtvmyjq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jyoumei.cn/gtzaofbhmq.html

C#:   list.Sum();  list.Average()
来源：http://hz.daria6918.cn/gtsryfuyvi.html

[D17] 最大值与最小值
来源：http://hz.yuxming.cn/gtgywmzhri.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtkiqmtwxd.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangdashe.top/gtfnnjmmrl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtfpoingti.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gthhazvsgd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gttjkgvtyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhijiandao.cn/gtygzxmaay.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtawajmznd.html

C#:   list.Max();  list.Min()
来源：http://hz.sweek.top/gtnzepbilv.html

[D18] 扁平化嵌套数组
来源：http://hz.zhongyouzk.top/gtvsiwnkns.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.9152youxi.cn/gtdsouqiax.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gteaceczmo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fzhhl.top/gttzthssip.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtnhjronrp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.quarkkingdee.top/gtpbogfcvp.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtzvivdzqj.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtvlmrbfkq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtcdwahbwo.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtninmptiw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jlsjyb.cn/gtbzwuafji.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtzyhnsegj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sweek.top/gthnitymqq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtqsdzzptr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnqzz.top/gtdczwcxvm.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gtvrfjdzlf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tanke756.top/gtqytqrxxr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtrzbotwim.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtzpgeljtf.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtvizfknqj.html

PHP:  array_count_values($arr);
来源：http://hz.cdnleiting.top/gtuaetnwaw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtukefuvtm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtgddsbdan.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtfnjeovst.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtctxfmngs.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtydfuqmrl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dianchejie.cn/gtsshkyuov.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtwsemigpv.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtascwarze.html

PHP:  in_array($x, $arr, true);
来源：http://hz.316326.xyz/gtizsqbjoj.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtvrtpbmrz.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtwnyeafhh.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gthephaybx.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gttqbbelnc.html

Ruby: arr.include?(x)
来源：http://hz.xuetiantiany.cn/gtkciwotvj.html

C#:   list.Contains(x)
来源：http://hz.yanxiufei.cn/gteoqaknqp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pengpengdd.cyou/gtmvdtydzz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuetiantiany.cn/gtwmsxpjne.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fzhhl.top/gtametcyzu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gtzltthxld.html

TS:   [...arr];
来源：http://hz.jinqigfzy.top/gtciqdiykg.html

Java: new ArrayList<>(list);
来源：http://hz.316326.xyz/gtxmhvynrj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hammf.cn/gtpprvjdvg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hfpthk.cn/gtarwrqkfn.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtjmdcownh.html

[D23] reduce 累积计算
来源：http://hz.aibaodan.cn/gtvoxhbvko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hongshengwenyu.top/gtgeraoozh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnxiangtu.top/gtzsweuqwh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtxdillqus.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtyequhdla.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtawvoyjkf.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gteqkydkwc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtwlxnhlwv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.feifeiyinyue.top/gtfjifipfk.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gtrtemaxqe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gthgipocdz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gttobqcjzf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnxiangtu.top/gtcwkevcql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtfjidizmh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtcwmyabna.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtjwhuflws.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.birdmap.top/gthhzylygp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yonumen.top/gtfqhebrtg.html

[D25] Set 集合去重与交并差
来源：http://hz.iojbl.cn/gtgkrylrob.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtaqacdtco.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenlongwang.top/gtiggxhauv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tanke756.top/gtljbmdhsh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtdesdiqqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guowangkeji.top/gtntmxgios.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhongyouzk.top/gtndkecqsh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtbjzavxvq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gteqkbfnvp.html

[D26] 数组转字符串
来源：http://hz.tianlin.xyz/gtpxyiklbs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.quarkkingdee.top/gtygrrkuqy.html

PHP:  implode(", ", $arr);
来源：http://hz.hammf.cn/gtnjauwwxd.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtiwsshsvy.html

TS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gttsmhtyes.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gtslptnbrj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ppjwa.cn/gthdnysdlm.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtubvdtusc.html

C#:   string.Join(", ", list)
来源：http://hz.ppjwa.cn/gtwppvmwmp.html

================================================================================
来源：http://hz.guowangkeji.top/gtmzehxsiy.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gthqjjpfba.html

================================================================================
来源：http://hz.hammf.cn/gtgwqenkqx.html

[E01] 拼接字符串
来源：http://hz.jiagoushi.top/gtqwinrgjq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj202588.top/gtgnrzwqjc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tanke756.top/gtevdhdtac.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtvrboieqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.svipenyu.cn/gtqwmtsvwy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigfzy.top/gtixyfeewh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aibaodan.cn/gtrpvjygkp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtjboaqvhk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtesioixmm.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtegatxzdf.html

Py:   "ab" * 3
来源：http://hz.aibaodan.cn/gtpciwisck.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gtoeqxooqw.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtmnmrfwei.html

TS:   "ab".repeat(3)
来源：http://hz.316326.xyz/gttlboxbra.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtgrfpqktt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aizwys.cn/gtronmouee.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gtebbkkyzv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.iojbl.cn/gtrewefqrt.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtnrfwnhjl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gthjsenpse.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtgkjcbupj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangdashe.top/gtpdvthuqj.html

TS:   s.slice(1, 4)
来源：http://hz.bjfxy.top/gtycgaqaka.html

Java: s.substring(1, 4)
来源：http://hz.yj202588.top/gtxselsmoz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gzhubu.top/gtrafqaiha.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jiagoushi.top/gtfsrkooju.html

C#:   s.Substring(1, 3)
来源：http://hz.zhiwuduotai.top/gtbuxgnzum.html

[E04] 查找子串位置
来源：http://hz.jqgufenzy.top/gtihwzplhl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtkccaqydi.html

PHP:  strpos($s, "x");
来源：http://hz.iojbl.cn/gtjejoneup.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtlinnguna.html

TS:   s.indexOf("x")
来源：http://hz.shzxlz.cn/gtvcepmhuh.html

Java: s.indexOf("x")
来源：http://hz.yangfankeji.com/gtkiiorzxd.html

Go:   strings.Index(s, "x")
来源：http://hz.feifeiyinyue.top/gtflhafgmf.html

Ruby: s.index("x")
来源：http://hz.snrcjt.cn/gtsrsqeuod.html

C#:   s.IndexOf("x")
来源：http://hz.guannengcc.top/gtmxjxhldq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtzpulvgsv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sysykeji.top/gtmgquoyrc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtalcimtsq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtyidyeppz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gtvvstrliz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtuyiibybx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.pengpengdd.cyou/gtjiqplwgy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258888.top/gtibvufbnc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hammf.cn/gthwqfpotx.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtcpriwpyk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigufen.top/gtbxuneiis.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgufenzy.top/gtutsygkea.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtkedlubva.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtxnebysne.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtivkkuihr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gotoacloud.top/gtptrsnzpx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.c1oappe.top/gtnjrlnvhg.html

C#:   s.Replace("a", "b")
来源：http://hz.aizwys.cn/gtqmklrehs.html

[E07] 按分隔符拆分
来源：http://hz.sxryk.cn/gtpbglvrqw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.snrcjt.cn/gtcwpvsxcu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtrwykhcor.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.iojbl.cn/gtvwodwrji.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gtafkjmnky.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gtjdqpnajc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxinkj.top/gtxhykgipw.html

Ruby: s.split(",");  s.split
来源：http://hz.zhiwuduotai.top/gthmezcfvr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhongyouzk.top/gtvnpotnxp.html

[E08] 数组按分隔符合并
来源：http://hz.shangyingyoupin.top/gtylterrhf.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtntbvxdph.html

PHP:  implode(",", $items);
来源：http://hz.hammf.cn/gtglgpuntr.html

JS:   items.join(",")
来源：http://hz.yj20258.top/gtubnuslan.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtqblexicq.html

Java: String.join(",", items)
来源：http://hz.zycfv.cn/gtfegblmki.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtcetlowsa.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtcygdrwir.html

C#:   string.Join(",", items)
来源：http://hz.xuanzx.com/gtrjanqbhj.html

[E09] 去除所有空白字符
来源：http://hz.pengpengdd.cyou/gtmtjozmrm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtnkfjdnze.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ivvv.top/gtsoqwrudm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtbrulxlzs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtpohxopur.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuanzhike.top/gtsusgazrg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gaohongyu789.top/gtiaglclck.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gogol.net.cn/gtxhbkwtno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhijiandao.cn/gtbrbfnvip.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydjk.org.cn/gthprnyrum.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guannengcc.top/gtfziqlkwq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fengsongda.top/gtpdaaqxai.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtezreasyk.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtihyfqbra.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtinrvrfbv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhoulong.xyz/gtfnorshje.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtuhhkpxze.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sxryk.cn/gtedqnnsem.html

[E11] 反转字符串
来源：http://hz.zhiwuduotai.top/gtbmwznowf.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtsfrteaxj.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtwirbodoa.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtqtsrqqju.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gttqmyquas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ybcxt.top/gtsghjitoy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cheryme.top/gtdmhvhgon.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtpuipeeie.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtihwubkce.html

[E12] 统计某字符出现次数
来源：http://hz.cheryme.top/gtmpxaznxe.html

Py:   s.count("a")
来源：http://hz.yuanzhike.top/gtrfxzdzer.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gthxoponmz.html

JS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtnwmbsmza.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gthbircgoz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtdymynpzv.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtpemhixwq.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtymhvmrmn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtrwlbaloi.html

[E13] 逐字符遍历
来源：http://hz.fengsongda.top/gtoisatxlv.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtyiryfqyz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nwbrower.top/gtfbuzjcgd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.meibo888.top/gtifihlgcd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtpaumcllm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtrpmpkewy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtvaoksgkv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnxiangtu.top/gtojkjmgei.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yangfankeji.com/gtzatiamkd.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtvcfnnjcv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtnhksgqao.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gtpyvttilr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydzc1.top/gtcwaedget.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ivvv.top/gtfirdabmu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtrtqcdehe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtzsxlqvda.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.redwolf501.top/gtpdljcbcy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xinyue.icu/gtabouxvxi.html

[E15] HTML 转义 / 反转义
来源：http://hz.ppjwa.cn/gtfazwnsny.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cdnleiting.top/gtykdksrfl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhaomingkeji.xyz/gtxiphnkex.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtmrjezrbe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhixingplan.top/gtwhyfyfug.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jiagoushi.top/gtfozxvuap.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.bjfxy.top/gtimftzuoy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtwmihwnnq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtbhvfxahb.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtufvjatsp.html

Py:   f"{1234567:,}"
来源：http://hz.nanxuanxn.top/gtqwgvpcfn.html

PHP:  number_format(1234567);
来源：http://hz.dashuyun.cn/gtrxgnyium.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtyvlkadsg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtbnhoyhqz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sysykeji.top/gthtifgemu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtewivkrds.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ppjwa.cn/gtcrergzvv.html

C#:   1234567.ToString("N0")
来源：http://hz.yuanzhike.top/gtxdbuxyve.html

[E17] 首字母大写
来源：http://hz.xuanzx.com/gtdymnwocc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shuidangran.top/gtcscbfxub.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sweek.top/gtfcxqfluw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtfkhkilxu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtlgmdfqxh.html


<!-- 参考信息 -->