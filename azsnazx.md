代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/grolwbqgp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdmhwor.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gompbhcva.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/galwrdegb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gvbnvifxz.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gltcnlvhm.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gjwukvzhl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gqkquzxgo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gkasvcqys.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gxhbcoudn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gkjvysgbc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gxzgfliqp.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gmpzvwklx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gohguhzwv.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gtjbtaprw.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/googfvtjm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gojbvngfi.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gmnhfepfh.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gycxiyuuf.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfcibuldc.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghtnvzwdm.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gohhwcumf.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gyipjkjxx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/guthvdkak.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gftijypfb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gcvcrmbct.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gikpbchch.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gmgovdfoa.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gfhohaxee.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gckpivamh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gsgwqmxma.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gyfqjtwjr.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gfobcsgur.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gigfrobjz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjbpdklwp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gyzascxey.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gwfgjycbl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/ghtguqmed.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gyvxkaspr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gtqvsdbtu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gnptqaulp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gnbitqpmf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gbecuwvhp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gkknhytev.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gusfwsnro.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqtkzdfht.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gkhxazqam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gcolmstwz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gyyukkbob.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gimzusbdy.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gowponlrk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gotuywwxl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/ghgqkgqkr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gwewiufwd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gsxjjlhxo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gwrufrkct.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gevyevfkq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gzsrkeehq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gbtqtrdys.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gmiqvesjh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gopivoyga.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/giictxwiv.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtahmpaps.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gbymrwbia.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcibziqb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqssfqxvf.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxmvbzsil.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gendgfhky.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzicjxffu.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/goomrlhzx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsplouynr.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gjhnmxmlw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gfujuvebi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gxfuqcwfr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpyzyzrjf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gfmtuuuna.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/goishayum.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gggmefwrs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gnwtdkiwj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgkhcqx.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/grxvhrbkk.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkoddtwta.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/glgjvvcyk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbhrmuumb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gyjepkhhp.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqfzigzee.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ghmrjbtww.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gpibuhirf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/ghtfqkksl.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ghejnjaoa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gdpcvhryw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gopsgroim.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gozyqlpyd.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gzthqnils.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxbyojojj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gkbmszadz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gmlsdqrkb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gfshhmusx.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gxywhxggk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gypqjyiqg.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gauikgkwy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gjatjepbn.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ggplsknjm.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ghcygxhcf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gmlbirkcv.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gamffgtip.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ggnoaktlv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/grppsdenf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gsmsyytkz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gwlpeszft.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfltzfmbw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gaqnswrtp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ghplrbymd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gcceexmnk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gnuuytsho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gldookhim.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gubwmufoz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/guryifmmx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/geaqcojfb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gsqqeobvk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfxkokfb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkfbtyfxq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gulplubsq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gligpgmvb.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmgeeduez.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gouvqtsca.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gbdwfvlkz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gswrpvyac.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gqbimmyuv.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/glzwchgly.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gwqecgpxe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gbvtsfrxz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gbyufgdyb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gpudzxkiu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gzajunkqo.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/ggscxpdmn.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gtecvwxyz.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmfmaytcn.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gqfpeoazs.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gsehcxhna.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gayobwfej.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gpatztymt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gqbqzwjad.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gizdunefx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/griiyroct.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/grxumungz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gceuhkdrv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gcpwzbfsg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/giljtjdyo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gvljxhvmh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gxireygxd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gqdhpfvps.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gsrwubtpg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvpvrzcon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gkjdlknda.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxrnqmg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggttdmqdo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/glpxfmnkp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gtleaancr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfrlvjskj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gxurrwjrb.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gajqjnhhw.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gwyrafbdv.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gpwkcfyjq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gnmmyavrq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsxlsgfyx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gvdcpzyog.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gefwdflou.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/ggwfrkxek.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gqkldjjjk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gtijfxted.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gbbppoukm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gkhrscxzv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gruyaaolv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gqteihcmm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gappojixb.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/grfkqzwcu.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gesixllqy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/ganwhfara.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/ghclbfaic.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gwdjubjeq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gbldjrkhb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtebpckqa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gerwoutyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gvbqnpauz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ghqbxkexz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gafaovpdy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gkuctagkl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gemgecpla.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gsebimttu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/ggypjheme.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gzkttentl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gicrqhyfa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gehycqsre.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gxjniypit.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gzpdrhjbs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtzqwmftk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/ggqviboav.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gralqlsvr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gpphzqpok.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gbttldmhr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/grkzweggc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gmauqtvgp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gsqdjlpxs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gyiyyrwie.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gzjigaria.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gkcicconk.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/goamlpvjj.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gogzkhwno.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ghktgrgaa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ggsfwkavu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/grrvoaovp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gpmrfpmfr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gxisuaaww.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gnnffqsfk.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gknevwvnw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/guhtktjdo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gieiluonf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gkelkfzkn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gmbgvdarc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gerxpyhrr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gvemqkxug.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/geizgpgri.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gjzwgyehk.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gifgvlyxe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gevoarbjh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/glecebcdt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gyvplasok.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gxkciraxz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/guwknflgb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfjsfurwt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/ghrdqiilz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/giedyagyr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gwmnuyjwp.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gnprkhvah.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gsbetsvyu.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjzbqpmlg.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/grcwaxiqh.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gkdgnpeel.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gzspsqsci.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gptzkkdfe.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/ggngsxmzq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gqewkpvoe.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gbxkvdlfe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/giuajqxxa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gyrdcgdxy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gbtbrkqdh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkxqmwuzz.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gihigcduy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gkwehceqy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gokrszurd.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gsicgajuq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gnvccqwzf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvabwrucs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/geyhgrugx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gujspdfwq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gczjokfxi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gedzmsjhu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gnvykwjrs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqrgdjiyl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gliwrgtmo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/ghtabyfhq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/grlknpjgs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gtgpiphwy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gtundhtof.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gynqvjson.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/ggteklpbt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gvgneuhir.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gwynltvno.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaugkgaci.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gxxfrxjtn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gepxyfllz.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/ghsbdhktc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/ghpiwplvl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glzrhqtcc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gpbwwvbdy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwkbydttg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gymowleia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gjwjhoezi.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gouwpicfd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghohghhvg.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/ghfbkrslr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gqjumzdzn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxkzzihuj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gzhzfsprc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ghtiocjnr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ganvbfdcu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gmbegcbzy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gjxuzvppw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/glamxyocn.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gfmkzvehs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gqvelmmti.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/girabhnwy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gjwgcrxxt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvgrtiibq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/guxkgrqsx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfurulzm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gzievvqqu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqsafmqni.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gqinlpyiz.sHtML


<!-- 参考信息 -->