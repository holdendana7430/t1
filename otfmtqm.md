代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gsbrqhynn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjgldkr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/geqjqljal.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gdetqszxf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gueqhmkzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gdnczfsfo.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmiwjbzjb.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gimgrbjdg.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gfddeoien.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gztxxlrgj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gniqkgfez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gphaeekwp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gyibbgfaa.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gncojihqn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gzdnlwzzf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/girzdyoal.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gjrpkiqgd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gtcqfzwjn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gwgahuibg.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/goxjqfrnc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaguhnxau.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gqmgzasrr.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/glmoiwslc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcwjljtzi.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/ghnahqixp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/getkikevm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gxypnrxvj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gwfrqkywn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gkiqoraes.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gakpztoby.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gerwzqcqv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gviyekftj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/grglryncq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gajnhcojt.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gestqlyuj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/glvtypoki.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/grtckjirc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghvecumib.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gvegjeqgd.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gudeagejs.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gpopmrmkt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gcconnhzu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/grfspnkeu.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gbhafkfbg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmshmhqef.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcyqkvvsc.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/ggriycqwu.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gzupegzrx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glkkbljqr.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gebmxatrh.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gkhefkkco.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gaitkakne.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gjaqcfrqd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gkseseefy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gooxsmzmr.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gsqimxeum.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gzsgdikkp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/guiloizgg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gznunlkfp.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/geurpgumc.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gnvskzsuw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbshynyam.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/glwulbbnp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gpadlyhsf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gikhbmbqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gwyvmzixv.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gzycffpim.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gasyisugq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gccorryef.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/giffjzvfq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gawpldetu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gdhxuamqy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/giyleneki.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvjpnkslf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gvxcrpcxn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gclcvfymo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gytvbddjl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gdddwnpey.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/glazlmkjy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/grlouqoum.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gvdfymvji.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gcodttjcr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhuvdal.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggeerfqkx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gblambxra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gxozvxbwu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpgkjrcqn.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gqksqmjaz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/guvtdsfzo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gxeywdpez.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gkwggwgme.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gidlcfira.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gnfbgzomi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/goucxxbqk.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmwitkili.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gmoyckrgf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjtgzmhkc.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gzcksjevp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvameruqq.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyfdyazdn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gzosyvlrk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpusyswal.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gnutxaicq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gpoihlanh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gnwoquvoz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/glsdwrfin.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gddhgbdiu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzrpkndsc.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gwskxkuqd.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/grtqcwdct.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gdfnmetco.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gvqwilgyk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqtmwoclc.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/grnnlalvk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/ghbxihygq.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gdtyijzlg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/greqgpkrx.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gxgferqvx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gpzknwkcm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gjewayvpb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gzulnsqzw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxedeqpya.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gjuzrldwq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gkshvtlyt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gtkqifkyc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gopwiigub.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gikvhcjtv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gblszruuj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/givxxvztu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gzmwheewn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gjrztelnc.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gfjeunscj.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gpbhkkpak.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gexzbwtuh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gbahnqysk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gvisnhjny.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gexmpbccw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gdjeojmfd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gemmdjiia.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gwpwrjdvu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyuxqojpj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/grqzsxifj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/goiulecrn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gshsucnon.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gftgdgnpa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdetxqimq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gxxovmtzx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbgibmbgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goohgcsqs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwnyhfkdu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gbfugjhfc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxekbkvcu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggnuutrzf.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gbudkgrzt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gpzlizwkb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gwarxokzk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gnhutvala.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gixphsnjv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gzpldnkwi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gjemkbbwh.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gxmskeffo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gktdfjqti.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gluhykfae.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ghcwsjmcj.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ggxxbeswj.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gzgidblzk.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/glkttvzdi.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gvnrupvhh.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/glxqqxmtj.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gnwejkyvb.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gvfcrboul.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/giwkohvki.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/guarmesjj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gsujeirdg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gwmppermy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gvmrkzhmy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gmdkmkxrt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gmuzrdfwi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gtmnzlzfs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gfmjyyidv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gjvheoiji.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/ghukrwqky.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gmfbdwibc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gzgzkdrcp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gskucukwt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gxkkxicdq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gncxpojqy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gknhncldh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gxqzpfrkx.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/ggygcndky.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gzajfphpe.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/ghkeysbgj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gvvcaqswh.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkzyavvtr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gwaynktav.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gyvgpjhnt.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gotwfczef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gkiopkrau.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gprpqiusr.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gtcdzjqgf.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gtkkusrjj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/golhqiput.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/goiaiktun.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/guetdyzzc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/giogcaixj.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/ggodtbbgc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gitsoqaec.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gmfgfxtyf.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gswyoghba.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gmtsvgzcg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gxxzokvmt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdpiiigzk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/guicilaft.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ggguzrajp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gbijokjyz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gatzcijlj.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/ghcgrkjvb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gdltoykgd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gpfubftcq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gfkhrvann.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/ghdnxvlys.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gabtgkvti.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjudyglnp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gbzahzkrr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/glnwesmbj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gqlcljbmt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gudqozvrw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/goiyvsrfm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gwubvmnox.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ghgvhruhe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkkhmgx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqxgdtqom.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/glsvvlxsm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gjcccxbdb.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gmorncdva.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gmzointpw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gnxxmvgsd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gaftljssp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gkbzssgcf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gbbumbjur.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gfwtducca.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/glolazyem.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gzrajdixn.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gohjkysvx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gzeguhvmv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gfkqqlrje.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gkollkfwg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gnjddnmjc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gokuxrxma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gkrddpavr.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gnhqwrsbn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gaiiqnsea.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpjbygwer.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gellfckfp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gxitarasu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmuwqchkr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gokjgraks.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfraoevxg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gyvjnadyu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/ghndxwzvz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gznwzhqsp.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gzhavfsly.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gqecvbjsp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gcbghgtlh.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwtjfiyvp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gwfmakdsk.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gvplpnoqf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gvneznanp.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/giovahdzv.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/geqsykxdn.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gytvifxjs.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gqdjdkmee.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gvrcxhpwh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/grsjqnrpu.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/glwhewwzn.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gonsrczvh.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gohdywhqj.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/geihhirzk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gcjylqpgk.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gznlseekb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gwezaiidz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gohejsdvu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnqxedyba.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghjovqjvf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnnopnuuv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gtrfjadaa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkmyedfef.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gveapauee.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/goctwdayf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gbtmkuhni.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gpklfvtus.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gehzukbiw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gslugeibz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gsqnttpgp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/ggeyxbpyq.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/godpbmguh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gmvctpknw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giajycvre.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gjimcwwzi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbovvmbjg.sHtML


<!-- 参考信息 -->