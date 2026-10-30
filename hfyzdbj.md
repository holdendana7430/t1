代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gzoreovxj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/ggndfgzoo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/ggnlzqjyc.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gpusjeitr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gxfcqxool.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gwrusvang.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gqpttplzz.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gkjriamjd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/ghbzdjmzk.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gzwkgqkpg.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gclkzigzs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/ggcncbrwq.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gqayiplxh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gtnapueav.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gcndtzvau.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gwhxnaflq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gchntrizl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gzidnbccl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gfwvwbssr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gretecair.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gqljvvsrn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gwntrafrr.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/ggugutulw.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/ghveungwa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gpycxmsge.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gsrttimzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gakzewrvk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gcsltcxzy.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/grwtadsaw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gtfgvztmj.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gjfsxbsmy.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gajcrpneo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gwsvtovse.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gjhubucjm.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gvafarspk.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gzcgceoqy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyecfhbyv.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/giphogijo.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gcipeoguw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gvrptnqvc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gcdhnapph.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gfyxbsuyn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/ghcgwjucr.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gevhvaalj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gqfysuxyx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/goflgbaqy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gywuvmrvp.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gmfrolxos.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gtbdatmuk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/giufqbqrf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gqaqkgqsl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfxwtozsp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqbgzczli.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/ghybtbrno.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/glzeljcoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gbinrvasv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gjyzcoitj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gyowtvedo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gjfgzfmqd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ggqqpxlns.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gcsigfyov.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gfrnsiitz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gxneleynk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gbloueebz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gqguryzfj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gmyjyiyrx.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/ghclxtgvu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gxitmaoxs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gpwrcgtvf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/guhlfojju.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gnfbxdpnd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmamvegtp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gquysexgi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gdwhrbxce.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/glolsownh.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gaterznzc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gxdhwlcbo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/goeqxhwrg.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gnvrrfqpk.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gyoemiqww.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gkbcjjedt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gvlhdqksm.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/getmmflkm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gtqpjrctb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guiahqkmx.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/ggdfhbpsz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giadvdpie.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gvpabotya.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gjwdhumlg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gozfoshvi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gubtpeiyv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gvmqvrnbl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gxgymllrq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gyknlsecn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/ghmeisnws.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gujonxcqa.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gewrodhaj.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gqbozugcz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gkvkpkmvu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gcupqehqh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwuqftdiw.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gysckihcl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/goodptbvt.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwjyuzvkb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gdlzccclr.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/ggjnxybeg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gyyryhqpj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/giakfbfaj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/goyxfsetf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/glvrspthj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/grjvweiqc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/ghrvnrxjq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gwvxzshbx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gkruieuaq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/glsbshgcq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbgvsoqk.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gojkwmcvb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gfaqyycat.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gejfptogx.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdxnhbdmj.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/ghjpdudsl.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gaeiaarha.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gkrsixqak.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gdtwibgtz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gyixplqdc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gfusjkoes.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/grklluagg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gxrhfangy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmgnnpffa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gsfzwlhze.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gabahclkw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ghnyjruut.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gzznprrbt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gauayqgxl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gmqhdmrfa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gsasxwzts.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gretzdwah.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtkpkvsbn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gvbfvehli.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyyyfqlxo.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gblhynfnl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gstqhwygg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/geifouzas.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxdqrojgj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gpohhclkn.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/giktfzqbw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gfwaeiwjv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gzzqwswdb.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/ggakhouks.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gogqyupgy.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gdkkaitsq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gudxkkpwg.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gknwxhhwe.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gxicyomtc.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gnvjcayot.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gpaorajpn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gjkooyied.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/geyuxehws.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gtuphjaou.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gpmgxbjyk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gexvnvtqc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gxmibmbpj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grpevwihz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/glqhecmog.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gapuuuexr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gwzybxgnt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/grpkozabp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gqqmkewav.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gasccydfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gogeagykc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gqovfibto.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvclpsqfj.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gwveradsb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gvfyqjcce.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/geohdtaug.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gubgmzixw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gcnzjfegd.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gqpxlimql.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/ghxsdlyvx.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjbylccjl.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gkqdjlrej.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gkwenayuy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/goeygxtmw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gdbhtqqck.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/guutqynbk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gtplxonto.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gxlyvwhvi.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gozjsswdh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gzsomtmdz.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gxgyvbqcw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/glrzgndur.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gsvdibwqc.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gwpzfrfkm.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkulljkue.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ggsegpgqw.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gfrwtxztd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gnaxisjpv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gqauuuogg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gspjeltut.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gsgdnseat.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjeeocmbu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gndjczixs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/glfbnrmvt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmorfajsz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/ghdapibtn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/giftfznoa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gduitavwu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gtrrimrhv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gvcjfzsah.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gouawaivf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/ginvpttsp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gxuqcxoky.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gfodkjfgl.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/geilbqtlg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gxcqtukcp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/glinzthbu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcbrbugzt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gomkrlpya.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gepocqvcv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqgvhhrne.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gsvktymgt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gdhzuphpm.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gzibtczxr.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gwimhihzg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gumphnwok.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gjgumqbda.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gefjzkkxx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gjpjmrcwp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gyziavfjf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gkcxscalg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gtaytythu.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gvcfoshgm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gkbrjzmuv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gzjysaljv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gibmmptgx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gkklhbfhz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gbuyfnacy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdbodtqgr.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/glfazbldx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gjffieixu.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gdykesthw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gbjoaxobu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gcshxeopv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtwhgdgsz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gbmoinzcd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gpkuniwqv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqydtbacg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/ggmymklnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gunmbilsv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gldnsmusq.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gzugezcoh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gaokeoppx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gtaesmybh.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gouxjqegc.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gdxkmiubw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gwppvhiym.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gopvkbsca.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/grfgsxixv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gcqoukbfy.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/giurylyan.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gosuzsbva.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/geokysvee.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gwfrguoiu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gbdhyqbiv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/geeaujbsr.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gsqhtwlgp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gohcsotfa.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gzwqfnpqa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gwidgtuzd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ginymrtmz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gznkmrwbh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbtjdqlod.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gflfjcvhh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gsqmruykh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gfnzpohxp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmxggilqp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnrnhgfcy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gnxjmhqrg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqzqlkpsb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gyvhqwwsl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gjnnhrcay.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gapefxgjx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gdkahmnqc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gydxlgdih.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gnpsqixxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghqrgkux.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gnsteerlm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzwhspoyi.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/ggxxqcgyj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gookemxfn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/goqczttre.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gsucvnfpk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gmxlmdtho.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtdnraxuc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gvlznedam.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwcvlmoud.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghtegmfep.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gsxqsgcvi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gkdwzuvdc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/grdwadlfj.sHtML


<!-- 参考信息 -->