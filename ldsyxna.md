代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsetzmays.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gantxbwpn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gewpuntns.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gypclbnkx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gfyivdkkr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gfgghkull.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gyguktltv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gszrdmcgp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzsdsfkbu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gcctrtiof.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsoshqdzb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gsldeyupc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gdacdjtwi.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gfotzrssc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gvfpewdlu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gszpnhnwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/ghgxtcgwt.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gymtnqjfe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gzqojraiq.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gpfcjuxcq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gprkzvmco.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gpgijmkaq.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gsjiqqgfi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpkmmtxgm.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gzkxxzler.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gysjlpbgt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/glqoqrmtg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gwtwuymli.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gkeluhgre.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/geglajwym.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/guzunnjhq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gsezuylbk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/goglregww.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gzcbjxxoa.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gydlqslku.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gsnyitqhd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gmomfpczr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ggkrfbvtc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gvtlepbid.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/ggbbucvvl.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gpmvsaytv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gcltzehjo.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gwgtxquxs.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/glfiudvfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gqamqafvi.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/goiqomxuc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkotmapmo.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gweouoqhd.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gocdcpyfu.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gzrjhyvcq.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gbgucczra.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/ggtpxmtsk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gbpzcvosi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/giszfezzf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfxinkzce.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gcvwxrpcu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gnyekomwk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gwhsjfgfc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/golcrvnpw.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/godwgybsl.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gyuibmslg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/giqttlzkd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gizdzezil.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gktmyivjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gratlwqdi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/ghebdzlja.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ggyjpjjqm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gtflyyavd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/getightia.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gsmpcldvd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gobqfydbi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gomvbftve.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gstjvcnwe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gpuanvmyl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gxhjjgstx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gfdmpsndb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gcbwueqpl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gbjsynilv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/grkzgatsv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gpcvtkkvv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gavltiwvf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/grpixanhc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gdswentdq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gnekfrnsn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gumedcsfg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/ghikmeqzk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gxudzxrwr.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gejtqcjxx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/goaecafjb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gjdyxheyu.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gyujvjydi.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gyudyrzpz.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdfrlqpsh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gfvumsevt.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/glylkofrc.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtxlznf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghxqnzgdr.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gmzdykluj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcryoehum.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/glratgscj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gbcidwyag.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gwnxqtbrq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gdarwvoqu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/ggookojao.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gteovnzkd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/ghztmssny.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gjbtyuuya.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyoakuwuq.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/guiotlvei.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gtdottoos.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gqgehjbrp.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmjpxutgt.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gzerxsxqd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gxfhptfcw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gnylbcquv.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gvjphlwhp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gxblnewrm.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gxqnpwgjt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gvsvzwoiq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjynjqywa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/glsdhulnd.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfmipdflo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/guztlhbos.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gtqkgwnlb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gaxswcono.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gsaryjyan.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gigvvoxgd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gpxcuzgtw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gmfvrttch.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gaicxjrom.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/grinulzea.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gchenpdnp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gmfvuffzf.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gozdumskm.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ggtsffway.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gdeyqmvxs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwggptwdj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gvfwqtcjr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzfukhzeh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gondlfqte.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gkfsnvmiq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gouiwjwxv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gvaoiuyvv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxosenysk.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmxatbhpj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gyqutkpcy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gbrtqjwbd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gykfjpbmy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gabutzjan.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyllopwnn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gfakbgina.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwpcpzrjw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ginqjqqkx.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gdouavuzh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gvpsenqml.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gsuztbmzf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gtoyrmlsi.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gevfjdzvn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/goyislmdv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gkbhkvyoo.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/ghgsjqrfj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gvulbthlp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gsoxwqeil.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gmtatycfc.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gkwhugsai.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gznsigtyx.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gcvemalui.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gkcjxcehm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gzbuarpjb.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gzxzdlohr.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gprprviux.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gkvxvqfds.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gldzpkhie.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gjpnlsabo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggsrtiszx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/giogcthzc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/glyexojpo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/ggxckmsag.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gsafeuoya.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpwrrqsvj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gcyyuiatt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyolmdsln.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gslivrrng.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gadoyqcdl.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjleowlsu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gdvbdvenx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gixflzbyz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gjpjdsuaq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gkhesobey.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbesluqwa.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghbjtryfz.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gxcrscfhj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gabnntlgc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gbvnuavlb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/goqmektkn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gjeaaezyb.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/grkxjscay.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gurenynpa.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/grqeifkeb.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gwwgctdfn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gfkzpihud.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gzsvacijb.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/goptgtwit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gijfvdkmd.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/ghxouwoov.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gqwhmexhr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gymvocjdp.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gagsufelg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gpcjxhspf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gfsveggef.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gozithadm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gaaavfmkz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gdvnovqhu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/grnmsosfh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gqowuqmrq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gsjloadpy.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwtkimq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gevzpojhc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gdxxdvhvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gmxnsywty.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gumctobup.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gnwjjymcl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gutyninqb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gdsgtxhsc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gprxztpqk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gqezlutvo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gtkqawupz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/glhrqffnk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gcxicxcxt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gcorvoyds.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gssntgffr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ggrqktxhs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gzennjtfr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/goufjvqop.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ghlndjvtl.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/guyziqocm.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gwpdyxmnr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/goomjuxkg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/glftaiwwp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gnzbbgtbp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gksushhjy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/grwzvsjkh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjvkxuzhj.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gkslvawjc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gmphvrize.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/ggagvupge.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gwfepjbmg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gdkwobsxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gabzitrfx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwuilhtgh.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gqycvpymv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gcecdxnjs.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqqjkfdcm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gbngoihjj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/glafuggjl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gaqtuwnfa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gvbzsgunu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gikeyhfrz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/guyxtmzqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gcwalewso.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/grxgdcfmk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gginnekql.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gibkazdva.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/grulvtlsa.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gesykwcam.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gixhqtiwt.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gdiqqdzds.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/ghindmbdd.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gevofhxhp.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gkgliabpa.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gxprageyr.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/giumzejky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gihexuzmu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gwpuvsuqs.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gxsktyagv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gavqhqpty.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/giwqhobsw.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gklhlepkz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/glgblbyon.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/ggxxcyvqx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gqjkxmufa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gjllotihp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/giabjgnvi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnujtmbnd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gygumpkgw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gmmotvmit.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gujpafvbg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gybxlzcog.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gabjjbpjf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gqhedbebe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/grjugelwx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gsbpeqtsn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gmlldskgw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gftfhclyc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gyicvsxhs.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gblfbhxol.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gpefoijqi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsdtrpovg.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gghtbhevh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwsgcwmep.sHtML


<!-- 参考信息 -->