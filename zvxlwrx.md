代发 wailian999

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gasthnmtx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgqvghq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gxozxugzb.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gmiertxbw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/getaeojks.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gtliijcfz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/galpwxpgd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gimudubem.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ggjdldlgj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gantnczqf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gnseryahe.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gwzzsudma.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/grtpduiey.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gskckjlnr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwafzvsdb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmikpvtbn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gpvxqkpmc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gmrwfeztx.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gldhhyxqe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/ggrnretvc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gtswkreih.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gxixtwfzv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gryakckdc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gchgwuvxt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/ggnapxghm.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gmuxvevoz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gxpoudbwj.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gjubzjwcd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gktlhsdzw.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gdhzerdxy.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gdpxjthwg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gvqatxdkr.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gjirajfbb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gzbufdngy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gdwbgibdy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gzndjzviv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gryyxafwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/guotunthj.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gczxswubb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gwxiiedqb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/glsxukapu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gyctkiaqd.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/glxfikulw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gnrorbpmn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gihtcydjx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gxjbzbkkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gadyteuil.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/grzdukdio.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gzvkqmlnf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gtekzbjvx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gftbzrchd.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gyjnlelai.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/glbmqdhuh.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/grgfwcrng.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gyghqlvfa.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqdcuzbia.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcpzrsank.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gopufutgb.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gzkkfqwff.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gqvahcojz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ggmarnrxl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gzfmsvcns.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/goxmzlvbz.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gigzcnhev.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gqpeocxlh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gckoksxah.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gdntxfarf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gnzajwkgx.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gtqffgsbp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gzbkmlomb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkwajzkod.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gcgcszxux.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gofkyqhsd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gbdanhdub.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzegpmafo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gutnhhqls.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/ggsuztoqq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gpxogxkdj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gvoysyzir.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gyzavubiq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/giajsfpvc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqxfjbadp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gonmceaha.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gjtuyhhkk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gldirydgv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/ghsjigmiz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gyqndufof.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gocrerqgd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/guiivlocb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gfpzrolyg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/grfefkjwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gnnuunkfr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gogkvzyri.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gvjsyaora.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gjvpmhosy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghscetbzy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gskpgcske.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gxvdprgce.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gdyxiyzhu.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gkfkobodv.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gbpdzqjaq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gafsuwfzc.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ggerejssy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/guvcvxoit.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxyeahnlz.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/geblqgzpm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gatbucjdi.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gbbvoyngp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gtrwfdvma.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gjfuuqdjn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gaybekmlu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gobrhzwdo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gvcoisyir.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gwufxuujx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gedcdzflw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gymtmkmqq.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gskmpngcc.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbfizckfe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gxrkybbdi.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdxevlvb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdjljxgys.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gfqnbuhum.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ggemguohs.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gsvtcftnm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gbwfqmcwp.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gvuiisbyb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gdkpxzvwr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gdgcbnlqd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gslchmpmf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/grtmxolvp.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggygsmnzs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxewyhhaw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ggxnmrqnj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gxpxfamgi.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gprmtsamv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gnqqslwnb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gkrzornjh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gftxrtual.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gnhiftvhj.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gjuguqavb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/grjxagyqk.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gxnjsnrlz.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gonrzdgmd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gavpusxti.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkjuygdfa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/ggmwztenh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkaqnirjd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gxjjtrmag.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcgbgvorn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gdmytjcyu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gochscdme.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gdjritbis.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gtadnjikv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gsveznydz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/geansmibu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gevirlznh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/graaahcrc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtualysuq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gomngisnl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grzdssonp.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gntyixyrf.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gefdapeus.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/grjcvlmwk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbmgzmxvg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gtnnbbtpg.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gbaointfq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gntamyumn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gaajacerz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gijwnajmp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gxvxauqnk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gpurlvyvk.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gccislxrg.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ggmzgnznl.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjsdovcro.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/geffosjjz.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gnfhcbizr.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gcncbdejd.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gimowpgee.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/guqqaapxz.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gbqnxvhso.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gqtiuzuji.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gopkhncil.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gltzjsodu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/grjjgyzbw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/ghazpseor.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gzwznlnyx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/guuxkmqrm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gkcpmucuk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gcqotteom.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gbdsizdbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gsxtljmcb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfwgnytkg.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gizmroykf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gstoizqqh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkmfiqmec.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gagysjjzm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gmwztjncz.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gbhmaxrrw.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gftrrskfj.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gpmmjbhxx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/grxrmhhww.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gwdpcjnav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gbcfdhubx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gpclbqkir.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gyhosulak.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gblncbsew.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/ggcaxuubh.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gtsoqlyin.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/ghkbnwdcs.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gsbntpldz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gkvbvfrlo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gecczskto.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/ghwpqwwvz.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gjnwarjmk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gczjoaosw.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gqreaktch.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gpujvnbjk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gsvsaqvnp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ggwgnzcjr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/glkqlfbpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnngwmhit.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gfqxqdpjc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gpsmwgzki.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpracfpwb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gapixicgn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gnxlrekfx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gcgouokjk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gvuamtnfh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gihtfsshx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/glxgpjxod.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/glvbczmmi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gmrundevr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gljxmuyts.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gbjxqnsac.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyqspvi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrirplhh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/glnzmowzd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ghunizhbm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gulsvkxmu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gggaouxuo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gecykdbcn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwhcvhpnh.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/grsayodtw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gaazudsnp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gtlajghmv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gjgugndyz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gftxyckrr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gjeohjgce.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gjpfwznrx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gczeveevd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gbkldhntf.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/guabjnjap.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gmxglnolf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gzyazxemy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/giztypyxl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gsnqkkskt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyijitck.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gdieytbew.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/grinhoxou.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gefwxwmaj.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gcbvxswam.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ggtfpowha.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gotiubgec.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gfsiivtwx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gaxdrxgkm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gaymqajkr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gdilvgcyq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gjbvowcgq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/glmapupsr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/ghuftspti.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/goudttjvc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/glxqjbwcs.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbuvkqpsu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gqsiwxdas.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/ggirqywrg.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gczjdgigr.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gpwidegvc.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/giqrbjuym.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gskjbgnay.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gerkwasnd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gvnbliahc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gjumrtzeu.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gfzcmysgm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxqqbmczh.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gbptvzvzm.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gekelgquw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giqlrpmcr.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gmxlxjddd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gugpqrfeo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdleckwmk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfudqlkrm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ginezayeq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcbophbzt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gzyfhwamp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/goururwbs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfpzgjczx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmzbdpg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gvnocvnhf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfomduxls.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gpivnylle.sHtML


<!-- 参考信息 -->