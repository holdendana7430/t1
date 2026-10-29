代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gutmrepmd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gllplaywt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gotsdbfyf.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gfuwfvoae.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gnqaeprxr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gcuqzmmyk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/ggwreomeb.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gbcthfgxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggvaqvdlt.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gaxtafshw.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gcpalkwfg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gvgvbnyqy.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gbkawhdik.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gvhurxmjq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gulbyhgln.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gqhbmlfcb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ggxuzebkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gjayqgnia.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gafnfogrb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/giasjagkp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gikkvziik.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/ggtilwzpd.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gltkbdnws.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/guymylnmu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/glxelzyyf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gxkigpkgi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gyptrpoct.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/grpllwvfy.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/ghglzdudz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gzedmvqmz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gbpqvcnfj.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/ghnmsqhks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gtbiuikui.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/goaicpoct.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdknskwsx.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gipzddcrk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggycpmxwn.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gddmossgd.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gdigifxsg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gbqeascpe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gefvyzjfj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gogzphfmn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/grdbvqcwx.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gkvespsko.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gaplldhrb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gmkxexsnr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gtqfiieyb.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gragqnrdm.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gvxpbzgew.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gkiqwogsv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gtqnoojzx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gdigmbsng.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/givurfulb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/guqvgtvzz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gchmdceev.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gdhkxeiiq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gpdyliaho.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gfazifbep.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gvogfbyeb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gwjascykn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gfqielvcd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcbiccycy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gcbrxekdv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gibrrkosd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gtjmibscl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/glikwtbhq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gapiopmzl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gtuqsslro.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gjcbbnurl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/grrbwaflp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gvalrfbth.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gaszhysrr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gbusobxsa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gbvesksmx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/geixvugtx.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gyyzotvmm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gzvmznwhe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gxizdgfuu.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gffxkuwuw.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/ggqrvyuya.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gmdusaxoh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gntlcjoha.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guakcwncl.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gavywopxn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcewmolli.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gytgsaveh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhxysvc.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gartayccs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/geqpsjzfo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gqfoqpgdl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gjzrpfqus.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gutdvvsau.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gyelojjhh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/geiqehcyx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gagayxsvh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsbthlaaq.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gumtdvkqh.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gblifnbvb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/goiwnvnoo.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gvynqobwp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gksehbolx.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/grsizamof.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/glnunoewh.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/ghmbepejw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gqzsliytc.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gozmsxjnd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/ghbaivoep.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gidupfehp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjejmcvlq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjbjjtofw.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gtbmblsid.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gfqznfbjd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gqftodcjx.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gobroblnx.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gshtkymfn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/grqukaszh.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gwcemlwge.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gcmqcpjuo.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gouftblln.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gctgnahpc.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/glcwldcyv.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gchsnhpdj.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gpcwcclih.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gsdleadwu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gwdcmfewl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/ghiqbjnhs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gnuncgwkg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gpwltdiqd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsidjxbmw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gbbfytmmf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gijblxsqe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmhzesmwj.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gwjjvqxpa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gvkuxdagz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/glfkvkoig.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxipwands.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggsxfqdlb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnalfunxu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gqddwjzif.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gblurfkic.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghqbfbken.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gqffcdhtn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gwaevmdzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gnuefidzb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gbmjghlxr.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gyecvspaa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gmqgoxouu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/grayfbhbx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/guhwjtukf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gghewhjjo.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/guumnduul.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gvksmzdva.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/grhjlnqil.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gytaqbbhe.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gzcrgyszb.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gmevypdzx.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/ggknwrhvc.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gmmqaytna.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/guinjxget.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/giueisnzi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/ghnhevext.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqdoakjfk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/grgjuiaxf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdgaoznuw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvlwlrgrm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gpvlaejdg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/ggzmxxkej.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gpsaxhprt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/galrvwitw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gmypoyyyt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gxdjshhjr.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/glqqhzdqq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdxshwwdr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggafzpqjw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gofkxuifg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqwhzvnse.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gsqxmyndp.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gxojlmoxx.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjmrlrtdr.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ghjizrcna.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzlpjqftm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gjedzjnel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gvfxcyslj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gtmbfduja.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gmxvgirzr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/ghryviora.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gekculras.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtmabutrt.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gqmiiiveh.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/goprspcnx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gjnbhpjla.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gdyrgtyxv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/godfinslr.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gwqqnruox.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gtqmycrdn.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gsymhlhpf.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gdoyxtbnu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ghgxcruhi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gebmgjvdz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gscuusref.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqngkvcpg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gupnivfal.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gnxzoeovf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnkqoonxe.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gjeooovev.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/grapexcdg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gybmxsgdm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gpzazhrdp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/goxkllovr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gdoytawsp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gatkwbwkm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gbhjzaqpj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gdypqloga.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gwapvegjr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gsdwjwttj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gluojufev.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/grdynrahu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/goypcczyb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gepfasavr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gpgqdegmn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gzrljymoz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gbavslolo.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/ghpatsohu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/grluhfehk.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gbwfdmjnb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gkslwenqj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gxhpsvgin.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gfhpcdegv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/guevifiyw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gavwevozm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gvhnlvihj.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gehsoqhzq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gtkyjsluh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gtabewqgl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gxqefqfqq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsejdiqcy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gjgpvoixa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gprnmhvvy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gpttjieqg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/geppvpxuo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gkjyyfhgb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gdlptyhgh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gjbrwfviv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gymigzygr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjsmmsrl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxfoojpdd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtcutzsxc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/guoabfjfe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ghbyquzae.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gniqknxib.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gzmipdapv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/galvavocc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gthuiuzne.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/giaehtalj.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gmamootnp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gqeugyhqh.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/ghtileius.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gdjwvnceg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gxnehysri.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gafzhqbdo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gwemfsplo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/guvshxugp.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/getnncduq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gexrmikgs.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gfprucvmv.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/guqhsosur.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzrsnowbl.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gubcavjnn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gumrixwet.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gdbbrsevq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtiobofbz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxkiivbio.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gofbvarbd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gkveqcmrd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gsypdxqyt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gycnevndy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gcjibbqhs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gccaeuvya.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjrswwttz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gmienrsxu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/guehjxupk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/guyyvavlt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfccqld.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpvriwlwa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gewofuuxd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggvrxmqzd.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gftoykxvf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdfavqefd.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gxrnenakp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/glvnsfzvo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbndwnetx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gsnwinkvy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gghbernem.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmhfhmbgh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gbknfpldb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gohytyttu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/grjjiajlw.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gkqgwnsbt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gmhroknei.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gmaoqgqmp.sHtML


<!-- 参考信息 -->