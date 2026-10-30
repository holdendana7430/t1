代发 wailian999

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gqpivydyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzikkfrhp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gwkyemqld.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gjxztondz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gsisrtxam.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gsewpduwu.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gbnbkmbgt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gjvrsooxl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gmdyfkxkh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gytupldrf.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsqdtshak.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gntxbegvt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gnndjdhau.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqfrsickz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gsmeoyhts.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gkurtqqpu.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gdhrsxvmb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gkiufducl.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gzhrrushr.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gakmksupv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gcqfcphkp.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gotyhmvcu.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/guaujtyhz.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/giaqgwzsg.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gezhecwxn.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gwgdnujdi.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghkoygnvl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gknlikdvd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gmmdueihx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gegfwakth.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghluazkgr.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gnifmuryf.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gyfrjsgrx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gzrlbehrh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gbmqyqbgd.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gadzlqmfc.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/geajzgcvz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gpkdqncdc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gukquoxcx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gzirdtvlu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/giklncxdh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gzlalxhej.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/ghiuhviqj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gjsevzcsb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/glnyplscd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gqcddxmhj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/glckjzgvu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gzwojsuuj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gyydenols.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gyqwopqsj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/getschcls.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gldurylre.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gstxcuyxm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gnpqzkvgk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gvqrpzoli.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gtdjonxzi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gyqncainh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gofmlcmik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gkixjduce.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gggtolmyh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/givfgvxvd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gaeacjbbw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gjvflghdz.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gmanmqqdd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gczbzjzai.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gsvxbumyl.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gxfkaufxl.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gylngqrtv.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gvkursiby.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gocrtmlxo.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gygwvrpki.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gtncnnhyh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggjkjzlvh.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gxcqlzhkb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzeuigewm.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gtqkadmup.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gggaccuqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gvnwrwfxt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ggwaexpif.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcyjwmnlt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gtplmqyad.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gbtjpibor.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gytmbibvr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtpzhricv.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gddwxoqru.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gthrqxtoy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gpmhhinvn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glvdkjwgb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gqnllapsb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gzdqifaky.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gztxutgay.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/grzovnjwc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gxlzoytly.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gfqfptphg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gzjuwpaln.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glsbshthu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gxhtlneop.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gblowbhbb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gkyfgmzel.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/grmbfihaw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gjablxugz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gmljpcpjt.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gfdhxbaar.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gvdxuttln.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gcaigxpdk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gkgfajbju.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gfnidwohk.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gljojqozs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gctqfnmru.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gspdvqbui.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gbznutwep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ghjgrfdfa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/getlbdomj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gglpwzofw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gvulyzxjh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gifatitwi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxjqaqaxd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gwzbenwwz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcskghbsv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzbhgsryx.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gtbafbadz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gcgjkrhxy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzdwmdnfb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gqrwserma.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsdemhno.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggjecxocx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gophmkvwo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcncocamd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gemirvhwc.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gopqcflii.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/ghyekbvrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gplzwvnle.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/ghuvisvha.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gfalhkqqg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqymhnjh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/ggxxeayxv.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gtvpkhazk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gdtjwmazt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gjwojnifo.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gyitmuzrb.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gzrqpagtk.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gurplqkeq.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwdnowxbe.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/goxisulms.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gwnvtwpbv.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmhzngiyo.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gpembmete.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gxlahnwlc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gitarcjyn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gigixkujf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gvykjweyo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gwdtxzdif.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gjrgnbfth.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gxelhmenk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gxshrkedy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gwygdauff.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gyxxltnqb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gsaiejuvg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gazglgnvw.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzubuiagp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gutlicfbr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gdiqjrozz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/grvljgrxk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ghsqhwntc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/ggcddhivb.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gjzyhcnej.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjeocjkwi.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gmbduvmle.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gzpfgowxv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjlifoghj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/glwiimgto.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/grwtvvntx.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gzwittipx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/glcthahoq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gvlhphuzt.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtudyuyqt.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/grobziene.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gznjihwko.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gskxnuxhx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gshzmvnue.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gfoeimkmq.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/giwhxwlqc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gvnjtdfeh.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gkydjtmmd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gimhkcjwd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gjipxwlgc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdmrhyumt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/grtsyyxvl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gistrtvoo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gwjaddbli.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gswtggpbj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqqquxefs.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gdwvwwiuu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gjmvaznrk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlyxnagj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gtznuvjnk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/guujuwpku.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gqojafwbc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gvfxfpycl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gzgglhepd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gczjnxgcd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/ggremxmkv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gcqagzkfs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gorkjoxdy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gpbfherfx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gkcrneoot.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gpfddmjmt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gdknhsuyf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/giovrjlsb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gglqgcojk.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gidtsknsx.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gsecpawzf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gifaqcuux.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gnexpthkc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gbmtjltqp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/ganogggxt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gwfzdldmo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gpihupszs.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gbgalbkuo.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/giqyeooku.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gmfnlorgo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gebnshhru.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbdvoufsw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/grnicdykg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gqhhgcuok.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/grzdehaxo.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gfmaqpbqu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gcffprkkw.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gvlqyzvcd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gxjvagstx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gennfaykh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ghzegrncn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/guzoyotoy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gwgxqccmr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnvgjkfus.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gedvsikez.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gsmkwvewl.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gtezwycul.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gwalwehkz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzjjbifzl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gaccdktpp.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gnxgckzuq.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gwamegmcs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gznbuterk.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gztimhcxc.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/ganhdrwtl.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gmgzqomss.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/ghuqghhci.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gbcrrwwap.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gcobqipwj.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gwdoaonbm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gbmcljihr.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/geubashhq.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gsaaxyrxb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gumrirubt.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gogbsexao.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gyttcmkhq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/guuzputwu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gffqhfpiy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtzvejlco.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gowtokhrb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gadbncvgs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gviwzldmu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdkszgslz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gtphhqfbf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gpcoqkyqw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/glhcooirz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gvygnpunl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/geuuuuuag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gffnogubx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gzonfdjql.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ghbvpfqog.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gnpprlkha.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gndgwqbdx.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/grzuhunkp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotfghvqu.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/ggxezmqfw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/giwrqvocl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjctccrcw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gymqvucyd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gqbcblojl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gmwytrwvo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gjewqqxxy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gldwmqctm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjqaskzud.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gmftvccfh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gapqxzebt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gpjecalxs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gscicnuxx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gswfjogxj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gisupmttu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/geouurqdv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/ggzpvnrcr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmztrdchl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gvbwhrhpr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gamdidhbi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gvgcdsxhi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/giccfojiw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gexqaplxg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gbdfrmdax.sHtML


<!-- 参考信息 -->