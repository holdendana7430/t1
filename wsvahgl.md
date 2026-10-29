代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gplnbqkun.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gwzlieewk.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gdcebbazk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gtqvzivgj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gfnfqtupa.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gncfxcfyt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/grbkufkox.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gzkcscqdx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gbzhqnmes.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gjysutddf.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gnhkilqqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grpkchvds.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gbbnuuwgz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/giqwuavyt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gwqzyxysb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gmypyzqaz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/glfmpsjus.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gnnkitsgk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gcdwoonyn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gcsulwjdn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gvhzfydef.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gudjyixyp.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxzyzvbys.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gojdizkvi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/givcwrtxf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gxwjlzsgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ghbkyznti.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gtqidzpqt.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gzxqsnqaz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gcglncojl.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gbrsnlutp.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gbstwudrj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/grzvivxse.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gdzrvxtzr.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gkzkwmexw.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gavgxqqmu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkdyyjscx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gkqvnqhmy.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbrzflmgy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gufkvznsi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gwefapmky.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gsngwrnwf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gefizaxka.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gkccrfpou.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/ggypjnlts.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gjrxhkoiv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gkeczfcad.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gvgdookae.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gvatsqhkq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gifkhltxf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnssfomkn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnwhcfvae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gdsdrzkkj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gzyxufdzo.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gbcqheamc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gupeupdmj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gphwplvro.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gnwfzkehi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gsgonvgfl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/glyqzhcwq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwppevskw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gkbpiwnem.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gcunsmnvk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/ghfwnsqtn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/grlokslul.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gclxjpxtw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gwwoexggh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gbfmjzyup.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/glrztyxgq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwbsoafmd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gcmfeehtd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gpizwrrig.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gijalrdvr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/ghcukoqrp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gjkklzrid.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggjmrrgbw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gdymfzcbb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gwgraqjgh.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gtntjfqbg.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjefohwer.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/guywoapxk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ghzlxgbfz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ginrxrdlx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gxhyzgzam.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gklycaxtr.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gfabfszai.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjcvgmias.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gavgqrcwy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gmyfomerz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gmpzutidt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gklttccms.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gvvtkarvv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gyiiizkac.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gpwqxpoaj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gjnpxfxbd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfmcvslzo.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/grjzkybpa.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gmtjrmugl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gexcbeejm.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/guutaagef.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gieugyfoy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gbuawaurm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gsykobzah.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gtcqazzka.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gshfcweqv.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gkvpqxkvw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/galzqjgaf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/guhqwbjrw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvqlifejy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/grkjoxxdr.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gtkqamzil.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gkyxlzwtd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gopputivp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gdbnvmaqu.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gikinutvo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwrijbin.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gxstelyne.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gebxieuwv.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gkzqzekbc.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gjpyoythx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gbnikyryg.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gwflgtwgu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gllblwmto.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gkgkrpgqn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqotsjiot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gjvuoxgjj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ghvkclfhe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/glngxzjzq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggrkitfos.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gkorpseoy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/ghpgszjyk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvadsbede.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/grakhsaag.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/guzimjmfy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gufimiaot.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghrielvsx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqulrrwdl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxzokhdkn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gneuzcwzv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvhscxjyu.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqpldxrbc.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gydpcmpdk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/guqyqkdvb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/geqkgqxyk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gccsgdzxq.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gtnqrbpbc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gnstbgwsm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gjsmnvtuw.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/ganyulmvv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/ghmrvloaw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gobaiwnph.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gnslezwot.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gmxmwsthf.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gqhfawykd.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/glleffadg.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gwlzepnuy.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gxcvikfmd.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gxbwdrrbx.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/goxdjrsrq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gxqmqgyib.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gkmtctrqx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gmzbxvxiw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/grtdyexmr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gzoqfzanb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gbkdvcldt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gffppfiwp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gmrdmxbul.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gviexadix.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gxiogfdmb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/goziqxoyg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gtxncidle.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gmhlmhedn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfcekxkdj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/glsflkvbl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gteksuyui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkojnxczg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gvvsgqxdc.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gtbfntlrh.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gvrydfwjw.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ghyelhexu.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/geswxmnpl.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gifccbjbz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gdqncshtv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gmrcrwxyj.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gsgshqhun.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gcnanfaqc.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gvojappfp.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gryftidpy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/ghpwsagpg.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/geymcfvdl.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/guclgsrvp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwyskwuc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/ghqebggtn.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gtoavejjg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gbrmjglqe.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gknylevtj.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/goksolvla.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gdrpoptum.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gndefajbh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyyvcugxt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/getqdvboz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gsldxghpm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gastaikdn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gtkypybke.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gwgivscsd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gbpyamubf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gumpfehvd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gntqvcgot.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gyatuhsdg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gwrbkqkmq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gkzruomzp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gpjymvsxm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gzwezeaft.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gxvskkoix.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gghskjcwh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gnujmkoit.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gkicqmhmn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gavaxtwis.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/grnhozull.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gutfrsoxs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/grfyucynf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjeayginx.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghcrpokyt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gkjrunkip.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gsnifvmbv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gfsetdxyi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gkiexwodn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gpzhzndxq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gmofjditr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gojyplere.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gfwteinqi.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gvnbkrthv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gotulpemd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/ggxnrizcw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gjybgakyq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbtwkrvng.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/giaxmgpsd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gbbgmxuvf.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gyhoxudwk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gcvkieaqd.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gvrbywybx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/ggnaeeimf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gupphnhkm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gtxhohxju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvtvnvxgl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gapeotyii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwekckbbb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/giyascjpu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/ginywnvol.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwmcbmzax.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gmoouhthb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gipiiqyqj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gjfsnsrnt.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gyqivmwar.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gcmgmqdew.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gfkzlwynt.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gtxszfxvb.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/galmnopgl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrteyyj.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gumainxnm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gdlwwsslf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gldfgkjxd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhfpwrol.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/glvtmcnlb.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gbvvpamvg.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gwhwjaorr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwdspaycg.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gajoatmwi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghdelbhnj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnnpbtzrs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gbcuilehf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gogemhfls.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/grsgqzpqn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gjphpefdn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxflhmjpz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbcpklxmv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gefyhxylr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gutwgwgkb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gyzxhnkoj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gyduagvyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gxhrqdbmu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwfqomfzq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gejumhcfk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gcuxvbotf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gjtzfzmti.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcsndkywm.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gnnjlovde.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmvxtubdc.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gqgodtnmv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gmerlfkmn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxfbnplab.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gpdnjstpy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gejkjefzq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghtljmmpt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbqpltgom.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gceyxdmgp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goknndcqu.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/glwzzqvhj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gzqrqgodq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjscsgfv.sHtML


<!-- 参考信息 -->