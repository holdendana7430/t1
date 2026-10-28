代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtggaspgge.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtmkndkbpw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.pycfn.com/gtssippynn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtqvajtdyh.html

[D11] 反转数组
来源：http://hz.aibaodan.cn/gtllgnwpag.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtctoawvll.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtefwmcmar.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenzaomai.com/gtumpahwcu.html

TS:   [...arr].reverse();
来源：http://hz.sxryk.cn/gtxbbxrost.html

Java: Collections.reverse(list);
来源：http://hz.ybcxt.top/gtpndcywph.html

Go:   slices.Reverse(arr)
来源：http://hz.pengpengdd.cyou/gtqfxahgpi.html

Ruby: arr.reverse
来源：http://hz.nwbrower.top/gtmbgjmyjv.html

C#:   list.Reverse();
来源：http://hz.yuxming.cn/gtbsapqymg.html

[D12] 查找元素下标
来源：http://hz.redwolf501.top/gtickurgsb.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydzc1.top/gtetsdqsnx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.redwolf501.top/gtsstjschd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtsfeeiduh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtdohjqwny.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtsqcshxkb.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtpevhjtni.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtexrnqnsp.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtoeegtfyc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jlsjyb.cn/gtfqswfoik.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yongpay.top/gtbteohyjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cashguo.top/gtzpqmwqop.html

JS:   arr.filter(x => x > 3)
来源：http://hz.havefunace.top/gthjsamgod.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtdzgqjoko.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gtnvyvxtrc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtwlwgmjpi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hammf.cn/gtxizwyqiw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtghkxweae.html

[D14] 映射转换（每个元素变形）
来源：http://hz.haohaochexian.top/gtiztwoemm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guowangkeji.top/gtmxzxqtys.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.bjfxy.top/gtexqtahmo.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtszbsqvlo.html

TS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtaogdnpiv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigufen.top/gtpiizmsuy.html

Go:   // 手写循环
来源：http://hz.pengpengdd.cyou/gtsprstkzv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gteqdwfsep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhaomingkeji.xyz/gtftpojght.html

[D15] 去重
来源：http://hz.xylfe.cn/gtichlitrg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtwspvmeas.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtmsnbatzo.html

JS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtppfhfivx.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtvvkvvwhe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.snrcjt.cn/gtzglqlxoy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gzhubu.top/gtrxvjwzaw.html

Ruby: arr.uniq
来源：http://hz.jinghuilouyu.cn/gttlodpgoq.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gtzdskhwrh.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gtlqpiloxf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenlongwang.top/gtykphbyxp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtowsmswjk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtlpzprsme.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtogpvvqan.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.havefunace.top/gttcpxndyn.html

Go:   // 手写循环累加
来源：http://hz.jqgufenzy.top/gttfzpfwvz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gogol.net.cn/gtgvzuvwjm.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gtijkkdlvm.html

[D17] 最大值与最小值
来源：http://hz.shanyushiyangkeji.top/gtsobpnmgg.html

Py:   max(arr);  min(arr)
来源：http://hz.pengpengdd.cyou/gtxsmnryps.html

PHP:  max($arr);  min($arr);
来源：http://hz.hywenlv.cn/gtinkhuluu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtvxqmpwoh.html

TS:   Math.max(...arr);
来源：http://hz.hnqzz.top/gtlvlebqhh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtqibmihdt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigufen.top/gtfnxehawv.html

Ruby: arr.max;  arr.min
来源：http://hz.svipenyu.cn/gtkxomusqu.html

C#:   list.Max();  list.Min()
来源：http://hz.xylfe.cn/gtlftlrgck.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtyajhjlkb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtrqrfitdy.html

PHP:  array_merge(...$nested);
来源：http://hz.havefunace.top/gtkkjudmty.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtbaxqarat.html

TS:   nested.flat();
来源：http://hz.smart0.xyz/gthmujcljg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtttghlqlw.html

Go:   // 手写双层循环
来源：http://hz.pycfn.com/gtctbkqfvp.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtpilcacav.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtvmfawyjq.html

[D19] 按字段分组
来源：http://hz.nanxuanxn.top/gtmbwmmsgr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtdkesmzdr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shzxlz.cn/gtmgzixtch.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtabujzdxq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gthcwkfgvw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtrcfzcztv.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtgghmnpvu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gtkeavumds.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtcpdzjffv.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtmhrojnit.html

Py:   Counter(arr)
来源：http://hz.xinyue.icu/gtnlhodwzf.html

PHP:  array_count_values($arr);
来源：http://hz.daria6918.cn/gtrorhoxsk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtwvcyfbuj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtscfjpeas.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gthqgdswdr.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gthsiavmsg.html

Ruby: arr.tally
来源：http://hz.shangyingyoupin.top/gtnsowjdkg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtjaxlllqk.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gtjgptwjbb.html

Py:   x in arr
来源：http://hz.yangfankeji.com/gtqzehydep.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daxiang520.top/gtyhbcxtci.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtxbcjediq.html

TS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtqshmhdpa.html

Java: list.contains(x)
来源：http://hz.fzhhl.top/gthqvtenaj.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtxvvknzwu.html

Ruby: arr.include?(x)
来源：http://hz.shangyingyoupin.top/gtfvnblouu.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtcxwiiphe.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fzhhl.top/gtsztenbsu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.svipenyu.cn/gtvcdepiwj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gtcjokwscf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtputhylen.html

TS:   [...arr];
来源：http://hz.cqqwz.cn/gtqzwyczio.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtxnwbumkf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aizwys.cn/gtnwtdykfp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtazghdjte.html

C#:   new List<int>(list);
来源：http://hz.zhoulong.xyz/gtavcgkdnr.html

[D23] reduce 累积计算
来源：http://hz.xingfuxueyuan.xyz/gtpbauufua.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtnesccooo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guowangkeji.top/gtkfxaxapu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtrqbrwmen.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtpedwidij.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtdtcpgudx.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtncnxzcfb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgfzy.top/gtwbgsohmc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fzhhl.top/gtmbrptvye.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gttkszmndf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tian-w.cn/gtiffeuwys.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.mhx1999.top/gteresqncw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cashguo.top/gtejbkkarl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gtkpidyavu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gttbzlqeey.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtnonyitxc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuxming.cn/gtutfyfrss.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtoasqdlkw.html

[D25] Set 集合去重与交并差
来源：http://hz.xuetiantiany.cn/gtxhaunryn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtcatamlia.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhiwuduotai.top/gtlycwirxy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.vqdsnc.cn/gtaftfwzgj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ppjwa.cn/gtemyrjlbi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenjidiqi.icu/gtvcrkrgfx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gtpzqibjdr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinyuanbaomall.cn/gtvacavkyl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtqsqdyidx.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtmuqpvxha.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gzhubu.top/gtezalgokl.html

PHP:  implode(", ", $arr);
来源：http://hz.meibo888.top/gtbbvtfomf.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtxxbbkhol.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gthjouhyvu.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtqzjooqsx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangshuangyany.cn/gtgxzbofle.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gttqrrgdic.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtfhuqbpje.html

================================================================================
来源：http://hz.gzhubu.top/gtahdbnvit.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtnqlchdtw.html

================================================================================
来源：http://hz.snrcjt.cn/gtixrtonfl.html

[E01] 拼接字符串
来源：http://hz.gzhubu.top/gtqtmjmssy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtvjizekxs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hammf.cn/gthlmbsusf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtyvzdywlq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtqmvsldoo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daria6918.cn/gtadzgarcc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yangfankeji.com/gtcqhuygvn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cdnleiting.top/gtisiwdxqi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtnjuuthwh.html

[E02] 重复字符串
来源：http://hz.fzhhl.top/gtppiqbkim.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtcwwsekhs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtvhpgxwbo.html

JS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtcutlpbkq.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtaagsxlbl.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtrmqtugsa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xylfe.cn/gtyfwvfvsb.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gthgyyuatq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtdosauhui.html

[E03] 截取子串
来源：http://hz.c1oappe.top/gthjlqokci.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.aizwys.cn/gtnowrdbbc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtjgbibung.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cucudq.cn/gtegxyjwcd.html

TS:   s.slice(1, 4)
来源：http://hz.hysaishi.cn/gtghqhwlsm.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtbblsmjrq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.redwolf501.top/gtnzhfyjsf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xingfuxueyuan.xyz/gtqsfwemfq.html

C#:   s.Substring(1, 3)
来源：http://hz.ybcxt.top/gtjcmbsnmm.html

[E04] 查找子串位置
来源：http://hz.ppjwa.cn/gtzvhgriqo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pengpengdd.cyou/gtojglurya.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtcssqqmwv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.smart0.xyz/gtltxjurok.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtiakimlfx.html

Java: s.indexOf("x")
来源：http://hz.hammf.cn/gtajnmlbgg.html

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gterphlkfj.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gtmplwzfbz.html

C#:   s.IndexOf("x")
来源：http://hz.wangshuangyany.cn/gtigrgqurs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigufen.top/gtnlnaauwa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.feifeiyinyue.top/gtvoqxwbus.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hywenlv.cn/gthwlqjhmq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gttrfbcdjx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gtwqlmbfth.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtxgdrqxjq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jiagoushi.top/gtauykhfpd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jlsjyb.cn/gtbyjajlqq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.meibo888.top/gtrdelphst.html

[E06] 替换子串
来源：http://hz.gogol.net.cn/gtoljxhaka.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gtfpaahiph.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.fengsongda.top/gtccxxwimt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtttnyzkox.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtgazsydyw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtpdhvcupl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtnfmpxblx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtceewopvy.html

C#:   s.Replace("a", "b")
来源：http://hz.zhengqikj.top/gtpgvnvqln.html

[E07] 按分隔符拆分
来源：http://hz.yangfankeji.com/gtulcolpjw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sweek.top/gttycmjcrf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daxiang520.top/gtskpxowcf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtoaqkfmbw.html

TS:   s.split(",")
来源：http://hz.ywan-chungtsiang.top/gtjuukjwjs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigfzy.top/gtftmfyfxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.meibo888.top/gtpvjlcdcs.html

Ruby: s.split(",");  s.split
来源：http://hz.havefunace.top/gtbtyyivdf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gttrhirhyp.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtlfjjqsim.html

Py:   ",".join(items)
来源：http://hz.daxiang520.top/gtwezowrmw.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtffsyhjxz.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gtshwkxsfs.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gtpotrzxyt.html

Java: String.join(",", items)
来源：http://hz.xuanzx.com/gtmbuklaan.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtvewuhung.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangkeji.top/gttvrulbdv.html

C#:   string.Join(",", items)
来源：http://hz.aizwys.cn/gtndujnciq.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtixqlgvmd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gttmnlfwzi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtiqvskxmc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gthbzbackk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnxiangtu.top/gtqmqazjpa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yanxiufei.cn/gttershzni.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinqigfzy.top/gtlhxtocar.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.bjfxy.top/gthhyqrpqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhijiandao.cn/gtkaivmkmf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.52xcode.cn/gtutxnbedz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtizwjswxf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtyrxtemar.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtqucjrrqt.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtwfoldhna.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtzcxsdyoz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtrymboewa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pycfn.com/gtgcsnnmeu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtuomctmts.html

[E11] 反转字符串
来源：http://hz.ydzc1.top/gtmtoyhtrq.html

Py:   s[::-1]
来源：http://hz.jiagoushi.top/gtydrshlgg.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtzeollkfq.html

JS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gtixqpdrzy.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gttnpfpdvc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtaavudzvd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtsywcwlti.html

Ruby: s.reverse
来源：http://hz.sufxvd.cn/gttlhndgty.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtdxrifigv.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtrraptyoq.html

Py:   s.count("a")
来源：http://hz.hysaishi.cn/gtwpgpkhcg.html

PHP:  substr_count($s, "a");
来源：http://hz.yuxming.cn/gtceaatvok.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtesdzdlza.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtcdjdaqkw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fzhhl.top/gtmqgyihft.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtlkbojvwe.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gtuicagqkv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yongpay.top/gtbbluyqdg.html

[E13] 逐字符遍历
来源：http://hz.sweek.top/gtlzmtrmfm.html

Py:   for ch in s: print(ch)
来源：http://hz.wangdashe.top/gtvkfarpby.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtvpwlbulk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtoobvolhk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtrvkpnksp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gthshqbwsg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gogol.net.cn/gtjmrciqky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cheryme.top/gtlbaxfhfp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtniowyopd.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtnpiczceo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuxming.cn/gtcuftkaqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.snrcjt.cn/gtbesajrab.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hammf.cn/gtvyqappsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tianlin.xyz/gtlhonedcw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cucudq.cn/gtupveudac.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtxijbacfd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.0kj1m.cn/gtevronqwo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gthgfuywyi.html

[E15] HTML 转义 / 反转义
来源：http://hz.0kj1m.cn/gtgmizkfqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtbqevoqng.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.redwolf501.top/gtldyqzbit.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sxryk.cn/gtdhtzkelx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtooxmfecx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigufen.top/gtvlznsbnu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sufxvd.cn/gttiwgtsaf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yongpay.top/gtrvruyjwt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gteskchpbc.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtdcxxacyq.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtuiiiwaqp.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtoqdimgqo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtowpwtymn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gteyyfxyuy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtevpnaujh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gthuwxnnhu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jlsjyb.cn/gtkmgnoadi.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258.top/gtbubyxnac.html

[E17] 首字母大写
来源：http://hz.zycfv.cn/gteigxmpwl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxinkj.top/gtevpwbhym.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtdlkzkmyk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtiacclkbk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtvdvucqql.html


<!-- 参考信息 -->