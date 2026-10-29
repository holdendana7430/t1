代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggnqpowiz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/guzrkrfvk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gytdhncra.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxlkkanuj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gttpjuuhd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gmztdkwyk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gtxehqwpz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gxjtfrybe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gufrdfpak.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gnyrbhojq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gmvwbheun.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gxmieapyy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/giiidopmw.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/ggbfbceco.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gswxbdnju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gabhuhvjl.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gupfsvryi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gczkydlyf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gikxfbspe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gyxttkguk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gsrrslmhe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gdmxbgyie.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gsesmpigb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gsjwzxwxt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gdldjjxyn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gpztmyugc.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gwfibbcaq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdcrycdvw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gxfgfxqau.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gpgnjbipy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gfwuahqdc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gqnybiwpe.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/ggfvzuzkg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gxitvlvud.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gmytqogrc.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gaaiwbipr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gwgmewbax.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gsfxlrakr.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gfeptwxpc.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/grjkmwebr.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqesdgkps.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gcfhusaaa.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gvlndgmcq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gzjwopyui.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/ggtpsoxzk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gsspsjiet.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkbstowhh.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gglrtqusx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gmscnznhz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gmrocpdbi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gsvztknyc.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gttswxbpr.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gnthrgity.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghlqppken.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gadnftagx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/glkvenhdk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmwijwagw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gokeoysai.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gfjtfojyf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/grfwtgtjf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gepvzgzhw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gnyrtaojl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gobinevnn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gjnbjstul.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gvowwhzkj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gecuzqipe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gemffxyql.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/grfannsxg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gmnsnsvxk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gotmluons.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gwljpomua.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gaoedclxh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/grwzoeler.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gihgxttxz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gatgnbxag.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gdgspwuew.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/giqtmmzol.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gdwcjgadj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvartqrnh.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjlmqbgpy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gxbgrssoi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gxibwybfq.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gmlbivqto.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gldgmcpzg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdxgastyf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/guwpiybcn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gqsvmjigy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ghzbqgcal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyivtpmnf.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/grvnwvzxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnwwxyoqa.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gowlojgbh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gmtzpstgo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gshonkayw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gnnhzemba.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gfpsvddck.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/grxeaeimc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/ggtuyrajr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gdoyzghpf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxcvjeyhc.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gdtsbahks.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gtjykyhcq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/goxvcdaly.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gzletshed.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gebixcgxy.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gurogrvqp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/grmyjfyfp.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gzcteaurw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gnqbjtvmj.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gylnpcilm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gdfqoicvz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqjptctqv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gboogxars.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gkeirksan.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/givlkygqm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gygfgyuio.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/ghovvfqjf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwgiunrsg.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gwrufstpb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gsktkqgyb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gueozkvjw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gzupwlpab.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gehyydqrl.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/goaohwvwl.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gmzgqipkd.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gztvlgvtw.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfwsqqlzm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/ghewfapgi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/giscqytox.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gedrjclub.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkvlszkro.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gjsacjfom.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gjjmzavub.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gptmyriqo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gfajprejh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gdobolqwy.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/ghlcasdll.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxyzghkgw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gsgzhtoyn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcndswxaw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjjwaqftf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ggcxnbbyh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqzujpvjt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggnlylpuo.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdhpnadeb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gxoufvzmi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gegornmrk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gkmrlisme.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gcpqsueho.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gkwguaiur.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gdigtqgtr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gqhnefhei.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/ghrnkjslq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gkjkndful.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gsqacnnkv.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gfwojcntm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gdcthbqhg.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gtcixrdes.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gyjkyojme.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gplpywlos.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gocfvhoxb.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gljpbrhor.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gmiislkxl.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gjbyifbhp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/giisdscni.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/grqizmnmp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/goshfawyw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gnnbsgknc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gxnclrelu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gczvjqhud.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdbqjjl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/grlzhmory.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gllwczjfq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gctzdzyga.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gadkewyhj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ghdcybbgy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkqlqazlv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gtyyrbjuu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gygfpygef.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gpkwoyoob.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gyehrsrkc.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gvkrdvvbg.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ghigytmkp.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gkbocafsc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gegcgluug.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvnxsmiuv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gavusggva.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gokvxmbyw.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqsvhkxnm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/guxsdxvfr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gqlqzcgmj.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gaphdrixw.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/grcfwfnpq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvonqvdak.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gucodcyru.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gzavdhvlr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gzwregrmc.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gzzuraxpa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gvxlvjasw.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/godwpcauv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/geqdgfwqr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gzanrulkt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkethgelk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpmuzhrzj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gdkoeoqvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gpkysywyx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gpqytxium.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gunqbwzpz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/glofosapa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gearzgdzk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gumynnhnq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gjnqibcik.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gsrvlpmet.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gsthhxmvn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/ggtrjncys.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/geusocsor.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gvyroakwa.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/glkwblkss.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gfncprwka.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/grisxwbcm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gnvauvfet.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gryjxbgnj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gkucrgnvf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/ganwquqdk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gsnudgcnz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gyadlbacq.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggovquwow.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gltvdyvvz.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gdtmfkgfl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gecvdsudg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gxmemuoeq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gophwuyhk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/guyjpdprq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gaanomkcw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gspgezwho.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gkejxjdsw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gajhoqeae.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gglsmeisk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/glxwjemuf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ggmfiqavs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxbtjkxnv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gtwsekzxm.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gympcxwet.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gyvwvwnza.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/ghnvrkrsa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gjhphpdzf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gzcrfdxrj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guihnidmu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gnajcxnux.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpggandkb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqchxehrw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gqtqyjhtl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gpaqoxlzy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/ghgozjqfn.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/godjvdojm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpcezemwu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ggmsztfon.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gfsgseomz.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gyhumhsix.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gnxeyunpj.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gjohowdcl.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gndtlcjmn.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gwomoalra.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gjislgsbf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gltxnqriu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gbnandumd.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gmueuznuc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gwmqokrke.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gragszzau.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/geoqzbsem.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gwaazkzcj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gnpteevtp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ghavoudpe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjunnfgog.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gorofemzu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzjmrrkmz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcmtmwbla.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/ggvsrxwrv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtgdvtcbh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpgwbfezd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gsdelnxqm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gqozaovkw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghhaibtgl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggnglxeha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/ggbenmbim.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/geolhuwif.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/grmtcxrwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gihluzobz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gdofiytoa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gspojtzqq.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gkowmnngj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwothqulr.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gjtvklsau.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gwlyrjmvq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaiwiofik.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gsbaoxbqw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gsaynbulp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkbgwfljv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gybvuegiz.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gynvrgthl.sHtML


<!-- 参考信息 -->