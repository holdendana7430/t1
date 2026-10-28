代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtmkgxejvz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuetiantiany.cn/gtgjagtawd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gtrpxfwzam.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxuanxn.top/gtvyvkvfhy.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtuakrwwig.html

C#:   list.IndexOf(x);
来源：http://hz.hywenlv.cn/gthzaztvzb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gtwxwsobxz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtevgxryun.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtwrwttckm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtmsuxurvd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtmzbazolh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtdqggjyrp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.svipenyu.cn/gtgwhnxupm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtbcxtembz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.316326.xyz/gtaqwihiac.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gtdnceyubb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cheryme.top/gtbxmmxvcm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dashuyun.cn/gtwrpkqdmb.html

JS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtvsmxudtx.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtaquwesrf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dashuyun.cn/gtcmmrgluz.html

Go:   // 手写循环
来源：http://hz.shuidangran.top/gtnvtwmtej.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gtzjueonhz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinghuilouyu.cn/gtmpqzsmbv.html

[D15] 去重
来源：http://hz.yj20258888.top/gtovepzomt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtaqezhgoq.html

PHP:  array_unique($arr);
来源：http://hz.mhx1999.top/gtshqooewc.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtyeglgavf.html

TS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtbvgpwebo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtavcpfqox.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtufkdunmy.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtcwjflsyn.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtvksguheb.html

[D16] 求和与平均值
来源：http://hz.yuxming.cn/gtpheewvvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fzhhl.top/gtqayqbmla.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtfasiohir.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtaivzpvbz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtwmlthhxl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gticpttcji.html

Go:   // 手写循环累加
来源：http://hz.vqdsnc.cn/gtmztiozdb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tianlin.xyz/gtjccghnsr.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gteewhsicc.html

[D17] 最大值与最小值
来源：http://hz.jinqigufen.top/gtnpntxfqe.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtlrtyhmpd.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtfbkaenxq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sxryk.cn/gtezdxbskq.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gtwiqdjuah.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gthspcicog.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtzzghnxiu.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gthiljvrat.html

C#:   list.Max();  list.Min()
来源：http://hz.ydzc1.top/gtfivwnjpj.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtylqlqdla.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jlsjyb.cn/gtaejxrlzg.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtozdlhgcb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gtofpjuqxs.html

TS:   nested.flat();
来源：http://hz.yuanzhike.top/gtrdbkckbu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gogol.net.cn/gtiyqoloir.html

Go:   // 手写双层循环
来源：http://hz.jinqigfzy.top/gtpfcrzasz.html

Ruby: nested.flatten
来源：http://hz.tanke756.top/gtqojgmloh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xylfe.cn/gtdgkpaeoy.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtozptyloa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yueranfly.top/gtcsgzdazj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258888.top/gtttctwvrd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yongpay.top/gtbnpisfud.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gttdxabeog.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtvfqnqvkv.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gttfycjkip.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.birdmap.top/gtsqggdiqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guowangkeji.top/gtddppmaxi.html

[D20] 统计每个元素出现次数
来源：http://hz.shzxlz.cn/gtwcqiqqpz.html

Py:   Counter(arr)
来源：http://hz.gaohongyu789.top/gtwcwsvtal.html

PHP:  array_count_values($arr);
来源：http://hz.yuxming.cn/gtljluefgy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtxbuslpwb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtcnkbamgx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtflpxfxco.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gteiyylkru.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtzjnowvvn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gthxjrqeyj.html

[D21] 判断是否包含某元素
来源：http://hz.guannengcc.top/gtdcdowexf.html

Py:   x in arr
来源：http://hz.0kj1m.cn/gtrbobnjjn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shuidangran.top/gtsziqrwtm.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtufsdembq.html

TS:   arr.includes(x)
来源：http://hz.yj202588.top/gtbyqttpzv.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtrkptjcpc.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtmmjyhvlc.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtyvlndqwn.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gticxlalsf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nwbrower.top/gttqurnavk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtgypvsete.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gtqipcqlba.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtilqkdvzo.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtestsjiyr.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gthhsnqjgf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shzxlz.cn/gtabyzpmwl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtxptinzlp.html

C#:   new List<int>(list);
来源：http://hz.iojbl.cn/gtrswpgpnr.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtelcausmv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.haohaochexian.top/gtitldnxru.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hammf.cn/gtnblpzxux.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtzkbfrtnx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtyornrdrh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sxryk.cn/gtzyljhayc.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtaqzcbvsb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gthlmzogke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guannengcc.top/gtpaicqqhh.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtpjszqdnr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtvtavlmhm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sysykeji.top/gtvcdjpomr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtbwkycyuj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daria6918.cn/gtyfzitnrf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtpaihnpuu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cucudq.cn/gthhwuroet.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtnisowjyv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hywenlv.cn/gtmkzsowck.html

[D25] Set 集合去重与交并差
来源：http://hz.redwolf501.top/gtsjdzdkiv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sysykeji.top/gtrllybcne.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.9152youxi.cn/gthfgkrypg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtbzurdvou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ybcxt.top/gtihnvxcky.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cqqwz.cn/gtxsgslqbm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shangyingyoupin.top/gtdqfcnnnm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gtizkcvajm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hammf.cn/gtbgtyopmz.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtxcqpkudw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gthbogevox.html

PHP:  implode(", ", $arr);
来源：http://hz.0kj1m.cn/gtvjmjfrhy.html

JS:   arr.join(", ")
来源：http://hz.aizwys.cn/gthqxtmleu.html

TS:   arr.join(", ")
来源：http://hz.tanke756.top/gthycjesca.html

Java: String.join(", ", list)
来源：http://hz.wangshuangyany.cn/gtzamgrsdf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangkeji.top/gtpqmhcqvw.html

Ruby: arr.join(", ")
来源：http://hz.chenzaomai.com/gtkeuticua.html

C#:   string.Join(", ", list)
来源：http://hz.cdnleiting.top/gtsccxsckq.html

================================================================================
来源：http://hz.dashuyun.cn/gtjlzagrvx.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtzwgalkwd.html

================================================================================
来源：http://hz.hnqzz.top/gteewbaoha.html

[E01] 拼接字符串
来源：http://hz.ybcxt.top/gtebkhpqbh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhongyouzk.top/gtqldwjwni.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtsvickpyv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtetlgfirw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtnojdxvsy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuanzhike.top/gtwnfvccez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gtrnqlzluc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtsqnazqff.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtrywgorgg.html

[E02] 重复字符串
来源：http://hz.daria6918.cn/gtbdivwkla.html

Py:   "ab" * 3
来源：http://hz.ydjk.org.cn/gtrxyolggh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtdgbfchjw.html

JS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtoubdtusc.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtnmxpfnmv.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtgwwqbuip.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gthfvckeqs.html

Ruby: "ab" * 3
来源：http://hz.wangshuangyany.cn/gtukhebcul.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtfsufqdlq.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtdgnxlaqy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtiyldrdzi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigfzy.top/gtmlxbrsin.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtihvivsba.html

TS:   s.slice(1, 4)
来源：http://hz.daxiang520.top/gteqqwmkcf.html

Java: s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtkytdklip.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhixingplan.top/gtkluapdje.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtnkoitljo.html

C#:   s.Substring(1, 3)
来源：http://hz.hongshengwenyu.top/gtbfbsrkre.html

[E04] 查找子串位置
来源：http://hz.xingfuxueyuan.xyz/gtjgwmlizx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtwmnnxuvi.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtnjfyruhl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtpgqkaqse.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtsgaciipk.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtwthyycsn.html

Go:   strings.Index(s, "x")
来源：http://hz.wangshuangyany.cn/gtpgfpohyg.html

Ruby: s.index("x")
来源：http://hz.xylfe.cn/gtvygshnhk.html

C#:   s.IndexOf("x")
来源：http://hz.hnqzz.top/gthkgeinsa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jyoumei.cn/gtdmzhfaoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.0kj1m.cn/gtgiaiysdi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ivvv.top/gtgoyesdnm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtyfaepkwg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtuucagqfz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtiemtrost.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtlolwwuie.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sysykeji.top/gtzxbsqkim.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ybcxt.top/gtmvkzgvkq.html

[E06] 替换子串
来源：http://hz.smart0.xyz/gthkmqnpjk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtfsunqpjd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtjjwsjopy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtgiuqzcsq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtwarbbdvn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtkvwpuenc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tianlin.xyz/gtacxtoxmz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sufxvd.cn/gtywppwlrb.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtbskbpyyo.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtopkgwvzm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.vqdsnc.cn/gtyogvwkwm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xylfe.cn/gtznrxrtqd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gttvuffkwh.html

TS:   s.split(",")
来源：http://hz.kuanghao11.cn/gtiaxlzwxy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtovmnfyze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.redwolf501.top/gtuulxhjwf.html

Ruby: s.split(",");  s.split
来源：http://hz.chenjidiqi.icu/gtsxgqxuiv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fengsongda.top/gtubzqqbpb.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtdbuuriqn.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtmpgnmdsh.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gtcsjuabjs.html

JS:   items.join(",")
来源：http://hz.andypj.xyz/gttjxxjsiy.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtjcbemrev.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gteohtkjtb.html

Go:   strings.Join(items, ",")
来源：http://hz.hnqzz.top/gtchdghhod.html

Ruby: items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtuclyvyur.html

C#:   string.Join(",", items)
来源：http://hz.jinqigfzy.top/gtwxsusuje.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtyxvudjlh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yongpay.top/gtgxlgjmnp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tian-w.cn/gtzszlyqed.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtjfcdkueh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtinmilpxa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtzdtrvpti.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtlzxrwpzh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gogol.net.cn/gtymejybgb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangshuangyany.cn/gtxzzvsmem.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gtvwfrexej.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtbgfynukm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtlxfrsefe.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtnrerzevc.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtopkuysso.html

Java: String.format("%03d", 7)
来源：http://hz.svipenyu.cn/gtikqmybln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtuuhsogxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258888.top/gtcdlzdino.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtttkwivnj.html

[E11] 反转字符串
来源：http://hz.shuidangran.top/gtldkjcoic.html

Py:   s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtwdgsoqgs.html

PHP:  strrev($s);
来源：http://hz.ybcxt.top/gtekxfraeq.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtwkiefpyr.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtnehiqjzy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtenjhucqu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gturzyuren.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtjlvlknkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtitqwlldo.html

[E12] 统计某字符出现次数
来源：http://hz.ivvv.top/gtfunutgfc.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtkqwlalsq.html

PHP:  substr_count($s, "a");
来源：http://hz.hnxiangtu.top/gtmkokueoa.html

JS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtqmgtsuip.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtofkohsvp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtqanjqwlm.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtjltyfgro.html

Ruby: s.count("a")
来源：http://hz.sysykeji.top/gtzckpsywk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xziqi.cn/gtpnklkcdt.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtulowsqyg.html

Py:   for ch in s: print(ch)
来源：http://hz.gotoacloud.top/gtmvqqsmnl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangtech.top/gtajwzfkou.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gthzprfkud.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtcwctccvf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtqdxbbqlz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtzeuzhhtb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ivvv.top/gtplgatvtp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guowangkeji.top/gteayzdaiw.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtiexxbydy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtqwnvgind.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aizwys.cn/gtguvuwahs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtxtofxyvu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gtymdxnpyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hammf.cn/gttplyjmiy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtyeqlwiki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhengqikj.top/gtwpnghkot.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtofmphxjf.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuetiantiany.cn/gtlvhzgcto.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtehzxpfep.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhixingplan.top/gtiacwozfi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtrgwdgooc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtutizdume.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xingfuxueyuan.xyz/gtxtljudes.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnxiangtu.top/gtgsqhjwbq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenjidiqi.icu/gtvglkydmq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yvedp.cn/gtucbxzndd.html

[E16] 数字千分位
来源：http://hz.xziqi.cn/gtmflmnpys.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gtobdhwjbc.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtyetrervu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gthfwezmyq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtpgbwsqqd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shangyingyoupin.top/gtnwaqilgw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shuidangran.top/gtjrvaaocj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258888.top/gtyeqycozd.html

C#:   1234567.ToString("N0")
来源：http://hz.smart0.xyz/gteoqdmenm.html

[E17] 首字母大写
来源：http://hz.cucudq.cn/gtwvkjbxym.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.0kj1m.cn/gttkggeqzu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtpyizjqtt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtummunvhd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gtgfxegttb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxinkj.top/gtkyirkimn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aizwys.cn/gtapaaksiy.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtyshpnbds.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtduyawdcy.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtvexynnzd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.svipenyu.cn/gtrbqzcysb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtkvtezzir.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtvokrqtrc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtwbkooihl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jlsjyb.cn/gtjtkmldyk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gteusihbqv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtgomikuip.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtrpytdplg.html

[E19] 多行文本按行拆分
来源：http://hz.ydjk.org.cn/gtcalostad.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtqkfazhqk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtnenzrkas.html


<!-- 参考信息 -->