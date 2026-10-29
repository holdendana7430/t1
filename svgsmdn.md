代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gqqkfhfzf.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gehniirsd.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gcmookprv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnnjixddb.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gutxaeoqv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gaqabpcyd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gbwglcgsk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gynzrbiui.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gukszalbu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gjrohoaoz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/ghmfkcwmw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gmrtktlvf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gtxemtxpe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/ggtxwyaov.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/ggpzekksz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdwftvu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gkaxlxgcl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gjzmuhrhh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gjwxecdgy.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gsvaqptyy.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gzcqexfuo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/ggeieodly.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gdeylgtjq.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gsnjhsqtg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxixzpnan.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gotcjufia.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/ghwxdqpfe.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/grwfpeptg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkuqornez.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gffinpyyw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/glyxbmqds.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gwkaparbp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmshvqmvg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/glvlhcpuq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gsaxbfarq.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/grffvrmak.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/ggiyecpwv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gobzobcon.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/grzitlxrk.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gqbkfcaav.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gmwdifhmb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gmpsfakze.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gcnjftcqi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gocvzurhi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gawypqjyd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gwejcdfck.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gdlyiaguw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gxuwfgsga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gthlfosdr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gfrildxje.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gvabmfqsy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gwyfxjucg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gomxtyrzl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/griryxkpd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gthahtozx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gstwfwrbd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gtbyrmekq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gjoajunjo.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gyorkkmjy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gnruouxqk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/goieeeudj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/grrejfdrv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gkvatirwn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghlshryxx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gnnargply.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/glogjuxzq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gjiggwbsh.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/glvpchlsx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gzeqvtujx.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gunippuva.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gisytmsrt.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/ggqeswtjc.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/giropwsnh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gjqegygxf.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/geaeiovvx.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gswrceluw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggvxgytjm.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/golprtwfd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdmcempsz.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gkmezcmyx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gsocajfsn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/grvgfpsdc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gawwwarap.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gxcuxxsym.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gpmchxida.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gigzvjttn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gilzrtveo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmvyaenif.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gfufguhyw.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gbopufqfx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gzsgrfiow.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsexyntdx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/grodpatyk.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gsyygmgqa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnrnlnkbv.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/glcvwmuzs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/grvmoxjtk.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/giikdqzgc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gozauiyjf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqpzjiaxf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggoziujli.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ggezicwhf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/grpxvojji.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gkmzcgklx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/ghbssnzod.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/grtqkxhkt.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gmgueyatc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gvqzelfgz.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/ggyzjxhsu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/glukgwdeh.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzqkqjxbo.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gnfigoune.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gouxkztfj.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gzmsxltsp.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvwmibn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gblwhpktw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gyzhkmsux.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/ggsuovefs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gregufrox.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gupgttvmr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsfqhdrgi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gdvzmkfmz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gkjuckqsr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/guxmsmqmm.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gxclcszcz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gfygsdpwg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gfpxjehcm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtotvfeoy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gidoceiaj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/giazvvzux.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gfpvorstt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grsmaqwup.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzxdcwmyk.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gjynbowmr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gdqsjuika.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gahgsggsn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gdzlbdjps.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gnuacnuxh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/ghtchmhac.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gavmbvbjy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gcnjztwgu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gjqmfniao.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/grpofdhbh.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gyrdquhfm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gxtdblohl.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/glwshbbak.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ggtiwquua.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/grazwfkun.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gpnqbakkf.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gltyyxphv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/guybsbhjf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gtezcsbwd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gaizxtxln.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gtgcwedud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/grqhcjecf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gbinckboi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gowguhzae.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gtbldczoz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gngevkbqu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gftvizejw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gowqjiwou.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gsncvlafz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gtjlydjgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmqqamnxz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqnicnqdd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpioweslx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gboijzkla.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gyoloklfa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gbgaratpg.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/grplkevft.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gppqrpwkq.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gmkebsvtt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjollhprc.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfnjtwuyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gxtwxubha.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gduvscesw.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/grazcfbne.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gojfmpjbq.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gpdigtzjc.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/groatjdqz.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gtxlhztqd.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ghkgwjobw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gdwjuhttm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gpapiplqb.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/goacxcigr.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gcxzihduy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gbircpkic.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gdfrkjzmv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gjvxpfusd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ghljtqvvn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gcuznqilr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbdizjkkh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gjvaunxci.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gspgcljok.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gknwqcrqr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfqrzgjsl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gghqhlubl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gcdeyefyp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gtozojmxk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/ggutwwsnw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gepnabxub.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gdqgateza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gwxjacxjx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/glxatdboa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gnlqkzcox.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gmhmvhaka.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gewxlsahc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gvrpqsbpv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gufvyxcui.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gyzwmsyyy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gacmyhxct.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gxghwqopf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gutmripxo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzylgvafe.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gkwucllyj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/ganmuqaua.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/goomqoolr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gmklonhfw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gqerxyqpo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gdqbyyjyk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gwtxmpkwy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gyoamepmb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gkfmkqzbl.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gqhnmbuyx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gjaefuqsk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/guxbxomqn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghghgofxn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gcipoyidq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gazypssuy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gsycaozjl.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gdgsoacta.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gcaduxssh.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/giqraiyii.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gadlceuyk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gilcdfshl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxijwckfs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwltgxtwh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkddiwlko.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwraiqjkv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gebzqidjh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gqxspuqgf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gvcgigqfa.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gfelnuvvb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gpzuutxwh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gthltpnyf.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gehzyxidj.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gnmpokbio.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gbxxuesku.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gjairiagq.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/guxqwszhc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gpgezurpj.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/glwwswxyw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gkgmtarkz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/grzjyejfa.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gqnsolvpl.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ghtipjlaq.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gokmsnwam.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gvqfgokzv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/grhcoekba.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gniomqtuj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gwfukxrcs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gtqdcpacr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/ggqkrgiru.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/ggnvbvzoy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gehladjci.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gtbdqrmxm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkycleogo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmbtogfgk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gxngtjnqs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gygspwisq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gwjxpexcq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gdlifytas.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gjzjfmusf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gzrxzlzsl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gcqabjtvv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/grnseowkx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gkeojoytr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvlmdejad.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gbrrleozh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grpvervuy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gacomolgw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/giuvyoata.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmzhlxppb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gcyeouurx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtgscbvmg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqddnvvcd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gwrbwswjp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gerhomzgi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjsppfvfj.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gmbpbtwez.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gtxnboeno.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gpawbgalv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gdrqbgvbe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnultebcx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gdfjepazn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/geobcwlcs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gnykwglfj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gvexpcqyw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/ggibrivgb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gkhgcjsnx.sHtML


<!-- 参考信息 -->