代发 wailian999

[D11] 反转数组
来源：http://hz.jinqigfzy.top/gtixoopdcp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sysykeji.top/gtobyijbbz.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtvyelyjqt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtzcxnlbqu.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtcmmovfiu.html

Java: Collections.reverse(list);
来源：http://hz.haohaochexian.top/gtdyqdeljl.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigfzy.top/gtluexrtsy.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtxiatgcuw.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtcjspuvrd.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtnbpvvyqy.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuxming.cn/gtgeusszwk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gtxknogyns.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtajozwuky.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cucudq.cn/gtwccvkpef.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zycfv.cn/gtcyxzzvgx.html

Go:   slices.Index(arr, x)
来源：http://hz.jlsjyb.cn/gtthgmraoo.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtknwhifmh.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gtywfwebgm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xziqi.cn/gtowqdwgvm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.quarkkingdee.top/gtfsalfyrc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtuhybyoft.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtxbexcage.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtmymdnvbg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtuxhaogjl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zycfv.cn/gtuhyqmqaw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sxryk.cn/gtunksuxxj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gtvyljoeld.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenjidiqi.icu/gtogtgewag.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhixingplan.top/gtpywwoyex.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.c1oappe.top/gtjqrzwbww.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtkzsbxcud.html

TS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtudqjqymt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtygsopmov.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtesaakqiw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gtjzhhllmv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cdnleiting.top/gtlnrjqizj.html

[D15] 去重
来源：http://hz.haohaochexian.top/gtthbmiken.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtfudkeiyp.html

PHP:  array_unique($arr);
来源：http://hz.ybcxt.top/gtfddbbhkv.html

JS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtarjjiqhc.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gttrswbofx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtroridbld.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.kuanghao11.cn/gtnzqjuayc.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gtknudpzpv.html

C#:   list.Distinct().ToList()
来源：http://hz.zhongyouzk.top/gtrnupcwcr.html

[D16] 求和与平均值
来源：http://hz.hysaishi.cn/gtqvvfqwtf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenzaomai.com/gtfdfgdvmj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtflbcugkz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtzvjjorri.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtbxjmazvy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtoudpyaon.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtjhklmkas.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtagpvngzr.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gtoohentkk.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtvnxoalix.html

Py:   max(arr);  min(arr)
来源：http://hz.hongshengwenyu.top/gtjatpaejh.html

PHP:  max($arr);  min($arr);
来源：http://hz.jiagoushi.top/gthyolagda.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ydjk.org.cn/gtleehriib.html

TS:   Math.max(...arr);
来源：http://hz.snrcjt.cn/gtcuolyxjd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtzjxvhjsu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gogol.net.cn/gthjjroldx.html

Ruby: arr.max;  arr.min
来源：http://hz.cqqwz.cn/gtloemuecj.html

C#:   list.Max();  list.Min()
来源：http://hz.chenzaomai.com/gtkwqbiyuc.html

[D18] 扁平化嵌套数组
来源：http://hz.snrcjt.cn/gtstwbhubs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinghuilouyu.cn/gtkxiigcea.html

PHP:  array_merge(...$nested);
来源：http://hz.ydjk.org.cn/gtygpcsnba.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtomoiudub.html

TS:   nested.flat();
来源：http://hz.zhengqikj.top/gtwqacjism.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgufenzy.top/gtdqmcaumf.html

Go:   // 手写双层循环
来源：http://hz.guowangkeji.top/gtndkmmjtg.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtnnnlwuum.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gtgkmavmep.html

[D19] 按字段分组
来源：http://hz.wangshuangyany.cn/gtrtdonzng.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtfhmwvows.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shzxlz.cn/gttjoaukvt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhijiandao.cn/gtdaxrmroi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gtgrfoptud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtfcgkcvtr.html

Go:   // 手写 map[string][]T
来源：http://hz.andypj.xyz/gtuzbljgml.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtzupyeihv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shangyingyoupin.top/gtzstayzty.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gticexychm.html

Py:   Counter(arr)
来源：http://hz.dashuyun.cn/gtlmhezxhc.html

PHP:  array_count_values($arr);
来源：http://hz.tanke756.top/gtpztcnqzq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtuybjiswz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtcoefajoa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtxqobajie.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigufen.top/gtbgpjbtik.html

Ruby: arr.tally
来源：http://hz.shanyushiyangkeji.top/gtqqlprruv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtmthkuebp.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gtogsravtn.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtwtjojeco.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtsrxtymsr.html

JS:   arr.includes(x)
来源：http://hz.xziqi.cn/gtozeupsad.html

TS:   arr.includes(x)
来源：http://hz.redwolf501.top/gtzszzmbgk.html

Java: list.contains(x)
来源：http://hz.316326.xyz/gtuzqhxocl.html

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtoqldnmar.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtvsppvlyc.html

C#:   list.Contains(x)
来源：http://hz.xuetiantiany.cn/gtjnrwffhm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xingfuxueyuan.xyz/gtnpqusukc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jiagoushi.top/gtmtqgfidb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnxiangtu.top/gtvaxlsxih.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jyoumei.cn/gtlmbvhbvj.html

TS:   [...arr];
来源：http://hz.andypj.xyz/gtuscjkfsr.html

Java: new ArrayList<>(list);
来源：http://hz.gogol.net.cn/gtxfqbwxgs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtywfvsmfb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj202588.top/gtadqohtdb.html

C#:   new List<int>(list);
来源：http://hz.nanxuanxn.top/gtyrdoneyp.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtkypufilp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zdqjudy.top/gtcqalgzgt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtmfuskstj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtavocnzxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtldsepibr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtwegpedki.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtjnlrvnxk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtfhnjpvlg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtvrcagxex.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenjidiqi.icu/gtkosjahes.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhijiandao.cn/gtlcvjggha.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gtxvgyrvel.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtdrgjrert.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtaolcszat.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.c1oappe.top/gthoxvwyub.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtaxriftyh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtnlhzxjyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.bjfxy.top/gtcqvpxprr.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gttsynrpex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhoulong.xyz/gtloovgpoq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtgpvssgyb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtbcutohlg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxinkj.top/gttytbporb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cucudq.cn/gtofyhcxiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtnfzwidlu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtouisfdur.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangkeji.top/gtjqgbfldq.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gteeoppjrp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daxiang520.top/gtkacrqyio.html

PHP:  implode(", ", $arr);
来源：http://hz.cucudq.cn/gtozoexibw.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtvuadswag.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gttjnisoig.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtdkpotgrr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.dashuyun.cn/gtiyzzxczr.html

Ruby: arr.join(", ")
来源：http://hz.sxryk.cn/gtojmbkxfu.html

C#:   string.Join(", ", list)
来源：http://hz.feifeiyinyue.top/gtqlzuvbsy.html

================================================================================
来源：http://hz.pycfn.com/gtpjyuixab.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtfqzveumy.html

================================================================================
来源：http://hz.jqgfzy.top/gtvaorpwuc.html

[E01] 拼接字符串
来源：http://hz.bjfxy.top/gtcxgdlzpt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.bjfxy.top/gtasshkdrt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cheryme.top/gtebecuorj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtxzywxnac.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtighfprki.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangtech.top/gtulfmsspw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gttcmlnvrt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dianchejie.cn/gtlrervvtn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.snrcjt.cn/gtcfkffsyl.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtbyuvhdkp.html

Py:   "ab" * 3
来源：http://hz.gotoacloud.top/gtfndwfgat.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daxiang520.top/gtfqmbojun.html

JS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtewhlpsat.html

TS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtserrhxdl.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtylqexxze.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hongshengwenyu.top/gtjptkezji.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gtugechmqu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.kuanghao11.cn/gtmclpfxqa.html

[E03] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtoexounpe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuxming.cn/gtdigorztl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gtxojgsvrj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtpehbqdao.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigufen.top/gtstcqmrse.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtbfcatcvd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jyoumei.cn/gtdqyvkpgu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtppsqzicl.html

C#:   s.Substring(1, 3)
来源：http://hz.jlsjyb.cn/gtqybznrhs.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtqvkbixfi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gtmbgectqq.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtckmeicly.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtvjxixplz.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtyffwxvfu.html

Java: s.indexOf("x")
来源：http://hz.shuidangran.top/gtpvuitrar.html

Go:   strings.Index(s, "x")
来源：http://hz.guowangkeji.top/gthjmnpaao.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gtrdeexcdl.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtyxyukyzs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtpzsjvjwu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtqgctvnxn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtzxqqlmoz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtfewvstox.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dashuyun.cn/gtxokszvdl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtxjdbvlgw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aizwys.cn/gtovndcciy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtqbfdulfh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.52xcode.cn/gtkcjifdlk.html

[E06] 替换子串
来源：http://hz.ehwqpu.com/gtxmzvlckd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtgjszyzcr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtvdatozlx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtrnmovbbh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtieisetfm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtcnmhrmzt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtgumqlhxq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhoulong.xyz/gtgeufugxe.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtcjgbnfai.html

[E07] 按分隔符拆分
来源：http://hz.jianghu66.top/gtxxmyvvhd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuetiantiany.cn/gtmbodcrib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtgrylvtwx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ehwqpu.com/gtnpggynzw.html

TS:   s.split(",")
来源：http://hz.xingfuxueyuan.xyz/gtcspiujdx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtypnznyap.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jiagoushi.top/gtdkybxijs.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtflxelyhl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gotoacloud.top/gtmeehtzmz.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtfcavxtww.html

Py:   ",".join(items)
来源：http://hz.sweek.top/gtclnsjfqy.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtxuphbzug.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtfxyazwfl.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtzjtcmmnp.html

Java: String.join(",", items)
来源：http://hz.svipenyu.cn/gtarripcvw.html

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gtksbovgdg.html

Ruby: items.join(",")
来源：http://hz.fzhhl.top/gtjfmywxek.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtrlfzhlla.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtownqrlnd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtimesgmwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtcdxrczgk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtyjvcxlve.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtrwwaumia.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtjccggpdk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtjrzoiisp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhijiandao.cn/gttrapnsai.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtmnxyceun.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gtczxztccb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.snrcjt.cn/gtlnqqnopz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtxrxnbepl.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtuwvrykln.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtignrsybs.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gtoesuhgjj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtvcuxpbkn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtfwfqhjgm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dashuyun.cn/gtbbiqvsqz.html

[E11] 反转字符串
来源：http://hz.pengpengdd.cyou/gtacdisjoy.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtctxfvalo.html

PHP:  strrev($s);
来源：http://hz.andypj.xyz/gterqliflm.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtirsgxves.html

TS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtvcplctqo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daria6918.cn/gtwfinefsu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xylfe.cn/gtuwkkabld.html

Ruby: s.reverse
来源：http://hz.jinqigufen.top/gtbthapysx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtrfqdiwlz.html

[E12] 统计某字符出现次数
来源：http://hz.havefunace.top/gtazbqvtnr.html

Py:   s.count("a")
来源：http://hz.sweek.top/gtuyyxinuv.html

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gtmdwhgimd.html

JS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtttqbhppn.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtuqkwkamd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuanzhike.top/gtkfduegkn.html

Go:   strings.Count(s, "a")
来源：http://hz.xziqi.cn/gtssbgjcvf.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtsksflnvw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtneprfkdm.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtgybzscgk.html

Py:   for ch in s: print(ch)
来源：http://hz.yongpay.top/gtelrrxsww.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hysaishi.cn/gtxwqeqzdd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gthuidrzfi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtdvbdzszp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtpubgeadn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtyppalujq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj202588.top/gtstultzhu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.iojbl.cn/gtfyqofprq.html

[E14] URL 编码与 Base64
来源：http://hz.chenjidiqi.icu/gthdntsnbt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.havefunace.top/gtnabjtfeb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydjk.org.cn/gtzvitlwyf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yongpay.top/gtewnepihw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtewsascto.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gaohongyu789.top/gtucevywgi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtfewdgmvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gthlzzvwyg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hfpthk.cn/gtezrwwtgu.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtraitrdpw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sweek.top/gtcebwkjqw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gtkuhtyodm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.wangdashe.top/gtntxubxtq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ybcxt.top/gtctartxwx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtyrdjzlkg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gtasiwvcjm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtllwkmuvi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.feifeiyinyue.top/gtynjjwify.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gtfequsdtr.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtovmhsrjb.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtkaiwlnlz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtkujbvill.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtowjqgrka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtloyomxfu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnqzz.top/gtrevxnlzs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sysykeji.top/gtkdhmmbhq.html

C#:   1234567.ToString("N0")
来源：http://hz.svipenyu.cn/gtoyednegf.html

[E17] 首字母大写
来源：http://hz.jlsjyb.cn/gtgozzzcan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangdashe.top/gtnhlujqgg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtpbhypiav.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtmhlhvoou.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gthqxbnbma.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yonumen.top/gtblccjjxb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtxkxmihyw.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtdskxqzxm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gtynznjjvs.html


<!-- 参考信息 -->