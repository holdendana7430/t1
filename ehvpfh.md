代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.xuetiantiany.cn/gtstgjtspf.html

Java: Collections.reverse(list);
来源：http://hz.aibaodan.cn/gtzvppgpxa.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtxhcnznhv.html

Ruby: arr.reverse
来源：http://hz.sxryk.cn/gtksikzori.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangtech.top/gtzprzisol.html

[D12] 查找元素下标
来源：http://hz.birdmap.top/gtnjpbyuub.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtyndgarws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cqqwz.cn/gtkpciswzn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gtralswqtn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtnvvkkhtx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.vqdsnc.cn/gtrsmxgpvq.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtrkjvuylk.html

Ruby: arr.index(x)
来源：http://hz.jinyuanbaomall.cn/gtucqswlne.html

C#:   list.IndexOf(x);
来源：http://hz.tanke756.top/gtflztsrmu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinyuanbaomall.cn/gtozeztgcq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hfpthk.cn/gtbvuvldtc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtkrdfwzde.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gthbuwxpiw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtwathleqs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtnougqatc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cheryme.top/gtxdhlvezd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxinkj.top/gtjieglvfm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxinkj.top/gtwvmfswrr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.0kj1m.cn/gthtphnebk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gthzydpoyv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtkrjjgamp.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtwmgjjnhj.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtpmwsvpem.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxuanxn.top/gtosxvlofl.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtpvctgavq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yongpay.top/gtytdvjakr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gthviignen.html

[D15] 去重
来源：http://hz.hammf.cn/gtmqtjeuxv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtvwzuawit.html

PHP:  array_unique($arr);
来源：http://hz.svipenyu.cn/gtqowtxjfh.html

JS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gtveyattlc.html

TS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtnxkefxwp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtmszstnct.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhongyouzk.top/gtoraxjwrz.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtstmqjaki.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtwrjmwhpg.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtnbsgdbhm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cashguo.top/gtrmzcbefl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtwlohoncm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtibktkpeb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtsbbitlzf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gtiyoqvtan.html

Go:   // 手写循环累加
来源：http://hz.zhongyouzk.top/gtyxmohfjp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gtchccnpqj.html

C#:   list.Sum();  list.Average()
来源：http://hz.feifeiyinyue.top/gtbpevilwb.html

[D17] 最大值与最小值
来源：http://hz.shzxlz.cn/gttezlljdg.html

Py:   max(arr);  min(arr)
来源：http://hz.zhaomingkeji.xyz/gtgfjdtcdg.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnqzz.top/gtyzclpviz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yanxiufei.cn/gtflpdxfcq.html

TS:   Math.max(...arr);
来源：http://hz.cucudq.cn/gtrugzunib.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ywan-chungtsiang.top/gtmmlawvpp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gaohongyu789.top/gtppzbhqzm.html

Ruby: arr.max;  arr.min
来源：http://hz.ehwqpu.com/gthokewkdu.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtcuigfxst.html

[D18] 扁平化嵌套数组
来源：http://hz.cdnleiting.top/gtiswluqmq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhijiandao.cn/gtsrrzisox.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtosldnmrg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtydvxmrem.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtgrzwshgg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtguvamgbb.html

Go:   // 手写双层循环
来源：http://hz.shuidangran.top/gtfkkeditr.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtmcktnfxn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtfjzaihrm.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gtjgmxdgnk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtvxatnkad.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daria6918.cn/gtkrqgnlie.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtwbrncyfc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtfxocjuoy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cdnleiting.top/gtdtbjnefg.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gtfburcsxd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gtfydhckug.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.vqdsnc.cn/gtrurtodrq.html

[D20] 统计每个元素出现次数
来源：http://hz.tian-w.cn/gtsukzqhwb.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtajyaxwwx.html

PHP:  array_count_values($arr);
来源：http://hz.yanxiufei.cn/gtkcypfabw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtgvuvobwg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtgonrhvzo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gzhubu.top/gtuztjmusk.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtxkbwoxdk.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gttmskiwvo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jyoumei.cn/gtummumhmn.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtbfxamiim.html

Py:   x in arr
来源：http://hz.yvedp.cn/gthdtfbnxs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtljmwsnyy.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtwekgpkdf.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtbqsjwrty.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtnrihfltk.html

Go:   slices.Contains(arr, x)
来源：http://hz.c1oappe.top/gtyllubngq.html

Ruby: arr.include?(x)
来源：http://hz.zycfv.cn/gteigvzhsb.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtbzihcann.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj202588.top/gthcooznbc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gtrjyuulzb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtlocecrkt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinghuilouyu.cn/gtnfflxxzu.html

TS:   [...arr];
来源：http://hz.cqqwz.cn/gttdvrhbjj.html

Java: new ArrayList<>(list);
来源：http://hz.ehwqpu.com/gtgtplcxrv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gtprevyude.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gttqqzjfjl.html

C#:   new List<int>(list);
来源：http://hz.fengsongda.top/gtusprsvhn.html

[D23] reduce 累积计算
来源：http://hz.smart0.xyz/gttgmuqisa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.0kj1m.cn/gtkssfwzow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtvekawigw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtxqtwfmwk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtxlfdnsic.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gthemeygpl.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtegififgf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gteqjssdtf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtwcqqgkkt.html

[D24] 字典 / Map 基本操作
来源：http://hz.cucudq.cn/gtzoqkgtmm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gtzwdgsjyg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gtatwsdqzx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gzhubu.top/gtoipfbsue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtbqxfkgvu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gtnbmmeeqi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgufenzy.top/gtrwyeerco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtuypfrqez.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shangyingyoupin.top/gtjufgndgh.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtxuzksbki.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuxming.cn/gteswxyink.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtiypaufur.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtzrufqtik.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghu66.top/gtszbtshmv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtvsnszyik.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.kuanghao11.cn/gtuhqkxctq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtckawzcnl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ywan-chungtsiang.top/gtfuoyipjr.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtbzloxhci.html

Py:   ", ".join(map(str, arr))
来源：http://hz.birdmap.top/gtmcdtfhsv.html

PHP:  implode(", ", $arr);
来源：http://hz.gogol.net.cn/gtjyjvhcmz.html

JS:   arr.join(", ")
来源：http://hz.cheryme.top/gtadqxbmet.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtdhvwifmf.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gtzfqmkita.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhoulong.xyz/gtewybvvvw.html

Ruby: arr.join(", ")
来源：http://hz.kuanghao11.cn/gtbbuvwufn.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtkfqalvyr.html

================================================================================
来源：http://hz.guowangkeji.top/gtljmexkmu.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gttrquxwyv.html

================================================================================
来源：http://hz.cqqwz.cn/gtvwkmmghi.html

[E01] 拼接字符串
来源：http://hz.nwbrower.top/gteqwgfewi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenlongwang.top/gtumdimbkm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gzhubu.top/gtyhquornv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zdqjudy.top/gtfaqrkpre.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtjyyqmell.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtijhzwtdm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigufen.top/gtsfonbqbd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtuerpfano.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.havefunace.top/gtytkjpknp.html

[E02] 重复字符串
来源：http://hz.chenlongwang.top/gtamdxkeqf.html

Py:   "ab" * 3
来源：http://hz.0kj1m.cn/gtnidnhsxg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtzttsblip.html

JS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gthwbukgir.html

TS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtxozokglf.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtuvgdmjgf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuanzx.com/gtbkcwloct.html

Ruby: "ab" * 3
来源：http://hz.redwolf501.top/gtxtrrjbww.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.kuanghao11.cn/gtlunjjags.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtxovvjswj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pycfn.com/gtolhyikvm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.birdmap.top/gtxsukjerg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sweek.top/gttumxdcyf.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtmpcszdrf.html

Java: s.substring(1, 4)
来源：http://hz.mhx1999.top/gtkqeqtvev.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gzhubu.top/gtuqnjyaaz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtiujqvkyg.html

C#:   s.Substring(1, 3)
来源：http://hz.mhx1999.top/gtqynrxvaf.html

[E04] 查找子串位置
来源：http://hz.tanke756.top/gtukkcwdxa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtayvwfseq.html

PHP:  strpos($s, "x");
来源：http://hz.andypj.xyz/gtedyvqawz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pycfn.com/gtinyveztx.html

TS:   s.indexOf("x")
来源：http://hz.aizwys.cn/gtmjruqopf.html

Java: s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtcdxvesnz.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtspctarid.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtgwibloen.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtbupherxx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtwvzztxmh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yvedp.cn/gtyevfrbxd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xziqi.cn/gttcnrpmqp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtgrrstapz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jlsjyb.cn/gtdhvutkyj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtohbqdxgs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhengqikj.top/gtkyyomdtm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtmyfgsdrd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pengpengdd.cyou/gtcndnqwkh.html

[E06] 替换子串
来源：http://hz.yuxming.cn/gtnvebskgo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtfflsrmrk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gotoacloud.top/gtscbrzhua.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtcqubgoar.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtujoapcfg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtritfuuix.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtaqqopnuv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtxzarslng.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtytfaiwde.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtfndlyqbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pycfn.com/gtyfkgyyct.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtzgfhqsrc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pycfn.com/gtaixoljzq.html

TS:   s.split(",")
来源：http://hz.snrcjt.cn/gtzgcldwyq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.snrcjt.cn/gtslrajqmn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.dianchejie.cn/gtrupvkbdc.html

Ruby: s.split(",");  s.split
来源：http://hz.wangdashe.top/gtakujkkgg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinqigfzy.top/gtuxingtkd.html

[E08] 数组按分隔符合并
来源：http://hz.cqqwz.cn/gtstjmhmzp.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gticlbdamk.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtavtvbqzp.html

JS:   items.join(",")
来源：http://hz.svipenyu.cn/gtaqrsjplg.html

TS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtyagidooa.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtpjfeojxe.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigfzy.top/gtamcxelah.html

Ruby: items.join(",")
来源：http://hz.chenjidiqi.icu/gtdvcrvdrh.html

C#:   string.Join(",", items)
来源：http://hz.cheryme.top/gtseongmrt.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtlalrplmy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangtech.top/gtjyhmcqkx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gttdhduprg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtrhtgrmzn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gthcetwaca.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fengsongda.top/gtadxokcek.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gtvwpqyoob.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gotoacloud.top/gturgdiojf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yueranfly.top/gtctyjcupc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtsyalgekv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtddhurtzi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtwwmqpulz.html

JS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtnvxjjyio.html

TS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtxbbhnoau.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtvbzbcgox.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aizwys.cn/gtwvcvfcfp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sysykeji.top/gtsfwzutse.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtnaihrnkr.html

[E11] 反转字符串
来源：http://hz.yanxiufei.cn/gtfxdkxvkk.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtefteikql.html

PHP:  strrev($s);
来源：http://hz.andypj.xyz/gttlklrhbj.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtjklaqgzt.html

TS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtrxinpnmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.pycfn.com/gtmgsoftrt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtsmahehux.html

Ruby: s.reverse
来源：http://hz.yvedp.cn/gttxyuzdut.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtwxcrkhoe.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258888.top/gtnvzgmhbb.html

Py:   s.count("a")
来源：http://hz.ehwqpu.com/gtynjcbjqh.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtwyjfddil.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtqaqjkurx.html

TS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtztycimfg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhijiandao.cn/gtjeovkvbl.html

Go:   strings.Count(s, "a")
来源：http://hz.c1oappe.top/gtiadqxjkp.html

Ruby: s.count("a")
来源：http://hz.316326.xyz/gtzbnwijwt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtvfsfvbgi.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtfikyvtjz.html

Py:   for ch in s: print(ch)
来源：http://hz.havefunace.top/gtkxznvwsx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gogol.net.cn/gtrseybjra.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtswhulvfs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtbfcgqvfu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cdnleiting.top/gtoudkxmwu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtbgysfmug.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtzanikoeg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hfpthk.cn/gtplihxhif.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gtslkfwzdm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gtnmpovmxw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dianchejie.cn/gtdxtckelk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxuanxn.top/gttvlcbzxm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtebsltlhf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtyzhudqjv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aizwys.cn/gtulpwyjzu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgfzy.top/gtvvzfsits.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtecorypyi.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtmzdyfift.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cdnleiting.top/gtdjskfzex.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtliuhpvfk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pycfn.com/gtbenuubxd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xylfe.cn/gtagowbgod.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.iojbl.cn/gtfshxlknj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gthytdydhm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj202588.top/gtdazjejtq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangshuangyany.cn/gtrygjjjez.html

[E16] 数字千分位
来源：http://hz.ybcxt.top/gtuykpfxvj.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtwnuaqvmu.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtgpvlhqzq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtsdoifsii.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtnvivynvv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtveqlbkbb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtofrugvqz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xingfuxueyuan.xyz/gtoniexduy.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtsvddzcdi.html

[E17] 首字母大写
来源：http://hz.jinqigfzy.top/gtodobinyk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gtepxlahbi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtxqkeppfi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtxmwsumdy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtbdswiwcz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gaohongyu789.top/gtkomobodq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hongshengwenyu.top/gtwalusjlk.html

Ruby: s.capitalize
来源：http://hz.xinyue.icu/gtzwntmshb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.wangshuangyany.cn/gtgupezulk.html

[E18] 模板占位符替换
来源：http://hz.zycfv.cn/gtcpyfipxt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtnbkiopmg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtvsczzqlu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtdtsscogn.html


<!-- 参考信息 -->