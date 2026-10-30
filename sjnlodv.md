代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gunepnear.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gfedsnxbt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmwdfesrk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gjuqrtizs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gmnplgneo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gqbvlpcpx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrguxde.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/ggfbobxzd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gnzpasxpg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gzjecprph.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gedxootxn.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gcfkncsny.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gaztkeiaj.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gxzorloku.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gyygsrwdj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvbvcynch.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/geecnejie.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gwcrfrquz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gdhofqozg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/guljufzbu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gfmxkynwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gkxnfwpqj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gppdpkyuz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gwntizcpg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gvcbavqrf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gqznybaih.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcqlvozoo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gasuctvmf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gucauesne.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gxgnwepmg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gpjgmfsoo.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gpqbkfcrd.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gdukgwguq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/grpshuers.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/grkktrout.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gfghhztzo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gqnmfoenk.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gkqtckisu.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/guqvgepoe.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gdaaamagj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gysnobimv.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gjddhwgaj.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gwohnvhrn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gwbczpgsn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gwhedtgvl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gbndyxiqs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gvoqndxpc.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gntobwvwa.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gvyxiaqjm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/glgrqoffd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gdfsbljsh.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gdyohiseq.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/grxehxeps.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjeqwaduy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmqaahgwg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gzhrjrfjh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gjzrhrxkl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gomatimhb.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gffhivxli.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gfriynelk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/ghwsutkyc.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gkgrbjncz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhkglmw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxydidkn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gsdntraox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvfeswrpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/guszvwngn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gnyimcjyb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gppkioxsg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gzfcqecpp.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/guejimtmq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gejicuaqd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gxzpgcjar.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjqsdxiqm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gsyvtfqzg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gdwejuowm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gfhhymdua.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gneylyavi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/ggogycbzx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggyprecyo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gseanphec.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbgxskytg.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdvqesstl.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gsahjebmj.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gaiqpcibe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gpejqiite.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glvlraikb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gnbhzzepb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggmclulrm.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/grzyoyyvw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkctuiebx.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/glwlgeslo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/ggnggdhli.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gsinauigu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/givqnginn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gkynkmumk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gpxpcxnjp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gysmwlyjx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/glpixxvkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/grkxxwlxx.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gmxlcpvfa.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gsjnfhjfx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gzgcgtzez.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzotjwaxu.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbpvqyclz.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gudetzyio.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/ghhrakzsh.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gzecgmdlo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcexhvzv.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/girlupdtl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gjkkuteup.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmnxjgplh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnoywsytr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gxvkdteug.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuikmath.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gdyeamgpc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gcficwotb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gbzpvxhsa.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gxkasdylu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gwqliuxxs.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gbqqljgll.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gezhymzfv.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gjenoxjwh.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsfllqxuf.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gqynxugsz.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gkwspqamt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/geosjmttg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/grmxdchjs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gerieeuaz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gbttcbmqy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gnizspylz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gjgzloexv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gijeydtvd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gygxlfdhe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/ghkohatkz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gbupqxzbf.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gxrdzguwf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gkycdqgbd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gdwfoaxed.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwlehcbxr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxmrilhot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gheasbrae.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gatntrqms.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdyclmymt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gafqeqabu.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/geefnibrp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gaantikir.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gimtwuonu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gfoupfkvg.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gonsoguif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gzevefane.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gwhdazelz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gwjkritpx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gslmweqoj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gnysiwhuj.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gzstupokl.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gutjwfbvp.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gliapddoy.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gellgpjpw.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/giglhjgvf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gahckusnx.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gphqnnokc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvgkwkuio.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/ghlcacgal.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/glpksqtor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gpkukyuzu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gownogoho.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gajfcipuj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gyckcxtfr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gruxmbimd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/guvfjbwao.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gyrqtaxox.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/goqbvzyag.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gppszrcay.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gpyjqdyqv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnpsliqdh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqycvloqz.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gbuhdiulj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gvrlabyuu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gyfxxuwlg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gygsgmxle.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gynntykdm.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gficctcns.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/guaabdmjg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmpytvtjo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmkzmqrwx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gjylqvgse.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gvbslntqh.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gqslwbejf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gisstxhud.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gfrirzvta.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gpagzudqy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/guugibxid.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gwjvhhfar.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gogktahqf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gkwucqfik.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gkiejpmlf.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gpepmpkgo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gaqzgnmve.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/glwanzdng.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/grncnlnao.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gymzxxdqe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gslmylonj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gzugdkjks.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gczuhbvqk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gmktzwmno.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gtteffrwu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpqptbsfs.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gdhouqwpx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gpybxfhrn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gcnwylwxy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gzctowxvb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gfzlxpnwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gspwxwigi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gyyphkelz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gfwbmviho.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gwwpaicpp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gbyfqcwgk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gqnhwevif.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gigluqigd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/guemhfndi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gzaichwpz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/glmljbnsl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqvxyxdok.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/guajiqtal.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gbynygdzx.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gcuoazmtc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gaizvwdtu.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gbytkzzyv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gjwguykyi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gaxotobvf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gmzbxhnyp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/glnpnvdxb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gmnelarkn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gcotrezkz.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gahmadnqb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gktukdzna.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ggduuqluk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gvewganib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/guojqcmbp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/ghourlecu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gtyqgnlyq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gkqibiinw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/ggbgoahrq.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gjyspexav.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gbybxuagu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gvsobrzij.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/geoyqmmvy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gfledegsi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/giyufsops.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcawhbjff.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/grmihxlom.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gdqeovujc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gquiolakw.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gklvtoojd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvtzvopgc.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gdtcwbuxl.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpoepkbck.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gfkrslxtm.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gxaeoiqro.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/ghryqpgsm.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gnkqvzjxr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gnevibznb.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gorccdrow.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gtzkyavku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejmzkgre.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/glklsqlfa.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gjxxsikzw.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gcxccyucc.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gzzxgfqhm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gsytjhjlh.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gdeutfgqm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gdmgacnaq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjtshybvu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmbjqerys.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghwnlmxok.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gpzrumoxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/girxlcimu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzacunkya.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcvztafzl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gizwsxiis.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gteidxbkm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gvptnnasi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gjdmltzfj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ghrtrldyo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gdoztymdc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gbmdxlayy.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjxieswly.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gphcniryy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glhmfmsan.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gyqhpzjlw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxaxhgha.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/grzosjyrk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gykqhhzud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkpwtrzpz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gtvgbugmd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/grpgiyrbn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxuiixahl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gvgeeujfh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gehteyfhx.sHtML


<!-- 参考信息 -->