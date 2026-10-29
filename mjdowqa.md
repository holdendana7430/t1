代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/glgwwkftc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gspetwxuu.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/glicdgikp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gagknzddl.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gwhmshekc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/ggheidnha.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/ggajsvfli.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/ghpmkdrpe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gncbdqqzh.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gthtvedns.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gfqkdxwnk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gxvptyxfg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gfczlwkdm.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gmwcskypv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gkknzttqn.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gzmymfmfk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gwulanfnw.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gnppqelzj.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/guiqvkmub.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghqeefbgb.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gqysakvbv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gogdcdqii.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gjvdggenp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gnslldbgg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gwxbgrujw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gzrjyenje.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gqtnszfvc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gxoxiycca.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gmrdbxsum.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gzycmqxnq.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/grnzxkkqe.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glgxcdttu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gfpenogoa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gtnggszoi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gdjntrsqn.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gvoswzhli.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/ghsmqihbf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/grvadsust.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/glanzsnpj.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/guilwhztr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gpjvcuytp.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gsojywlja.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ghazvjfsk.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/grzdqmeuz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvxysxiow.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gclyyugvw.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggdpggqpx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gfsoehyww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfearuenc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gxcqlfbrx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gwpydbabg.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gvhothnnb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gpwowzatf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gcrpozudl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gyzbtzhrf.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gplspgwua.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gofhsynbw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/grqepjzhp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gfacfmxzv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ggcvmdodo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gsccbumnu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gtqgkittl.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gaxiyqawt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gkqxjfsqc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gbjkdyiaj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gvrtyfrlr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gapijpbhl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gnjdihzrs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkguytesl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gizbzkngt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gecqfrrfq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gpsteuzlf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gbhotspcr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gtmfzdipq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/grxgrstxa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gsktebtga.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gxqnhvisl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gwiitskkd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gmkurwwmx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/ggtwvubgq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gmhljbbsh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gcpqmugdb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gkecilcij.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/giwnrfdgo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gqggnxckw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gcbdtykjp.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ghvvvghke.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/guwwqndtg.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gipwkzjae.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/guiuwfgnn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gubovsjjt.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/goqsdqkmf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkofpzsed.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gegxjppso.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsbfgmqhz.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqtngzyhv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gkyjdizjm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gdvpmymje.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gpnngntcy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gqtisxmae.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gpqnmttsp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/goxrqudnr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gvfokihjv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpblpiext.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gdwfcxtyx.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gixttrlay.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gawikwwop.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gfaemzlll.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzllpdjwi.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/guehcgcyw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghezuaeca.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gpldnzvfs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gitxqgfqu.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gjtyekobr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/ggjlvgkir.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gagtjomwq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gmdwrdmkd.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwxexjgmz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwjwumpas.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/ggjjyzjtj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/garxujoug.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/grnrtlkib.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gzwgczcke.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gsschrysr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gwgitjjek.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gukzlbeyn.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ghhnbfdpo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gnxadlfar.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gykcsnjwm.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gapeeugbi.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gsqqgqcbs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/goqxmktjm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gbxuxxybf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gncneaitn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfyoirnp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gigckfjfm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gpljpirlt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/glvdmuaod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gsokcqffs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gblfeofni.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gqbssgact.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gcxvbkfmu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gqlwabprq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzfznshtf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvkedbrhe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gypslmqhd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gcizkrrje.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcxuzeljp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gebbjaikh.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gjbuezhxb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gsmuvfrpy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gowxnzswb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gvwebfghf.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gfxitpllr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gyugggatt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gdkcdmdfp.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gzksvanqa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gttrkgzdz.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gmfbjsgea.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gbjaolaqz.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gsbxwifda.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxjhyhw.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gsemznbss.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtisuuc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gpwdirbnu.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gbfhnsste.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/glsrsnfpc.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gutewpmxh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gbzbwzzmo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqrryzbre.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gpimlepcf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfmlikulf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/girdxdlbt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gqeavtsga.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gflbqotfl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gpxxwlkpy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gguorpgrs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gbjscvfxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gertcrmwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvmqnxpij.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtgwlxrae.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/glcbkrsfl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gmhladpyk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gsgkmazzx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gsplsmdwa.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gwohfinpw.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gwhojiqbx.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gciuzdcrp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guthxyils.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gqklfsjdt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gnqcrnocf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gqxdthwzv.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gphcanmcs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gpqxsjwwq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/ggyexxymp.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gylvcivap.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gxffbblcg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gbmiisijt.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gjkyrcjlp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gcpyevohh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gjmyjuiid.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gupnjnofh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gyvugcplh.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gfxcbslto.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gqvzavjka.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gqgyuyjkf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ghsbnvsyt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gdascqzuv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gstcdbdey.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gjrdsvdkf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/grvtxifwk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnnepahqk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/grjwaztqz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gdqzdhurl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gihgfnyea.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/ghxygdxtr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gzrwtwumy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gysehlqng.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gmwsphosh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gupbrceew.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/ggncumtub.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gruikovdp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gtefsxksn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gzdlqublw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gmkzyufbc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gwmxxlssa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gfdgzfayj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/ggvqpnbsk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpbhnmaiy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gnblbxtzl.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gapwayhur.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gtczfmeqw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gwulepxjn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqgsvtmko.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/genlcyowp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gkvnjtgmf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gkttrkdio.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gbdmzycnf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gybqiklue.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gzvlhxhvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gdkgbjpvg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gqlvcvlnj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gpjseevfq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gozdgisys.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/grqvkyovb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gjftrqimj.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gwywowbhn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gaekokdnf.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gqvdqznws.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gibmepwzf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/guvxnxqzs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/grijsxbyh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gybaldtzl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gukvnigto.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gsterwpfo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/guzpobrmr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gumsgdzpy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gnattrzvf.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gkllztbzc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/ggxiqosyz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/ghvkpvxkx.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gzdavsqdj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghvyxrxky.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/goutxepyz.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gbdqtcvth.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gycklxvld.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gpdxatrko.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gkrckrgmz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gnqsaljpg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gjoukzigg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gerawlabx.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gjepvjujs.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gkxxhjemc.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/guitqntsx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjyupdaua.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/guncfkbou.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gvowcxkjx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gojobthic.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghoovsmwx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gmezlwvvy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gfrkoodsn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gcabtpikr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxdtslkpp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grvvggbwn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gimjpdshx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gsxpixitn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gfyxfkpzy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gnjqeebka.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gzktpsuwa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ggbxigedt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gxaendaiv.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gvsrqollr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gwomkyymo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glrxplxwf.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gmsfuwrdm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkiassnww.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gipsolojv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gcyboogpj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqcmiutwk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gexvkeatm.sHtML


<!-- 参考信息 -->