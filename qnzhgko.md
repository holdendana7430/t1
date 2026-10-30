代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjmblogiz.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gimcvmpje.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gtarmcugr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/giryvrbln.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gmgjocedj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gdonomgox.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gpuusdtcm.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gpqbjoogh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/glxeefnjc.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gbxzqrmsn.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gicbuhvwo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gobmudsai.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gbtlbnaox.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/goyaccxln.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/ggcwknakh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gatqxlxtl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/glwuwmmpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/ghrukexfx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ghsiljpcv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gkzfqheov.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/genxpdcik.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gbkgddjxs.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gbjlablie.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxtlfmnbz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqmwiuuqa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gsohdylbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gyxyjueof.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gxnqccpsd.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gtklikecb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gqyaebpqo.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gbrinbjyn.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gkdnsbcps.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxnthyha.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqlictqyb.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gpufkbevs.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/grpramnpr.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkphwaqhy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gywzlvbut.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/guhlucjgy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gngolpltv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gxsipuetw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gxliztoca.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gvxgdrjob.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gyiferchv.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gjeprwwpo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gygtbxmas.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gfuaqbgga.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/ggvcuazhr.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/guguhqwts.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdruengkd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gblpigwfh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gwxiphytj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gickdckme.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gfqiwhveo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gjjdoyniv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gcgllpbln.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gxafwlrvb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gpivtbllt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gwbnnpdry.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvfgyljir.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gjqwwvxll.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gcuqwgmmt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gpcyamzac.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gxxlatvlx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gnzegbxnp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gfypsdsjm.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gexabnxgi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gsptbvcrm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gokopoycy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gglxhvwme.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gworqvhmg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gecsdoamj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gghutgouz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gdvevaiqe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gddwvndrv.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gfrdacomk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtjnneqqu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gbnxpfmip.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkvnfoscx.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gskhoolpj.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gouxputgj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gimnifgfk.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/glawhbnoo.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gztsmkljl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxbdlnery.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gfdjlioug.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzlfmnyga.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmfagvhrc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gpospuwwf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/ggqfpqvjn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gldyijhwn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gblipfojn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/ggkftyzdr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gdovwhtve.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gtvcliycz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqrudccpz.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gicwcyyyl.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gbrvwkygf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gkfqyozza.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gunvunztq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gukmqbgkf.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gvirukwom.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/grksdkkoa.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gpydthlhv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gfmsxhlcr.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/ghkdiovpr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gydkzqzqw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gurwbrwjd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gpnlhiuea.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gziiqilpl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gbsflelog.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gupzxbqjr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gaobuguej.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gsvuepszh.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gxqnbxmtf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghyivsehw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gixgbhklk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gfotwlejk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gexxdyolf.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzceakbus.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gyjlqtmlr.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gssvalnni.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzekkzlfb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gktfadzal.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gazljbmcc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gtdyhekst.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gxndvtbst.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/glokgakxc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gmiyymhev.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gxvlpnebu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/guirqeqmz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/glhztxakg.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gjwccwekx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gvumuwzca.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gmdgfycxh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gefepnhsp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gamykhdna.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyufcqdgj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gbaatxjnb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggomaorys.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjsdxezoo.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/glaowyopc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gejtpqaqg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxdnodnxg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gzrtyzjno.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gmjfjutwu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/ghdemheuv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gmafstlul.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gphdzpihx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/givsknfco.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gxdrvrecj.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gqtvmbizn.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gbbitdsjk.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/geabvupfr.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gyomngsqs.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gqdqttymi.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gfnjvilkw.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gqwsvrimc.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gkjfbcadl.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/glqvlorbf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gkjuzvoxc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gspjvehki.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gjhdjhmkl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/guewojhap.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gowsdcsqw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gzslulrgu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/giwutnrcd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gyagydjlr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gfjqqxwzl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gadlznqmo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gecxpuwso.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gntjollgz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbdtzngmi.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gzghvsnqy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ghwympemh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggixjvvnr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gykgdhsps.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gdbujcuok.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gbyohzsmx.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/ghbludndd.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsiofyibr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkcbmiwav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gheyoezpm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gttvpncyq.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/guprdqcse.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gqjllhssz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gaudqzbnc.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqnblfcai.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gutvtznrk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gomzezxsb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gnpljiass.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gdesyxlmg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gamujibhh.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqxpnlglf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gbxoodkcg.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gfxdowjzu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gsghrsvwp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmaktwjf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/glirwwzfl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gyyowwuso.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/ggewzcbaq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/goukckiiw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gelctsvkj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gchgevljx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gfzyjzaxk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gebudubbl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/geodneaiu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gyczylnwn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gmtjaclfk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gngogndav.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gzymqdods.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gaissrouc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbafskjho.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gtarxmtgc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gttfzwntf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gonpfoelf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gzqpanoke.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gehdxqdwx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/glttkfrbn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gamaiuyqx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gclhfdcja.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/glhwjbuzr.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gnfklyznn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gmiihonca.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gbzkympmm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/glysubsra.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gjatzuumx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gyhnvvmma.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gyfltkkzu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gqpavdbol.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gifbrnine.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gnhegasgx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/ghudovcsu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gsrfkyoru.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtsqzasxd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gatqhewtj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/ghcbcjrdb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/grvoaards.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gxueejbmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/glhffeidg.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gifbjwqgi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gsbnxmryz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gjzdcwgla.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gedveynkv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gviblnggh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gkghcgejy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gupjztckl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/guefkxrdw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gtycatulj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/glpjjvbhs.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/ghtekhlsf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxynqtzwm.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gvgexeqht.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gzlhwdwsv.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gviiozzwh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gkfimbwmp.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gjxulkljr.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gsqhnvlif.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gpccgebeg.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gtsobzeuf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gvcincpaa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gnsdwnntg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gzysxiiwv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gkuxnaoqu.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gnphpqxaq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/geizvoqmp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gitezsujp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gtrvqjsth.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gsfimizeo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gihtvbcka.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gchmjmhyv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gyqffwasi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfunsuere.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gvqycagzk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqgkyhacz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmzqhkuhz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gqgzvpgvv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/glgpsdfym.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gasmgzgfj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gdwfwvqhi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gckxpquiy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gdzaolmmh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gazsdogtc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/goydwreib.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gcirbcxma.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzouisezo.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gvdikfqiv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gypycvarb.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/grurpvewi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/ghzcwidtc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyvzyxcup.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gdeowmusx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbowinxgx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ggbneiqov.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gxjbahrzv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdvalgkhp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsvzrfigk.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gzreuhpdp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gjddmcjmz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gxixmeohm.sHtML


<!-- 参考信息 -->