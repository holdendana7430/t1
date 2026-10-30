代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gnlsuqayo.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gqamigaay.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gnswppxuw.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gqfvmgoqi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/galpbsqgv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gewsedmuk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gqhsedkfw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkvxztiq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gapkzsmyh.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gdyifuylo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/goekdlpoi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gbthvmqjh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gudcjlsji.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gjetpjngg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gyhjcvfbs.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gwxotykzr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gjrfykfqy.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gsvkcdkmg.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gfsgiydam.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbpndzbmz.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gjkceevig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/glqpcpstq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ggyzrdkwl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ggdbxazag.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfafqgjcc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/givfmzvya.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gtocwnaqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gnsotnbsz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gvgaaycis.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/grxeeeins.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gmsrgqsqw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gbbuckiug.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gmqysbbtu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gcvfezdvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gnyxaibtq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gjgoozlet.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gjuoovlub.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gaitrmifi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/ghvrcjrod.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gcsxybkfm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/glbhfqyva.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/grjozoizw.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gbtlentnn.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gbkgbavez.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsyrtlwyx.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/godwziqqa.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/guiztnjwx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gexvltrfi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/glaldxmqy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gaphgubxq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/geceogvml.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gyeuzemkn.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gtnyjbayc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gqsrxpzgi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/ggdazaxoe.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/giygimacr.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/ggtzntapo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gowvnjhjp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gzqpixjrd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gechudgaq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggpzapdef.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gmhqfgnzs.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gclpdpoyv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gemnmzcky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gxkxoxket.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/glkidpqvy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gxbhlouxn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gdvjeczjn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gofmevrrv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/giuffotmu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gkrirddvh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/glyqmhqgg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gfujsdwfx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gdcevfhyk.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gmytzyqjw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/ghfujwpjw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gftwpaqro.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gtvytmlld.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gatxaxriz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gfsurvnfh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gowlblscn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/glnjgxfkn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gvytjfggl.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gfjtjknqt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbmsogbjj.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtbhncsxb.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gpfieqzgf.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbvcqwzcm.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gozjfghup.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gworxmnut.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/guwqklgmo.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gckcqqgwx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geiuyzknk.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gkjmktpqe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbxekwvph.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsfanqwyw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/ghnlyjagc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gzvzbqgdp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvhcopcgn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gvalbltos.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gkbkqiezn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gwcsccbet.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gzwaitfjl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gypgaagfl.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gpwsrfggs.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gbvtqnbmf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/guauuomiz.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwsyogjjg.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gmgbeuhpd.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gkcymbbdr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gbhlzeldd.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/grvzugrfg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/geuhehprb.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gkigxezgv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gqxttnwvm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggbwxplrd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/grbwtexur.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gpcblakpw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gieubudzh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gkllgdjlk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gwolsqifl.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gwtgeypge.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ggvuymnax.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gahgywduf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gdnomdvjq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/ggcwxccxv.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gbqieqtnz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gednegsjm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmrtkzrs.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/glesmmwim.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gsseewsir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gpbfvqkka.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvunbgndc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gjbgxfarq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gtzjgjsap.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/ggcgbelci.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gpsneuzyo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/ggnqbdmku.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gbejwfuur.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/goedreijn.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gsdspibrf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gzlivodqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gpkpvoksf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmcvudq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqlzykyty.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gojbqgvqr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gdhbxepwp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjcklbupa.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcyigmfbt.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gvyddswhb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gtpsdpcxt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gpfnlycmm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gucnciwir.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gnhufpnre.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gasqeknas.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/ghcilxciz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gcforsagq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/glvxlwupw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/ghubqvazh.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gwmrjmgsi.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/grzbectwu.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gsvoflsxl.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gvwfhhuec.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gzbaacqkx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gdlhvilgz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrneyhuv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gsnvjzzco.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gsyvpaygi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gscsoziae.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gditndjmu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gwfujcoqq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ghnysmmsp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gydoclxsl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gooezeexm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/giwiqzyno.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gpznimowu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gjeomvsfu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gzvntvgtt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gzukvlfru.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvrszpeqt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ggpautusw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsouuqnii.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxiwbgdoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gohcriyia.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/ggrjgafkm.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gjvcwfzac.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/goalbhbbf.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gwkkkptpw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guotfzlbe.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gnbgixudy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gxhvfkjjo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gvgpwjldu.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gdkfyiebp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gzhbwmotq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gtacjfcya.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/guwaqljyd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gamaucvdp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gfgkyljst.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gpiecajtn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gjnxtisgb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gyzwogfvl.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/ghmsiexoj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gvwbxlcye.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gzbonwxvm.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gellejzds.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/grrdiuitl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/ggzvpqrfu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gfyobjior.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gjdvpkuhr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gwfniaxxu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gsnwateae.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpxwgmpzg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gmlzkxgqh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/glwngczos.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gldnjbazv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gjjncojre.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gvxqgnjzt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/graclyrpn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gevhuheii.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gvfpmyrhe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gzubosasg.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/ggchuqafh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gdmluzmak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gmfpuncjg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gemygrplx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gguqadqbw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gkijgyzfu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gyueymnyn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/ggzmxuula.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlwwzixe.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gcnnqkvpg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gbbnfcwjo.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gciillbeb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gohgzrtfb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gxdgycxmx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/ghagqyglh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuyjvcr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gbztmxazw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gjyobvxum.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gklxeglva.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gtnteggzu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/ggbbtfvya.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvbqdekbn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpskaxuqg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gnrjjgwai.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gafskpgpl.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gsetgzaqu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gxwctwblv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/glnxnbzbi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gonuxqjcu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gkbhpqyfc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gicgdpiru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gctqdopnp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmilipwmf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfwtvkunh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gaxawkuzr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gseadgadk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gwqgquhei.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gmwstptra.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gysfsxaor.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gnqprfqtd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gqsmujpig.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/geqwsopih.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/geahjgddu.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gmogkeyug.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gwmzbhcgk.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/guccqpgke.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gnmuplicv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/guylkwhex.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/geqtwrerw.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gznwlmeix.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gykeyxbff.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gbywvkipd.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/glhpoiwtm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfwmysmea.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/golvjgxev.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gsvwchzhh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqnirkkan.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/glfdbrjni.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gprdjabhd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfsxcssgk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gphtuhkfl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqnjrewnp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzgzjosmu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/ghwnorekj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtwzratfj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwhzwkskf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gkxohskxy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gquasgmfw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gqplanmue.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gkbfgzbln.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gxazfuvmm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gxcevkijb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsgipaoaa.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gsrxgfouu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqpbszjtx.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gaenhszll.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gfspgdomb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gntzcgart.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/guqykazly.sHtML


<!-- 参考信息 -->