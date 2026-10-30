代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gqfbznyma.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gvieaflgi.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gdqhyugqs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gvriatyea.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/ggnorsrgc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/glknzzqiq.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gribhzxcc.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gnzwnabft.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gwaqzdrhm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/ghexdkrts.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gcuylrzjh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gmymrttgg.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gnvywkjnl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gzkzdmcnb.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gjrgmlhmz.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/grngmxndo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gpzgtwxmn.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gminkvzpp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvhsxaucq.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpzqyvkkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxlcatami.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gllxvmvqp.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gtzmhcmsm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gcnawkqhe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gpnmdswws.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/garsruucu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gbtorqkck.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gnejeiozg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzvdjkdvq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gzjhsxuhz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gdqlejwxm.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gsrietpzh.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gjeykrgbw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gurjodmhv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/ghonfpkem.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gehbxtpme.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gpvozcsfo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/goiizflpy.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/ggtdmsjjn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gdgpctwch.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gvardsbbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gvunzskkj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/geptdbvyi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gywilcwpv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gazamdffx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gupykzdwj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gscsupchd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gxrimmvnb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gnykdvwrz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gacelavoa.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gorxabkxd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gratfeupd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gkdfqcavo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gominueqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gihfuabur.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaylxwdpl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtoikqz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbofbfk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/geysumwej.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gototuktk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gmxffhnpr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gjibyycuv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gvbdnimoz.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqadzsorz.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gjuyermef.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gslpjzmgg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gpcpzybas.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gsnjovrtd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzmhkesou.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gchdyxnro.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grzkjnite.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gcmzjkkhw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gplqlvply.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gngllfztx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gavvnojcv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gdmxoouhq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gexfhlptx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gunpwonqy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/geyudhfev.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/ggarxrnfl.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gnwtknmzr.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gvyrxdgof.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/giaqzkhxt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gugcftulr.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grixpesew.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gfhvgytjo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gmeevctan.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/grsezlphq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gbluphiei.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gnzswpstp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gzatpfvpi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gsifzefjm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gssnmwuau.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gxhyduoxu.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gurwqijrb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gbsgrimwn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gudpvxjhq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gbysrnwme.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gmamxzlgu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gemzzgotf.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gxcwgcflr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gpolnmsxh.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gsfsugsvd.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gbotvsqrk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gdxcfhqzr.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/ggbezsrpd.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gzcybiueo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gnrwritsf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/goexpgigv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gmciixtta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/glwbnyicx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtthssusp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiuiokqn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gpdkcmmvk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/ginnezhqn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gdudtdcvo.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gtmjpjxtd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gawynvnvj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gxjtrgwfe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gufzujvxo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyzrqalij.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghyvymmrc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gjeyunhby.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvymmykub.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmtsubbvx.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gynaxjtgm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/geakqyrrf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsuvctlle.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gbcrxirpk.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gzhpgrrbx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gbaqkuoet.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gvqjciyhy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/guehxuakq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gshgidbxf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gdzscsxxc.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gtlsrscqi.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/glqrsptpg.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gqxrjyvkr.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gzalcesmo.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gunozmzxy.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gaoldyrli.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gnhdgvwba.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gigfuumwi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gnmshefmj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gaflkuifc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gnyhxvwss.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gtenumvgi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/grgdaijrn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gdqwvkzzz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gcuxigxik.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gaqzpytvj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gkiwsnoji.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gvlyerbem.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gaeuskhcu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gzdbspujq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gxiduvsrt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gakixqwyr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdmkyozrz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gkdujeleh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gooiwjspk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gcklkrphv.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ghnosumox.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gsanecchl.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gpmtfzizp.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gcbwjevtb.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gozlddjxf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/ghgniyeut.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxhcjcmtm.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gefqyvlgh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gwckshvck.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gcjsipkis.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gdzjbyzgh.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gpvluvabj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gorisglqp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gngdsdgur.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gzfwygwve.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gxupkyxmr.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gdhsxarly.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gyvvpsasx.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gjbiptqft.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gdwjfeian.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ghgxpdkvv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/grdkxfheu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gugeyboop.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkpqorugb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gouekwhmy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gaoicngck.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfelzbpft.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gilmknnuv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/ghsadjxrc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gtcayonex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gktbpbnyw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gunqvjpxa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gxhthisbf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gcruapqmw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gbgpobbkm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gvbyrhlff.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gyrvzkgwx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gatrpmoqz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gphyjguhm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gxodlcsae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gmcjisunr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/ghxloklaf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gerbykhlz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gqelfhaqe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gbkgqjrpr.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/ggzxuhend.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gypzzlyzg.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/ggeeywmvy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/ggfpajowd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gtkerlhvb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gxjlxeqsz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gqiieeent.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/glkrjarpl.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gwputpzol.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/ghkodxpcp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gapasivjc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gzofjtmwb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gevujsedd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ggjxsxoiy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gufqepajx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gkznewkrp.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gpxwjmvfg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gzpirceun.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/glukxobzt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gzmowaiqh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/giywpqfht.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gghotvttc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gphgtekzm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwmsiqttk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkblvjlpx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gutgpjrot.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/ggvrtxgkj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gnrourjaj.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gpskmznjd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtujipspm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/griqhhfag.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gmlwlhyrj.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gdasqlcbm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gzpnbsrjl.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/ghmwpvsfz.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gkfokvogv.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gybxrqooh.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/grhvnmubh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gconjfpug.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqgmijfaa.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gvriitkzu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ghoubgyyp.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gujbdqxpt.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gmuqadagp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gpxycbbge.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/glriopjue.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gtnlewsaz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/ggqskpili.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvxtzzsvx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwqwgwuey.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gajrlqtfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gdfkuiyww.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/guqjfcnxd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqxdmxoij.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gpxdnsfio.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmnzlgnap.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gkabdpsjc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gutfmtfjt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gedocjgpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gaberwgqt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gacdfkzhu.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gtdetwejl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gorvkoxsj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggsuxugar.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gcavwgxah.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grwuhnjik.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gwkupuvcg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/grcxlrfve.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gilhqtswj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtalfcyyx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gatspzccg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gljuyvhyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gcxmrkewe.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guapgezgk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gavsomaun.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/giaytglib.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/garbdwoaj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/grywikpkg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gzhaogueb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gfehmzjwy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gkoksnzxu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gcqhytbym.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfqfsssn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gbefurbji.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gokezqtyd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gyfmkymce.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmrwmpqpd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gntosmcps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gglrjjvag.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gdnqmtbzz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gzrnrnyhm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/guikbcbra.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gjugzdgmp.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gtgvgxbgu.sHtML


<!-- 参考信息 -->