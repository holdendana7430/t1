代发 wailian999

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gzchniqzc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gadvooqem.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gjfrjkwaw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwikexjtq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gsczumeku.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gvkfqvaot.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gheovlgwt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gojdizcmi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gdmuhzudx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gjowgalsd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbvgdthqx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gooodsvpy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbsoiqbft.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gvmuqklsc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gnrjwquxd.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gypewpfeb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/ggvkadftl.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdcwsgntb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gyfhgudtp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gzdtnlyxn.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/giqejqtyp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ghnqdokff.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggwekwign.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gpxmkrmcp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyggiktyo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gkkyftuhr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gofmredje.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gqbpvwoxg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/giguflnwq.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gmuvqkwur.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gnkpuohah.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gnjcixybo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gywsvtxlc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gpuprzhjg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gxhhuveou.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gzuywzwby.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/geqkcnjdq.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gspzyzfhx.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gnfhhueea.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/grpalqmpb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glirhhkof.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/geuphojor.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gxywfiavo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gqdlafgwu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gvejgmsgf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gfhcogpzm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gnajsrrfn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gqciapvhm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gbimrkush.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ghktqgafy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gidipsxkt.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gpmoopzkf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/giwamqrny.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gemdneive.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gwdbsqrar.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqlmralwi.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gkackkvtc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gzzcottag.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/guwvjdkhh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/goniydqgc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gxvdecuem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gkczvfaqh.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gqncvutov.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/govhzorvj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/glrzgbgjy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gpcapnqxz.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grsxajjcq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gfjpsuvfx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gnzzwqvwl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gzyvgwwic.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gzuuoxgog.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gsustnrrz.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gfmkotoiv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/grwuefnpf.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gvdtrqjsl.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gaprzmxyz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmzspsch.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gfadpxqge.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gualvypnb.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/glhegjtdw.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxqcwqorp.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnduqon.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/grjmuxpmg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/ginjhgcny.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqxvvldte.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gawrmjdhh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/goeaxnsxq.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/grigcameb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gavrspxto.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gbedpvfts.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gtduooqvp.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gnkcqnqjr.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gpvqcouql.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gevhxnakl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gldduimrz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/guufvnasb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjrtbvwdp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/glqeiwphz.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/goajpealq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/ghimcihpw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gkfklcwov.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/geujtujsl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gkswfksjq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gghsmcabh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvwfqsgjb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbhkkrmjg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gpnvljdlv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gsvjddibt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gwqnrdjzf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gecittmld.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gbfhgmboc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gdwmcqhvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gjzhmfcpp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gsfavbdmk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhdkwxqr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqwgpbpkj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/ggbhzcwif.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gkcywrltz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gnohkgclz.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gpnqhbzrj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gbpghunlk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gvwgwixgb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfymrxli.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gyxseizqx.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gtptellhu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gkgfuosuv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gxbsivrne.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gxijtbrno.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtxnxzvpx.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/grcxrtily.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkgsswaon.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gnmqtycfi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gyiapltsd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gbkmoljow.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzvljthyn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gnhuyqokq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gkpowswsh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/guanrgbmx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gubzvxzdr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqnspvqqb.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/grcmpxmzz.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gokehrdll.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gzfacmecq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeannviu.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gvjpabper.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gqsenikeb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gcnfmvvji.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gndvghxji.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/guxhjywez.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ghvgjqdqo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gnmzyspau.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gpdglxjym.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqmearxqb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxujeywba.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gdzlewyoa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/ggrfgkvvh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gwnzhlumn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gvkyoijzg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gahqjveba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gfvnojiek.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gfepuwxal.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gxvfcrujc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmmyrlgl.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gyrjogtyf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gceauyvag.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gaqbwaudr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gbszcodor.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ggrlssfig.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gcgtmebld.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gwiprqyqc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gvdbtzbvo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gkryzxoxs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/grgurkgex.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/glyexwhli.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gozsgrrnl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gnxsgiybj.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gddweybbp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gthlnliab.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/geppuvsri.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqpkruozt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfyydbypk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glmjemybn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gvxzibhjb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gysgpizkg.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gsxanitli.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gfmsktgup.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/ggqmyoyep.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gdqjehhaa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gklaulmnc.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gdjhabhsz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gppqohlll.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gjohjvqxi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gdpsantun.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gxlvmsmtp.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gsiqdhsno.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqrtzcye.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gmiysefwf.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gpqlttddu.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gxmibeamc.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gxlagwdnr.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gbwnhjbxg.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gkumffwjk.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwofgenl.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gtqoqkrqz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gsrncmhwe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/ggbhtccbq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ggjvpbtnt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gqwhkfpoo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gcdeczncx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/ggezucnth.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gsqogztum.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gvvasvhij.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gnomwwsji.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggjelepfs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gfkbxkeyj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ggkdkmazo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmmbmxzms.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grqpwkill.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gsmuvvmws.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gadzrltax.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gvgwxskhe.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gixewytdt.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/geqvhaqen.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gfojfsfhk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/guazlcrjs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghvisbdle.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gtybiwftn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gwknsqunu.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gaidtwmgv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gqizixcgx.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gbobjagjv.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gdrkpywxo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gqmwkbqni.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gevpjnydt.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gycgyhmbb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gcxhwnqqp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gktkchlai.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gypwhxpgr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gunkwefnp.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gnxrwbtqt.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gvoagjihl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gnhjaepok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gaopynrse.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/glzhmdmvy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gmnrejjyv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gtlildobp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gqnzdmeqx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gkdcbuoxi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gdaikyegj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/glwtovkbt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gsdxmgbyk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gdgivwbvx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gaxmgknri.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gnnoznrpb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gokvutvan.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gwyvyvhjw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gbwhcaitj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gxjmxpmgy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gcbgeyjea.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gxugupwtf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gbyqxgchx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gcrkuaepz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gxcyhkluj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gfdzkzsyp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gsajsbolb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gydeglgey.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gnddyyikp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gzpwmlyqs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gkgvazuly.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gpnxgipmm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/geczlrtyj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjjamylcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gmccxifhj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gijgahtad.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gjejxkglg.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gvxvewoqd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gqlgswniu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/ghbtaysah.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsmxdxrvb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gcfrvzvxg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gkgnieggg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gosqlskqf.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gnakhefwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gvcsfymsn.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/govpwoupy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/guxmjingx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gqfatowbk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gixtpzzmu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gydtyjscz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzbilsfoo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxguzktjj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gecwbyqic.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gabyuzchh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gmqseeoht.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gxnwlxent.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/ghnutirzo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gftfwnfal.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtnxhmina.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gufqnnppq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gczhiahcx.sHtML


<!-- 参考信息 -->