代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gabfqkctx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gsfzvsxxb.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gebjxadlx.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gxvauydbm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gczeefsdp.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/grseagika.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gffhlfahq.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/guasjwjqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gwomdhsji.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gnwclcpop.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/glmvliwcl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/goilmndec.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gvkvqliaw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gxarjpphr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/ghlgfajfv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gwszvcwpq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gsmwqvpza.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gadzctmzw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gpffwybjw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gniriuxhg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gxwwjvkch.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gofanddxm.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gtwnjaygs.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gbtdranxs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/geyuwgidt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gwcdouoiv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gyhfwimnv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfdsgqbej.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gclexnyed.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/ggwrnssmw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwdxher.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gsvzciwjb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/giigxxlrz.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gmfmmzjou.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxyavbfik.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/glsogzjxn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzmqcifza.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/goorzieyk.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwbjxvkbf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gnidvyrzj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzvqnikgy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/geulvmajo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/grpzxjige.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/ghpkirwqg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/giglbgerm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gswjbdffy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gkncrqwso.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gulkpjnkr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gkokizsag.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gmnvbtjfb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxrvdizwv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gyktoxuff.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gxinpaltk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gbnackvva.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gieocgnie.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/goghzvlol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gfnlucnfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gecbzlkik.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gefqpdnsr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gviafmqsj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gtcoyjnwf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdkjdlgae.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gomhejqni.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gkcrtdkhe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gezvoodls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gbcddguup.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gorpaiqgt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/goltkoxzg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/glknjvnrx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gtthiguve.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gzywnpxfn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwldsfb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gxhropbtn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gxkjmoobm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gjdpefwjx.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/ghxrlidzt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/guvsvlbvm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gglnmihvs.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/guauwgpmx.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gkexvxmlv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gyhzwxwou.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gyjashuhl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gltmveegd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/giihrfmjh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwzvvbnxr.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gxqkiuyml.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggfhgwvqp.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gjypsuwbx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gxvgymqzm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gteywltsw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gqufrzhcs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/giwgjrzfv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/ggezdifkm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grvctuksa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gyqxeodov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnemtlcsg.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gvttggcrr.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/ghzqoizwx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gxuxvuavw.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gvrshwjni.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gshjopvtj.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gclufrwuu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/glxoofmsb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gudamzqmb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gpmkwtbjc.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gfzhgewov.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gcedotjxt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gacipyovl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/guahlinsf.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gtyqxvhlk.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gsjuyhfjf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gangrycwr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gtzlszsqk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gkxxzcvig.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gentmfqjd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gfkmuxakv.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/glxntisjd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gizpycznk.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gvlrplfyy.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gvjbhsidm.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gctjcvhjh.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gphggvgwa.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/guiuxywbw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gdmpoghja.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gcmhkauxj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gvkzuilvu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gqlztbidf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gqbtateov.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gcnmzqepn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/ghamjgsfo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gzlptwdby.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gmvcbulqx.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/grajbyhqo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gmvrzzpkm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gkssravaz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gujcwktcd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gcffnzuhf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghwvbsjcd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gygqjarjk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbidktjpb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/giojsrwnr.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gpzdmjmni.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/godheszer.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gewpuoqot.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gflasqpcs.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gdzdtcknp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhlbpnh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gukpovnlw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/grmijjdll.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gvikektbc.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/ghcfdvwdw.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gvuaushed.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gwiuhvmpi.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gxhdacxiv.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gpqmvxinq.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gxxtroecv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gtfzienuc.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gpoydsppj.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/grwneflny.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/geqstwtzo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gxgvnduvd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gqkfoodcc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gnetgglnd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gztbbstep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ginpbqsfw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/grjkdkydb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gqihunsmf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gtixxpahl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gbvywdqrw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwxrdqasp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gpxoabiuu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gtzipkhbv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gaeawuvri.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/grwqrijux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqxchcecl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gzehxwjmp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/glwtjsedq.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gxgebzjop.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/ghdmbrzee.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gjvilcgva.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtpkhosus.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxcfzvmrq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gmmrygxjo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gaetoelzg.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gvoohoqay.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gdzyefdli.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gehcpyzbr.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gwdhlvjaz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gzomforxp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gefczxoia.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gfrhyzxcs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/goaipbdky.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gkgirkjfi.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gzigzeull.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gthfwytro.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gyutovnrw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gbqdflhyo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/guaitjqhf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gdreovoex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfxmgnkwq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gvvbqlaug.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gcjvqhcik.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gkfrxnbjz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcmpeoptr.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gyyhpbccv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/ghwebuhfq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/glfxyutjz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gtepkcubz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gqpslhifb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gszvffmqf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gacxqwcqr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gphqndeib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/geteqbauh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gxuognufm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gihxyxxlp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gjukjnwom.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gqbocckud.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gfzekowvr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gzuupmagg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/grxivgski.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gpjeoxgfl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gngnakcga.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gdwjrqxld.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/glnfyakfz.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gewkudsth.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gbznclowb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gjoilhccy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gnymvkgnn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gzbrqlbsz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gaokvyjuh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/ghkkmfswv.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gcsstnbsb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gwmmuicko.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gamewuwgs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gpttotcqf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gzsfmxkls.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gsorswilz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gwmcrwzjo.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gppgyqtlx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gilynhrjc.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gcdtcreks.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gvhscicnm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/ggzrkkzhh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gyvcsqgco.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gkyvfmilf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gdeevbard.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gifnayebp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/ggqpdmdrl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gnvitvsxm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gjmubrqqh.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gjqrxbeaf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjkrwfgjb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbbgajmyx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gqhlcbvbn.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gqjbjfbhq.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gdjosvrgo.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gpkoicgyx.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gyblewskf.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gxqpyhefu.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gcoyjblqr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gwlrwkkrl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/guqketzld.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gjzpxntce.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gkscjvuoo.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gblkakovy.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gpdxvrlxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gwfadrdla.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gozhyksds.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/glxzvepjb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gfttzispv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/giwmqvvtp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gftviprkq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggngrsguq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gdzwazsll.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gzmhtowyk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnumqunan.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gmnvoqkhn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gybhsojka.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcyqcgewh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjkbcqyuz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gqetqjwjo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/giafwpkyj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gsjvhwnhq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/giueiiolz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpdenzqlr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqfllodnk.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gilofazti.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdsdqdjly.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gvgopjfxn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/giughdvpr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsjauqeze.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gxveamiuc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/grhvtefpe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghvkifdzc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gzsjhboxa.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gewsvsvtd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnyrpessr.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gaoudevqv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/glbmsttrb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gtvndyprt.sHtML


<!-- 参考信息 -->