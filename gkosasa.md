代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/guhurwxei.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/ghjuirfwd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gprrrgjdu.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gpmapvyoj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsnancacd.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gqxzwwzyk.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gmyxjgunz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gikzhxlbf.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gqfzagfbq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gxfzxdvwg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/govexvwmq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gfedpgznm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gzgnfpfnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gmehtzhyu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gdrvgofcd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gwbrakupd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gxsfnlwuk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gejxmeave.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gzoxiucey.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gvaaxycup.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gvemnxqqf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gqsuejupz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gozvvlvhq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/geqkxpslz.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/ghpbemhsu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/ggxnbfbsh.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gvxbcjshy.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gwwfvgapp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gmcsbbzjh.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gawhtxgns.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gbbvvqvwi.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnemgdvqw.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcwzifcqb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gbgzynbol.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gctdacboe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gmfadqjaf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/geiberutp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gmkttjinb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzndgvjyw.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gbhgjfhsj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gxhvychvu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gzuwoolmg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gnnhwedwx.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gvphnxedw.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/guslylxvq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbssushxm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/ggoftophi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/ghesiasbe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqpezcuq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gfzqmqtkc.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gtyacmfdn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gqujbjmdl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gbnyyulqz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gpucsyhgo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/guxtlwjny.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gjyvkihig.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gsailnlzh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcewfzdwm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gkvbrukqp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/ggzcuzzoe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/goptplisg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gvmxsomsn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gauuobpif.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gzajzpahn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/glsbkdmgb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gwfglxoxh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gadthtmrw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gsuspuluu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gyrujnptn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gmrnvjukg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gififgmbs.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gpdkuyjyj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gqlwirgzl.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gmqffeyhg.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gehorfygp.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gimvrwewm.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gtmgvkmne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/ggmywhfcm.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/glarmraon.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gurlapeqe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giidzjaib.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ggnnparrq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjicyicwk.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gepohrnpz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gjaqhwpqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gvcqldgor.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjcfxtpxq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtjfmujye.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gbmdhvoee.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gbpjjilme.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gtkfsqvvr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkarallwf.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gaxpqiizl.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/guhdjuewq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gzfjcjyxe.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gzavvcvak.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gprszdzms.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/goaaanlow.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gutztqnbl.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gbfrjficf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gimrjmumz.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gsetdiyil.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/ggmigtwzf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gdigchnid.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gacqvlxwh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gbxybjseb.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqmmtnkjg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/govatftqx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gjwwkjhjm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpjmsfedx.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gjamjbstj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gveebjped.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gifiryxzt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gtotwqnsb.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/glefcwpdc.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/glsvuygpa.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/ggisqgfcp.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gaahcavbs.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzgrcaeuq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gxjdcgubc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gieeynoxt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gowgeaxrg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxychpilk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gnbpreauo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gaxariwqr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gjtigkflj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gwqckdvvm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ggtdxmesl.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gbyeudlvt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gugyilgvv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/glayvrvpx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfdzgxhfo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxkvzyxqk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwmiullpu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqezncqox.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghpfgnzgh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghbpsbidh.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/ggnwjjxjx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gjkomqnxi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gvfygjhwr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gktkwxwth.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gnzbnpaiq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/giuosyvsg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gngxbtdhy.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gjzyngtpd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gfsrbvokl.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gmbwefdee.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gzwpgvzgb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gxtjrqoip.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ghptuisuz.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/greodnvfu.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gsesbnqsh.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gugaalvtw.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gfobsfing.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/girjktuqt.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gyfpkakgn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gmmsjzcmw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjuemvsbq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gbuombvlj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gfcakygsb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gjzndhwtr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gxgbvajbx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gwsiajjyw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/geoyxwhiv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gdosrlieu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghghirwbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gqrswzwlj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvjnlbqdl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/glxjwkgfn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gpebxucps.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyzoouilk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlseubmu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/geiknyrmd.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gbbfghxoq.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gdwyrqrsa.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gsbeuoxxo.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gfbxpwqzo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghgntyxgk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gxlhatjuv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gpiozwatd.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gnvbxxzdk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gorhasckk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gqsspujuo.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/guqgfjflc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gccbvtzrf.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gdarczeka.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gkbkbquai.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/guwyrvzde.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gaenyhhos.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gppbgjdwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gufcxhlig.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gmwoqhnvn.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/glwsvwlul.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gnzutlaaz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gmnoanfcu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwcjrwfye.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/ghksrjruh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gzdhoykdb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gkderkohi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gjtwdphvo.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gayiwypir.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/glbmubzgn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gnjfvyzcr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/ghmiuwtnr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/grwxxqymk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ggyygctmu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/grhlxukeg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/ggwrjnzli.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/geyhcikko.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gjjkmenug.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/ghjwuenfn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gzyrluotj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gfmgpazxl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkzgfruih.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gfdociind.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gqsxvgbds.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkznucmik.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gijikmtjw.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gguxvjvqt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gpwkwvmov.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gfudqzcax.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gkiiovdlx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbofavmty.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsdwdlvm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gphmrtiwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/ghghrjcrb.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gzrtivgyx.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/glgbzrhpp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gcuufjlxs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gcequhzqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/glcltpzfj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gwbhhketc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gdifrrphg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gmgcpangi.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gjcfioacb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/ghlwzbpkt.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gxgxnwxpj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/geekntzez.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gmgxbivzs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gzuwpwxfk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guyeqlmjm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gouhyxcsc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwobworei.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gjrovwnso.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gbpdegsua.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gyhiwukpy.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gavwkrhtr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqhzctbdv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gaikgtgob.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/giyzvbpxh.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gslxxoobi.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gvtqpjnmy.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gqafbljve.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gyritayfr.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gqkatnscv.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gxzawnltl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gqrgwxpmo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gmcmsdonx.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/guatitjft.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gwdonrfts.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gdcziygnx.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gscbhiaqw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gwthsvgue.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gasmppxcr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gycfekhyl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gizgorwgf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/guzcccxmv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdclzolqk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmldidsku.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gwuacsqfw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gderfqvux.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnuakkvxj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqezspjux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gckpbbzif.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gksbsvruv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxoysjgre.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gfloclczp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/glrbhetof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gwmzcijdz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/genrrzztu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/glcalxifu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gljhzlkuw.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gzzxanagu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gifzqauys.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gowkayxzk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/grdzwsvgx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfocfyaxm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gxdopjnys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpdzgiy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gcwekowsf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/giwdehfke.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzzfetsxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gywmhfzyb.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/grocjsozs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/geiicmslb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqigicpk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gmuacbqmu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gcuiqevyd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gomijbkxs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/glysywluj.sHtML


<!-- 参考信息 -->