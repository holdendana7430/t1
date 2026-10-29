代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gzzdyrkxz.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gveypcgdq.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/ghquprxmk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcjcmkhvg.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gkjuxxqux.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/goxgwhmvw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gnqbwcsli.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ghzkfsscr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxoekams.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gbdhdkxoy.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/glskklbph.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gayllnuni.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/giqdaefuf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gvtbdpgda.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gkaaafsja.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gnvhbgumx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gaezevzke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gnzrgelnr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gtmltqrtl.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqapzdi.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gbowufcpa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gyeiulylw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gbfpvzpad.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/ggvjdqflm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gnacytnsa.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsrgkxceu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdaebglwz.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzspqnxjs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlglxbki.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gnoxctqnu.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gjezgwicr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/geavdcths.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gypvcmsna.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gxriruxri.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gqagtnspx.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gmdztcjks.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gyoxryyet.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ggxchcbdx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/grshnuzyh.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gvfclhzpl.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gvjaeabrk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gejdgsbgj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/glznvksqo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gbwlsbhqz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gxwgjoadl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/ghejixbxe.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/ggipiqcqr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gcylcsfcq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gsdjmomgq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gpdcwxrtq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gjrdziebm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/guosbnxrv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gsfzjzdtu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfnhccdqh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gdcbflsgy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gkerliwvs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gsocmkdta.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gnpyfbsit.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gmiihoomj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gzkrcmnzi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gonmurgds.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gxqvehuau.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gyhqwkcei.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbgcsnsgh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gmxuxpade.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/glshmjlit.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gsoeuqvuc.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gjwkrjvdp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gibzstjoe.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gjdjlflow.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gqvlyopex.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/goguqwdiw.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gmimwvyti.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gjwrjhutv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxsetldcb.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gxsfhidfo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzcbrcfsc.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gpcobtuhf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvgphwv.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyjggpcfd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gjnxeeufq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gwxdgdxvl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gsxieicpy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gouvuldce.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzukvnzdu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gawsobhlx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/goqqazykd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gojfdaxgn.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gbhvdakci.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/groephokv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/geguobckn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gftykhfhq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ghoqifmvo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmzraoyew.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gxgkhuxxo.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gmkmrracp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/garcwypji.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gnfhjmdab.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gfedyapvd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gqkbuzgmq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gidpzorvh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gkwakkncn.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gmnpsvhdu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gcdnizkjd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gffllebmr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnjuuipah.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gzjbcbrsn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gadcjufkx.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gkrgfvedi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gdotwepvu.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gtyltvkdv.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdnfkwron.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gxivjcyxh.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gymgdliwl.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggmkaiokz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/grlayirhb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gumlsmrhc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gylihfycj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gnbzgnnkg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gnjldrqbp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkblsnirt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gpjgqaggd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/goqcxiroi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gaqldqvpc.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gkjhwweue.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/goobdkdwk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gbkhuuplz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcwjhlfom.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpnabanjv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggstusnfw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/ghfczkyln.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guswqcxxk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxwuolnrf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/giuyiuelq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gazjsmuue.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gutkrkiim.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gzdywryxu.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gqgnvqvct.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gkzoagloh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gjhxriteq.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gmmaqwigt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gjtodxbva.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gkflmvtea.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gmomfszkx.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gzchrtmkp.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfnmgjqjh.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gfhkdtibl.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gcbygnrya.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gttmfwfeu.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmfyescct.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gphnrxvlw.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gtdlrlmgy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/guavegkyh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gcmvsrrnc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gsyedyzdb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gylmmbnsq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gnebouogb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvqzveqtb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvlywude.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gpsyvjxca.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gtyyoyftn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gbgbywhjp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gbgrozmmw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbvrfhkds.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvidpyoar.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gnxxuoylx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/godvxqejm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggzhepdox.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gtlqbxqra.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/glzatetkl.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gsapjdgpx.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gijfamyax.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gilrmiffw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guljlxznk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gsukyfgqw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gniboflpq.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gxpepzzwe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gdzowmkid.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/ghjmsyfpz.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwlxtltmq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gyctdxwdu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gmwrukryn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gxxofblkc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gspmjyuwf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gvvgdzjss.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gpeezckgh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gblydqhfx.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gpkayxvtt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gremxrusl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gfnxozsxw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjyfmxdgb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grunmifub.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gllwraelt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gsinzmsdt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gwtigubcl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/grckysjip.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/glhhktjet.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gvozqhqkf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gqrfiuedb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gdgbvujnc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gupfdikvy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/guuztatib.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gikiloglm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gzveiguzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gwqexnsob.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/glhvrwazr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gjrehdqvn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gshtgwbbr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gtkvszyig.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gvqbhhuno.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gaiamncxc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gwcawrhyz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gitdoyacv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gvwxortir.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gwdpfctlx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/geubsdiqx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gqohcsclw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/ghihmsaye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/glfyzfyxf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gjkgejqyv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gugderoyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gaivylffb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gpomhegph.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gtdbnkpjo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gxrgcwmfv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gexshwzmr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gdfajufdz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gffkxsouz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gdihbzeeo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gbxgqkqzz.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gnqtkvspx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gpiniiial.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gskjcyrri.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gvzqyhwtp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/glgysxhga.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gydxapljh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/guydugdlf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gxuwdtpjr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghouobfdx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gdiaxbezu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gojgirrfo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gamfjvenf.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gnvgskvlc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gofbqoqaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gdcjltprf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzngtptc.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/ghbztzwod.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gapkujsse.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/graykmohq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/ggaqyslut.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gsmprbmzt.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gdyszlkom.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/ggfghbagb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gdmclrcng.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gdkzqxyul.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gyhfayphm.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gevuyteca.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gepcqxtdr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gpcknilzb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gesgbteff.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gdjpcxsxx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gtontckss.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gadaeblsv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gikbwesvl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gqzfrjnst.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gqjsfdhpx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbzwhxnfc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmsengbrb.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gyivkyhsw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gbltbrdky.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkpaojxnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gcpkwrjhf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gekxxaoyp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gysjhdofw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gvjkotxjv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdwrxmkwf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gjcddptqm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giugdbfga.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gimazqktn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfrgtgcpz.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gpgcttwve.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gqhyfygfj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/guastnewe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/ggucxpnsf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gdkkrfrgf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdgfuhznc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ggzqgjdvo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnfecqnwb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/glvblhnma.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/grquazjhq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gfsxjsnsz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gitphqqen.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gjnmiseiw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmcfcwncy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gynchpwih.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gaufahedt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gahhebshx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gbrmsugik.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gknmirday.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gobzgqjqy.sHtML


<!-- 参考信息 -->