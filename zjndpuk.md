代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/ghwcxwtxk.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gyczwmsel.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gvpgiytoa.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gpvbmoaoe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gllgteegq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gifbypwzr.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gfbwyylil.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gznnjrraq.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gwfdbubmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gccakncqi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ghvqipkss.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gsgltqmpt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/guzkgmskq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/grwmjqtmg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gkaognvhg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/ggelrbbdr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gdcacspcf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gebwfyufs.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcinitybq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gshscwysx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gfwwfroqx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gfilnfbpi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/goxkujcjv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gnbsaxwec.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gaqqpdmuv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gzifigjwe.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gowdwbbde.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/grrcelplk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gjistshmp.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gaqijeqzo.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/geifgwwfx.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gkcebfkcf.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gytgorcrz.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gehittrig.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/geyiwmxel.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gcgoplctu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gpgcgjzcb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gzqgxgnjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwxyqmccv.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gteqeypjx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gjzaklyaj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gdnemambj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gtfadrglv.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gcxhmvyos.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gluaizpuj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gwmgqmvsp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/ggamnglbj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/ghlyukfkj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gluqgjdho.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gnnujnxny.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gbhcgtewm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gmravudfd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/grgiqvuuz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gujmjqmvw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gwkjjzqwi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gfjaafhsq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gvjklhifa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsttiovep.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/giuetnggj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gtzvvxanb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gbhfjeell.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gzflwckhq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gtjhmlyts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gktbwcpjp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gpdyyhrgn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gsipzfrfm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gbreoxopc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gchtcqzjf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gfpawspae.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/ggnncdhvt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/glpultqqt.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gcvcfunui.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gpkjatnzy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqfecwnsu.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqfhscdms.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gttgbbdee.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gooobevbu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gtmnixgtt.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/glbcsnauw.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gzyldvxgo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbgbgcmpk.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gguwcelkv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpbnhxixx.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ghivlqswi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gnzzgcshd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gmxqcfxmh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghpzgsodx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gmvelcyxv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gccghkhky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gowqxgxew.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gxjdkjcdn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gcokwtbqx.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gcvgrxjuf.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gidgiragp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/ggtcktajb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/giiuhozbm.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/getwscpcf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggxhewvpg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gcyhonzdy.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/grgmxmzyr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gkxpmhdnk.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gjnntnsps.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/golqyivka.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glyvrbeue.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gxwljteor.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gzluvgjek.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gwdnxzsrx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gyelbriwa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gxcrjdrlm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gtcaylupk.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gneoeaibu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gilkgblkx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gawhpyoju.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gvbuxviqo.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gtkjnkxcm.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gebkhpghi.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gfloprdkl.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gdmouhlbd.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gabjhuhca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gvlipmjkp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/geyfjgfnq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gpldxlbqb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gqdeipgpf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gzxxmwcnn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/grjrieqhh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gooykbqsm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gnhiukbmk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzzwbpfem.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gqdjtpxfw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gujkqhszv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gtfrjnzyn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkjfhnhhh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gswjmxdsw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmbtramdk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gwarstlje.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwpwmvez.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/goizllscx.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gvviicggl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gufxotpwk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gddydhtxk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gzbmqblul.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gpmcgutul.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gjpicuyqc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gdqlwduam.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gypokcoud.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gqasjkrvx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/glzvpolmz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gqydjzluv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gcosnqkaz.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gylkzloto.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqjwthlje.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gmpmtckqj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gqvlvamfx.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gjxfdrkkp.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gqfmclkrb.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/ghujogmop.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gmdwgbngs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gchbifoql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/ghovvqlup.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gfstndubg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gckllwqnx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/goosrynvn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gbtudabgq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gyludkmqt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gsyhtysmp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpqkgctua.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gastzqlco.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzkmdepds.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gjnnzxnsp.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gavprhovx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gofkpksak.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gihyobcpp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gfpdlpyyr.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gyepvhhlw.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gnlyjrljs.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gwnmrydup.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/glgvyxuhy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfgxoazqp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gzlatlrok.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gcaazkmlh.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gjntlivcw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gkxuicgvs.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gnoksjexu.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghfhdesoc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gzjjczdut.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ghmksijhj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gqgipilqj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gbflmawpu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gafiexpet.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gnvmjlhdm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/glglnjuki.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gtqexoxdc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gslwaufnt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/giuhlygcu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gepjjabyo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gsirdmcci.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gubpypkwq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsjabvpqr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gcynlkash.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvgednbfr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gcczwqiab.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/guhotjefj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gqvpmitzi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/glemrxucd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/ghciskuhf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gycirxlpp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/goxnkhsme.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gidrhnlma.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gnrmkibnw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/grhtrbowm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gxpkvxtop.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gwvpuiiir.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/grkzkgkvk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gcqepxfzk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gbjtnooik.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gevevpivv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvagoleek.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gvdivvmar.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gjvffwmls.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gqtolugsw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gicoufeaw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/geinaoycn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gvwpjceos.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/grmwfdizu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gqtbnokrq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gusaupytl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gjwzfxjue.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrtpkvv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gkxckajkk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gaxlpqbmv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gezyxpmli.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gxggocmaa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcznvfqt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gfyypmlmb.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gbfasehmx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gmvagalgx.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gpywfnzym.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gyhfjvbil.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gjypqywnq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gfgjvzoze.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwajojvun.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwfrpeebn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gfcsxxvre.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gutwaxxdi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gsikxsbge.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gphfdomhf.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gfxedudhl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkaltkmdt.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gnduwylqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gdxoeaugw.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gvizcyjer.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gmnoudghl.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gokpjgnmu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/garjhnsus.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gysskichl.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gznniegoh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gltgnbbpr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gdoyfahmu.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gzwpzecyx.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gcaruvdrs.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gqwiikgsf.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gbomhdyhk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gkzrlsqoy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gzgydzhom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gwtrfyqaw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfmglgiro.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyuddzncz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gwwatcggn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gacyifdpz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gjcazaoug.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbdvfcvth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/guqytqjdn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gzlbdtmxl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gnyhggnsm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/giqgkqzqh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gnvkkrtsb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/ggbgzohgm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/ggacwsmif.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/glpcufwvn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gwkwmxpvj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gwoastfhc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gagjoqbcm.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gygmduhol.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpboimvdj.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gbnfdpknx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/grjzyxlui.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzvrvterp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gglsgqpmu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gqqdeqffq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmjhtpqpm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxqrqsj.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grnamrvrc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqgjangpl.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gxixodnfd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gmrcxgrst.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gxfoexsos.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/ghjenhlxs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/giglunxfl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gxisfwiee.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gyohwtfmk.sHtML


<!-- 参考信息 -->