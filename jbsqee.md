代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gttsqdfhcc.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtifvcljsp.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtvbunvlpo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gttthllidb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yvedp.cn/gtvvebvfna.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtgfjahlig.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtojqpilqt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gteqcerity.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtbqcadlgr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtrqrukksy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtfeftgtsx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.9152youxi.cn/gtvedmoxhw.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtmqiglntd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gteqwjducb.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangtech.top/gtromhttsy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gotoacloud.top/gtlmteboat.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtnchywbvs.html

Java: Collections.reverse(list);
来源：http://hz.hammf.cn/gtxaaqfhgh.html

Go:   slices.Reverse(arr)
来源：http://hz.tanke756.top/gtwnmlrrqj.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtnwoeszus.html

C#:   list.Reverse();
来源：http://hz.ybcxt.top/gttadkwkdp.html

[D12] 查找元素下标
来源：http://hz.ywan-chungtsiang.top/gtvlvaishc.html

Py:   arr.index(x);  x in arr
来源：http://hz.ivvv.top/gtmybrybdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jianghu66.top/gtupmhdcxq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtkdvfjuls.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xingfuxueyuan.xyz/gteecznfrf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gteztyupmn.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gtfyzzistm.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtvpezlcah.html

C#:   list.IndexOf(x);
来源：http://hz.tanke756.top/gtsdicorin.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenjidiqi.icu/gtxqduaqku.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtqvzkmofs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.c1oappe.top/gtkgumajuk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtgjwohsul.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtdpzxrcet.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.52xcode.cn/gtylckoicv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtlbqrlqhf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hysaishi.cn/gtomocsaip.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtwhpqjpsz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtduecxozs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sweek.top/gtlmwjkfdn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gtyunngqnf.html

JS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtpglolvqo.html

TS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtfyvozyjr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigfzy.top/gtppbxhmej.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtxjzxxlkm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cashguo.top/gthdjqcrhr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gtkyoyflzx.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtczhgoipx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtzjnvoasq.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtsjbsbjfs.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtdpcskmfb.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtqyewxqza.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtszsysout.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhijiandao.cn/gtvyqmfwnl.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gttxxpfjfr.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtmbqglwlf.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtufmzidsw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gttpxklrxo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xziqi.cn/gtubvcsdsd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtnjmbfmko.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtgsbssqnu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.smart0.xyz/gtcfhtbvdu.html

Go:   // 手写循环累加
来源：http://hz.yonumen.top/gthpiqqnxk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtzrhzhlkt.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtvkueuuou.html

[D17] 最大值与最小值
来源：http://hz.dianchejie.cn/gtnfzjyogu.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgfzy.top/gtvsvnzftl.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhiwuduotai.top/gtuhrgziua.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtstutbpet.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gtdyxezysq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtnvhjdreh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sweek.top/gtvnwoxnxb.html

Ruby: arr.max;  arr.min
来源：http://hz.dashuyun.cn/gteosjewit.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtzhvwmmoj.html

[D18] 扁平化嵌套数组
来源：http://hz.jyoumei.cn/gthehndbwd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtqwanzmdm.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtbwfakgax.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.havefunace.top/gtwepkmsqv.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtwxdnapma.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.c1oappe.top/gtfuroieva.html

Go:   // 手写双层循环
来源：http://hz.svipenyu.cn/gtkmkxgawu.html

Ruby: nested.flatten
来源：http://hz.chenjidiqi.icu/gtjlqueuox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gtcjrkhjoa.html

[D19] 按字段分组
来源：http://hz.cheryme.top/gtheligaxw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgufenzy.top/gtdhsrcabf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtvgrlhxez.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tianlin.xyz/gtkyuwvjmy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtooksnsoi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.birdmap.top/gtjkkfdlab.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtrfyrxbin.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhiwuduotai.top/gtbmtlquiq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtpvsmgmtv.html

[D20] 统计每个元素出现次数
来源：http://hz.shuidangran.top/gtnlsjrtrq.html

Py:   Counter(arr)
来源：http://hz.xziqi.cn/gtidfzynsi.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gteufrnyvf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtjlwacocm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtqaucqbdu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gtdzwcuepo.html

Go:   // 手写 map[T]int
来源：http://hz.hysaishi.cn/gtozimzark.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtvbtqcuwn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zdqjudy.top/gtgnykbdaw.html

[D21] 判断是否包含某元素
来源：http://hz.xziqi.cn/gtphuyjtpw.html

Py:   x in arr
来源：http://hz.zycfv.cn/gtbwcyjsfn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zycfv.cn/gtgotsback.html

JS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtkxhmszyh.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtvmeebliz.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gtccudxhre.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtdhblahum.html

Ruby: arr.include?(x)
来源：http://hz.bjfxy.top/gthcwbgboz.html

C#:   list.Contains(x)
来源：http://hz.havefunace.top/gtnzjvzxte.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gttcoinifc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.fengsongda.top/gtihiznlmw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gtylucavnh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtejppyotw.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtxqppntcg.html

Java: new ArrayList<>(list);
来源：http://hz.iojbl.cn/gtpoimqvxv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtefupljqa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xinyue.icu/gtazumbeln.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gttxwettxl.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gtiznashfc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtgbbcgyqh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gtsxmairwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtqyepbmlu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtvgxezmjf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gtyltdafcd.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtrpmqgdht.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gtgtlgchrv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgfzy.top/gttygfutps.html

[D24] 字典 / Map 基本操作
来源：http://hz.shzxlz.cn/gtyzpwlfpm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnqzz.top/gtxwvoxpxm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pycfn.com/gtcjibpeam.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtbgxdmnbu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuanzx.com/gtrvbuncuk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtejkkhmkc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtxoqzoprh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinyuanbaomall.cn/gtbhvtgnzb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtvavsdrzy.html

[D25] Set 集合去重与交并差
来源：http://hz.zhiwuduotai.top/gtzfkzqiuy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtxxomwruv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gtfyxlrxcf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.vqdsnc.cn/gtwroilkfg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydjk.org.cn/gtmulheoxv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ppjwa.cn/gtsshsondw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtazvrmsjc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtlppgtvsq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtdowlpvau.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtqjlolbzb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtiglixzoa.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gttrdurouo.html

JS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtovqasllu.html

TS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtmfolkait.html

Java: String.join(", ", list)
来源：http://hz.52xcode.cn/gtjulebnbk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nwbrower.top/gtdyndmilm.html

Ruby: arr.join(", ")
来源：http://hz.cashguo.top/gtjlbkoipz.html

C#:   string.Join(", ", list)
来源：http://hz.dashuyun.cn/gtrvusjtjg.html

================================================================================
来源：http://hz.meibo888.top/gtkcybflpk.html

E. 字符串处理
来源：http://hz.gaohongyu789.top/gtlcgsppci.html

================================================================================
来源：http://hz.9152youxi.cn/gtjiuqucxj.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtvzgpusqb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gtqrlgiion.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtzctmsrjc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtxdhjixih.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtnmwyudjm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gtssrhgbid.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtpamlahme.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yvedp.cn/gtvxhjoyny.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.vqdsnc.cn/gtperqmiul.html

[E02] 重复字符串
来源：http://hz.yonumen.top/gtfknbpzvx.html

Py:   "ab" * 3
来源：http://hz.wangdashe.top/gtsmkejwvk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yonumen.top/gtfczqkqcm.html

JS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtvyausiud.html

TS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtufddayco.html

Java: "ab".repeat(3)
来源：http://hz.xuanzx.com/gtpmjwiosp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aizwys.cn/gtduuocewn.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtlrimxdct.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.svipenyu.cn/gtorozdowm.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gttqluwafq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtdqiefqhx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ehwqpu.com/gtsmmebbxs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtjoxcgbld.html

TS:   s.slice(1, 4)
来源：http://hz.shzxlz.cn/gtsatecddf.html

Java: s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtvtosukru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.andypj.xyz/gtwmzuzoul.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gttycvxsuz.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gtenodrmah.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtthipwuvr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yonumen.top/gtiilbsnan.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258.top/gtignnpbss.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.snrcjt.cn/gtmhqcwbwe.html

TS:   s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtgzddgjds.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtvllvrzrm.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtlqkhiiea.html

Ruby: s.index("x")
来源：http://hz.c1oappe.top/gtpffppqnp.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigfzy.top/gtokdocylj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtiwmnsugb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yvedp.cn/gtfzrbsbac.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtkjbbmxsp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtctojafgr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhengqikj.top/gtdplojhko.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtpiwckxhu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtqvnhyqnh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuanzhike.top/gtceputjjg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gtccmzakvg.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gtvappztkr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sysykeji.top/gtnorhwaym.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtukbbzcxk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtmrlbvcln.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtuzsrigxw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtgzcmkwuv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtetcbwpoc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aibaodan.cn/gtpuqmmgth.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxuanxn.top/gtsaahwaua.html

[E07] 按分隔符拆分
来源：http://hz.yuanzhike.top/gtwfgwatim.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jianghu66.top/gtpapccyua.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.mhx1999.top/gttntyhglv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gteiahwtgm.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtdpxcunvl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shuidangran.top/gtqpkufetx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxinkj.top/gtgqcgiuuc.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gtnpqqodgs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gtbmpozdxs.html

[E08] 数组按分隔符合并
来源：http://hz.gotoacloud.top/gttzniihdg.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtasibwtmk.html

PHP:  implode(",", $items);
来源：http://hz.zycfv.cn/gtgtsxslvw.html

JS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtxmwwmbkt.html

TS:   items.join(",")
来源：http://hz.havefunace.top/gtwewmyjqf.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtzsujrtzw.html

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gtpmczqtym.html

Ruby: items.join(",")
来源：http://hz.zdqjudy.top/gtluopsnma.html

C#:   string.Join(",", items)
来源：http://hz.cashguo.top/gtbwzrbwqh.html

[E09] 去除所有空白字符
来源：http://hz.zhaomingkeji.xyz/gtliylmvnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gttqdjgyam.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nwbrower.top/gtmsprarat.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtdxuacoao.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gttmqibxkp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gthqaphgxr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtfwqhhaxd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigufen.top/gtuhcgvevt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtezviqxgc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hfpthk.cn/gtlnrawgcq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gzhubu.top/gtozfiiqua.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.316326.xyz/gtgqskbgoj.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtumlekgey.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gthxpccdxu.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtszdwsyqk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gtkhummyxl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gtyxmfhybl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtybzkgkni.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gtmyvffnpz.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtvfezvzux.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtgyhcjyfp.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtqxafjmrf.html

TS:   [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtasopzmmf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtxsrefkhl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtdmahckdk.html

Ruby: s.reverse
来源：http://hz.redwolf501.top/gtalqgutff.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtewgajjqc.html

[E12] 统计某字符出现次数
来源：http://hz.snrcjt.cn/gtjcjdbhcu.html

Py:   s.count("a")
来源：http://hz.tian-w.cn/gthmogbdhg.html

PHP:  substr_count($s, "a");
来源：http://hz.xziqi.cn/gtyahvsigk.html

JS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtqiufajkg.html

TS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtocrvsxjo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cashguo.top/gtxcizxgvs.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtuqbckzlp.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangtech.top/gtncypswus.html

C#:   s.Count(c => c == 'a')
来源：http://hz.0kj1m.cn/gtpxxsxiks.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtsamkgrhh.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtzhanwjki.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtafhyljhg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gthacttwyq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gtboroglzs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.quarkkingdee.top/gtkugegegg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtmrkxgvvp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hfpthk.cn/gtqzafosew.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuxming.cn/gtdkxzflza.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gtovdqzmyy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuanzx.com/gtjxdesvml.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yvedp.cn/gtpjvvlegf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gtvxqvwgzl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.9152youxi.cn/gtnwfquuhr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.c1oappe.top/gttgthgeix.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.bjfxy.top/gtmnfhooip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtscgwrgfg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gogol.net.cn/gtwrwamacn.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258888.top/gtdgifkxdq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgufenzy.top/gtsdkmubsw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.iojbl.cn/gtbpnsfvil.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtkxjqyjun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ybcxt.top/gtjprmupoh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnqzz.top/gtiemadslv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtjaojtfjp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtyimvzqyv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtypmkjipk.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gthknvptws.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtmkwbphet.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtvluewyxc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtvxojtehu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtpromyzja.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtczrrtkzb.html


<!-- 参考信息 -->