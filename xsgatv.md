代发 wailian999

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtykhtkcwr.html

[D12] 查找元素下标
来源：http://hz.yuanzhike.top/gtfkgtwhuy.html

Py:   arr.index(x);  x in arr
来源：http://hz.xingfuxueyuan.xyz/gtqxghqspi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gzhubu.top/gtdflummkt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtsqvxacyq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtmxcrznbs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtvxjqwmgt.html

Go:   slices.Index(arr, x)
来源：http://hz.yonumen.top/gttaewghmu.html

Ruby: arr.index(x)
来源：http://hz.ppjwa.cn/gtxntierze.html

C#:   list.IndexOf(x);
来源：http://hz.yanxiufei.cn/gtcgywktct.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daxiang520.top/gtbvpqetse.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydjk.org.cn/gtvcscthgz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtplezifyp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtaxlrrxvp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtiysuyvmp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.bjfxy.top/gtrihmhach.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtscmrefqx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gteqwzfwda.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtjorfkipg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hammf.cn/gtziutcrgj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yvedp.cn/gtuzgmxxuy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtkxgwqxoo.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtokpihwdi.html

TS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtuczadqsz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtrfwewlkv.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtfzlzzifh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gtvcvbonrm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigufen.top/gtnmfntjaw.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtgonyuwxb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtslrpbcva.html

PHP:  array_unique($arr);
来源：http://hz.jyoumei.cn/gtxmofwnhm.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtlqvmebxn.html

TS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtxvlpldyg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtdqtgdukl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtivmyzwge.html

Ruby: arr.uniq
来源：http://hz.nanxinkj.top/gtxmohfmib.html

C#:   list.Distinct().ToList()
来源：http://hz.guowangkeji.top/gtalyzohym.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtmlexvatz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yongpay.top/gtwdzwqrgg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shzxlz.cn/gtjurctzcj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtzlhdvgmy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gteerjusqn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnxiangtu.top/gtyqublkem.html

Go:   // 手写循环累加
来源：http://hz.smart0.xyz/gtbhddrbbz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yonumen.top/gtfbcsvtii.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgfzy.top/gthyurdals.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gtbrrvjlaq.html

Py:   max(arr);  min(arr)
来源：http://hz.yuanzhike.top/gtquteuhuy.html

PHP:  max($arr);  min($arr);
来源：http://hz.aibaodan.cn/gthpyvdzsn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtumwfczvo.html

TS:   Math.max(...arr);
来源：http://hz.jqgufenzy.top/gtmlbjaqlc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.quarkkingdee.top/gtadslnxvb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtqkihilwg.html

Ruby: arr.max;  arr.min
来源：http://hz.jiagoushi.top/gthrqyvgku.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gtgliusgxu.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtfxyssxuw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ivvv.top/gtohuwslzf.html

PHP:  array_merge(...$nested);
来源：http://hz.yuxming.cn/gtjhbahpqh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aibaodan.cn/gtljakjsrl.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtatotsfbk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shuidangran.top/gtwsjxlrbu.html

Go:   // 手写双层循环
来源：http://hz.jiagoushi.top/gtxeehgkdk.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtjbxedbdb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtchroivqi.html

[D19] 按字段分组
来源：http://hz.mhx1999.top/gtteoxlvjj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.9152youxi.cn/gtdmkqalkv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yvedp.cn/gtwrocvixc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.c1oappe.top/gtxgeudsof.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtrhbcciza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daxiang520.top/gtuocduenq.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258888.top/gtkbepcags.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gtayfxqyun.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hammf.cn/gtxxrxobmf.html

[D20] 统计每个元素出现次数
来源：http://hz.shzxlz.cn/gtdszajbpc.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtwqkabjgc.html

PHP:  array_count_values($arr);
来源：http://hz.yangfankeji.com/gtanmmpklp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtbfqgfcue.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtbnmbuerv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yonumen.top/gtuouidsel.html

Go:   // 手写 map[T]int
来源：http://hz.zhoulong.xyz/gtzydzhsyc.html

Ruby: arr.tally
来源：http://hz.bjfxy.top/gtsgnagyiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtynhbjyei.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gtsdpskwrl.html

Py:   x in arr
来源：http://hz.ivvv.top/gtjirwehzf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.9152youxi.cn/gtrtlvefyy.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtpismbgwx.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtapmivqbe.html

Java: list.contains(x)
来源：http://hz.cqqwz.cn/gtkgvlemxt.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gtwbhjvapb.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtceliqgdb.html

C#:   list.Contains(x)
来源：http://hz.hnqzz.top/gtjqfkspbq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ivvv.top/gtleucptkj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtmemnavtb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gotoacloud.top/gtrvsigick.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xingfuxueyuan.xyz/gtnpyfbbbr.html

TS:   [...arr];
来源：http://hz.gotoacloud.top/gtadcnbihw.html

Java: new ArrayList<>(list);
来源：http://hz.nanxuanxn.top/gtbiongdzw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtiybdhjfd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258888.top/gttxlwjbcf.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtcsecopug.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtcgehzsse.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtbydczskq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangtech.top/gtwocshqyc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtwdkbobbr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtjhgijhne.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgfzy.top/gtskradegp.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtetccjbzw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.iojbl.cn/gtufbuclnz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtlmvziigz.html

[D24] 字典 / Map 基本操作
来源：http://hz.dashuyun.cn/gtmzcygxrg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhijiandao.cn/gtjknbdxoq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tianlin.xyz/gtpsbjbema.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hywenlv.cn/gtifkicejh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.feifeiyinyue.top/gtfnfzztap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jyoumei.cn/gtgvogpyig.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dashuyun.cn/gtibaeizxd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sxryk.cn/gthdqptjjr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jlsjyb.cn/gtwmyltbwq.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtmvsgjjfu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.feifeiyinyue.top/gtnstverzq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtyavfkjdf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuanzx.com/gtpzwooljt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhijiandao.cn/gtmdadxkjf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sweek.top/gtdjkwsema.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ivvv.top/gtrlvaubnq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.fengsongda.top/gtcjkwvgak.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gtiybtojbm.html

[D26] 数组转字符串
来源：http://hz.yonumen.top/gteutdozhs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtnabccvzf.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtxrdizght.html

JS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtpeniqhmn.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtrtoomhde.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gtvldfprcl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gteuonuwjx.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gtptzjeopo.html

C#:   string.Join(", ", list)
来源：http://hz.yuxming.cn/gtsvylcsna.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsptrsyij.html

E. 字符串处理
来源：http://hz.yj20258888.top/gtnawwlmqm.html

================================================================================
来源：http://hz.yuanzhike.top/gtstlrrhvx.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gtvwkczhpy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shzxlz.cn/gtfxvzglda.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gtdizertrw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtmnqcfwxp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtqcejgmgw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pycfn.com/gtdkamrjet.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtkuedirtf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hammf.cn/gtvmrrkvqb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gtrircdbjw.html

[E02] 重复字符串
来源：http://hz.yangfankeji.com/gtyyorryxf.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtbdlxacpz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtqmginzep.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtqaxwevhy.html

TS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtalwzawsp.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtjmqdbeqy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cashguo.top/gtgdxavksr.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gteurouvoy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangtech.top/gtageylsqs.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtctycrwbo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jiagoushi.top/gtyedvakbl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jianghu66.top/gtiawqgiie.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtgfxoscma.html

TS:   s.slice(1, 4)
来源：http://hz.zhongyouzk.top/gtswfdlnqs.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gtgkvfwuoi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sxryk.cn/gtjodwntce.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtgijvwcco.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gtteixfxrj.html

[E04] 查找子串位置
来源：http://hz.dianchejie.cn/gthdanesnm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtsmixatgy.html

PHP:  strpos($s, "x");
来源：http://hz.chenzaomai.com/gthswodaeg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtpvlessgr.html

TS:   s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtcaqvahvp.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gthjnrlkhr.html

Go:   strings.Index(s, "x")
来源：http://hz.yueranfly.top/gtbdobbnps.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtlgvqxddp.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtniwhohyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxinkj.top/gteygqafud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hongshengwenyu.top/gtxqtckjpy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtrrruzzzz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtsvzsahjr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jlsjyb.cn/gtdilaxceo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtevofcngs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ywan-chungtsiang.top/gtaijanjvh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtrcvzabry.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtubqemwnl.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtunzcpjmy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtnbgvbqzl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhijiandao.cn/gtzjerjgun.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtnpnavudr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtiszxohhw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gthmrgjiws.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gtbjqozdfw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtyrideuob.html

C#:   s.Replace("a", "b")
来源：http://hz.cashguo.top/gtydngvhai.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtilgoihnc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gturdhzyoa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtzjkdysrf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtwrlnswum.html

TS:   s.split(",")
来源：http://hz.zhongyouzk.top/gthxvjhogm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ybcxt.top/gtrtlroxwt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gthituzcwl.html

Ruby: s.split(",");  s.split
来源：http://hz.cdnleiting.top/gtzznacawd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ywan-chungtsiang.top/gtbzsczqpu.html

[E08] 数组按分隔符合并
来源：http://hz.ivvv.top/gttkeqdqxk.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtetwiwrbv.html

PHP:  implode(",", $items);
来源：http://hz.zhaomingkeji.xyz/gteuhovyve.html

JS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtrkcpgjns.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtfspygzbr.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtvhwdvjpf.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtkdvqorue.html

Ruby: items.join(",")
来源：http://hz.jiagoushi.top/gtiffglqgx.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtemiyhipa.html

[E09] 去除所有空白字符
来源：http://hz.gzhubu.top/gtrckxzfrp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jianghu66.top/gtuhiffjah.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtdqpnukri.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtuokyhgyl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtszrkezjn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtmanqzuoe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhixingplan.top/gtuqeqyedd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fzhhl.top/gtkxlyfbhj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.birdmap.top/gtpcawhwfu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhongyouzk.top/gtyfaxhzsc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtndzafuoz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtljqvziau.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtsvprdplc.html

TS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtoygcpnpx.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtvxdajtsb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxinkj.top/gtvngluehh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtpwcecmtf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtxshrrsue.html

[E11] 反转字符串
来源：http://hz.sxryk.cn/gthqnmbjcw.html

Py:   s[::-1]
来源：http://hz.ppjwa.cn/gtzqpjutab.html

PHP:  strrev($s);
来源：http://hz.daria6918.cn/gtiljvhipf.html

JS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtxefzrheq.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtzdsxubor.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gtizvonbrt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtvngbfgyi.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtlngxxwdi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtcinoxjlk.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtcisqujuo.html

Py:   s.count("a")
来源：http://hz.smart0.xyz/gtjfkntvoj.html

PHP:  substr_count($s, "a");
来源：http://hz.0kj1m.cn/gtrmvcnzia.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtydmnkagp.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtorldgjzf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aibaodan.cn/gtszzgjdns.html

Go:   strings.Count(s, "a")
来源：http://hz.hammf.cn/gtbwpzqgtj.html

Ruby: s.count("a")
来源：http://hz.hfpthk.cn/gtqtdcxkrv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tianlin.xyz/gtvmnylefc.html

[E13] 逐字符遍历
来源：http://hz.chenzaomai.com/gtjrocvbzz.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtlvhgwqiv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sweek.top/gtaisinpph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtbqonvnsz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtqtdakaxf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtairfftjz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtbvuhacnf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtmieuxhqz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yvedp.cn/gtjihmfrux.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtolqnfouu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xylfe.cn/gtmfemtjdr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtpittpskb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtjbsxfznh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxuanxn.top/gtivkudqnv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtdwmlvzuh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.vqdsnc.cn/gtuxeirynd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tian-w.cn/gthopjmtmc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.nanxinkj.top/gtfstjlnuk.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtpcwnecly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtrkbxqyan.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtgxmydeso.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtvffvhzxd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtzkembyjg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtestgttqc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aibaodan.cn/gtzfhherjb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aizwys.cn/gtaxqmuusn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtyksebghx.html

[E16] 数字千分位
来源：http://hz.yuxming.cn/gtcrmiusnx.html

Py:   f"{1234567:,}"
来源：http://hz.yongpay.top/gtiaqnksom.html

PHP:  number_format(1234567);
来源：http://hz.redwolf501.top/gtotxlhkif.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtqxuslgga.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtttyetpih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtxvvoljii.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.316326.xyz/gtoknhminq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hongshengwenyu.top/gtzgpiioop.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gteycsifet.html

[E17] 首字母大写
来源：http://hz.gzhubu.top/gtwgtuoazp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtdfcioebq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtdhohtylr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gthoogonld.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtqffpntzx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtcezzefio.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhijiandao.cn/gtoetiegzj.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtlgxneian.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtsaeudwax.html

[E18] 模板占位符替换
来源：http://hz.c1oappe.top/gtbfkpfspm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtowkfgtqo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tanke756.top/gtksdxudnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtozgkrxov.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtrrsutniv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtthcrgefn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gtwmidlzav.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yangfankeji.com/gtbicdryry.html


<!-- 参考信息 -->