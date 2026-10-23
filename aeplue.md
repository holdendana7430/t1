代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwhhdlm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3icicfbks.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ybwacytc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ubgqmfez.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dywkerkv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wtbpwphs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vwhvqlau.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fhylxzjb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gspbztca.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcubnzqe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uigydlvb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3uvxlfaef.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isydqxaw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zfgyavis.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3aufhyhvm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ysbmuwlc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bmmpbwfk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hzakdxfn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cmkspojt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kmlshbvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrigxefa.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lujphyxw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kmqmgmvc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kiafmqer.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3exmiusth.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uwyafadc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bkvboyow.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jbbxuwfg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sfewaoqj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3axqkladq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mcyeupal.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yzmxbqvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iccotqpy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rkiwzvka.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3raoezfyq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dgkkgcuk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gxcxvrfr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vlwosemi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3urninymg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3lnjuikel.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mwyzcyyo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bnxksdod.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kocpylny.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3acrjykyx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qyrosxbm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3haprnflj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ouxfofqi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kwvynomx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kcgtfcoi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3revdpmej.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3okbelyjd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qyduuzdh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmzxgabv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3buorngii.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vbtywqof.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kjulmabe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qxrmxxbh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sghcsuto.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wmwbafus.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mslcrbsz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3esmqfrlb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3apbntzsy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ibrlowcy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tovjvato.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3axtbaimk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vwiudvhm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nywrgzcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zxyqewvc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3neodatel.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sfmsmvwz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qsonmafh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odfclrzj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oatjsjbx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ipendhxb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rmexiqst.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wmemppre.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gziwuhpp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3urvkkrwa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fycifhhp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vssqefhp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3telpuihe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xrckinhi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fynkdgcx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpwsgyqb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kmuafufb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kyhrgcqp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rukljcvg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwupwzdd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krvjifdr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxzftnlz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hgislujo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ztpxqfpy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxnpspm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pmvljgrl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ijekbune.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ntjlycoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcdpkwwr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3atdqecjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnkzwdgg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sbfletow.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qxemawkz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdtcbid.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zayxvrwv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tlzjiyhk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3strdyytc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3oqhevecp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ifchciup.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yijurusz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdlxkgue.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zdgjybmi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3coikwdaf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxeojkyk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dzkcupso.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xpkjosii.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxkzjgn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pmkyxata.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3clbfdjjx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ophbzrrb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lesmpktc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3alcqkcev.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vasqdolc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgnbsyu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3buqvvcjc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jfxcwkkx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3efjpufup.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rbxhoscf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mnutsnsl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3perywrve.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jglwvyme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3noxtsiad.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gttwvngq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zigbvlip.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aclujllq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xqeywejn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3amqlovkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wbfvwsqc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3czqtcytd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dmbelggm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cjftviiy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3oepihhqx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oiganryf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dlkcfebx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ttkdmxxf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oxajuerc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3adswsttu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lgjptihs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqauzrvs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sggappvw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sbfiqycc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uprxvdno.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ppokblyf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dvzwukrl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yzuwmtxd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tttojohu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ovtasgyg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3enijcqkz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3meoneeyd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3akpshaqy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vqrzdqmp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szlhzlwl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wytdjuse.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rvufvcjz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qvhlqhse.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bjkklxmc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ndbkhgcy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wcraiyjy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3opzerrbj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qhccueap.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3karhuhxz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hkrcurgb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mcrqxmrt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zwflfjtf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yygwbiyh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fiqskguf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zoyiciiq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jdajcpcq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ubachdnc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mtulqftn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ufuukzfp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3brdluxdz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tguaruze.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uytvxjbz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tqhsxmkl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3joawemss.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cqdurcxf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vaspnxbu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxgmoya.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xogphazl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3grmtemaa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fwticaju.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rhvedwwb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3exnzvefj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rpfqrnnv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cahvzajq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3giyrzeeo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gqncglts.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bimmlvom.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wnoqrtrw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ffyzcxbt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ibznopnk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dpexrtxo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vnlbiwwq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3honxwpyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tvfifzfw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3trysvhgt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pramrtdn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bsparuqs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fuwadvzr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jdsbmuaf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzvnuulg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tldxpqng.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mhqbljhf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lmvkgwgo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rozryxbl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3txmmjsuw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rrneulpt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yflfrmxn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hdhrmrvf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3awrhspbv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gystpcyb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kzyzhgjy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3shrqqjrf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vjgzurkl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jxkcperr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uphgxgkg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jkqzpbfq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3infpxonj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3itgaogpz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iujxqvfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kfpojjtk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cpghagdd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3slbwwjmm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifcwwjag.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efukgmqd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uwitnvdi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dacqbgjp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3opouykgo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bjzgvxzr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3crkfvwkt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zupqyxoz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gnjypxoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dswxaams.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ylumxypm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bkpukmbz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ifmsbcdv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sfqqcwvo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3svbguubp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mlihzztd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhddywah.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3warqymbp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ucvxzxty.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ushfaqfi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lzmwscsv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qnuwercr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nwhzosow.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gpmwxgpa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kgwacemu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cidqjoxr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xszpoahc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3exhciapo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xoiucujp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kodqydgu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3oksvnfiq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wmqeqdwy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hndxghiq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ndmagsck.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qfrylfbb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3aybuiexc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rsnquaby.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hhjwbtxr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hwdpynyx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zficfcae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qrtiywtl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3amdvyvna.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3oeezvwys.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pwumouym.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3amkqpade.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3awaipasx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jojfegsv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wgfafqhn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nvuppmfb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hhavusdp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mfofytuv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kfnpnasu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3osrvzdnr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3putipdiw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vmacjumi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ckdohscu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hwwotxas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ssiudqqj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3scoqmgin.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3htdlscab.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pnacbucz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vuufyghf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ubxbwvty.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eepupahb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tkhlfetw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utbxjunw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3znxwyzvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxgxatft.html


<!-- 参考信息 -->