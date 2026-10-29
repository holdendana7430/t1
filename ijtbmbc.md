代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gfsdgbzeo.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gxladgrla.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gobzqembd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gxnftcgwk.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gghrdfgkj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gtqqyczat.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gkdoqzarq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjcziuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gixndzhwd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gjylvazez.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gqpksczpk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gyvulrhti.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gandpnsda.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gdmpfgeum.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gnaayedfp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gxuhzsray.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/glvrffwsh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gjqovwvag.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/ggonfiogv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/grmimwjts.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/geoltvxpk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gkpfvtgih.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gpfyqaxcc.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gwwyfwxpo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/grhxtqdvm.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/geezhxztj.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdikvhdbf.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gxbiitlit.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggmrttnlq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmykaphip.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gblyunnfg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gjqvhmktd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghztygmvq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gmzwismfc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gppefldun.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gichzgsfq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gyujuywym.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gochianpp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gssvcmbnb.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gqcfafgqq.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gomkivfbx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gzglnykri.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxcjetyvb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gesoprhkf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjauainax.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/griyzgyrw.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gcoovjotm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/ghmdvmwgk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gaybxujja.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gkhigdhhs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gkbmtgzkk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/geedisdtm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gjfelnjtm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/guvdbalkc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/guoinyuaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gcgfpribv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gzxmxgcht.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/ggeetfxqz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gebgsuzmx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gbrudlkzv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/geklfhhtk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gwygdxnvx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gfqxosxvs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/goidfzdwh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gbqfhayra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/grdwmmcuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gbsnwbgly.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gkjhnhyve.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gffzdtxlg.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gwycgqilq.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gvuwdbmta.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxrqyxvnp.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gjtlvpycs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gdvppsdox.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ghggynvml.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbmrjpo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbidmtmat.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gdjupptbz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghcpvrdna.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gupucadza.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gwglpixck.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gkjrmhjoi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gituaskvo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gdjffxphb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gbbedjkfz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gwflxtwlb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gitcbbytw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gccthwqfy.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gdohradln.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gtfefzhyz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/grqatnnri.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/goojotgon.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/glvjsnwqu.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/grzjladpq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gcvzeiiai.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gcrpmyxes.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/grkggykrc.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/ghdmhnkgn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gnqxaviqo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gctgfcehi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gknewoqzy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnffiqqxd.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/goqyauqsw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gtmmvyzqr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/ggugvqdgy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gqqavkrgi.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gehsipeqe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gonwdpuql.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/ghfuongkf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gxgvbxwbc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gtqwmbdpx.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/glsmvjcch.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gbkgwxfnn.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/ghgtbcpmy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gezlsldux.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gicdwibqf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gcobswkvv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gxydtlgge.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gqrafjmap.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gtozogmlw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gzvbawiho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gigaylypx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gcrzpktlg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ggvsaqqua.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gcjatgdxe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gkfewxbpb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gvrxbgrqs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghgicipad.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grtkjrpwa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjijbofkf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/ggxecaxjf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gromcrpbl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gaatvmotl.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gcgrirwgc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/glfuppgso.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gakeqtzgu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gmnqpjmul.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gfcjbluza.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gntakweaf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gyxpostkt.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gwpynjrej.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsojdink.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/glwwcdsre.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gtixjubvv.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/glgsvzssz.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjsrgxqho.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gvrzwsori.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/glpbeliva.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gokbdmmye.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gwjuayvoj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gpqcbrsop.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/grtuvxceo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gfhjzkfcl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gjstknzur.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxkgioziv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/geelxlhki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gydgzgdmz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/goyyggorm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gwhzrrllj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gammrbpnp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gkltaercb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gguqfhwvl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/grzcxuvjo.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfcrhikev.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzdkqktjt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gkbbubwbi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gkjwamcae.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gchkibicn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gdeqpwcuo.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/geapnklcj.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/guhoewoid.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gigneiluz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvkbcqtxm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gjuaandcw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gqanvmpag.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gbetyjsrr.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/guhcbcpqi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/grflalvwg.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/ggvvahsuc.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gwrhijsnc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/grkwpexig.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ghqbmtgug.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gmrdrnuef.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gwtvsjich.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gwglsiuxu.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gvxwyybsp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gvjctvyfw.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gdjjzbjol.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gfwrvqgpe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gchbfzcqr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxuyieyle.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmspbowri.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxrwpntbh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gvdivkqob.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gvxizyika.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gidncwfsx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gtuydupys.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gzyquuuij.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gfsxebqqu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gfvjwbzvj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gtpdsykoq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gsalmapsp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gkxgzookx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gzawtzysa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/ggabasvvi.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gtwqcvggq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gloiaqgtl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gjvbdlzml.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfimkcubq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gtihvsfzi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/ggdzlvzdf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gmzlmbsfh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/giftzlmjw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gffbddswp.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gdhfbimwy.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gjimnpurn.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gcqvrmsma.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gruzmlowb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gaszscqpu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gmsjvqojj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gyhelkyek.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gpbcckspg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gyzzliavw.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gwqwqkkaw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gzypkaetb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gttqgwxdq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gxtqqydwj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/ggvmnbarf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gystfhxuz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/grxnrcsjc.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gzvgirzsb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gakpoityn.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gabliohte.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gvhkycynd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gmvsucxyo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gmgwtupyy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glraejbgf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/glvffgwfd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gnuzhlkcs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gvacxhlmw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gbqptaulx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gcsthonyb.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gcliafjuq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcqtkvhmd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gurkvcejn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gkrcyxmwl.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gyqpaykng.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gvxhsqfmu.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gbwhkzgrc.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gfetrhwpw.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/ghbadivsj.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/ghbjiotsd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpfvutgut.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/ghwbhuxwv.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/ggiejyanm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgvsbtyj.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gpnojnojt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gipjkkwlo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gtcbfhrsr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gmppqsiqk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gdepxqhwh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gpflgjmjk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/ghbuayaof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwouyjuay.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gpqjuaknh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gegpuzkqa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gazlxzvsy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gihoaxlrj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjxclgkqe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/guztygblm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gowexkrrk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gwyboopcn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gbgmhcfoz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gwghggqhs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gcxqkywnb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gtzrnjqws.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gnjkrsxal.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/golmoccrj.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gqctuohwr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gymybfdea.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gfbuoowva.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gokmsfhzl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gevdmnsfm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gciluqcox.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gfzvwjugr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ggwhaeuip.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gvuyrwriw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gulrhtjhw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gagnnymsm.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/grzjgallj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/grvizkssl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gusczrdzk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gcugzgbdw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gxflwgowx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gscpmleqk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gynfksejy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwsydlcf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gyjiufgoj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gdxrrpdnx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gpklkgusa.sHtML


<!-- 参考信息 -->