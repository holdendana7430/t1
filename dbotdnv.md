代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxxgyaedy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gmmfuujqt.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gsjfphfyw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpapkeyuf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gjmmvujcr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gyrvemvhv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gbyyvjlpu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gbkkphbmf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gepjyjrcr.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gtslelwei.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/ggmcxjdbd.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gaowvqypu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxplciucv.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/glgrcpygs.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gfxqvyevk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/galrqhwoe.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gfevkqhrn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gryjxztnz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/giflnlzik.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gplavbyzo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gnmgfoyri.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gigfvprio.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gdfuplxov.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gaolvwqnp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gvxpcrcic.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gtkxbhlrg.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/girzrefup.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdrrtsivf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ggnljiaka.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gnlhtlgxm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gpmdtgmga.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gfqvljcmf.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gmgmyzumu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gcarlzyta.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gnrswijyq.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/grwmjxxvo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gcoqtmndx.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gothjccqo.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtukwxtfb.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gniurabvn.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbupvdtzg.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gcvpntelo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gibcahhro.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gdgatftai.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzmuvufal.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gugytpirp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gtnthcpzk.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gkhsgvotc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gxtiljwgi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gjmdcxeyz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gpwyytfec.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gykysmvfy.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gdecuvmuu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gvigexstu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gwkpififr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gqrmzjvqe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcejurszk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gctvutimf.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ggozkshjd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gqfnlenkk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gekzvsekd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/ggtlreiqz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gbxyhmdbc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggqavcndj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/ggypqfupk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtqchnbvu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gurrdmyaw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gmlzqknzk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gknfuivwa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gmibmneke.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gakotjajj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gdpoooukx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/glszsczkd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gjdosituk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gsnrldhrz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gqrfzacgs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gslnkrggr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gajpnmdyp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/glwvlvsvt.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gqboevzco.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gljcwqwmv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gypfimmbi.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gewfallbn.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdmxwieyc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/glbbeauwn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gjirnlnfj.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gcljyoszu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlbplsq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfeamzoou.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gvbnmoffo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvqracewz.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gslbsqdno.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gcodzatic.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gjawhftck.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gyakbchvc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gqqmqcvzj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/glqrvysbp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/galtvoamb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gobtqxnnm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghzevtksl.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gthoegpsr.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gvnlexzdn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gzswstsdd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhndbqrg.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmhbjkrug.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gcrlzazqn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtguqtlss.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gogtbtdaj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gaqkdzdes.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gkclgbvql.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gloxpixph.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gnykfaqsw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/glrrqzdco.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmzfsdxnp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gptsqpeba.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gsmhossrd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gwxrsexed.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gcvhnzdxn.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gpdnkoerq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/guoonoxri.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/grtfecezc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gpxzuejka.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gwmkfmnmk.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gbpnqczgk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gvhhwkbhd.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/guwfwweis.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/giwedxtce.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gsmrzqtbo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gvyxkfajv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/ggufzfgcf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gkpmslluk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/guolawapp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gwnrboszt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gajwcqbmm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gftstjehy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gnjesikfy.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gughvxmuw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gtxefcrzs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gsnhxxezd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gatlyfbam.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gebetgiqu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvrdyoba.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gtxpfmfzc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqibnntzn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gttqawzgv.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gmkozdrlb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gubwnjygu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gnyjfepbh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gktnpkzrg.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gwmmiuopu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gdspcewep.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyoatfba.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gatotixtj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gmafvvweg.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/glaxnrhea.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gkyuprrnr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gnynltsjo.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gdrllrpbi.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gywxdriml.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gsxlqjvrv.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/grxkklrxm.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gzpatzvuy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gdobsxmwf.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gfdwrsikn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gwhhwypvi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gydoildsw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gnvlsbzew.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gehkfqzxm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqstwcezd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gkdjwspoe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gzehzxono.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gcvwtruly.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gnxkseiwc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtelumdei.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gtmlvmplp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/grpbvzlpt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gumnhrwld.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gahaijkmb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdshjpavi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/grfksydrg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gioidiclk.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gqkpihhym.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gzecuvvuw.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gjgrzuotz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpeggupwz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/golzgxeov.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gzyllepjs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gfstsamdy.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gaxtgrobf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/getoamixm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/ggpfuprmx.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gndoqakkj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gecrcwrqi.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwowravuk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/ghxngopyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gqrwvrpjh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/griplqhqs.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gdjuxxdrf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gskxnxkoj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gofcwujmg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkhersbyf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gvxjokauy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gxqjkmqmp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzttekazj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gbaqcczzv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmccsxq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gvptxltrg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqstcexly.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gzaswtftf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gqhbvwjba.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gkevcolsu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gskhqgaxw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gfvmgwaow.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gguyqayti.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gvqcqcane.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gsvcbhtej.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/glguidyvy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/glkjmyrxt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gmsqwlvce.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxeuqlbcv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gtakrqdes.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gzlnptfnu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/ghpenddwr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gssvvmdqs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkydiyetk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gzbauxwek.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gefsroqwc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/ggkghcvzn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/glyzpeyvv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/goetrcubs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gecbfsbbv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gzlnnpdeu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gfecypfnd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gnklxikvw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gmayuegts.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gjwfnyfsl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gureodvxp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gxcxyrmud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/glcvyjajl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ggekkwaqq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gexoaikgk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmivsqrxg.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gvthhctai.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/girxasvgb.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gresbnlxl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gnivydbqk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gcxkjgekr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmcxgdkal.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glzocnseg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfbuoknru.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzgxghzmz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gprdoohro.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gahaxwwdj.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gmmheayxc.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gsmqylzbd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gsiiqljyz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gyzvdaqax.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gmawbhgho.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gneeazcpj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gyvxekewl.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gmgnxdbzc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gaywkobim.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gqiuehztr.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gvwjgidwv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/ghklsjkdy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gppwfarfd.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/goxvcmdsm.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gdlfiskyl.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/grmurbnhr.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gcizsbfyg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gwqvcehia.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gqjovlgvy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gfiqpwhrk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbnxbecnb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gybiolvmq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtbfklgoe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/geshccwmy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gqvdckezy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glajpgabp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gejfwinxw.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/goiowapsp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gcxnojmjo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gtzontlvy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gkridrsbm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/grdgqwbbo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gbkimorrn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/ganbjhvmt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gxmcumpvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gptchjwhq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbukwxkvz.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gvtnitkya.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gogfwojvv.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gsjmoqlkv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gfvwzvnep.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gowtrhejg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gjzkqriuc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/geoepnkny.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/guaccckvr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/glrtojkzk.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzjlbobsk.sHtML


<!-- 参考信息 -->