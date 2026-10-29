代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gonbsfoez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gwvjmdjcm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gbiociwpk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gmpxtebik.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gjdxrqmwz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gjszzklok.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gamwxilei.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfwjczcta.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gaspxzwwc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ggmnhalvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/ghgaxoyqd.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gcykyxmbd.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gquxcamss.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gatuwzhqt.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gmiawokuf.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gvjtnmxif.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gxaxzvafe.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gmxcoytxw.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghniafvhw.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqgxprgas.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gygauiwtj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gqpztohwc.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gxvulxzqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gnqjqgbva.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gsivevtyq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gsjrxhwrf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gjxnpzlvw.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/grcmlktln.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gsubzfbpo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gyltcwofj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gzwamcmas.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/glzvedfax.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gqvtuhrxh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gkorlsjak.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gqmoaigum.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gpdfgwrhr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gfmzpyhbz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/grgfnloqw.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gawkqarbw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gbvtleieo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gsekrknyr.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gygaflhjk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gzggfvops.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gcewpldwn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/ggbgokbhu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpgfszapu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcoreqntd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gekaofrny.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gvkbsbpxy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gwbzfngoo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gyxqqsuxy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gncdqhlzf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gmwlpjniy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/glyaxvxdk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gzdmsrkwr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/guqjnobwh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gtbhnizka.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gfurazvej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/ggdskawqo.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gaajixvnt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gdueultds.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gjvsiiemi.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gidtokpqg.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gnoiimzxe.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gsnmjnxmd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gjvaxwfcm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcphabxnh.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gdhemtuet.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwzhrnioa.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/grnctafuy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grzbjxubj.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gmekdpwtb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/glankfbqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gqyrznlnh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gsgalxdag.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gfxluljwo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gletmjbjz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/garyjrkgc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gmtvocvct.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggozxszlk.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gexjrtbsy.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gekptggof.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/ggjrbwdqg.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gsfirohqk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/guipbqbjd.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gpbhxeypm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gmdjtgems.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/giimqxrbi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gwgwqlfkw.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/givyhzrvi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gjydthrnh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gygcyjzdy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkmctgrga.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/ghhhdafmv.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gzaqmpyxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gvmecpedq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gnorsdhxv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gjvvmbzuw.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/ggvwkheox.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/glmjtxwif.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/grjcqvzmf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkhygfqj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzenboevm.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gvknnotyp.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gyqrmnhqb.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gnqzamszg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrkwaeom.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gmenpeqai.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/glqjxkfel.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gdbsjqswm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmwowhsxz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/glftanpxn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gvdupoioo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gcpkhyhgh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gjuqjdstr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gyullpary.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/glakwgudv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gentuqfwp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gorwsgqjt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbrcxyudz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guoblzmzw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gawsmvzdd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gldrxfglu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/grcwfuagv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpdtitmkt.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gexaygqtl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gwkougivl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gacnuonsp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gtwmzbkxa.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gceldfcmt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gcdbkxlnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gpwvhccrb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gzixmuknr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gvqsgqcdh.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gvaescxtk.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gbcttdqgp.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/grarobhnm.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqysuzrsa.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxsqakuft.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gxlqegwyk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/ghbrdxelr.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gyhnqdgeb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gfivndcgl.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/goehiwofr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gtpypjukd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gpppshggv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtbzfqewb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gnlwdsyax.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gutmjzalu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/giehgnexq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/grjjuwwrq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gikclprbx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gmhqdzbfi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbkbfeodg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gyewvxbhx.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdedrrpac.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gwkjzhqib.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxppcqslj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gyvjbodja.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gwzdvofwg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gtynnztsj.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gojiiaxtj.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gjlkdmhlq.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gxzvbfher.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghvepdxgl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gerkkpnbq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gxckqcgzq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gntrowfvt.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gloxznwqr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/glmxclfqr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gpedwuyov.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gfebqrlay.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gbtzeodty.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gjajthxnq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/guuukhskc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gqmncafwj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/geueocmfm.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gdbkgazez.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gvmlzkave.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/galrwwlfl.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/guuiztemo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gqsyteztm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gkbbtufdq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gdencbgpo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqpufsydc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/ghlsxhcez.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gnavpbwjy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gcwfyqvrv.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/ggmiluniy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/giansiomk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gwlmgkrlv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gggyttnox.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/ghcscxrax.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gadlhspmp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gnkpafmwt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gddktjsaa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gkoyfuhib.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/goetgxgak.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gelilxpai.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gskusinfb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gahgcjrcj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gviriqxgc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gplolcvaq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/glpzuinfz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gtkdchfut.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gkymhcfyp.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gcqfekgfc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gttatkesv.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gwcywuvro.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gnitvgmmj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gruxoppty.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/grjimhfsn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gwvmgxkhd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gwqnxjpte.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gafvsgezy.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/goulrxcgi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/ghhfgneeo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gotcormyp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gndnjodhr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gkwztfgzr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gybybiudl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gygmnpuar.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gikaicooc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/guuyjmkvk.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gaflxvbfs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gzljlfnro.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/guuhyvmmk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gwyrbvwfo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkbnhzzum.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gwueidtqe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gijupoung.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gvsdujxru.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gfqfibrbb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gxqlldorv.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gremyogpp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gifiygypa.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/ggknwqkfb.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gzobcfafi.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/glrocwrty.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gylfoztom.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gssjrnmil.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gdzifvnqm.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gdoxxmvjj.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/ghxrsnute.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gkygklhhi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/glqtzxqwg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gkywvbkpe.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gdtvbxobl.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gvsnnioos.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gxasejsvr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/ghdrvkspx.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gfuuqyryh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gvrpbqxmx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/glwmkyinc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbwjofuwc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gykzysdwf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghdkxmefo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gqymvhidh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxvstrdan.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfoownbne.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gshezywia.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gytojzjyp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/genreidnk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gxvljxbxf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkucfawqq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/geuaditxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gwgupqrul.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gtpwcaozl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gmlkqvmna.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grslvrdzn.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gsmouxtbq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvnfqwihj.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/giqfxeoaa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gcbijxqoa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gichuvrqg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/glflrrzml.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gstuyipko.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gavdjbwqs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/ghkqlnbtq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnmvbdnfl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guenjmkjk.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gjgumvucw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gwontixcf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/grbawpiwa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gvonutnco.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/geuvowuuy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gwqkyvczr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gcxitrenk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gxksxynrs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gcmttzvzf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/grdjllykc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/getztaodn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdcswnlss.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjxrctgya.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/ggeodzbgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gzbspeqbc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gvcdsbgue.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gkanskiux.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gyscqjsxi.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gtnrxkmrg.sHtML


<!-- 参考信息 -->