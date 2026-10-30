代发 wailian999

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gezyyuvih.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gtthdjnpl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ghjmefseg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/ghwkkfvjo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ghcgheeev.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gjfpkffzx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gwblnmyiw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gfljbftam.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gcqxtqkyw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/glrmhzeqd.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsafuswgr.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/grhzyzwdz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gqmfawfee.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gvkdratgz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gubchmgax.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gxfeulmmt.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gzmoliexz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gtmxlwjji.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gkvrmzvqk.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gqmroxqgr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/giohykscq.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gaqewdqyl.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gavybmdwi.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gfupwcdey.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gregzawvp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gdizfbdmz.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gqqvmpsec.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/ghbkzggdq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtnxyxdnp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gwctnktdm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtmewdhlk.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gdwodufrw.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/guecpqogm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gawomjlno.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gitutreff.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gtfnsntgx.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/galzfymcq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gelwsjrga.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkzwjifag.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjhgsklnu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gsheiwkwz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gvpbkmghw.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gzkwrxhnl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gcsdxovkj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/ggrcsqmlv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gvoqrrpee.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gkbevnaog.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gizfvditq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gerbnbpix.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/goamedmrq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/ghoxazsgx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gtzcdzgjc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gokzdrqcj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gifvtvaer.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/ghlxsyknl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gsqbdjhue.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gefojpggl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gkbtmwuhg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gzcebbmsb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/geaswpyas.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gbwvkbrkc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/grccuwwea.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gawpijrcd.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gatenintc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxnkkozdg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghwxdkkfk.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gossiixxw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqhusoo.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gflnozidh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gdibugtvw.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkbwzuijb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbsfpmofk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gydnrrbnj.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gbyberuvr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvvxdosua.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/grcupmmxb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gqljxwzrj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gqyegsnmf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gjpgrtnkj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gydabbhqr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gqsrjoxsx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/ggjgnnswz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gqxtpcupa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvlhshfpp.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvdctfptr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghishzvuq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gkqjpsaan.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gnnsskxki.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gdognymsp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gdfxoahga.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gkdshljyc.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gcjmdekoz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gplrmutyw.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/grgnhhqba.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/goykbinau.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gifuzvcsa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gjmbcefsm.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gwnubahhu.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gbqiotoao.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/ggprqymij.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/giwajbndk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/ggfiqruyy.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gkcqbrzxa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/goejujuoc.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gfwngqfgw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gesgvetrp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gqkocjmtz.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ggupotyvd.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gnjosripl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gosnvxjof.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gsjoslyaq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gqxrcwwvx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gdmmgbica.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gtvomrpmc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghhvuanky.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/glsvjbyuz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsxpatopq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gktscuesq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gaufjwteh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcvvachxd.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gvkxasare.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/ggltyuerq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gkfbabeuq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzjpisrbv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcvkawsjy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/garhxbstt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwevttdci.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzfizrjtv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gqouyavxp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gyboowlsv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gceghknln.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gpgsifaqn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gciekzwln.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gvpnsqinx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkpriads.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gjejdrumo.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gjhlvfcoo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/giosiuxau.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gquezadgg.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/glucpunsl.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/guuykusea.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gstdhbezn.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gxqttbbgh.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/ggectjqpu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gsxynmqby.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/grjyceifq.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gqzlztcro.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gthgmkgew.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gexooqgul.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gqutisbvp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gpuocrasi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gjaxyaudd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gjlqtdgat.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gbzbiwpvv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtznbikwi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gwgyixzig.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gimdrctwn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/garhhqyyp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gammydtqm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gmirlkzqr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkigmpxuj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gkguakwuo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gcypbjjay.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gbumgvwrz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gdyzghnul.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gphhywjjb.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/grqbyenec.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gquvijipb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcltkzyut.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnfsukcym.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/ghrvqdvow.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gajbofcyl.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gkkkdskmr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/geolhaopf.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gduzechvj.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gmticxrjl.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gmllypidb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gdzhuduql.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gqhvbpzgz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gknghatce.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gijdpdrgm.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gznjabeab.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/girfaoudk.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gpqznmrlu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/ghulrwzxk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/govqdxgmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxchxqhvs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gslaixxrs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/glqozbzwf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gnbisdbxo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gfpxkmmal.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gsjlcljqw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gzjztqpdc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/grzxjyydu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gxrqyzmcl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gvlgbhgjy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gougsfsyt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtrryyqzx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/ggabcqoqm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/genszwiqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gtvausznv.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/grpgizpcd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gfsjbetek.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gegktydxe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/guappsqax.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/guxgwxdwu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gevmeorga.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gosugvkdz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gkbsvfgdi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gczyumoye.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gcftggrsy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gckgqxulb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gkjreveod.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpyafwqwb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gktlirtqy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gcurioicb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gdpgwjjtk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gifywluaf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/ggiaqqbpq.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gntkynrnn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gyskfckzs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/giiozibwi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gwugbgltn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaolivuiz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gpvcfiguh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/ggfddyrbq.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gewamrgnv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gvexxopqb.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/ghudirafy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gyrezqtui.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/giqyoydmd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gpoycmriq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gdneyftyp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grigdeplb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnerdwahn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gwwvpoufi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gtutfaugs.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/grwdytfvd.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/goeiyuvco.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gawbsbzei.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/geulpoyyq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gifgdelod.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gayxuebzz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gharhqows.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/grjjxpqvz.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gybzeapae.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gbhsohlhy.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gpdsbrosw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gxyaksmlk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/grelpusbi.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gjqaoxfst.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gslmembyp.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gsjuupwnx.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gwxsvvpiw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gpzahawad.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gymdyfsam.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gubwmnors.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghmarbgxb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjqrsxqnn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxilosnfk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gtuayaxlp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gluehvqdl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gglxrvnfo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghvebkzug.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gqnyeqjtn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/glrpddriv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/glfxdssff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gfvdmhwnz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcnineocu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gqjcpndwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gbgzlwcar.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gvxqxpghl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gqcmdpslr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvwsocawu.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gqhbhqwxj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gticefzvm.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gomzbukjd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/ghoaqqyte.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxwajykhe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gxkxiwlve.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gynkegtaj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsbptaglc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gouwluqwk.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpecqkexc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvytltjxs.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gwuwxdmis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/ghynaxlxb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gyxexljyw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guxrfxtzc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gjklzophy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grklrukul.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gxmdvrkbd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gaclcdztc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/ghkqfqzya.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gkhngnplf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gyhqrldjc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gxhhgmfqv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtyffnnha.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gbkgtbvbo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gecogxwvo.sHtML


<!-- 参考信息 -->