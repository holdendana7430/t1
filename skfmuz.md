代发 wailian999

[D11] 反转数组
来源：http://hz.nanxuanxn.top/gtlipcwlpi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenzaomai.com/gtuutbrcuo.html

PHP:  array_reverse($arr);
来源：http://hz.zhixingplan.top/gtbnqzikrm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gttbywzqok.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtzukqadaf.html

Java: Collections.reverse(list);
来源：http://hz.jqgufenzy.top/gterwebapv.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtoqyzoowe.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtbxzsvcng.html

C#:   list.Reverse();
来源：http://hz.zhongyouzk.top/gtcmmzhdom.html

[D12] 查找元素下标
来源：http://hz.meibo888.top/gtsmcozsuo.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtwegislzn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtgmsjyttc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtjfmlmjjj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtmpcsgiui.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtxhmmusxy.html

Go:   slices.Index(arr, x)
来源：http://hz.gaohongyu789.top/gttzuwkmsk.html

Ruby: arr.index(x)
来源：http://hz.snrcjt.cn/gttxxoyvbi.html

C#:   list.IndexOf(x);
来源：http://hz.nanxuanxn.top/gtestbwtmy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gthjabbcki.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gtvatpjlxs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jyoumei.cn/gtvoovmsud.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtecrjrvlq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gtqixsszfl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinyuanbaomall.cn/gtkannwqqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pycfn.com/gtcgcljdqq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnqzz.top/gtoqwzphlz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtnumxdymb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtgblawkqb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jianghu66.top/gtlvwqrrbm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangkeji.top/gthkgosgsz.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtybsskyha.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtraebosnr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtwpgfyufn.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtjwemmiaj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtowjarkfi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtodddrsqq.html

[D15] 去重
来源：http://hz.guannengcc.top/gtjdpeyxsx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtfmnmqqhj.html

PHP:  array_unique($arr);
来源：http://hz.vqdsnc.cn/gtaovwwktn.html

JS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtwvsidslc.html

TS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtmpabxxoo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daria6918.cn/gtdkrihgby.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtpwyzlpar.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtjilgcnus.html

C#:   list.Distinct().ToList()
来源：http://hz.dashuyun.cn/gttqpkmfsb.html

[D16] 求和与平均值
来源：http://hz.sufxvd.cn/gtgptrzhfc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtzovedwmd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtitgduyfq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtjaomgkus.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtkrpdcbii.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigufen.top/gtdutemxzh.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtkjqtdhwv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gtqbgkqbnw.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtpdhkfvrj.html

[D17] 最大值与最小值
来源：http://hz.yuxming.cn/gtodpoaugs.html

Py:   max(arr);  min(arr)
来源：http://hz.gzhubu.top/gtyilfhden.html

PHP:  max($arr);  min($arr);
来源：http://hz.havefunace.top/gtykidkswl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tanke756.top/gtrjycqexv.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtttgcrowp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.snrcjt.cn/gthsuyougx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtexuvzcfz.html

Ruby: arr.max;  arr.min
来源：http://hz.ppjwa.cn/gttjhedevf.html

C#:   list.Max();  list.Min()
来源：http://hz.xingfuxueyuan.xyz/gtnohysosx.html

[D18] 扁平化嵌套数组
来源：http://hz.pengpengdd.cyou/gtllkdhyoe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtsgvfjqej.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtlowzkvii.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shuidangran.top/gtortyosjh.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtjyldpyob.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenjidiqi.icu/gttsftgsrq.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtlksywdtd.html

Ruby: nested.flatten
来源：http://hz.cqqwz.cn/gtjsxfhdre.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtlusxesgm.html

[D19] 按字段分组
来源：http://hz.zhongyouzk.top/gtswgkdpgg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtsrdrlrpx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtbrcandzr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtwwgybzrj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.smart0.xyz/gtnpxisgvt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangdashe.top/gtmtgfbfdo.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtmzlnefxm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sweek.top/gtvqedxmhr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtnfrcabil.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gthqbszbzj.html

Py:   Counter(arr)
来源：http://hz.hysaishi.cn/gtzetnmoca.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtvccpejem.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtujdihthf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtmzffnncb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtdcaxnrck.html

Go:   // 手写 map[T]int
来源：http://hz.yuxming.cn/gtllvalvkz.html

Ruby: arr.tally
来源：http://hz.zhixingplan.top/gtqkvvgqed.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtmnkwnoea.html

[D21] 判断是否包含某元素
来源：http://hz.shuidangran.top/gtjbydnuup.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtpmpcnpoa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gogol.net.cn/gtjoenlswf.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtuzumzejv.html

TS:   arr.includes(x)
来源：http://hz.xinyue.icu/gteejktttj.html

Java: list.contains(x)
来源：http://hz.hnxiangtu.top/gtlbvvnitd.html

Go:   slices.Contains(arr, x)
来源：http://hz.vqdsnc.cn/gtrcsytgsm.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtvxtubksq.html

C#:   list.Contains(x)
来源：http://hz.yonumen.top/gtlivynelp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtmaejrcws.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtshfnkuhy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtdlulggec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hfpthk.cn/gtcuyafuke.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtkwqsiefa.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtjzvnasia.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aibaodan.cn/gtrqzcuecl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gtgfjuhlxl.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtrifdrmcp.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gtseioqovy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aizwys.cn/gtauhyuyee.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhiwuduotai.top/gtnqqzvcjl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtqacvrdxp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gthzluzluf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sxryk.cn/gtzgsahzwh.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtrvojtiye.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guowangkeji.top/gticydbtqf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gtolubsqws.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtnpnaswan.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangshuangyany.cn/gtkipyfrio.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gogol.net.cn/gtwrdkavln.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtxsrmhthc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hfpthk.cn/gtjwwofzfo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuxming.cn/gtvikkrtiu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.mhx1999.top/gtvqnuinvx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtiwrkkwua.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtimtptpsi.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtfsaypbgu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gthhpgemqt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yangfankeji.com/gtnpicngrk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtuylekbxv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtbbiqyuky.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.smart0.xyz/gtvbajrymp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gtxjcnhgto.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nwbrower.top/gtqnrbelhc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.svipenyu.cn/gthjcvnbue.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtqujovthl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinyuanbaomall.cn/gtmdzirfpp.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtbbsqqvrh.html

JS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtjqkyshya.html

TS:   arr.join(", ")
来源：http://hz.hammf.cn/gtykgxlahv.html

Java: String.join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtocanwsds.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gogol.net.cn/gtwkmrwcdw.html

Ruby: arr.join(", ")
来源：http://hz.shzxlz.cn/gtbndzdpiw.html

C#:   string.Join(", ", list)
来源：http://hz.chenzaomai.com/gtqyfqbyzs.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtuzydcsfl.html

E. 字符串处理
来源：http://hz.hnqzz.top/gtoexylmyk.html

================================================================================
来源：http://hz.havefunace.top/gtrvtnyitj.html

[E01] 拼接字符串
来源：http://hz.shuidangran.top/gtqiosxgcg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tianlin.xyz/gteetnjvcc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydzc1.top/gtmiztfbwn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtkalbyodz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtgszsusxu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenzaomai.com/gtlhooxxfm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtdbeaksem.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gtuiggeaof.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gtgrilwich.html

[E02] 重复字符串
来源：http://hz.nanxinkj.top/gtvfadgiqw.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gtvdnhfmbf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sufxvd.cn/gtbxstisef.html

JS:   "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtjwpcdjnv.html

TS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtuxobsneo.html

Java: "ab".repeat(3)
来源：http://hz.gzhubu.top/gtcuxdurnm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtjgcmbitr.html

Ruby: "ab" * 3
来源：http://hz.shuidangran.top/gtoczjlgih.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtwswwkcpy.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtwdksaril.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtghipbzre.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtfouhnovx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtuudzwwel.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gtlsfruvtb.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtbcsnkoer.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gttgwxevqi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xingfuxueyuan.xyz/gtneirzhlc.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtusypoauo.html

[E04] 查找子串位置
来源：http://hz.gogol.net.cn/gtvybkfszn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtotdaprml.html

PHP:  strpos($s, "x");
来源：http://hz.tian-w.cn/gttluintrp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gtnjelpppe.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gtdfbjcbjz.html

Java: s.indexOf("x")
来源：http://hz.tanke756.top/gtzejiyyaw.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigufen.top/gtccypenzd.html

Ruby: s.index("x")
来源：http://hz.wangshuangyany.cn/gtlnsmoqge.html

C#:   s.IndexOf("x")
来源：http://hz.mhx1999.top/gtgqzedjal.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtdszefxnp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zdqjudy.top/gtfvmpbcvk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtmpadjuwf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gtimozoxit.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtyccahjqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtgeozivtg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cdnleiting.top/gtynowolkq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtpgjebsty.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yangfankeji.com/gtybyaduds.html

[E06] 替换子串
来源：http://hz.chenjidiqi.icu/gtblcedewz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shuidangran.top/gtverafknl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gtdjypkfzb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtydgminug.html

TS:   s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtlnkyvqcz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtkmhymelm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtdcjczxsv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.9152youxi.cn/gtrjrtbkvz.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtcurwcclt.html

[E07] 按分隔符拆分
来源：http://hz.sweek.top/gtxnncjbbn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.quarkkingdee.top/gtmklmkuii.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtnripdaeb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.quarkkingdee.top/gtwskbgydt.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtxlqbcvlb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jiagoushi.top/gtbytsesxv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuanzx.com/gtflrvqqiu.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangkeji.top/gtymqtnico.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yonumen.top/gtwnajgpkt.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtyftevrgw.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtejxlkpfv.html

PHP:  implode(",", $items);
来源：http://hz.pengpengdd.cyou/gtnuufmcqe.html

JS:   items.join(",")
来源：http://hz.havefunace.top/gtqzriqkgu.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtijlkmsoe.html

Java: String.join(",", items)
来源：http://hz.fengsongda.top/gtckqbwgdb.html

Go:   strings.Join(items, ",")
来源：http://hz.hfpthk.cn/gtfkuwspss.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtslyacblp.html

C#:   string.Join(",", items)
来源：http://hz.shangyingyoupin.top/gtxibgsdri.html

[E09] 去除所有空白字符
来源：http://hz.gogol.net.cn/gtrjrreoxh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gteoifrrst.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtrogzridx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtdbgoxgmt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtspdeadsq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtvoutsoqn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtchqmbcim.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gtmypgpdso.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gtavhkkmuh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnqzz.top/gtqurwzczs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtgohqbsqa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gtjqhlspad.html

JS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtmusjerpw.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gthrlofrmt.html

Java: String.format("%03d", 7)
来源：http://hz.nanxinkj.top/gthebldgau.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtxesjggeg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtoixhsxpx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.kuanghao11.cn/gteycvdkpo.html

[E11] 反转字符串
来源：http://hz.hammf.cn/gtaiautlll.html

Py:   s[::-1]
来源：http://hz.dashuyun.cn/gtzhzuzkmu.html

PHP:  strrev($s);
来源：http://hz.nwbrower.top/gteplpfvkj.html

JS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtwljkzuyy.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtzhfexiaj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgfzy.top/gtjstmkkqy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgufenzy.top/gtyzrlrlvf.html

Ruby: s.reverse
来源：http://hz.meibo888.top/gtwdwmgely.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gttzwylfdr.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtvpfkaoml.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtenerxiga.html

PHP:  substr_count($s, "a");
来源：http://hz.yueranfly.top/gtfaolvgfu.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtiyhwqkuc.html

TS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtudbmxfhf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtirhjmkki.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtxoxqpjfu.html

Ruby: s.count("a")
来源：http://hz.fzhhl.top/gtzszgyipv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtnjzgsnoi.html

[E13] 逐字符遍历
来源：http://hz.xinyue.icu/gtfrdpfqxk.html

Py:   for ch in s: print(ch)
来源：http://hz.mhx1999.top/gtyasqibhk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.vqdsnc.cn/gtuavguhmi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtoxvyyucc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtaoiguseb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtojgfylke.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtvtivpbte.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtnqritcxr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.9152youxi.cn/gtmbwikbth.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtegmirxpt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtabegdhic.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gaohongyu789.top/gtdgeypuma.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gttkrwfpwt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.redwolf501.top/gtiagsbato.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtnzktnfml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtvfzpbfhb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtxejtptls.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guannengcc.top/gtmdpnttvj.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtwtyajfhw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtumibzhel.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtgbcmilal.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtgeolucit.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenlongwang.top/gttehhtzsf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gtsbabnjga.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtjqqqqmjj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnqzz.top/gtakvqpehd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydzc1.top/gtsfzlgrjl.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gtnjlkgvwq.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtfnvosyad.html

PHP:  number_format(1234567);
来源：http://hz.xinyue.icu/gtpvtkeopm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtvvovutgw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtblhzmwwe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtmsyilpep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangtech.top/gtlqqhqlvz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtdezsijuw.html

C#:   1234567.ToString("N0")
来源：http://hz.quarkkingdee.top/gtjasbtwrc.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtxxopagkz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.aizwys.cn/gtorgxginq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hysaishi.cn/gttybllfxt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtbiwgmffy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtlsaprxtw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhongyouzk.top/gtisjarurt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258.top/gtbzikurbv.html

Ruby: s.capitalize
来源：http://hz.hywenlv.cn/gtighsdrpf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aizwys.cn/gtheclatwr.html


<!-- 参考信息 -->