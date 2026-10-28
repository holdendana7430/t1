代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pycfn.com/gtlijelvlp.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtpgwxpxlq.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gtaaakqnnn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gaohongyu789.top/gtijoxfugi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigufen.top/gtkbfncahr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtohhjutqb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtnrvyylqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtbfwshydj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenjidiqi.icu/gtsovlgjrr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.vqdsnc.cn/gtbvuzdupx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhongyouzk.top/gtqnymukzb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtbvtrriov.html

[D11] 反转数组
来源：http://hz.fengsongda.top/gtzangyaxo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtbrvmokhz.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gteaqmiwhc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gtztygntyx.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtjudwujlk.html

Java: Collections.reverse(list);
来源：http://hz.dianchejie.cn/gtivzzwcoa.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtjlccqnko.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtcnhqrwyl.html

C#:   list.Reverse();
来源：http://hz.0kj1m.cn/gtojnnmdmn.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gtwzhuqbkb.html

Py:   arr.index(x);  x in arr
来源：http://hz.aizwys.cn/gtpwhnqxrt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtnbujodlc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtqhxesbfh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtpcorrbzs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtyewezmlv.html

Go:   slices.Index(arr, x)
来源：http://hz.chenlongwang.top/gtsbhwnwre.html

Ruby: arr.index(x)
来源：http://hz.cashguo.top/gtmcsxobri.html

C#:   list.IndexOf(x);
来源：http://hz.hfpthk.cn/gtfxnnkvja.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtpfsscyir.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yangfankeji.com/gtufkkbdgq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtidohwgvq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtspanjlsp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtwidmdasz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtqjlswtrc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydzc1.top/gtlfszwbej.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yangfankeji.com/gtxddseecq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtgjbquuxu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xylfe.cn/gtfjvctblz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtwtkiiimn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zdqjudy.top/gtnkzddlog.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtdllnzafz.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtyvvgkfed.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgufenzy.top/gtjwtegkyd.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtqdyntfdr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtfwafvsnd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtehdwarli.html

[D15] 去重
来源：http://hz.andypj.xyz/gtxsaykzyv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtintdftkm.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtxnbguhzf.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtlzfuzkly.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtlyctetln.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gtulifjszt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtisfbsfkn.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtveobmvqk.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtusoikalb.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtkbihujxb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258888.top/gtzxiwgvqg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtvzvafwpp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtcnlfwjhd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yangfankeji.com/gtylsnxcmv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtbnayutpy.html

Go:   // 手写循环累加
来源：http://hz.xuetiantiany.cn/gtfojztyss.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daria6918.cn/gtwbedrpec.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtleiugcxc.html

[D17] 最大值与最小值
来源：http://hz.hywenlv.cn/gtuemsljwk.html

Py:   max(arr);  min(arr)
来源：http://hz.zhengqikj.top/gtljhtwspk.html

PHP:  max($arr);  min($arr);
来源：http://hz.yangfankeji.com/gtpdtbruav.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shangyingyoupin.top/gtauugdxoy.html

TS:   Math.max(...arr);
来源：http://hz.ivvv.top/gtigmhyqjl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtdzuopnmy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gtwgnasrpg.html

Ruby: arr.max;  arr.min
来源：http://hz.yongpay.top/gtkpsmqnfc.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtmjsvlftf.html

[D18] 扁平化嵌套数组
来源：http://hz.wangdashe.top/gteiyggpwf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtlznngwac.html

PHP:  array_merge(...$nested);
来源：http://hz.xingfuxueyuan.xyz/gtwtrbwfla.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xylfe.cn/gtetapvskv.html

TS:   nested.flat();
来源：http://hz.yangfankeji.com/gtsmfasgdd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jiagoushi.top/gtpakvhljz.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gtdaxobeka.html

Ruby: nested.flatten
来源：http://hz.pengpengdd.cyou/gtbsnmogxe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenjidiqi.icu/gtjpfrbduq.html

[D19] 按字段分组
来源：http://hz.cdnleiting.top/gtnkqlowat.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtyfulcemp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtuwlrzcky.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtvltzmrmu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtlurdijux.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtuqjnnfej.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtemytpxlh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yueranfly.top/gtjytxhseb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ybcxt.top/gtmjuixfkd.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtgpxfvcdl.html

Py:   Counter(arr)
来源：http://hz.xingfuxueyuan.xyz/gtmcijlgxp.html

PHP:  array_count_values($arr);
来源：http://hz.bjfxy.top/gtwdxcgnnd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtjyevmxwr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtbbjfmfcv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jianghu66.top/gtxjizwsqs.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gtibwqcsqs.html

Ruby: arr.tally
来源：http://hz.aibaodan.cn/gtemzhqtob.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gtcxgjinub.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gttmkyuxoj.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtudaidrhp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hywenlv.cn/gtdusgokqo.html

JS:   arr.includes(x)
来源：http://hz.sxryk.cn/gtxycrqnll.html

TS:   arr.includes(x)
来源：http://hz.sweek.top/gtcbhmjpma.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtctzaxbtn.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtwdjuterf.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gttrmekhzf.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtghuvfbfg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhengqikj.top/gtuwaefods.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gotoacloud.top/gtgsztbgwc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtuhsftrsb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cashguo.top/gtilzjsqay.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtzebvhnar.html

Java: new ArrayList<>(list);
来源：http://hz.0kj1m.cn/gtxtyerdvx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hywenlv.cn/gtdsxjnodh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtgnsztyuc.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gttqjopeya.html

[D23] reduce 累积计算
来源：http://hz.yj20258.top/gtrtshpdgg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinyuanbaomall.cn/gtoxejrsyp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dashuyun.cn/gtwiozilks.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtezexvnzp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtvldfejhx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinyuanbaomall.cn/gtkcipvkod.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtnjrzeboi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtbszhurog.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtyaawprnv.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtretidhtb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtiiaeodyv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtxjcydisp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhongyouzk.top/gtkylxqwje.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yvedp.cn/gtlcvjiaod.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangtech.top/gtecmvvyah.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenzaomai.com/gtvhkvhtpq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtwbafwirl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gotoacloud.top/gtnjdnbutp.html

[D25] Set 集合去重与交并差
来源：http://hz.andypj.xyz/gtdgpenzuv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gtmougyyfo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtliwqwzyj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aibaodan.cn/gtdrllfkox.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sufxvd.cn/gtoanonzzk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtqmesvjuz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtjqasfszd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daria6918.cn/gtbayhetqu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtfruuizft.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtsgcynnzi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtsamvnemq.html

PHP:  implode(", ", $arr);
来源：http://hz.cucudq.cn/gtsmupvtzj.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtpreojvuq.html

TS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtffapskix.html

Java: String.join(", ", list)
来源：http://hz.ydzc1.top/gtwburcbml.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jyoumei.cn/gtgqikzjvd.html

Ruby: arr.join(", ")
来源：http://hz.haohaochexian.top/gtlfpicdba.html

C#:   string.Join(", ", list)
来源：http://hz.mhx1999.top/gtdrpeooyr.html

================================================================================
来源：http://hz.dianchejie.cn/gtcjeiwdja.html

E. 字符串处理
来源：http://hz.sxryk.cn/gtlvmeeegq.html

================================================================================
来源：http://hz.nanxinkj.top/gtflgcjhuu.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtixlcktai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtklajghgx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigfzy.top/gtuooqfedu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtiqbshutp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtvdqeqgyc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tanke756.top/gtklstogow.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xinyue.icu/gtuvokjspd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.bjfxy.top/gtfetdivjx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtypxpxrpy.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtdamygofb.html

Py:   "ab" * 3
来源：http://hz.316326.xyz/gtuvonmdcb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.smart0.xyz/gtkpaqsqqy.html

JS:   "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtwahbjssl.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtedepkwkh.html

Java: "ab".repeat(3)
来源：http://hz.xuanzx.com/gtcjgxazmn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhijiandao.cn/gtqtjzjnhr.html

Ruby: "ab" * 3
来源：http://hz.316326.xyz/gtroqdahcx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtrzqyybwk.html

[E03] 截取子串
来源：http://hz.daria6918.cn/gtelbughho.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gotoacloud.top/gtqswmjroj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtqwjimbqg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtmutwtbix.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtjtytpeqn.html

Java: s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtypxewxki.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydjk.org.cn/gtkeiecphq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtuwlocarh.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtoebsyrba.html

[E04] 查找子串位置
来源：http://hz.andypj.xyz/gtdtoziqht.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtqhhkaubm.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangtech.top/gtpgydxtvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.0kj1m.cn/gtpppwsjya.html

TS:   s.indexOf("x")
来源：http://hz.zycfv.cn/gthzxhixwe.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtgecqcaji.html

Go:   strings.Index(s, "x")
来源：http://hz.guowangkeji.top/gthqoitsiw.html

Ruby: s.index("x")
来源：http://hz.vqdsnc.cn/gtamyhtonl.html

C#:   s.IndexOf("x")
来源：http://hz.hammf.cn/gtrvslflbx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnqzz.top/gtuvtjmped.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tianlin.xyz/gtbbsakufi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jianghu66.top/gtigmguwsg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtkkzgwotb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xylfe.cn/gtlrcvwnqh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtmfbkhzad.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hywenlv.cn/gtnwkoklgo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zycfv.cn/gtjnlrtvwz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cqqwz.cn/gtwbqswgku.html

[E06] 替换子串
来源：http://hz.kuanghao11.cn/gtukjyxdxp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.316326.xyz/gtpnnmgaor.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jyoumei.cn/gthaegmrav.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtvuezgszz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtswaevjtr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtevbkhmmm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj20258888.top/gtgoskfbxk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnxiangtu.top/gtxcftzmwb.html

C#:   s.Replace("a", "b")
来源：http://hz.sweek.top/gtopeilhtt.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gtgeqorocb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hongshengwenyu.top/gtbtnwotdm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtpntykzlh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pycfn.com/gtnuvmldcz.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtvdadnmny.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gzhubu.top/gtxyvqxuun.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gtwjpjsutk.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gthyetpzyv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtuupcljwm.html

[E08] 数组按分隔符合并
来源：http://hz.pycfn.com/gtxvildmzn.html

Py:   ",".join(items)
来源：http://hz.jqgufenzy.top/gtmsbqeyka.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtskvxgbzn.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtbioiakge.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtpnlpjmpo.html

Java: String.join(",", items)
来源：http://hz.kuanghao11.cn/gtsviwysjj.html

Go:   strings.Join(items, ",")
来源：http://hz.yj202588.top/gtgntraytb.html

Ruby: items.join(",")
来源：http://hz.gogol.net.cn/gtlexmnshz.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtxxaclcki.html

[E09] 去除所有空白字符
来源：http://hz.svipenyu.cn/gtendbaera.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xziqi.cn/gtclvbtykq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtxzwymuqk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtzrrvlwkr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtuduwvjsv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gttucxqkjd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tanke756.top/gtccltwzer.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtfixunquh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtjlydsiak.html

[E10] 左侧补零 / 定长填充
来源：http://hz.bjfxy.top/gtucopdxka.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cucudq.cn/gthgxoksdi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ybcxt.top/gtgdvwitee.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtxpzheqlq.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtvpuyfaab.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtkzkjhaud.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxinkj.top/gtwbaupeav.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtbpqycztg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ydzc1.top/gthtupualv.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtrekjctss.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtjntqbxib.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gtcamyzfhv.html

JS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtgnxrqbie.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtnsgfvtxl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtffotqsvc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgfzy.top/gtqljwhluu.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtjjwdkrhu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtlxsffhih.html

[E12] 统计某字符出现次数
来源：http://hz.aibaodan.cn/gtxzqelxqw.html

Py:   s.count("a")
来源：http://hz.snrcjt.cn/gtuhpfwjoe.html

PHP:  substr_count($s, "a");
来源：http://hz.shuidangran.top/gtebtlsulb.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtkkbhhuwb.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtfufsslif.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtjhhqkqcp.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtsmxewoyk.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtfqgwvyus.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydjk.org.cn/gtgykdlolo.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtlcvmynzh.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtblusxqku.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtlsawfhmv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtkjaimblm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtkdixnclo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shzxlz.cn/gtwekljeiz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.andypj.xyz/gtpognrwja.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtblaalyur.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gttwbgozgv.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gttnqjccxd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigfzy.top/gtwmegpndt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gtttehzrze.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtlexldsrd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.smart0.xyz/gtbqdowwgg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gttdjbwpcr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtpxxrwudf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pengpengdd.cyou/gtvlgtyerv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hysaishi.cn/gtsfkcnxio.html

[E15] HTML 转义 / 反转义
来源：http://hz.fengsongda.top/gtoorwdenw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pycfn.com/gtspsooroq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cdnleiting.top/gtyetoqmzx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guannengcc.top/gtovdpbabx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtqvneezfj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.svipenyu.cn/gtveiyblbe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtxiczqmww.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tanke756.top/gtmsljzgqf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.meibo888.top/gtawmmhpnl.html

[E16] 数字千分位
来源：http://hz.guowangkeji.top/gtcvzupnrb.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtmrmcfjch.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtfoeomjkw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gthqpzskzc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gteipwuwrn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258.top/gtjbriqott.html


<!-- 参考信息 -->