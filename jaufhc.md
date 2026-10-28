代发 wailian999

[D11] 反转数组
来源：http://hz.jinqigfzy.top/gtkpbyfbeu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtlfkhexku.html

PHP:  array_reverse($arr);
来源：http://hz.jlsjyb.cn/gtozrusbyi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.kuanghao11.cn/gtdcxnahsk.html

TS:   [...arr].reverse();
来源：http://hz.cheryme.top/gtkaezaitz.html

Java: Collections.reverse(list);
来源：http://hz.birdmap.top/gtmphdefrg.html

Go:   slices.Reverse(arr)
来源：http://hz.zhijiandao.cn/gtnfjqiqkr.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtcvuhxolg.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gtecziblcg.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtacnybfyo.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gtbgwjplsd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zdqjudy.top/gtquplccsw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtltlmugld.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtnmmakvsz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhaomingkeji.xyz/gtbrqqkgvt.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtcmdebvrs.html

Ruby: arr.index(x)
来源：http://hz.jyoumei.cn/gtwmrdiaky.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtkiibzfmf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtzijfmyih.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tanke756.top/gthtsezlli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guannengcc.top/gthnzbmhrn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtprpbtdtr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtokwaaaue.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guowangkeji.top/gtgxjkpone.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gtamjhhicv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ppjwa.cn/gtwbsxctcg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtxfryuuie.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xinyue.icu/gtbtguumnj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenzaomai.com/gtgcadzzvm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yonumen.top/gtjsloufgb.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtdsqnjnjz.html

TS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtkjywpasw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zdqjudy.top/gtskqbwyza.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtsqlxypnv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shuidangran.top/gtibvctomu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxuanxn.top/gtelrdmnio.html

[D15] 去重
来源：http://hz.ehwqpu.com/gthktdzvms.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtmdopcrcq.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtdljezgwi.html

JS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtihixbrmt.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtjddnvqky.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtndstdfnq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtvzuhferf.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtjtjvjsck.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gtylesktgf.html

[D16] 求和与平均值
来源：http://hz.yvedp.cn/gtwiwsjqmo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtcohrtqmd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtsqhoukvz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtdbfoguqy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtcujqlgfy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ivvv.top/gtpoeksmhl.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gttdchzvqt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtloofpovt.html

C#:   list.Sum();  list.Average()
来源：http://hz.havefunace.top/gtibcwxsgh.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtafmltfhw.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtowctofic.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gthhrhhqbe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xylfe.cn/gtsabwxjaz.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtrcnzgjma.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sxryk.cn/gtidvufbwd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtubobjcgn.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtsbpnrtjo.html

C#:   list.Max();  list.Min()
来源：http://hz.yj202588.top/gtrogyinae.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigfzy.top/gtjuhjzwoe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtiylagfpc.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gtggryiluh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtltxmtvty.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtqfxaarys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cheryme.top/gtpjetbhyw.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtanfirwpc.html

Ruby: nested.flatten
来源：http://hz.meibo888.top/gtsmqhmncv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jiagoushi.top/gtmmjwfkjv.html

[D19] 按字段分组
来源：http://hz.smart0.xyz/gtfqrremzm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtiijvtibe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtaccqxsfk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtwjclwosm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtugqlsazl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xinyue.icu/gtyjwjchni.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtbgbrfyym.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zdqjudy.top/gtyoclpikl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtqrsdecza.html

[D20] 统计每个元素出现次数
来源：http://hz.c1oappe.top/gtaqvhvrdk.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtsngbjrjf.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtatwlbwex.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtqexcavtv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtluqagalg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtmpvceeuc.html

Go:   // 手写 map[T]int
来源：http://hz.9152youxi.cn/gtatlcztpx.html

Ruby: arr.tally
来源：http://hz.hammf.cn/gtsdbptdan.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuanzhike.top/gtwzqgrxie.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtcgejcxrv.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtftgopdjr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtoltutvrg.html

JS:   arr.includes(x)
来源：http://hz.xuanzx.com/gthlgonxcg.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtipqpjxfc.html

Java: list.contains(x)
来源：http://hz.cqqwz.cn/gtoatvgsmj.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtgfgfpuml.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gthhautztb.html

C#:   list.Contains(x)
来源：http://hz.chenjidiqi.icu/gtvqvjpjqn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gtggwcamud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtugegfxyo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.0kj1m.cn/gtfjcojulu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fengsongda.top/gtoxicugci.html

TS:   [...arr];
来源：http://hz.jlsjyb.cn/gtqgrwohzu.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtxgzrldrf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuanzhike.top/gtitrbgttr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xingfuxueyuan.xyz/gtvaqokunl.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtbiizzvsp.html

[D23] reduce 累积计算
来源：http://hz.nanxinkj.top/gtxivqciqf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtiypaehvt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ybcxt.top/gtxfwdybjv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtcjerrmgc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtyhycdbhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gtnqvuxjyw.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtvrokuxfp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtutydxhyd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jlsjyb.cn/gtcazxrpkg.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtjvgvjvmk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhongyouzk.top/gtiiivyztn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtsofclrys.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jyoumei.cn/gtmfnetwmy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.guannengcc.top/gtggtrbyfk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jianghu66.top/gtihsiqssl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtpcpwbynt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pycfn.com/gtjmcfakyo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtxxurhgha.html

[D25] Set 集合去重与交并差
来源：http://hz.pengpengdd.cyou/gthkvwbtak.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gthcmubtef.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtlxwnweld.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtwjvotphi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tianlin.xyz/gtkdxiuvbi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtvdzvldip.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.haohaochexian.top/gtmcjjnbnr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daria6918.cn/gttzxuonyr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.andypj.xyz/gtokclhyfq.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtcstbuhay.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtvsuztadi.html

PHP:  implode(", ", $arr);
来源：http://hz.gogol.net.cn/gtupffprki.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtcnukbvjx.html

TS:   arr.join(", ")
来源：http://hz.meibo888.top/gtbcugciqh.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gtqpfduqfc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jyoumei.cn/gtqrlvsdnl.html

Ruby: arr.join(", ")
来源：http://hz.smart0.xyz/gtsncxkwnj.html

C#:   string.Join(", ", list)
来源：http://hz.xylfe.cn/gtdzdimpfa.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtolhavuyh.html

E. 字符串处理
来源：http://hz.sweek.top/gtsuughehf.html

================================================================================
来源：http://hz.zycfv.cn/gtzoxdamki.html

[E01] 拼接字符串
来源：http://hz.hammf.cn/gteosvxrgw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hongshengwenyu.top/gtcydacxkn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtittbvxqg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtoiujizkv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtbxskhgcy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtduwbzcda.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtviqasqgt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gtjwstopyq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.quarkkingdee.top/gtmiqzytuk.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtuwjrwsmn.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtyrqpvbmr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gtmjysydom.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtotavense.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gthcxgfnrg.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtszkxurxs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtumehujzy.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gtgxivipvn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tian-w.cn/gtdylsgufs.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtzklsycsx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtecgmfsbo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cdnleiting.top/gtotmoorld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtcebbykzg.html

TS:   s.slice(1, 4)
来源：http://hz.9152youxi.cn/gtonzdsnur.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtraveblzl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tianlin.xyz/gtjgojlgeo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cdnleiting.top/gtptlcsrnc.html

C#:   s.Substring(1, 3)
来源：http://hz.andypj.xyz/gtemgmwljc.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtcjvbsohp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gthennsdja.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gtpvmhveis.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jlsjyb.cn/gtlupbdvrp.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtfvlrvcmg.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtbdgozufa.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtbzcdgvxy.html

Ruby: s.index("x")
来源：http://hz.hfpthk.cn/gtvztvduxi.html

C#:   s.IndexOf("x")
来源：http://hz.316326.xyz/gtrceahqbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gaohongyu789.top/gtgtoxvqzf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cqqwz.cn/gtbwrbccsc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtfwumbpew.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtystggzng.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hammf.cn/gtikasiewj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtkowlygxu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtifhkynld.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangtech.top/gtezuvptud.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxinkj.top/gtgfkpwnfn.html

[E06] 替换子串
来源：http://hz.shanyushiyangkeji.top/gtwkkhmmfs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtgjjsbiil.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ybcxt.top/gtkrpaznsb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtrtujiofj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gthsxkhplf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtijebyxcm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yongpay.top/gtdvewttvu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gtxeqiiudk.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxuanxn.top/gtclugxhsq.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtuiboumaw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cdnleiting.top/gtmfalrnga.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtuxwcffre.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenjidiqi.icu/gtcngdkrbf.html

TS:   s.split(",")
来源：http://hz.zhongyouzk.top/gtbviagfwa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtpaqxryld.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gzhubu.top/gtzunsqpfs.html

Ruby: s.split(",");  s.split
来源：http://hz.sysykeji.top/gtrcuchdqo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtsktfaowx.html

[E08] 数组按分隔符合并
来源：http://hz.jyoumei.cn/gtsksuvzlq.html

Py:   ",".join(items)
来源：http://hz.0kj1m.cn/gtqtgalzsd.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtbsvacpxg.html

JS:   items.join(",")
来源：http://hz.hnxiangtu.top/gtrdlrefmr.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtkjeuqggs.html

Java: String.join(",", items)
来源：http://hz.zdqjudy.top/gteeekorxv.html

Go:   strings.Join(items, ",")
来源：http://hz.gogol.net.cn/gtcdcqaqoh.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gtoqqggktc.html

C#:   string.Join(",", items)
来源：http://hz.dianchejie.cn/gtemqkdhkn.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtxeoxaanf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtulpmlntc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtwuonfrle.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtbvhofscq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtszhzujmk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gtisanwarg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gtwfqnucwg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jiagoushi.top/gtjwuslqsy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtvqzrxrzx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gttaphfyci.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yueranfly.top/gtkstxwoii.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aibaodan.cn/gthteapwbm.html

JS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtrxqzfcek.html

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtjpbihpge.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gtcvjhulxd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zycfv.cn/gtzgpwhfes.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.52xcode.cn/gthqdssogi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtunferpfh.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gtqrqdcetf.html

Py:   s[::-1]
来源：http://hz.yanxiufei.cn/gtnxwkyqil.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtmtiesfgy.html

JS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtanwmorhp.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtsldfuonl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ybcxt.top/gtsztmmpsw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinqigfzy.top/gtyibtwbfy.html

Ruby: s.reverse
来源：http://hz.jinqigufen.top/gtvlcfqhdv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtnzvwdsoi.html

[E12] 统计某字符出现次数
来源：http://hz.cdnleiting.top/gtyrvbgmio.html

Py:   s.count("a")
来源：http://hz.xuetiantiany.cn/gthpizmgnw.html

PHP:  substr_count($s, "a");
来源：http://hz.quarkkingdee.top/gtqxodynto.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gttfslieip.html

TS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtppiocesy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtwaztdzkm.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtqakpfhym.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtidlshlxa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtvpuxblxi.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtshnsojet.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtpwavyhvj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gtkbrggydu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtonraidlx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtjvhfgdfs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gtlyfctzrs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yonumen.top/gtttzzvtfg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hongshengwenyu.top/gtjbfgvrkz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xziqi.cn/gtilfugimo.html

[E14] URL 编码与 Base64
来源：http://hz.tianlin.xyz/gtwyeepjsv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gthozipxbo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtssfoympd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gtcxagixmb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtbpzmdsps.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tanke756.top/gttbgieayq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtzztsjqed.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.iojbl.cn/gtyigjtozz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtjcdglnxe.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtslyioure.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtuhjiybul.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zdqjudy.top/gtrpaawtzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtrpunnncn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hammf.cn/gtemdifleh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenjidiqi.icu/gtqvgirtyz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangshuangyany.cn/gtumrcoezq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhixingplan.top/gttnjnknsw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtylrlgvog.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtsanrlrnl.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtoiueflwj.html

PHP:  number_format(1234567);
来源：http://hz.cheryme.top/gtnjlirouy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtcxzznokj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtdpjkeylr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gtwwcwyewh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangdashe.top/gtpiaslgcp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtxerzycdf.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtdnghqsvs.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtlfbfxiiw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cheryme.top/gtnnhveybx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yanxiufei.cn/gtdjpntlsw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gtvrzbpkbz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtykhwhlor.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.9152youxi.cn/gtdqxcldqt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangtech.top/gtvniumeco.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtbjlefhmw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtmkbfngfd.html


<!-- 参考信息 -->