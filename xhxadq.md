代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gtocioetyw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtvnlsilma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aizwys.cn/gtvcyuhqbb.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtpmlaexoe.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtqkopcvlg.html

C#:   list.IndexOf(x);
来源：http://hz.xinyue.icu/gtdnqowkyt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtwsswjccg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pycfn.com/gtikfnztku.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jyoumei.cn/gtdcrselsq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtmjomfaqt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtwjwxyvnv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gtsmutvbnt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xziqi.cn/gtwdslhlgp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.birdmap.top/gtyehpnhdc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnqzz.top/gtnacfrgbe.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hywenlv.cn/gtqghnwyqr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtrpqmvjyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xinyue.icu/gtfsfpkmuz.html

JS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtybdzibst.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtvhuhwjyn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yueranfly.top/gtoyjtfbjn.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gthliverzb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtmscgwnqs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shzxlz.cn/gtiioulfns.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtbbnctjif.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtweglyaap.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gtzztghcyp.html

JS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtmeblahnh.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtivtiidsj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ppjwa.cn/gtcwrlvadd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtxzvarzvs.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangtech.top/gtrlkwismi.html

C#:   list.Distinct().ToList()
来源：http://hz.ydjk.org.cn/gtildkiubp.html

[D16] 求和与平均值
来源：http://hz.hysaishi.cn/gtdefyqecq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yanxiufei.cn/gtrksdayff.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhijiandao.cn/gtdmispovt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtjjnuekxl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtvcpxyivu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hammf.cn/gtfehnezii.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gtijbietzi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xylfe.cn/gtgctrcfmd.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtcwmglxxh.html

[D17] 最大值与最小值
来源：http://hz.hnxiangtu.top/gtgvidawxi.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigfzy.top/gtvxxqonij.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtcupjuwyc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shuidangran.top/gtzmxkddsv.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtdwikxhxd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cqqwz.cn/gtskvwdfcb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtimkzmsfy.html

Ruby: arr.max;  arr.min
来源：http://hz.shuidangran.top/gtkdbbfsyr.html

C#:   list.Max();  list.Min()
来源：http://hz.xuetiantiany.cn/gtlzppgoml.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtoilxqnsw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daxiang520.top/gtrpuboxvq.html

PHP:  array_merge(...$nested);
来源：http://hz.yanxiufei.cn/gtwyybutiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtixyzpnsu.html

TS:   nested.flat();
来源：http://hz.redwolf501.top/gtwzlznqlb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtbsvlotoe.html

Go:   // 手写双层循环
来源：http://hz.zhaomingkeji.xyz/gtyeggjniz.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtwsmqxlfb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtsdauembu.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtueuquxya.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtlnkzgbsd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinqigfzy.top/gthnmitope.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gtkhrpubrq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtubfhpsyq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangdashe.top/gtsoyyoaxb.html

Go:   // 手写 map[string][]T
来源：http://hz.ydjk.org.cn/gtdghtnjpw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtgncqmkzk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtqebckyfn.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangkeji.top/gttodamsgu.html

Py:   Counter(arr)
来源：http://hz.guowangkeji.top/gtfebftnab.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtbfkmokgz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtfqqzwkfi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtpaanxxws.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtcwbrilhf.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gtzgkfkllu.html

Ruby: arr.tally
来源：http://hz.tanke756.top/gtfnnqotuu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigfzy.top/gtinwhnsyd.html

[D21] 判断是否包含某元素
来源：http://hz.ydjk.org.cn/gtyhtlggbc.html

Py:   x in arr
来源：http://hz.daria6918.cn/gtkxflzadi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinghuilouyu.cn/gtmbjmommm.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtgmqomsxu.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gtboibtapg.html

Java: list.contains(x)
来源：http://hz.xziqi.cn/gtyjshknma.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtxqzgfhhv.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtcncyzrjo.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtulkubuvv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nwbrower.top/gtuvilwlwb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ivvv.top/gtfhrrdgke.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtizgbukat.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.kuanghao11.cn/gtnnoanjky.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtzdpnpifb.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtdazhrmyq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhiwuduotai.top/gtdmnepzib.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtzubodnsq.html

C#:   new List<int>(list);
来源：http://hz.smart0.xyz/gtuctjlmkt.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtrirprxag.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hfpthk.cn/gtbugnbqlg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtkvtkffhl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtyiertbvo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtikcbrzzv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gtjdliahvh.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtsexpydpl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtcjshlpgt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gaohongyu789.top/gtxtrljufo.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtlmkhphow.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtepwbxlgu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtblsmdnfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgfzy.top/gtlfwhwrrp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ivvv.top/gtvhsbllep.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtiphyazye.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtunotgejj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shzxlz.cn/gtxghowpfo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shzxlz.cn/gtwqjtmdmt.html

[D25] Set 集合去重与交并差
来源：http://hz.vqdsnc.cn/gthkywnmnt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtetdhdlqi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yvedp.cn/gtqbgxwlih.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangtech.top/gtwkwkjzjn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gtjgduyihd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtcllsuwcm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtyhxuicck.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aibaodan.cn/gtgcjzbvyw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gtjrworqsa.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtwhqcackq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtloufrvfs.html

PHP:  implode(", ", $arr);
来源：http://hz.fzhhl.top/gtkvngricn.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtbaofexcz.html

TS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtscsoaxvz.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtpicisufb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.9152youxi.cn/gtsjhmjjsw.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtaihaheof.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtawfxirpc.html

================================================================================
来源：http://hz.jqgfzy.top/gtomvlcjid.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtrsokjdgi.html

================================================================================
来源：http://hz.yvedp.cn/gtktzrtlhm.html

[E01] 拼接字符串
来源：http://hz.9152youxi.cn/gthfbfnpur.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtkchbocot.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinyuanbaomall.cn/gtxorzjduz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtmhypblnp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gttgzuecea.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.birdmap.top/gthgjyohhi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gtlokxjghh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtrqzlynqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydzc1.top/gtrqkmptkh.html

[E02] 重复字符串
来源：http://hz.yangfankeji.com/gtwcfdhptn.html

Py:   "ab" * 3
来源：http://hz.zhijiandao.cn/gtxxhqfuhi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtrtxqmdcl.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtpleebnhp.html

TS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtdbezignu.html

Java: "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtetlxbhyo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtuafptanj.html

Ruby: "ab" * 3
来源：http://hz.mhx1999.top/gtrshxwcjx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtwgrgllsq.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtfkfuiuuw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtelqzfkcc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtcncbnkrw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtrhyxolgz.html

TS:   s.slice(1, 4)
来源：http://hz.cashguo.top/gtxdzozyqo.html

Java: s.substring(1, 4)
来源：http://hz.daria6918.cn/gtcmtvuygw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.feifeiyinyue.top/gtnkamytgn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jianghu66.top/gtiovbdfwn.html

C#:   s.Substring(1, 3)
来源：http://hz.sweek.top/gtmmzmmjfx.html

[E04] 查找子串位置
来源：http://hz.jqgfzy.top/gtxetptjva.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nwbrower.top/gtfhfrmyow.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtrtydaqxi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hongshengwenyu.top/gttymtsyci.html

TS:   s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtldqdtaig.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gtjjbrqkck.html

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gtfadaqeqn.html

Ruby: s.index("x")
来源：http://hz.hfpthk.cn/gtxrvpuxrw.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtuwsuwmrx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhongyouzk.top/gtckstdijo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shangyingyoupin.top/gtudiygjyd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtrratnwaw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtkkffgovq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtsxcltsoa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtedvqfckg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shangyingyoupin.top/gtuqmvpwsw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hfpthk.cn/gtdlqxlrvc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtjmbholmg.html

[E06] 替换子串
来源：http://hz.jinghuilouyu.cn/gtlzjihira.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtwzumsxfi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhoulong.xyz/gtahnsyukx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtbtalflbs.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtwqjqtmdb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtdxpgzowk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.bjfxy.top/gtfzwjccgh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.feifeiyinyue.top/gtsvqodsoj.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtkoprdhzj.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtolcdtejr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zdqjudy.top/gtzmniofdw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.svipenyu.cn/gtzrafopyr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jyoumei.cn/gttcvpexow.html

TS:   s.split(",")
来源：http://hz.xziqi.cn/gtmysbfrgf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gttucfhpfi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtkkyvwmin.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtugxirtct.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yanxiufei.cn/gtojfzxxav.html

[E08] 数组按分隔符合并
来源：http://hz.guowangkeji.top/gtdtdjsbzb.html

Py:   ",".join(items)
来源：http://hz.xziqi.cn/gtetevkgqn.html

PHP:  implode(",", $items);
来源：http://hz.yuanzhike.top/gteuoueopj.html

JS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtubjbfwaf.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtmfubhtnp.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtoofkcauy.html

Go:   strings.Join(items, ",")
来源：http://hz.kuanghao11.cn/gtvibcckcr.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtwvyrfpke.html

C#:   string.Join(",", items)
来源：http://hz.gotoacloud.top/gtcwfxkpzq.html

[E09] 去除所有空白字符
来源：http://hz.nanxuanxn.top/gtgvkvteeq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtmvntrudf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhaomingkeji.xyz/gtxqftbzfx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtnczgfasx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gthaezcebz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuanzhike.top/gtmxzjvhnu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gtuvzrplys.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258.top/gttjlcsoum.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258888.top/gtlzhgnkmt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtwilxqveg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtpkizlzjg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gtoachgjob.html

JS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtmvmgnjto.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtgtjkvoco.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtsrrifrbh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.52xcode.cn/gtotlxpcsa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.snrcjt.cn/gtobhduycf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtiwxboqjc.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtbqosoaxf.html

Py:   s[::-1]
来源：http://hz.quarkkingdee.top/gtoxsxdxhc.html

PHP:  strrev($s);
来源：http://hz.aibaodan.cn/gtkeifvbyo.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gttjrodblz.html

TS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtboxdncof.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangtech.top/gtqfiyikzh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gtwfwimanz.html

Ruby: s.reverse
来源：http://hz.hnxiangtu.top/gtiuxctfsb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gteeitlfta.html

[E12] 统计某字符出现次数
来源：http://hz.iojbl.cn/gtinehdryd.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtcrsxddnc.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtwaudehvp.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtamqqjjep.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtrtjczlee.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtxtodxcuk.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtjtuaimdl.html

Ruby: s.count("a")
来源：http://hz.meibo888.top/gtrjmpfclm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.52xcode.cn/gtghpqefra.html

[E13] 逐字符遍历
来源：http://hz.xuanzx.com/gtxnvsuery.html

Py:   for ch in s: print(ch)
来源：http://hz.gogol.net.cn/gtrskyvxjo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtlmdnwpsy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtszmiqryw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtalopmifh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtlmnjstnt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tanke756.top/gtxwnxhpro.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aibaodan.cn/gtzyyzvhbk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gtrvcbcail.html

[E14] URL 编码与 Base64
来源：http://hz.nanxinkj.top/gtbwteumnr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtutbepupf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.redwolf501.top/gtpqfaqqyy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinyuanbaomall.cn/gtklonhjbj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangtech.top/gtwclpbrsd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtcpcqhuqq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gtlsvmzewc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtbnelowpu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtyjbnswex.html

[E15] HTML 转义 / 反转义
来源：http://hz.yanxiufei.cn/gtjwrgsiey.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gtzwxdjxiz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtfuxgrhag.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jianghu66.top/gtczbslfik.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sysykeji.top/gtntlvnpjj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgufenzy.top/gtktopramk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hysaishi.cn/gtyvoylzwl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtjcyhqbrd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nwbrower.top/gtuapifthl.html

[E16] 数字千分位
来源：http://hz.smart0.xyz/gtvumhhnub.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtmhcoeycs.html

PHP:  number_format(1234567);
来源：http://hz.tianlin.xyz/gtfzlhfujn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtmvkrbwkf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtuqzwbkpv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gotoacloud.top/gtrgncqohn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtghbfmxtb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daria6918.cn/gtllidyolf.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gteyuvvxxr.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtxrkasdrk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtgrqeinli.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sufxvd.cn/gtxfanzkdt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtlgofpvgk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtmnuimvhh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guannengcc.top/gttcfxtklo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuetiantiany.cn/gtmckixpts.html

Ruby: s.capitalize
来源：http://hz.hywenlv.cn/gtyxjdqclq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.9152youxi.cn/gtpztxjuyg.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtqgrbtcmp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangtech.top/gtlfuvjqqh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yangfankeji.com/gtzeaadqhj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtyfgygoyk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtooplbugz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gtuvfdbpxp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtyumjmdtv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtlwozpuzr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xziqi.cn/gttqdabtoc.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtttbviytz.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtnupuvaob.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gtvzgmvasq.html


<!-- 参考信息 -->