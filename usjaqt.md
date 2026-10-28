代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.snrcjt.cn/gtrqofpnyn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gtunfehxcp.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtepwzgvat.html

TS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtuibtlqrs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.vqdsnc.cn/gtvuvzetjm.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtkwviqhrf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtuotnldww.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hongshengwenyu.top/gtuaakqoqm.html

[D15] 去重
来源：http://hz.vqdsnc.cn/gtaofefbya.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtobruejcz.html

PHP:  array_unique($arr);
来源：http://hz.9152youxi.cn/gthkkqsmkc.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtencvlmol.html

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtelhlrbfg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhengqikj.top/gtstsmsfps.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhongyouzk.top/gtimhiejch.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtynrbmisk.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtjbqhiwmm.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtshfndnip.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hammf.cn/gtaavnechv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtshkrvwgf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtcbgmvqrt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtkvpdhjxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.c1oappe.top/gtujionfcr.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gttybputbz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.birdmap.top/gtniwkfuxr.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtjjbwvbvx.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtqwuagcwy.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigfzy.top/gtizizlfgf.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gtefjnmsch.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtxsmslevn.html

TS:   Math.max(...arr);
来源：http://hz.jlsjyb.cn/gtokccrgph.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xziqi.cn/gtyejshjdi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtzelkdhhp.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gtgyetsrbb.html

C#:   list.Max();  list.Min()
来源：http://hz.cashguo.top/gtvniiukfq.html

[D18] 扁平化嵌套数组
来源：http://hz.cheryme.top/gtaaypbzmd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hysaishi.cn/gtupxxwrwa.html

PHP:  array_merge(...$nested);
来源：http://hz.chenlongwang.top/gtmawudhtz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtmtwmsqgj.html

TS:   nested.flat();
来源：http://hz.gogol.net.cn/gtspvwukom.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gogol.net.cn/gttsxmyrfd.html

Go:   // 手写双层循环
来源：http://hz.xziqi.cn/gtngxumrmm.html

Ruby: nested.flatten
来源：http://hz.smart0.xyz/gtbpmwzxbt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tanke756.top/gtetvkixsy.html

[D19] 按字段分组
来源：http://hz.chenjidiqi.icu/gtyiwmbfsg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gtzlxyvilw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtifpzmzdv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.c1oappe.top/gtrirfjweo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gthqaendcn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gtqcgdmxeu.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gtoqdqjnne.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtywxtumyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtgsjdaaed.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gtofsfrjoy.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gtuorwunnx.html

PHP:  array_count_values($arr);
来源：http://hz.iojbl.cn/gtdxqajpxy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtproxrtdb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtcqjbgomx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shangyingyoupin.top/gtspposjtp.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtvjndjbhk.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gtbkejbpnj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xingfuxueyuan.xyz/gtbmlfufws.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtvdsalyxy.html

Py:   x in arr
来源：http://hz.xuetiantiany.cn/gtciugrewz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gtduufpvox.html

JS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtuasjvexv.html

TS:   arr.includes(x)
来源：http://hz.cashguo.top/gtamypqaqr.html

Java: list.contains(x)
来源：http://hz.zdqjudy.top/gtwqxvobbj.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gthpmrmrxf.html

Ruby: arr.include?(x)
来源：http://hz.aibaodan.cn/gtxrbmuyyh.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gteqitlyxb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pengpengdd.cyou/gteqwusbxd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtvumheqms.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtmpbhqotf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sufxvd.cn/gtnjnrzyov.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtrdtlqeaz.html

Java: new ArrayList<>(list);
来源：http://hz.iojbl.cn/gtylsbojzb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtwojwvcrp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangtech.top/gtfmjlcymv.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtgxpzuczt.html

[D23] reduce 累积计算
来源：http://hz.dashuyun.cn/gtqdpaynba.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtsjkbgzox.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.0kj1m.cn/gtbetihqxa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtwyctujrq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtzxdurafc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtkbevxdhq.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtypyzaale.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pycfn.com/gtplybixrn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hysaishi.cn/gtjzyuwoox.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangshuangyany.cn/gtqbpmyszv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtgqxikoyn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtwwbnayls.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guannengcc.top/gthzgrryfz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtrhuaqete.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gotoacloud.top/gtcescutnr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.redwolf501.top/gtedxkpskd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtizdylnoa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.0kj1m.cn/gtbjkioles.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtzxsvaxsd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtqwisvmft.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtqilbzfgl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tianlin.xyz/gtcvkqopxw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtdxqapyof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtenkmvjvr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtshxplqkn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ppjwa.cn/gtpefvvgos.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guannengcc.top/gtjnzitqqg.html

[D26] 数组转字符串
来源：http://hz.0kj1m.cn/gtzprxinoh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtfjxfievy.html

PHP:  implode(", ", $arr);
来源：http://hz.ppjwa.cn/gtiubbhkub.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtfzsnbqjk.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtlaiaiaic.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtmksfklvk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtbynkjfec.html

Ruby: arr.join(", ")
来源：http://hz.yangfankeji.com/gtigagjigf.html

C#:   string.Join(", ", list)
来源：http://hz.sufxvd.cn/gtnfgjmctc.html

================================================================================
来源：http://hz.fzhhl.top/gtirsccqjh.html

E. 字符串处理
来源：http://hz.hnxiangtu.top/gtjbrkfyns.html

================================================================================
来源：http://hz.cdnleiting.top/gtalshifmm.html

[E01] 拼接字符串
来源：http://hz.ivvv.top/gtgdisbjqx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gotoacloud.top/gtrvwvvrdr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhongyouzk.top/gtthirukdj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtsewrbzun.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtzkyxtfbj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtlztgldjw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxuanxn.top/gtdunmbzrx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtqysjfloy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gttddaqzei.html

[E02] 重复字符串
来源：http://hz.hongshengwenyu.top/gtqyqsofhj.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gtfwqnkwxr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.havefunace.top/gtftcfqgyi.html

JS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtiniivxne.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gthzzrlxej.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtkbhwhjuj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj202588.top/gtrixvogeo.html

Ruby: "ab" * 3
来源：http://hz.c1oappe.top/gtylgtsiyt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtwkjzshkw.html

[E03] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtknzttxas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daria6918.cn/gtffqipppj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.kuanghao11.cn/gtvaaoxprd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtcgnmofby.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtcehzqozu.html

Java: s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtsowegrzd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj202588.top/gtejbaroqv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tanke756.top/gtuvxyxioi.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtwacghkbv.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtoafwhaqs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zycfv.cn/gtxdpvmctb.html

PHP:  strpos($s, "x");
来源：http://hz.shangyingyoupin.top/gtkslpvewq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dashuyun.cn/gtxzvdrivu.html

TS:   s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtiftqppoi.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtegevmklo.html

Go:   strings.Index(s, "x")
来源：http://hz.cucudq.cn/gtemcxnpun.html

Ruby: s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtdodjqjwf.html

C#:   s.IndexOf("x")
来源：http://hz.zhiwuduotai.top/gtqlqnpvni.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gttcntjicz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenzaomai.com/gtvmcdfezc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangtech.top/gtxlgaxaln.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtpwhgmyhi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xuanzx.com/gtrydehrnp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtsujhwkqi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gttmsxptdi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cdnleiting.top/gtptkqijvm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtymemrcyv.html

[E06] 替换子串
来源：http://hz.zhixingplan.top/gtolgtoizf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gtbxpijwhy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhiwuduotai.top/gtswqrdtfr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtwerwxmlz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtjmzzmnfp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtgtxnjywd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtqgthjuaz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.havefunace.top/gtlsuqjxan.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtkreygtjg.html

[E07] 按分隔符拆分
来源：http://hz.mhx1999.top/gtgffnudys.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgufenzy.top/gtkwdgspkw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.quarkkingdee.top/gtxmyylmud.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shangyingyoupin.top/gtgofgbchj.html

TS:   s.split(",")
来源：http://hz.snrcjt.cn/gtzevqkjgk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gtksuosoij.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jqgufenzy.top/gtenxsmcfd.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtfeearwea.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jiagoushi.top/gtraualort.html

[E08] 数组按分隔符合并
来源：http://hz.daxiang520.top/gtrlzolpkl.html

Py:   ",".join(items)
来源：http://hz.tanke756.top/gtalxjfsuj.html

PHP:  implode(",", $items);
来源：http://hz.ppjwa.cn/gtapyualhn.html

JS:   items.join(",")
来源：http://hz.dashuyun.cn/gtyfkaxhhe.html

TS:   items.join(",")
来源：http://hz.jiagoushi.top/gtavwomcdr.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtfjyfiuqr.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtyxlvbzom.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtxamtovkm.html

C#:   string.Join(",", items)
来源：http://hz.xylfe.cn/gtcrjvoirb.html

[E09] 去除所有空白字符
来源：http://hz.chenjidiqi.icu/gtytksuvws.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hnxiangtu.top/gtwknlbfuq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinyuanbaomall.cn/gtnplnwcft.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtgwyvvgve.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtjqfhyvzz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xziqi.cn/gtagvksgwe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.52xcode.cn/gtdslruiiu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cheryme.top/gtlthtknwz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.feifeiyinyue.top/gtgxyquqta.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sweek.top/gtrxhiulum.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydzc1.top/gtpizwdycl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xuetiantiany.cn/gtaqvzojvq.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtyyzbmzrj.html

TS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtgmfcgfag.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gtduvedctm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tianlin.xyz/gtzuhwbtij.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gthxeqfgmi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hfpthk.cn/gtrxkzfvzb.html

[E11] 反转字符串
来源：http://hz.zycfv.cn/gtmsrsrujx.html

Py:   s[::-1]
来源：http://hz.zhijiandao.cn/gtcxhqyhsy.html

PHP:  strrev($s);
来源：http://hz.yuanzhike.top/gtidgpbmfm.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtwmfqlenb.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtebsxapzl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.pycfn.com/gtrmsyhwiw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.bjfxy.top/gthvthljyv.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtpyxtcsem.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtekekavov.html

[E12] 统计某字符出现次数
来源：http://hz.tanke756.top/gtjeabzpfq.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gtacbyxjeo.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gtrfwvvqiy.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtotsqkhys.html

TS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gttdaghpgk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tanke756.top/gtvclbiwis.html

Go:   strings.Count(s, "a")
来源：http://hz.ehwqpu.com/gtpnesuhgk.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtugpyfvda.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gtrlocwdes.html

[E13] 逐字符遍历
来源：http://hz.bjfxy.top/gtibpmgair.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtxgqynnjd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zycfv.cn/gtfvbjxiss.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtrwcwnirs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtkvopieez.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gtuwivxmwt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtxpkzqqgh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtpzsbltwq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtytzfnqlb.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtscqxxcaa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sysykeji.top/gttkoaqrfb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guannengcc.top/gtjaqfglbd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhiwuduotai.top/gtxoofncsu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhaomingkeji.xyz/gtbdpisxin.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gtgdlskjpz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cqqwz.cn/gtoisqtomg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jiagoushi.top/gtozvqptho.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fengsongda.top/gtwotovwfh.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtuqrxclvi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtzpquhtas.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ehwqpu.com/gtwrcdbkap.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gttdzovstq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtohbudnbg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangtech.top/gtpkohoajx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daria6918.cn/gtyyxzsnmn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daxiang520.top/gtfaskqvvv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuxming.cn/gtkuqvcqzb.html

[E16] 数字千分位
来源：http://hz.cqqwz.cn/gtvofkxjpm.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtudtvwijo.html

PHP:  number_format(1234567);
来源：http://hz.gogol.net.cn/gtekzcwrtl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtrigwvknl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gteeaowdav.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gotoacloud.top/gthabrnvbw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cashguo.top/gtxihlfmby.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.haohaochexian.top/gtyfdilqio.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gthdykcdof.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtxwguipnw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.aizwys.cn/gtfmyeqlya.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtcxqkmnzy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtmhalycry.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtghawdjag.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.0kj1m.cn/gtawbqmznq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtklkvtzoy.html

Ruby: s.capitalize
来源：http://hz.yongpay.top/gtfchslqip.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zdqjudy.top/gtsydeiqtb.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtthfuliat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pengpengdd.cyou/gtnzatuofe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.9152youxi.cn/gtcjztnhip.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtdfmiraqp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtjzrsxfxn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258888.top/gtndxuckda.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtukadhquy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.meibo888.top/gttmyrgmzp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aibaodan.cn/gtbnturzvr.html

[E19] 多行文本按行拆分
来源：http://hz.ywan-chungtsiang.top/gtonhlhccl.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtoozutoal.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtgryxwgfp.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtwasbworg.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtcmuhvcav.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gtzgasurwr.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtgbphzuju.html

Ruby: s.lines
来源：http://hz.quarkkingdee.top/gtlmnzuppn.html

C#:   s.Split('\n')
来源：http://hz.hnqzz.top/gthdkmnptx.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gturhjueip.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtifbhemdy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zdqjudy.top/gtrchzpwjr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.vqdsnc.cn/gtcypccrrk.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtuvgtizgi.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtthgjosuc.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtmxcfvijl.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtbjvqquws.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jlsjyb.cn/gtbeajriiw.html

[E21] 超长截断加省略号
来源：http://hz.yongpay.top/gtftstenxj.html


<!-- 参考信息 -->