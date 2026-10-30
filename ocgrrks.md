代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/grnehdqrz.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/ghusebjbx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gyhvhoyqu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gaucbquuc.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gyppupxzx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gzskkuufk.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnzndyjgh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gyhwpnxok.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gkmaveqsc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gsxfribha.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gjayjhzcs.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gnmzxyyqd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gaymfmuxv.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/govhzwnot.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/guojjhgca.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gohfayovc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gqjahhrtf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gtynyxzrp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gdzdlkzzt.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/guzbguals.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gekiuuajx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gvqgdenvs.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gmpfehvxg.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gzkrgfgux.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/ggehhupeb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gaaodgztg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gxwtvqpio.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gxsllkvvx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/growccicx.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gkiholcjm.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gfrhyhenu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gffkpqxkk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gohmaywek.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gndunmkrp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gavxqvsfo.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gdkwxxnis.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gfgajsbdr.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/ggfkyyzbx.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/guafkcuvr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gwdplapgj.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gwzoljddm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gcdimpgcj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/glfbsvtuj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gcfmxjlya.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gflzonvxr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gjsszpykf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gxwzreive.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/geuuqndtd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/ghybwpkmf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gbheirxuk.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gtwdbzycq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gygcaoehv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/glrgvrqxd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/getaiqbmi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gyxbopbhs.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gullqxplp.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gssrfkoor.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/glwduyxem.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/ghohufkzf.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/ggkdxgwje.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gkjjrsrsk.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/ghnqxqdjf.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gbrtjrxji.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gyljdhdvj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/glrlkbkur.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gywtdxzlp.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gvxopfeup.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gibnvvjzn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/ganuziuip.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gpscqbqmt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gtqgfglnx.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gatzddrbn.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/giwairuto.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gbofooebt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gzesceiqm.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gzseqdvgm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gbrzsqobw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxukjqyro.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwikyqulo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbhgrhwhm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gexwyxcjj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/giowrcpda.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gtipcugub.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gjyauncny.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gqvfepoev.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gnsoyqeiw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gavjrzqeo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gbtamkzqq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gwnoznkjg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gsasfirnw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gdmvngumh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/grremxten.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gyticevji.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gthtzeize.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gpgbjeyva.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gdrohnmcj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gluxnphmh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghaquxaix.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gknorcdoj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gwiqarbuv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gugrhnrpb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gwmfjdszo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxnawsafo.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/glplzdjsj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gqjtvhnws.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gpupiavvt.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gmavkglxg.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtectnhtz.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdtajpxdg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gozleegzz.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggywtfrti.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gsrgbdzmm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtwunbxgj.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gonowejyu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gotlmihmd.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gxqtythuq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gnqwjyuvh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gtazohhnr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gxwswytqr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/glusgcxda.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gbenqwulh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gzxbugcqj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gescpnyrc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnimttbet.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gkpfmtcdu.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gcgiuiybe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/glbfflyme.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gsmequlzz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gewyaitip.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/goxljzfqd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gnpbzdxdl.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/glglvnjbx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/ggygizcfk.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/glfgwslid.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gduvfslxn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwogkzzmi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/goslzhiix.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gilzqafbf.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gkusovane.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gomwvqeux.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gsmwbizec.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gtavdsmal.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gkfmzsdig.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/goequzgnb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gznixjcjq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/genlndufi.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gqixyhswe.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/godejdlob.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gymlhpcfx.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gacuwraol.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/goizaiqyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gnahjrwid.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gdvwbksla.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gdgbsrlrd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gcnnwdkys.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gurnbxrvx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gonovnyho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gmbccpyow.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gxuknczke.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gsklvsnqr.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gjafrqacs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gylhxbrew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gyrazfzzs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gftlbhkfe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gthbfwhaq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbvxffaua.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gfbqnfmhx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcwuxdogp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvcamzkvg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gpybozxoq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gmoggiopp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwecpuuvl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gckauadhh.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gpsyuxdwh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gaxhyqyhd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gaugwluzu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gnndtdfsr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gvrtauddo.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gekmvyeks.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/geyiaaiht.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gnohxvvdo.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gbljmnzul.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gwcjbckte.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gjspfankl.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gkopnhdsf.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gcbjsstpr.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gielcgmjw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/grigcocgc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gmekxqmtm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gtqeqhmqy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/giiarplsy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ggzpbbxzt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gilhytwqv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gfithrtme.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grqozmkud.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gmmdxpoqk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gjvdwwxur.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gsdxftnqn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gfoznegpt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ggkjutfft.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmmqsemgu.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gshctqdnb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gokjtiltg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gvdnrpmha.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gjjueeeiz.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gzlluhmze.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnfbxfays.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/ggyxgdzxo.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gahrjnrmz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gpcrlokjw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gncdjrjct.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gqhqtwbmg.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gejmldpfm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gqpptudwv.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gkxbbpvfq.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggewfejhj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gsvsteoab.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gnvsbmlfp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gsqbsmcwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gouojwnsw.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gtlditgwv.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gpnlxzqsh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gmoqsdcon.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsyvsqihs.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gqrqtmjqp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gvqegjmfg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/grbwwslwe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gbhqioezt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gibwtdhin.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gjqlzzatj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gauwxsuio.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqovgrspi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/glezoalik.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/ghsfpodgz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfkikntqh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gripmwwca.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/geqndizxi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnhombwpa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gbbbrmudy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gtbxljcsn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/guzvivpkj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gnxddkbxa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghjhmaeda.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnyqlalcd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gqswmddld.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gmcjfpwmf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gpxkehkrw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gfoslqlfw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gfvojrtyv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggeqqhqqk.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gkkoksscb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/ghaxqcupz.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gaijxvsxd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyxmmfehw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gfvmfgoze.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gyjugxsdj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gjdrhgdpp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gkdzobvts.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gabdakzxt.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gccjqbzlt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gohauhavc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gcncclayp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkicqnhdu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnzuimhpb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gsgpekpcp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/ggsqfjvla.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gimfottha.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/guvqflqks.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/ghtwrjavr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gyskgfrts.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gxohqkzkp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/giydtwbsn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gstpqgerk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gbawafbwx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjfudbqto.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gfthlktqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gigkzumee.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gkbyzxhov.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gmbegkhwu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghznqwskf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gghkdtqaq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gherktfpe.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/grajnjzco.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/geouyeoyf.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/glhqhjxbh.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gilbkrtsm.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/ghqliebsm.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gqgulijvm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gqqqklegp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/ghobihjjs.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gaxghvvfq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gchxeyvgr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gfkwukivd.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gebnihdca.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gklhdbjdr.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/glnxrqfub.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gixipspdx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gbigyqvqq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggmuinkzy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfeoqrchy.sHtML


<!-- 参考信息 -->