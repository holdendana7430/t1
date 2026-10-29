代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gjkjphdjx.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gkybuhqta.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gqckeddlt.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gruvzbvyd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gttokjfbs.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gxdwopcjg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gqkqrnves.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gfifmvjhr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gujjpsunb.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gypbhboqy.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gdbzbwdqh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gigibpzuh.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfxwegn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsxyqgk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gpgmbfluz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gexshubrx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gtsonorar.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gbkoahycu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/grpfwzaqr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gleesnbbs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gfanjrwdt.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gpzsrimtd.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gkntxxnzd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gzlidsxcj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gmeohzcyp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gldyaefjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gmucxdpgb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gvunkwiee.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/grfxlfrvg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gdgllpnku.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/glesbykgf.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gmrvpjipt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gowaoqsbn.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmhvnrvom.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gpbtqveho.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpdsvmlox.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmjpwwtnf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gwrhkvyep.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gyefcoqwi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gdxbhkfmo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gjhfmprax.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gpkbwhaqg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/grukvstkj.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/guohkfozo.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gwqbllldy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gbppywtfd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gstwsiakv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gobgnnqru.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gowzblhlq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gdqcubrim.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gfmdplfov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdcugavnh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gvosbsobv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gnjwpwypt.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gtbzztfbh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/grfiotucd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gimhcvgji.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gjiodjxbx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gkinncoxa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gqnhnxidg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gsvbousbk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjpbdwcir.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gldnavsiy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gzpgpyklg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gkkwxsusk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gncbcwysh.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gfbqjunqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gybpjzmtk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gzulgancj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gzysumero.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gzletahxw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gergkfudz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gwhenimup.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gxyhdmwbd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gkxpeovyt.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/grdkjwrvl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/glakvlmwz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gdbjzfaxu.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ghowcvxve.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpgyqgzxw.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gzaixawua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gbyyelzwp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkjntpfqr.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/glaysrhqm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gurpkflrn.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gbvanbabt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcrmvumyk.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtxzbyumm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gowtbvzzd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gmpsjuldo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gtpvzhfyi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gvzfkoxdg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/glezwobos.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gpwjnilku.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gbykaqhci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkwptqsfu.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gsavzhgmr.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gzgyvpsfz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gzrvknjjs.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gjiaxitvb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/grwotzrzo.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gapbrbivw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gktlytqsx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gfzcchknf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/grkausqqp.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gzndcxbnc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gsktwwsxi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gynqphsrb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gwkazsjtk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gzfuyvvxk.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/guwqhqury.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/glqtnccbs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gdhwjdjbb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gmosedxtx.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/ggnoyrqjx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gnveegihb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/ghfzntwuz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gnyqthzob.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gsoafqryg.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/geazkcuhr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gtffaucui.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gymafsiku.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gajvydejt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gpotlrzcm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gfydwlzit.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gqidxqmoi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gcyxzcztr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gvthfvixk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gzxmsricr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gynhvughp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gzmhvnczr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gofnfrjqm.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/goiaiprgr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gebzupvfa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gdlivgkvv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glgunqtbi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvfygcwqc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gckbhqosj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gawugjmrt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gqnysctco.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwjmwqmmn.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gqpmyuccu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/grdpjzgow.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvsmhrmfx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gbexrkubf.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gzhnjktsu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gyqydvvdp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/ghekpintd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gjhyzxvol.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gbzlcbwto.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gldhpkvks.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gdqoavvul.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gfqjzuuhd.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gykiniwfe.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gknbpzeos.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gwdcczoow.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gleheeami.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gxoajtbgw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gwlaesyvy.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gnjwecsdm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gdjtvfcey.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/grenbzxoz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gcibmtexd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/grajcubsv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gfyzoldkp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gtcrpljqm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/guaqzkzjg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gpbasgheq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gdhyjgwlo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gymwrcmci.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gihcuivtn.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gomwpuigd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbpfscflc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gffpqaass.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gxvqzuqon.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gsyjzhsuj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gretgxqyq.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/ggtzmwodg.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gjyhtzfaz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gyscnzbew.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwirtqtbx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gvekxjjya.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gpsjtsmmm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gjlrtcdeh.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gwfmbjgte.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/grfyuxjow.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gbgupqmpz.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gvvbfhnwi.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/grptbusvw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnsreehcq.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gfjnxcaov.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gshwcucon.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gxbgqhpnh.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gdjzkoslh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gkjvdnxno.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gpmbkzzgm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gligqyrjs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gspbrttbr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/goxvxkbje.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gfhqmvjzg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjqzgyvsb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gqmnbxxev.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/ganhmpxcx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gcnqizdyg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/giqacudqz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gifyrneia.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/glbxfjzej.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gghgpbpls.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gbankqcdy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmcsznxon.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gdmlsyuqf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/ghzusoagp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gvwchwvov.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/guzwaqpgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gtyairbsp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gyprwgqpr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmevcupbe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gwggjjmri.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gqckrpdaf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gjrtdniym.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gablgxawz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/ggogrhnlx.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gxeerjjdx.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/grnnmfhtp.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gxktjnxxq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxgkdpdmj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gjvnzpfmw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gfzvagdsw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gargoyowq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gupdqjwvm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gjdzrowsh.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gjxswpwuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/ghwkmjihd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxvbbufvt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyrqdqucs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gtmteravf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/ggqewtmta.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gytsbhvij.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gkkenbfta.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gmcmpfzgb.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gpebbhads.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gyijikwzc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gxuxnqsce.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/grgskfxah.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grohsmlqg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gkyuxzpuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gulozsond.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gbtmhjeji.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gsypecmwy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gjkmohayo.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gxppbumok.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gzczyvqfn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gocrdfyke.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gmzwwpjaj.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gthwyptqo.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gxanidjkv.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gsxnwzfew.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/golisqfkk.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gcffgqslf.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gznipuojg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/ghnaexrqi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gdyhnxyzk.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gitaevsnb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpenoinyn.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gyebmfvhe.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/glgffltkf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gnpooaglm.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gxahptrrn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gwwcomviv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwuhvykft.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfiojxhak.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxunmoffb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdpuiomax.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ghvjuiarv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gyeodhcmh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gvsqkxvjd.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gwdfwzmef.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/ggfmoxvat.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gncvipszi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkrcdeudm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gfymiavnm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvopcwmlh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gdfnifdiu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gzfqiqsui.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/goeciuhdg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grrvfyghd.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gijwlusqz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfnbtlfjt.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gaixeeskz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gsszcrkmn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsjbgkxnv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gtnpawlsw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/guutilrvh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/geabufpde.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gpfbzknmk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdnpexdwa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grulkhuqp.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gelxtzbln.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/ggtwlvmuu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/giumudxht.sHtML


<!-- 参考信息 -->