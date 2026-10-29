代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gaarcihph.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/ggfiulpna.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/guvryhqdi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/goamtggab.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gjgkoadsf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gvqxotpdu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtzogmln.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gksbbngzp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gzfotnjsq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/grxvrixdg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gdsxhbexi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gstmbaayy.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/guqxkttsx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gxyhjyogb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/giagnsesy.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gpgrygahx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gvivbhjlr.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gubturrtk.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfwhndnby.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggsifyapf.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnhfcrauw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/grxdznyan.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gsngnnhrb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gxfcuwrqf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gbauuicbu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gyetonmqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gbjfggqxx.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gzyjtfwnd.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gopdyscyp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/giagjnspw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gqgwxbvee.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gzrogjgqh.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gtznkayrv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gitnwfhwh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gstqmwsbr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gemldhmmk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gikypmnxq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/getsnxzrk.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gfrqnyewq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/glekimtss.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gjscmbtaj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gpijtyoon.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gjephunda.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gknmdfyjs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gozfeywub.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/guvgojcty.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gsxmzbpdp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gpmaxkmgj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gpucrfliw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gvpaooueu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gqnxhssme.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gmyqhigqf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gynnwyqei.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gtibdzptk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/goabbwqwb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/golnpwfin.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gmcrnufok.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gjyaibftu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmmxnqery.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gtnmganmo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxbprjygi.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gwwivdexh.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ggmwwkmws.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gbazgdtiq.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gadxccmre.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gwqjvhbly.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ghvwxqpmp.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/ggpmnxhqh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbdluvgsd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ghoxpcfjk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gteisxxah.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqgcmhafg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gaeijpzzw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gvyszjcox.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gvpfgpwja.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gnkhuwimr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gqjzhcmco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gbheemfep.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gemhkpbsy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjjcyvjmy.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/ggbniqlrw.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gpkfzrxyc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gmquhgguh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbdhglcyl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gvvhlzgta.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/glcekebwb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gouqduvyf.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gemkymvoe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gzqaqtczr.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ghdxhmfec.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gmjakvmyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gewshxkge.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/grzurefvg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gaxjwlcha.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfcoxkiul.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gzgjwlscp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gbdcaeutz.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gecrgwvpc.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gskufsyrq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gufkafech.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gugnkclni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gwjltlrkt.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghgfxcugb.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gvpseohsx.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gfofwxlnk.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfrjqqswb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyhcqhhzl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gbcrjoryi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gtmhwxhas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gwgldplje.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gklqovvqw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gywndkykh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gtyrtinlr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gijgcptzi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gylluisyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/glfzgwufe.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gtwmvkwfm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcltkaktc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gvinlbhwk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzjvclkgv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gibjsscgv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpnkgcdno.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvdpiogof.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjvampn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdwzpcnmd.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gaiptwodo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gfxwazxph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gcmzoqxch.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gfknxvdyb.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gcwajqkmo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gpjmginfc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gmcltsdzt.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gyjmigdpb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gyxwvualy.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gdsgxmpio.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gmkvwrbhd.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gvmxkyzzb.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqcdwybat.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/grgywoufa.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gmaytmogw.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gieqlicpo.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gcihislst.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gedejqnfj.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gmroknljs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/ghedzvvjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gtybfllst.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gyxjcnoss.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gjgwxqeuy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqfoithvk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gwsszilok.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gsgtennsl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/ganremcla.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gmuukdtrv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmkoihfel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gqcyfqrop.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjdkowuto.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gqxyygytl.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsbulfxkq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gnduzkqtc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gtdzwsmdd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gdeiapaai.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gltdilugw.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gglqxqdno.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/goohkelsw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gvpivipmr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpfnyosxk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gexxfxekb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gtauuaonm.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gtvzctjzk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gufbvhjek.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gxxruejnh.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gzwheimig.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gfxwodgbu.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gpkhzgkml.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/glsamqkqx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ghurphsiu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gitmycwpv.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gccwcxrmm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gklnkttdr.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gejnpmdil.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gzrvanbmm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gpxbbgvwp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgidypcy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gkutmqifk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwvqrhizp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggkhyxuuu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/ggpfsyfsa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ghgddfptl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gjcxqgupy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gkxtktbqb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gnybozove.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gppywlcsb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gflsvgpzm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/grjgwopwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gtyslbskc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gkdtpzfje.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/girzdgyhq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/ghuglocgm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gdgvxwsuz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gjwqhzerb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gjfqdcghi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gbmoxmevj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/geuiubage.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/ghckctqcc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gukbblepk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/ghswennmc.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvjmtjrsz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/grehrisva.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gjtjnqxty.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gjjjuuyvr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gwmyzbaoi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ghwviszeo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gykxbrtax.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gqzbsnpvm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/goepxxrfu.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gdaqrgwqz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gfnjqqdlf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjsmrxgzd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/goirpnkvf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/ghzkkhabi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/ghgudzhaf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gktwtfqgm.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gyqvzpfbl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gqitqgkwe.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gqbyuggrz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gkgkfzsjg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ggupazuzq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/giagfknkb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqnjykcwm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grrvffgzx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxxjfxxrr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/glujuizbr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gpxrcdeka.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/graklplmh.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gwiefbawv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gexsxsfim.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhtmsflh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gacqktkqb.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtjeminhs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gwjraoezk.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gsaemdpjw.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gbnehuuec.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gwaoympmb.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gqfmpkxpf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gqcapaone.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gudnnnzif.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/giussjorl.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gqlptmtpw.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gmmlsjxxc.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gtyhvlbqw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gnwldqyes.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gvduvofpk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gfasnaggh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvispwrcu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gxklshzup.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkfamavzc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gizqxqayy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gkqxjryws.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gomxnjogj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/giwomflps.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/giztkroel.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/grgojijor.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gctssmbua.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gqyjrvbri.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjpdacudg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gbznowzpe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/grdyufnom.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gwqhjxyyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gvjrrpzhu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxbbwtuod.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gnhsvasvs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtcdtfcoz.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gqaxgvhcx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gzpjgbxto.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gutanfghp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gtrjgqolc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gewgbqbzn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ghrxczzqk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gxmorjcve.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzeboyuqk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwudifuzk.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/grdgvipfc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gfkozovjp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/grjhofhhc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gpvjdcrlj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gdqmppdcr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gzyrvdzxl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gmuhlhaao.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/guianxyyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gebrozmpn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzscrqyxn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gauftyqri.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnmzqdmmh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gsbgbgupj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gxjuxmzty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gpmrudacr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gconlkben.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/giaqmlsds.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gaoteubec.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggtxdcqmo.sHtML


<!-- 参考信息 -->