代发 wailian999

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gdzjjybbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/grbhzrori.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/giiqetwxb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gfmrhoxoc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/glcobgihs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gcnbkyxla.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gtebwvoue.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gzvueijnc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gkdyktpkj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gezddmhbk.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/grveuxlbi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gdlkuxigb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gcilaonxm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gkauwdbqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gfylsmuig.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gaitnfkzb.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gtqzcrsic.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gyvwkexjw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gevmtabqq.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gfbeljxxg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gedyhlvay.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gzwefdvtc.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gwuwtvnjy.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghlrhakpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggkdvdvde.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/grknrlydj.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnkgvpqqv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/glzpcuyan.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjdkkucey.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/goxudpwgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gxvtmhzkr.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gmcvyvzvc.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/goxaobrji.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gblfuzkrc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gdukwpbdk.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/goucdfhdr.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gddncrgge.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/guuhbugoq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmckpvlqd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gyfbuxblo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gymqagxkf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gsrmoycyx.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/guxlbadsa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gnxuudycj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gpebxlrob.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gxmggykjl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gfdhtjggf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gkyardfto.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbrjtjmiq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/grcmpwjaa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gowawwpqt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gvehiibcw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gckpeuxcu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gznhlitly.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gmfukbsre.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gpbwwfxud.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/grldzretf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gohbqsksw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gkqyndnqj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/goetqiiyt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gylrpqznn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/geehgrmdo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gqevxnpqk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpztmixqs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gxzazsawy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvgcdasud.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gohpafxld.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gtncrofnb.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gryhoaunh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gopmxaysf.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gmzqyzdpo.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gokmuodcb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gftnnidwv.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/guqnhyrey.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfnrjagdh.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gmuuluxef.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gcqbbucvy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/glrrbwhkf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gypbtkchk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/goqyyvdrf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gmbtkjwue.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gyahoqlzf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gqttrbmzk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqveltojs.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gefbwbodt.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gwmsttdhq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gjlsbkfnh.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqxsylfzo.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ggutdtmir.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gjxaouxxr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ghnfxztzb.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gpbxdoezq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gkudzcxbu.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqtxjwnar.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/geydfkqfg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gilxndqzz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gnkprsebr.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/grsixryfx.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpoflmvvr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/govyaqxsp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/grilyettv.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gwtbmhabb.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gvdbxbqud.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gzrzqqmtn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gufxezghw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/getfycptl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gcclwcgkn.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gnktvyreg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gdkaaznkw.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gmxzupsjp.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwunmbmkv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/ghdohnnht.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gxylauxip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gymvqeogi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gdohgvaxf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/giqrbqdfp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtvdehmah.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gbbzplgtq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gscmdmrxb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gabimjuwd.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gfddptizd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gohdqilws.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/geixjgdda.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxvfujtbc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gsejsxbji.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxksvcpwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/guarmqdil.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwjqgfnju.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvvbecbqv.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/ggsadhqiu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gmaeakjfn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxmrxvwtm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gtbsqgovy.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gnijhabpb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gsdfsayvv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gkccsixhr.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gmbeevixj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/grfilxvay.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/ggdrxepuh.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/ghklzyqlc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgdkmobz.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gidylgshz.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gxzuwpjhc.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gklkdvdex.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gpfkkewag.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gfifbopzw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gitnkyoax.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gfztstuoq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gzgpfyrst.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gwnakalbh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/goddqmjzl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gixvnzkcr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gtifmdfqv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gxbdxmoto.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gflcqsylt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gemwgcarp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gxotrthzl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gxrkhrfmm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gdrmazhao.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gphhidunk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gbnadzjev.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/grtukzaut.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ghfsgvcme.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvohgwqfp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gfiomplyk.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/galafzxlq.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gwqfifxoy.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gfcqcbdci.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmirjjryl.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gxnspamjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gkjglzvgv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/guhcmxsxe.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gidoehosk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/guivptoip.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/glbcdsrnm.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ggloqvgpr.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gffuiiluu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gzrbrlhzx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gfpahesnp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtnuhkszs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gofunxcsn.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gupbggmni.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/glndfcssg.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gscdzsgwa.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gebslyqfz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/glkwfqmej.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gbrkyyxxs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/geghjatkc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwmkkslqs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/grtieyoaf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gzpdobcor.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gqhbpgeza.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gqjtmixgm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gbmlvslvt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gmsuixynq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/guazsoawe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmnqhqdey.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ghzaayoaf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/girxzfiri.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gzcrofkbu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsqxrlzxy.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gbutlepag.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/ggglqzzch.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/ggxgqmzho.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gtmhkyizk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/geqkprwjy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gtgulbioc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcvrjemnn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gnodxufqb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gvxlbucdf.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gnawqjauf.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gmfubwcfg.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gihlfnojl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gxbhiofnz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpznuccix.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gzdiadlfw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gtuuncacf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gyzqzxfmd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gwjhktcmr.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gacdnoykq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gwsgbohyv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gywfnmtmn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gqnkvavkd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbezuhior.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gmtnxazie.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/glvnowbdi.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gnkuqwftb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/ghsnbyhie.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gkfzdbkuu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gvoirlpil.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gxheewugz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvwjidhdl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzlknonci.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/guavtgedz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwsqorzba.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/galfydxje.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gpnflmzbh.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/ghoiwapem.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ggpmjwpwe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gakwocyyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gibucvyvm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gzkmcwrgz.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gqmbvyjwf.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gajcjudem.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gdqsjcriu.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gijvzkdye.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gwbwzlcig.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gpmfzbwec.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gzszikdwk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gkijmmahb.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/ggizuclvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwuxjbdkd.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gztbmmwvy.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghzwevdnp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gxmskbbbd.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gfyxpsqkr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghkftupht.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gcchgyyco.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/giknwacsj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gozzweyyr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmkukxygi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gbxhfmysr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwesbfdca.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glfuhcsnf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gnylurjrj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gbtngkegd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdexojewe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxwapodrn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gqjalkxqg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gvdqiiceb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gbxxbbfmr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gjrmzfjva.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ghaszxffu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbzhrlseb.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gkqhuzjkc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfqqdhutb.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gvezahsjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gyurxfvnl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gktwotagl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/ghickqpdg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gfxkyvflo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwwzzekjg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gixkpowxz.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvddyvoqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvpuzvwrg.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/ganhqwdfn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gbfbhpidd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/grcpifacm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gefyhzadq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcmfsjrnj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gxsbjknuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gfzvxqyxn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gowasqpzu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gtnmcfcvr.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gxevefelr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gonrhpuus.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/glguhelzj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/ggrlywupb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gfbndnrbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gxqrosxdt.sHtML


<!-- 参考信息 -->