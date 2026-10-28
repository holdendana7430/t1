代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtnwizkgbi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtsiocgzfb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gthwrzcpzy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtcrkjuakj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtpykdzlvv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zdqjudy.top/gtwiewngbw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yongpay.top/gtjvlmkbwp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenlongwang.top/gtqbnmtbxk.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gtzbubtwtx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtmjmhlzrj.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtttjlgcyk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuanzhike.top/gtommlcovn.html

TS:   [...arr].reverse();
来源：http://hz.sufxvd.cn/gtldcxrsoi.html

Java: Collections.reverse(list);
来源：http://hz.zhengqikj.top/gttpsuyxhp.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigufen.top/gthrgdende.html

Ruby: arr.reverse
来源：http://hz.yvedp.cn/gtzjiprrya.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtdhwnkdty.html

[D12] 查找元素下标
来源：http://hz.ehwqpu.com/gtovycnzss.html

Py:   arr.index(x);  x in arr
来源：http://hz.dianchejie.cn/gtdnuaxcfp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtgfxjhmno.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gthtgrvpme.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtwewgiqgt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jqgfzy.top/gtcjoqgrfz.html

Go:   slices.Index(arr, x)
来源：http://hz.zhoulong.xyz/gtfbakngef.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtejishzzs.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtjvqhvbmn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxinkj.top/gtydnxogqs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.birdmap.top/gttalmirgs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xziqi.cn/gtbiffsups.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtqqwkbbse.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtgagpuhfj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yongpay.top/gtrutgrxbs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gthfrxsyuh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtneiengrl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydzc1.top/gtdeccjfsi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xinyue.icu/gtzirbbjbg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jianghu66.top/gtjpppyacd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtmmuevmsl.html

JS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtogdyxhti.html

TS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtdeguvbvv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yvedp.cn/gtljtcerug.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtwzxtgolq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yanxiufei.cn/gtzceotwdb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hammf.cn/gtqzmpotfp.html

[D15] 去重
来源：http://hz.zdqjudy.top/gthkrawffa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.redwolf501.top/gtxhmosbst.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gthtkdzxda.html

JS:   [...new Set(arr)]
来源：http://hz.tian-w.cn/gtfbbfydfj.html

TS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtunmnsrrc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtdijdcouc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.9152youxi.cn/gtomioiedy.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtfqeduugf.html

C#:   list.Distinct().ToList()
来源：http://hz.daria6918.cn/gtwkxmkbhd.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtusrnmdic.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtghuirtha.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtglpdvtpi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtcsgkmuku.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtmhrxpabs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ivvv.top/gtcgtwgpel.html

Go:   // 手写循环累加
来源：http://hz.ehwqpu.com/gtdusxrxzr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hywenlv.cn/gtfujcdacr.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtkjkzuhjm.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtpcdnxiel.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtjdvcsvxg.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtdlhaekcb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenlongwang.top/gthitmmbru.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtyfxtxozi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cashguo.top/gtcjofvwjf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gtbyftuyqz.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtnlzvxbvr.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtouqwkxye.html

[D18] 扁平化嵌套数组
来源：http://hz.chenjidiqi.icu/gtcglsnwdm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinghuilouyu.cn/gtugbybkwk.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gteyqzcpqf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtallxiiur.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtnxhcaxuw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gtflycnbgm.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtanrrewbe.html

Ruby: nested.flatten
来源：http://hz.ydjk.org.cn/gtacdlruta.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ppjwa.cn/gtlhiyersu.html

[D19] 按字段分组
来源：http://hz.wangdashe.top/gtdzznvymy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtnrjnuzly.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtunoncvon.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtiuifnmdd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtdoxyxynj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtnvfsithj.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtdntxvcgq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.meibo888.top/gtkebskytz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ybcxt.top/gtxjrlxjdg.html

[D20] 统计每个元素出现次数
来源：http://hz.cheryme.top/gtkhenkllm.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtsiyafhru.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258888.top/gtmokfsnsb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtixpwzpxo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtbwnqmvah.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jianghu66.top/gteitdtraz.html

Go:   // 手写 map[T]int
来源：http://hz.guannengcc.top/gtghjrqoha.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtmeoyewox.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtomcympzl.html

[D21] 判断是否包含某元素
来源：http://hz.guannengcc.top/gtroiwqyyx.html

Py:   x in arr
来源：http://hz.sweek.top/gthuvtivgg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigfzy.top/gtsfjiyfjz.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtwzazljyd.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtzwoqgfwt.html

Java: list.contains(x)
来源：http://hz.meibo888.top/gtpkszdisj.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtsiamkpfa.html

Ruby: arr.include?(x)
来源：http://hz.fengsongda.top/gtywifdyxo.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtmvjucvnu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtdzivargb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgfzy.top/gtqnpzyweo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gaohongyu789.top/gtaxndymac.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtcbctmarq.html

TS:   [...arr];
来源：http://hz.hongshengwenyu.top/gtdlwweute.html

Java: new ArrayList<>(list);
来源：http://hz.shzxlz.cn/gtxhhhktng.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ivvv.top/gtoxogljad.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yueranfly.top/gtvirrbhuh.html

C#:   new List<int>(list);
来源：http://hz.haohaochexian.top/gtdttodyba.html

[D23] reduce 累积计算
来源：http://hz.pycfn.com/gtliqcgkks.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gturibrepb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtvbvribhe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtugplwabo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtzmhdbrcf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtflglnanm.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtspfnuhqa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnqzz.top/gtsehjximq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gtrsambqru.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangdashe.top/gtcffpeotm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtzzqbsnnb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtavozlaba.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zdqjudy.top/gtrqykdeop.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtutnietwu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cucudq.cn/gthiqdfuuz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tian-w.cn/gtsyppkyfu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yongpay.top/gtobxkvuvx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhiwuduotai.top/gtptzmspgo.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtslbzsvbt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ybcxt.top/gtqugofnjw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guannengcc.top/gtevmnclnw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtshakiogf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtzvwzxgww.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xziqi.cn/gtgqvhamst.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtneiwlbfb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yonumen.top/gtfxrdpipy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangshuangyany.cn/gtcpnuzdve.html

[D26] 数组转字符串
来源：http://hz.yuanzhike.top/gtwdiistid.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtoneeyprb.html

PHP:  implode(", ", $arr);
来源：http://hz.ybcxt.top/gtsmrxmlmy.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gtvmzdnctj.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gtgdhfxtxa.html

Java: String.join(", ", list)
来源：http://hz.yonumen.top/gtspfvgvzx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydjk.org.cn/gtbonlgize.html

Ruby: arr.join(", ")
来源：http://hz.mhx1999.top/gtbinxbcdc.html

C#:   string.Join(", ", list)
来源：http://hz.yanxiufei.cn/gtvmatlmus.html

================================================================================
来源：http://hz.cqqwz.cn/gtiuvzjxyh.html

E. 字符串处理
来源：http://hz.zhiwuduotai.top/gtuvstgulh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjcgojpsc.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gtzytpkcfz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yueranfly.top/gthcxgedtn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.birdmap.top/gtshlrfjfj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtmtclfcyv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtemezhrgr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yangfankeji.com/gtjmodzvzc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cheryme.top/gttwltdyyp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtkwnriwwb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtvbxusmwx.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtyslyvxwu.html

Py:   "ab" * 3
来源：http://hz.gzhubu.top/gtzfauuihp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sxryk.cn/gtmpkeojrw.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtwfjicbad.html

TS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtejsteduh.html

Java: "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtfxxrmcsk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtxiqevwua.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gtxmebyber.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258888.top/gtpqhzosyx.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gtsqhoioyu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yueranfly.top/gtdvysmfil.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnqzz.top/gtlcelofun.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuanzx.com/gtfzrmbarw.html

TS:   s.slice(1, 4)
来源：http://hz.quarkkingdee.top/gtppuygzxe.html

Java: s.substring(1, 4)
来源：http://hz.yongpay.top/gtffoeulkr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yueranfly.top/gtmhoikbfw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxinkj.top/gtrpyjnllh.html

C#:   s.Substring(1, 3)
来源：http://hz.hnxiangtu.top/gtkuhsnvzh.html

[E04] 查找子串位置
来源：http://hz.tian-w.cn/gtklrqgpgz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhiwuduotai.top/gtfdysypzl.html

PHP:  strpos($s, "x");
来源：http://hz.sufxvd.cn/gtvstilzwo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtoswhrepg.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gteawwscyr.html

Java: s.indexOf("x")
来源：http://hz.cucudq.cn/gtrnslmjuq.html

Go:   strings.Index(s, "x")
来源：http://hz.cdnleiting.top/gticyarlzq.html

Ruby: s.index("x")
来源：http://hz.ydjk.org.cn/gtuazvjjpx.html

C#:   s.IndexOf("x")
来源：http://hz.tanke756.top/gtqhpztvds.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nwbrower.top/gtgeusukkv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.andypj.xyz/gtwfdayqlk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gogol.net.cn/gttuwcbnsm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtzotiwlbr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtznwgyibe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ehwqpu.com/gtetbcmotl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hammf.cn/gtyrunfidj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yanxiufei.cn/gtzkpumohn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhixingplan.top/gterrsmdan.html

[E06] 替换子串
来源：http://hz.pengpengdd.cyou/gtnmehlexo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gttswppovk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinghuilouyu.cn/gtdsdlqwgk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtfhnebkma.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtcnmkfmlh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtfkjnsrxu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.birdmap.top/gtkytdypxj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtaexmnomp.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtevmlgvhh.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangkeji.top/gtzhfprhle.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtdseaotjc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gzhubu.top/gtwjyfnfdu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtbkmjpzln.html

TS:   s.split(",")
来源：http://hz.jyoumei.cn/gtjoypgukv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.9152youxi.cn/gtnklcyorh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.9152youxi.cn/gtfpljohxi.html

Ruby: s.split(",");  s.split
来源：http://hz.chenzaomai.com/gtpedkbllk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gotoacloud.top/gtcvncuwmm.html

[E08] 数组按分隔符合并
来源：http://hz.ivvv.top/gtsstbymqn.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gttkzvynas.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtqalxndaj.html

JS:   items.join(",")
来源：http://hz.gzhubu.top/gtywevrtkn.html

TS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtwwxovwlq.html

Java: String.join(",", items)
来源：http://hz.yj20258888.top/gttmzkzuaj.html

Go:   strings.Join(items, ",")
来源：http://hz.yvedp.cn/gtzacfqfzw.html

Ruby: items.join(",")
来源：http://hz.nanxuanxn.top/gthssaceyh.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gtdfzpqknc.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtyttguivo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gthbxcjmsj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtrmxyxavk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtwosvwxes.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtceqwjsnm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.haohaochexian.top/gtovqqdqtj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ivvv.top/gtvwcqymkr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258888.top/gtwwyulhan.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yonumen.top/gtjmhfgcrt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jianghu66.top/gtbezabipa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ppjwa.cn/gtyjvxsyev.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.c1oappe.top/gtjmaaeaoe.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtsdpnpulf.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtmwoidlcd.html

Java: String.format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtxzjsycxz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxinkj.top/gtmamfbdbi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtobywownt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtfgjsgbck.html

[E11] 反转字符串
来源：http://hz.pycfn.com/gtdbsjdpmi.html

Py:   s[::-1]
来源：http://hz.havefunace.top/gtgsjlvuuf.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtpgicgtys.html

JS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtkqpcqiqb.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtnmxdoduv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtldzxxjen.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aizwys.cn/gtdhubygth.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtwjwfbdps.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtzgczfznq.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtdrjglmqx.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtujeopnno.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtxheszazl.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtueychusx.html

TS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtxoomdvrx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtceliufem.html

Go:   strings.Count(s, "a")
来源：http://hz.chenzaomai.com/gtyseozjsa.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gttfsnrykf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtwipoxusg.html

[E13] 逐字符遍历
来源：http://hz.sysykeji.top/gthyrjdbmq.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigufen.top/gtfapeqxsw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yonumen.top/gtfjlfvmyc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtpwuqekpb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtgxayocxo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ppjwa.cn/gtysemajhl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtpifweuap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ivvv.top/gtowokgtfo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gtsfifghdi.html

[E14] URL 编码与 Base64
来源：http://hz.xuetiantiany.cn/gtklvmbktb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shangyingyoupin.top/gtskoebbdp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.vqdsnc.cn/gtqzrpjsbj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtjthqjnkw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtawvteklr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hammf.cn/gtapjhvjfy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtvcmrrmvd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtuaxqpadd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.feifeiyinyue.top/gtsvwqsvdn.html

[E15] HTML 转义 / 反转义
来源：http://hz.quarkkingdee.top/gtopaedtji.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fengsongda.top/gtjkfpjlqf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gtycqvzmtl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtlwlvdfvh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.feifeiyinyue.top/gtddxqisqy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cheryme.top/gtasjehbyf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shuidangran.top/gtdnqgdtka.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.kuanghao11.cn/gtctorhath.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gtzagkncxn.html

[E16] 数字千分位
来源：http://hz.zhaomingkeji.xyz/gtvkfabiys.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gtabymaedq.html

PHP:  number_format(1234567);
来源：http://hz.svipenyu.cn/gtdigrmawr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtrklyavcv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtdkpynsse.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gtzdyylbyu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtvbouyeuw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jlsjyb.cn/gtezcznufo.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtzhencdbw.html

[E17] 首字母大写
来源：http://hz.yj202588.top/gtxhfxzhrf.html


<!-- 参考信息 -->