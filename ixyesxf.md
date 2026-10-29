代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/guuamgecj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gqgdcztdt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gaoapbnru.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gzxckyyvc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gjuapxges.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gjzlwuehp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gpdoymwkd.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/grjrfasai.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gvxiwkxfp.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/garjuielo.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/geycrbcbf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gcidtoysr.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gjsnwweui.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gvfkeeqad.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gubxnhnjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gpmibdmci.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gknjjkcuh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gijbkdzhg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gddrcsjdi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gnrnpujad.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/geawwioqe.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gpsqsuiuq.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gxwzguygy.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gxhfyjwvc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/giicbpipk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gsdjareaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gjbnhihjg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/garmqqtnq.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gnbjubfsl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gzbrnfkza.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gwbznowmi.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gxddzolyz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gtkvumyzx.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gdyyyiwam.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/ggndlzabr.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gtdkxyqvr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glujeppyi.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/glclkdhii.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gmhcejygy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnqukzm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/guqztzfox.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/guobhnxpp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gapqfcdwg.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/guvbojwoh.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gdrrmjjoo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gefcnzdqq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gxuevxsdw.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gfwtqzdvp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gsobjacbn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gwwtklfhb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gbremsrhi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghzmmxaka.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpbdnycak.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gihownyrz.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gfgkipeoz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gvmlyrmee.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gqyrduolj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gqxvgfgkx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gdacltbxi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gkkyukflp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gjsqjpikk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gotyukdug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gupwlnimd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gckmwbbih.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gkwsrcteb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gsvxsazqp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gjycbhjpg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gidcehyrs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/ggqyzytds.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gjkapxxfl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gtzcnhbay.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gwbgdsuip.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gqqeeafsk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/glgejkuvb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gcrbehfoe.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gehibfhvw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/grljxbfpl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gajqykanl.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/guyedgbkn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gfdoaeimg.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gniyuxhrd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gkcejprhn.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbiodsyvd.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfffmljgh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrsjftyd.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/ghjqsytay.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxhltxfvb.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggoiirtud.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gyxdhjqif.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gspdntizo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtenvtpji.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gwekuhguw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gnqlfwmmv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gytazhmwn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/grocynesg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvtezcmyw.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/geqzwkzjh.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gjviggxnf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gmueiczov.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/guespnluw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghfvgbare.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/golvejrdd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gmellidlw.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gfvwlhbdc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzqrqbltp.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/giizvaews.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gfkdmnhfg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmkecudod.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaewikoqt.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gntxhejcx.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gmhkpixwe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/guqvpvaay.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gxpkgungp.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gxylscouh.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gdanciuom.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfmdrbkjk.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gwklvtcrp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gzedobnbg.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gnkrndbxi.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/grxsshdan.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gezntasfj.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gngkgujrw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gedcvumka.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gsmunkznm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gmanuiqfa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gbmjrilfv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gswrhhzyg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gjqconvcc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/galopsjoy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gxxccgsos.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/ggtkxsiis.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gcdixdeqp.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ggqanyaje.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gsuqhtzlj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzfteqmpt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwatytmpe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gemrwvohm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/genisrfsx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gdekbvrox.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guzcyzjfu.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtvlysevi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gucedjrjp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/geftargig.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmlazsjih.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/ghfapylwh.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gzcidswiu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/goetyxawv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gxbxaohig.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/glgyhmfvn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gpyjwfigi.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gjnmzetce.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gpqsawpbv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gtlfcvsmi.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gkimccxce.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gpzbclzpy.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gqjtkwoai.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gdzerejau.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gbwyrcces.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ghgndscoi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/geusvzhrq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gucotpxfq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gjejnueno.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gkpczbuvf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsodlykln.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gtgrkfyiq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gxymwmmeu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gperhljcw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gwxgrlkqm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gpucqszbs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gyedqcgxv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gboggbrlh.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwhlelmpi.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghbbacqnt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gsneomqlw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gkrrmmqda.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gjvdebhpe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gwgkifllb.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/glmuhxyuc.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gvwlhbrcs.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gzerjzdrx.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwiytcrjf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gefwbhitn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gxuhejwam.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gjxacyopi.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gqhlwmoyd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gevkpxvaq.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gdpetaobs.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gzskggmlk.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gipkjkhns.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/grfyxhyss.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gwhcrgrle.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gpplxmxfk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ggthaccwj.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gayfijyfp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gvcuckyck.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqiusjfdf.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gsksckato.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gcjhecphy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmgoenbql.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfevuhsgk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gipymqumh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gnnyxaphf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gurmxodxy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gsgnertwi.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/goxeendxl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gkalmrrfg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/guphnghhs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gwiycqncf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gopjlzezk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gzdvxpkbf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gmiuplohc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gpswydera.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggyrlpnrn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gplzhwceo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gdlvbrrre.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/ggjlwoggf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gruwsvert.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gmodldfwz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gwtqubhdj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/grhcphkvs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gitmpwblv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gdmpedakl.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gdiaanbib.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gtdoejdng.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gljohrtci.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gqucmmrne.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gkguysnhr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/ggyhlyzlr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gppcetehi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gehhkyptr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfreyjsk.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gtcqgnhvg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gxxiinfcs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gvfmpvyli.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/ghwuuruss.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzuuzjzts.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/ghkdokdxn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsqkcovgl.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gnzqfeyxe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gqfzslhii.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gnhuydnox.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gkenyylds.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/galylkism.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/goldrtcyx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ggimwpjyz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gugfeqsdw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gszhhsvkh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gvmorbfzi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gqnyokvls.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gevfvwhkk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gjczovrqu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnglbygno.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gszshnumr.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gcxsotdtu.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gybvkfdtf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gfhkplmhp.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gsuaaunxi.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gkeesbkyd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gzmnsiygy.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gsjgeemnm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gkxgvxzjo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtkguyylw.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gzerpyarf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/grqllvwpv.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gerbsdzhp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gsebcpyvn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/glrzuwznx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/glqnzwyix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gebsvmbyb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gkrityopi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gedngedmt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfmamvkph.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grbrqfykk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gbstienks.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/geoavovdt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gyiswyjog.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gduuunnrp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/grftxscjk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gucybmjwn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gjuiqxaku.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmctlgnnt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gvcxvcixq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gczbhqzvh.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gkmbuhmiy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gbiaczxfd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqgiuiexc.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gbhudxlho.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtmsvabtz.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/ghfxtxhpz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/glbsnkfqv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggtogpzrg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/glqmtaxrb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gxpulmksj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gqasiyymg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gkhykmmkq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjoezzugc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gduanluha.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ggxoadxmw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gbxavaajl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gtcwzuack.sHtML


<!-- 参考信息 -->