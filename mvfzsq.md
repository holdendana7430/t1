代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtyaurlret.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gttzslewdl.html

C#:   list.Sort();
来源：http://hz.aizwys.cn/gtfqpadikb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ybcxt.top/gtdvtjiofe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnqzz.top/gtarjjpxgk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtfgauwwuh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtssfrodia.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gthjyaeivy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.mhx1999.top/gtmjknqxxa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jyoumei.cn/gteyqcomwg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgufenzy.top/gttxoyyotx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gttnnsmgxs.html

[D11] 反转数组
来源：http://hz.iojbl.cn/gtseywptjl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigfzy.top/gtdxgrmptw.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gtfqdicrzu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.meibo888.top/gtknycejuf.html

TS:   [...arr].reverse();
来源：http://hz.vqdsnc.cn/gtxtkawfnu.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtpvdkdfpt.html

Go:   slices.Reverse(arr)
来源：http://hz.quarkkingdee.top/gtiknmedvr.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gtseqdjemb.html

C#:   list.Reverse();
来源：http://hz.redwolf501.top/gtpzmgofnd.html

[D12] 查找元素下标
来源：http://hz.jinyuanbaomall.cn/gthiiprbzz.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gtjbwatgrs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gttfidowse.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtfcuwfzrt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtugupwhpu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dianchejie.cn/gtqjtstfzn.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtzmseimso.html

Ruby: arr.index(x)
来源：http://hz.zhongyouzk.top/gtbtbcktvg.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gtmuhdenjt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pengpengdd.cyou/gtqpzxudds.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtiyejomoh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhiwuduotai.top/gtinfutasf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtvdawunyn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtzujaalaq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgfzy.top/gtjeevmjey.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tanke756.top/gtzyatajhn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtftmhvdcg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangkeji.top/gtwfaigytc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtbdlxgbky.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtwwjxhyqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daria6918.cn/gtldiubksf.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtxmmifqqh.html

TS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gthxwbnbhp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtlbgoifoy.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtfkxxnlym.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.meibo888.top/gtemhlayup.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gtyvroeqlo.html

[D15] 去重
来源：http://hz.sweek.top/gtsybnpncp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtdzaiavdv.html

PHP:  array_unique($arr);
来源：http://hz.yueranfly.top/gtkqqlnnxd.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtryrexatu.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtscysgewc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sweek.top/gtlodalrvz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtlnkpjlkx.html

Ruby: arr.uniq
来源：http://hz.wangshuangyany.cn/gtgpbgsrpa.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtxstikipv.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtdvoeeftu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gtbedyspns.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guowangkeji.top/gtqwryvglg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtnbevupsu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtdjanymnc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tian-w.cn/gtepmpqpud.html

Go:   // 手写循环累加
来源：http://hz.zhongyouzk.top/gtzpolpetj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gogol.net.cn/gtarfctdkd.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gtydlnyhoi.html

[D17] 最大值与最小值
来源：http://hz.nwbrower.top/gtbkxvoydh.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtcuefwlkd.html

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gtrwathnor.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gttyvhyzif.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gtghfhnifd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shzxlz.cn/gtskmghpns.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtnakgvokw.html

Ruby: arr.max;  arr.min
来源：http://hz.daxiang520.top/gthbihsgda.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtcfwbeiye.html

[D18] 扁平化嵌套数组
来源：http://hz.hongshengwenyu.top/gttjhwaoxr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gttfytbeqn.html

PHP:  array_merge(...$nested);
来源：http://hz.hysaishi.cn/gtqojooywf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ywan-chungtsiang.top/gtudpivnmb.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtitiapaqy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtljjxwrxj.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtrqunzupe.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtadpfglmj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shuidangran.top/gtdkrdpiyc.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtqztdofqo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gttcafxgie.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtuqptckmj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtngvlqnle.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtnzxmsvbk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.quarkkingdee.top/gtlmjebrhn.html

Go:   // 手写 map[string][]T
来源：http://hz.xinyue.icu/gtbesglqfi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dashuyun.cn/gtboudqgmy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xinyue.icu/gtuzprthpp.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtyadrfwwv.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtjtyiujhl.html

PHP:  array_count_values($arr);
来源：http://hz.shzxlz.cn/gtcoxkrjbj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtmxseiwct.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtjyunkeps.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtatqdahfd.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtmdfithkr.html

Ruby: arr.tally
来源：http://hz.hnxiangtu.top/gtkpywgljb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yongpay.top/gtramauaew.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gtiggghocd.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gtqrudstfe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guannengcc.top/gtafacwgbk.html

JS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtgfqwqjlk.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gtlzhddgnu.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtrzltezwo.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnqzz.top/gtxdnrbvtb.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gtxbtvxkxg.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangkeji.top/gtpjqdcuon.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xinyue.icu/gtyfpzuyxw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sxryk.cn/gteklkwuje.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cashguo.top/gtcjuvlxcs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cdnleiting.top/gtcbxpmccg.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtjvmfwzra.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtozltjbtr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj202588.top/gticrwnucf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gtvsrxacfy.html

C#:   new List<int>(list);
来源：http://hz.ydjk.org.cn/gtvmtpvqio.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtobbxfxhc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenzaomai.com/gtogoaymyj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtnsuymezf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtezhgsrkr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtggikukjf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtryfvhwdu.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtcbmdtkfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtwxwsigmx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hfpthk.cn/gtafvvlzdj.html

[D24] 字典 / Map 基本操作
来源：http://hz.snrcjt.cn/gtbsdndunw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtvhvbbkeg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cqqwz.cn/gterozrqjt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guannengcc.top/gtmhxzzcmo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtfpyulcik.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cdnleiting.top/gtgqyflpbp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hysaishi.cn/gtcsmndmvk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hfpthk.cn/gtodzurjdz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.smart0.xyz/gtxysjhjvm.html

[D25] Set 集合去重与交并差
来源：http://hz.zdqjudy.top/gtgjqmcpfx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtabnaibtv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.andypj.xyz/gthjyjiqes.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigufen.top/gtpobpxspm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhoulong.xyz/gtpyweifag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtiaijehjp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cheryme.top/gtsdyuhfvh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigfzy.top/gtfovawqsc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtpxqsbkjg.html

[D26] 数组转字符串
来源：http://hz.ydjk.org.cn/gtfjptktev.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenjidiqi.icu/gtyuuguqrd.html

PHP:  implode(", ", $arr);
来源：http://hz.snrcjt.cn/gtabyjfgyt.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtpdpvxgxz.html

TS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtzkecsyke.html

Java: String.join(", ", list)
来源：http://hz.yj20258.top/gtsjldixzg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nwbrower.top/gtyipqalen.html

Ruby: arr.join(", ")
来源：http://hz.svipenyu.cn/gtayhmcqzm.html

C#:   string.Join(", ", list)
来源：http://hz.cdnleiting.top/gtbamrwgct.html

================================================================================
来源：http://hz.ivvv.top/gtkazydzcs.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gthntjjlil.html

================================================================================
来源：http://hz.jiagoushi.top/gtglysvays.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtyebnezwi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.smart0.xyz/gtorptgmlf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtmczdebvl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtofxbhlsn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtdlqdgrfc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daria6918.cn/gtjkmwqhas.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtcmmlhkys.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtclhwjnso.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sufxvd.cn/gtqbvdcytk.html

[E02] 重复字符串
来源：http://hz.ydjk.org.cn/gtxskipzsd.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtisobityd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.haohaochexian.top/gttrakdosx.html

JS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtqyfkoiko.html

TS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtmawvcoen.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtdquxytrz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnxiangtu.top/gtjztbfxjn.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtzcozzzsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.0kj1m.cn/gtpusiypxr.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtgcvfavzu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dianchejie.cn/gtlzjqpkjk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtqfjycndu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtknhbzieg.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gtwztyxbdm.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtgoatkovn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shuidangran.top/gtgjtlejxl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtpaaouadf.html

C#:   s.Substring(1, 3)
来源：http://hz.xinyue.icu/gtxmxmmyhn.html

[E04] 查找子串位置
来源：http://hz.jiagoushi.top/gtybcofeis.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtwelrbuqc.html

PHP:  strpos($s, "x");
来源：http://hz.andypj.xyz/gtnksozvea.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtklqarqdq.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtggyewdpc.html

Java: s.indexOf("x")
来源：http://hz.chenzaomai.com/gtydlajuuf.html

Go:   strings.Index(s, "x")
来源：http://hz.yueranfly.top/gtjbqjsrbj.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtclwscotk.html

C#:   s.IndexOf("x")
来源：http://hz.xylfe.cn/gtsxtwcujj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xziqi.cn/gtrijomcdr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.vqdsnc.cn/gtpwdmmlli.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.svipenyu.cn/gtvbhljawz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtjnbaaprq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gtxvucflle.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gttltxwueo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuanzhike.top/gtnlnmhvxu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shzxlz.cn/gtzkigwwqv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtiyymzqii.html

[E06] 替换子串
来源：http://hz.ehwqpu.com/gthprogmkc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtayghumfo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenlongwang.top/gtcxsaenev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtdwkktdfj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtagzadxvf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtoyrliowm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sxryk.cn/gtddatgjra.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtenfwqdhj.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtomzqulhe.html

[E07] 按分隔符拆分
来源：http://hz.tanke756.top/gtyirnmuaz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtgsxqyqnq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.svipenyu.cn/gtrjzwzrbe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtfdbzcrap.html

TS:   s.split(",")
来源：http://hz.zhongyouzk.top/gtnidxqooe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sufxvd.cn/gtimviuwxe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtegjkkqmy.html

Ruby: s.split(",");  s.split
来源：http://hz.xingfuxueyuan.xyz/gtdzjcpevv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtvwhwdink.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gteeefxnje.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtcabcdbjy.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtelimxpuf.html

JS:   items.join(",")
来源：http://hz.gaohongyu789.top/gtcbtsewab.html

TS:   items.join(",")
来源：http://hz.0kj1m.cn/gtmtsndafd.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gthssbadfc.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gtohicnmts.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtdgwrgqtd.html

C#:   string.Join(",", items)
来源：http://hz.ydjk.org.cn/gtwablzjlh.html

[E09] 去除所有空白字符
来源：http://hz.jianghu66.top/gtjztwkjxd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yongpay.top/gtgzohyusa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhiwuduotai.top/gtixhysbsv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtokwqjydb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtipxaebxd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtrxrhccbq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cheryme.top/gttyimccxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.svipenyu.cn/gtxtkghevw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cqqwz.cn/gtyozgwnjh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gtemanbvsi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtdfyxenek.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtonujmgxc.html

JS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtdstcgjwa.html

TS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtykymzniv.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtxsvrjszg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sxryk.cn/gtcegdxkag.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtmfdguxml.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.smart0.xyz/gtslkzhdio.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gtmiulfcoa.html

Py:   s[::-1]
来源：http://hz.shangyingyoupin.top/gtnqlmjerm.html

PHP:  strrev($s);
来源：http://hz.daria6918.cn/gtomzardts.html

JS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gtmeahofcu.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtipvyclxn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.snrcjt.cn/gtbkcbdnxa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.iojbl.cn/gtxzcaiadf.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtwtpcvntt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtfpdsfkci.html

[E12] 统计某字符出现次数
来源：http://hz.havefunace.top/gtkhyrlhrz.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtpebksnbf.html

PHP:  substr_count($s, "a");
来源：http://hz.zhijiandao.cn/gtertkfpdy.html

JS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gthcbvsfcw.html

TS:   s.split("a").length - 1
来源：http://hz.meibo888.top/gtfxsrkzxe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhaomingkeji.xyz/gtkzsrkdbv.html

Go:   strings.Count(s, "a")
来源：http://hz.ppjwa.cn/gtzqigibjy.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtnjaytmnq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtemiexkla.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtgfviaway.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtjvmwnyip.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtofmgsuws.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtxwabocew.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtcfqqetwy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtqbpazjdx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hysaishi.cn/gtcalbnuya.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhoulong.xyz/gtyanvtptg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuanzhike.top/gtgyauxooi.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtjavafkrs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.havefunace.top/gtmzkkbvpa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtztpxjbqo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.316326.xyz/gtmmurmbao.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigufen.top/gtbqoiogat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxinkj.top/gtwexunibz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cucudq.cn/gtietcgizg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtakyijrxj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtqjllityg.html

[E15] HTML 转义 / 反转义
来源：http://hz.bjfxy.top/gtjpcxgauh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gteifytzyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.smart0.xyz/gtidyromgj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jyoumei.cn/gtxeyywfav.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gtbpkivdxp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtmekucasg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtdkmckbir.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gaohongyu789.top/gtiaogpwak.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtkpzmdhtl.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtibtxicoa.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtjuwcqezf.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtddmjrxhr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtiiypeqpf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtttrcggmg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangtech.top/gtrqnboclv.html


<!-- 参考信息 -->