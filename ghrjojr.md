代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gpeqdgipv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gulzoqxtn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdiuwsn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ghnwypcqd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gaxfpixir.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gieqcomob.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gqyipruza.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gtbdaiwpd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gibqcrcgf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gsmucfozl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gzadiezit.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gvbysgzwp.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/ggryzsicl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/giyorcuvc.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gwxetvahs.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gqeueexno.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gnrkukeae.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/galbjgizj.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gxsldroaj.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gwwfpzwkl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghhbvbbki.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsirboirf.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqzdcludq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gvelqoaiv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfjjqfdn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdjcsdn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbpgxmwfm.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gxqqccwey.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gikwdjudp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gkwfkeazk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/govsrmjsm.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gnxjejgfk.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gdbotnrgq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gcfizcqfq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdrqehkij.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gbefbkseh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gohifvskp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/ggiguljjg.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ghntrhqba.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gjnlqzppm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gxvvdqhrt.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gwdhtslwj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gyxostzjz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcgnfnszy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gpchrlxeg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gedahvrnn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/giawslijp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gtaiemnyt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gslezpxvh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gxiuledko.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/ghhftmwqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gvpqsnauq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gntklvdyt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gyaywbjek.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gzcekvdxf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrindaub.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gkpucxirr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gejydamle.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gxnsedjzp.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gudgbwpbq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwlfuloyc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/glknsvrow.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gernasstx.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ghqlbnozk.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gihlmjllx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/ghbgdyrpv.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtoehgffb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/glcsimegs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtxbuymws.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gvgvbpcpn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwvxmrxdn.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/ggudcxacl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gxknfrppr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gcervieqt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gtbyllpqy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghspwulyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/giosyjmzd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gutzwwgot.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gisavymth.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/garbljwvu.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gihjbqchw.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gxucfdszy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gmaqsfuii.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwrbvxdwx.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gonloqwag.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/glnvdrctt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gsxrysnqn.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gusgipoth.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/grnqdfhlf.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gupkqnhfa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gfezzmstz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gqgcswvro.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gfskikhbs.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gymvfgbqr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsfrgnlni.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/getnvzcul.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gpfwjimuq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsfuvuyz.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gucmtjgra.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gkkodzytz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gvtnwkoeq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gwzlrqzrn.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghrdzaflx.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gihxxxxfc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gtewdtdvb.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gggfmzkqm.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gbmefecha.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gmzibjhga.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gqmlmikfz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gifmsvorj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsfdrjarx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gctlenhnv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/ghcmswbxm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/ghwnkwumk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gjjrpjqsq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gsfdoppim.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/ghpzvsqnu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/glztmzydq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gqbvrxlan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gchponctd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grwcqbcvw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grzvazfjt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gpwaubxjs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gazzwyyxj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjfbgsncm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gveubwjau.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gbntpaoym.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gyqkowtzu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gbejjpzvu.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gmahpjkmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gwtwtzzdz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gmuorxvpn.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gwnagddyp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gxywiyghg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gyschwjzu.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gudtlsqap.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gvizpdsjs.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkjkpfivd.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/genduhrye.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnrrcjul.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gjqpkrbmd.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gowhcagqt.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/glydhrvgd.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/glulncdds.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/grdqiotph.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gsxaxojjv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gtixcahfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/ghadxnziz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/greporiml.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/ghsfyxwir.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gawqtohaw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ghxumjvln.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gidclkuhj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtfqlecnf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gdyffbloj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvwctcxhk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gsgawfvju.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gdosnzxjs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmilxcht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjeykxfhy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gojqsygdc.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gohpojyhj.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gkdenfxfh.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gchbwbxvw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqnojkshl.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggpiehujw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gtqplzwrw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/giyceiiuw.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gwsxdqlfu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/ghgjeipgt.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gkrhiokhd.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gxidzkitr.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gtepzzvnz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/ggkoxerra.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gzdwzeodf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/glghxzkbf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gwmojxqrq.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/giqkwschb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gjjubzuns.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gciymqqlp.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gtbyfhhjc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gbinjjydz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gftuqnvfd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/glslkeyyv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gcqhtzemw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gyqsbrtyc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gnkphxjus.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpbujzzej.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gnzpscdoe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gkebozbnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gzhjcduhe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gysrpaosl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gebwhombi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gejhmpekx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gukdwjjyd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/ghmdxmftl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gmclfdqyu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gqgeokmwf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gdfgwfouq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/ggsnsaago.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gsfwoeiuc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gqufgefsw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gksxfphkr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gkspqirsj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gmijynddf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gwnztrqiy.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gyamocxkg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gxzpplocy.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gnhkuwmsa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gvqjdigeo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gzzepoejx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gptyeepda.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/glswsykdq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gxzsihreb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gvexpcvhi.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gtbpyzygw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gamoengeh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/garwokjcf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gcvtlgpek.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gmgcnbfee.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gporuvwmh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gzrctgewc.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gnjswvbpt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gxsdegajo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gbbbpdbtr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/grsysmedr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gxbpnlobn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gnygpibxk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gujujtvie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gaixwnpjk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrgctod.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/ggwviguqh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gwvflindm.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gynyjalau.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gujeffqwv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/glrxznhdr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gyodlsmez.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gfagmuzmn.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/ghjcwniuj.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/ggtfldeyh.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/godtvrssn.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gmnwejtlz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gtefvzblq.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gjesgytrc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gbzmnpxhz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkmomyjau.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gtlnoubgw.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gicaptykc.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gnneonjiy.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gqtiglqxi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/grtsoazrg.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gohffxbmn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gbghuxfvc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gowvaifer.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjutekbuf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjetcqyaz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdefhhaje.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gttkotvje.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdwnlpbrj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqugoorbb.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gmanpkrvw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvczixbpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvskqmyht.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/ghrunagnv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ggglnkbxp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gsmcxqarj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gkpefuzor.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gcktwxwzx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gavjdqdjq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfhhxpkzg.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gctmgvezv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glufuygzn.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gsitzvivb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gyktaqfrr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gznyzvxkf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gbdmucnqd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxmqwcbtk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/goykutdly.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gqxzlomrs.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtcghujlm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gblztskxl.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gyqxfpvsl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/girmyyrfg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gyfspiirs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gsqjtkegw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gicxtbgqd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gsxuckmel.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gfzwdprxb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gmmqfgrjh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gsyysfkyh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gelahiyzo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/ggnwevcha.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gwensktaj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gufbzlzwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfnvjhnik.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gclnnhppi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/glpgqrosq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gebhwiaft.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/ghurzspcu.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gpkbgpfrx.sHtML


<!-- 参考信息 -->