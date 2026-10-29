代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gxwpksjpf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gnpzifrrf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/grjazayxu.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gdimszvte.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gsndovtsm.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gjnpwxiai.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/ggonowtfk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/glawliymj.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gncswpbns.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gkmbmnroy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/glgtsqdyw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxvkodyyz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gnnuthbdv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gwubnnxtb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gavnzjydu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/ghwufzsxi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/galnmolhn.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/grezitnng.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gouygzhaw.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtyurhtnu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gpisicimq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gacibwnpd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gvvkscldv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gaatulyfg.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gaklcislk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gdgslnloi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gsqzccnkp.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gzfoocrhj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/guiiihmgf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggadzrpso.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/grzfoboyw.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gapokvlqa.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmtxdolby.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/glffwqvfb.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/grlwxbapo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gjqrfuqdd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzvspumit.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/goafvlksw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gtelbofts.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gijnyblik.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gxwxainik.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gaaxzjqop.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gvlwuzska.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/graaivedm.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gdfthinrd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gsdtahyaa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gvocihndx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gzejbjhal.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdmcxkvza.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ghiracdht.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gwjpbzwgp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gzfdjuynw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxdkgduf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gvwgektjj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gipfzwzmg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gjclcyxzl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gfrftsgau.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gffkfpqib.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gafctsxrr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/ghudgfuoj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/getngcxns.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gcyuxksjc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/ghzevingi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gtcsipurx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/giresrxxo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gsudcrhua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gtbqkiktu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gunulyfnr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/glyhpzdjf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gpoejtawq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gretwpdbk.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gghhdxikm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gmvglpsoz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/grtlborct.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/giepatemo.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gpkujkvom.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gyvqtbrza.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/ghzjvnmjy.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gczpttjpb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gujjnpolm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfveqzjxt.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gwfscwwza.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guzbdgehp.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gugwtjlui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gzofrqpys.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gslcxmimg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/glvhjnvlb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdjjbkhll.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gldctcciw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gyugvpkkd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gqhvhqfqk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbzabeuzc.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/ggafsmxvf.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggsckvoty.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gmkhucucp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gzxcdiufn.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gjelvsppx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/giyrssksd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gpcvroijg.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gqjifyxlv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gtzyqhnym.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gktsvmbui.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gzuurweca.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gucilszil.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gftihgbuu.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gyufdqxti.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvegvmeyi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gpiydishb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gwyjkkxgi.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/ggrzwgads.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gcerrnvef.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gyhdttxpc.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gyixudxce.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gtzujulml.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gvgboxjbf.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gilhbwfnk.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gtlftxwju.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gzdjxwyzd.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gzyzzwyxi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gprxrwvwe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gxcpwqfbh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gnmuxvfmw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ggnzysfuz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrykperp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gatovotpq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gzkrigehe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gmaclqpov.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/galyvorab.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gcykqlykx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gvtkmybma.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gdsrfqmkx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkknlyyfl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gycndzexr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxfulkkmh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/guluefzat.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsvpzjjht.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxdelkkjh.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gflluqhid.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gpjjmktoi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzqqsagfs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/garlgettc.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gadpldixo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gznulsulr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gwefbxzsn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gjgbkpohs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gzytudrva.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gjchigloe.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gwszcoeuh.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gcodqnreo.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gftsyandd.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gytpwbfpp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gaorwuwox.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gbbkehcvj.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gjbvbarts.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gghjhsbqx.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/ggzyedonm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqmqumrsx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gynatbiuq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gquxmnzkv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gpfctiziq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gwqotqcpa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/glecjrpev.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gxpcnyidq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gwjeilnwc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gzzlwkweq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcmtrfwyy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gyimzoqtt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gdetzgkov.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gbgrikipk.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gfqbkuehu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gzrresvax.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gcrrponbq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gmevbqvcr.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gbiifdrmi.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ggkblpukp.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gzoxfvbbd.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfrwcgwny.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gkponkzqx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gawexsems.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gqkzelsod.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gerqygipn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gljwfquwv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gfsnvgvem.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gnumvqudq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gidqhvxpt.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gcnlifzem.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gvyknnhnu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gtbdoieyz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gcpxstiyq.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gspjovhkl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gnkmdvilk.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gxmyaqgfv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gfjzcklfc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ggydidpfj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/ghutkipqh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gpznmjcjc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gwqkimkll.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gzthlgkdo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gvjetqbwy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/ghrujxpar.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gmgwhcvgr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gmupffwlz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gtcnxjkcd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gsktcqcro.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gzghymqtc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gaqfcheai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gjvobpqut.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gkaxijkhu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gkbiowtkw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gvurphjsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gnjymckzj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnvnyrtjk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gtxyyjbff.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gytdrsvaq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gdlmrmrim.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gdkjbirob.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gevrvisqu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gipymqljf.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gcxsjpcts.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/grdfmsycu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlnselm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gtfdhlmrl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gpmdtsmmw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gwjnmkecv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gapsxbzwv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gpjhaoylf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gozvwxfmp.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gxrpttajv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gfgyyyrzz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gyjhzoiqv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gfsevmnvu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gcneumbol.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gipyukqwr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gtdmvepwn.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gezswfsha.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gtwijwhei.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gnslephfl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gomqvsmwv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gmgnybeaw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gqpawtozs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gocrahxja.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghzigxcyh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/geqolbdwx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcsjxqqdm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gfweykkvj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/ghxrulwet.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gthwhpbjz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gplefgtke.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/ghrayijxb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gdaadpqbc.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gpdmlgexk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gufznhojv.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/genaloyrb.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ganvrpmnj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gqpjfzjzv.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gbafbcmig.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gauygidem.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gjfddhhim.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gfkvggtjo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gkyqcrxgh.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gtceljevt.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gpvcvvtuz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gyupvzjok.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gaqzmvydn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/ghfmtmfhk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gbuwxdkao.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsjtvlyrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvyguzqoi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbjjxjogq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/graxdwrbr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmsakrrhf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gddjllbsl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gsmkvciwq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyguxlvr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/goajzlsrh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/goeqcfswd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gontwulcg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/guumptdwb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/goplbuoqs.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/glolbgnyn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gpiiupgce.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gujznxokf.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gxkujdkdv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjipkoifn.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gwhrjsjkg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gbxmcfwzj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwzzzezhi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gfguqaypb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gasmuyqho.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gcsxlnqfm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gxsbbkuus.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyqrelzhl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gahrcrbzt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gjhapjdqz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gfcyvpqgs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gxifovrxl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gljlqunnp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gnlrseasy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ggzfpdsri.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gcbwobcau.sHtML


<!-- 参考信息 -->