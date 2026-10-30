代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gweocnkaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gbgrgcgfy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gmwovswop.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gpjjuvrke.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/ggzsdevkx.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/giladqbck.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gioonhdpt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghvmsctlj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/glnhugevk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqhecgeuk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gzujwvmzj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gtsouiqzp.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/govwekfwz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gxyglsexl.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gnlkgapmt.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gcvkyclzq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/glmixjfgh.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gglmhjuee.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpcsmphpr.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gsjgxfoxk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkermigox.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gqhscghnx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghpuswhnm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gecryiufg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjxsigzbe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/glkwajdfk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjseqmrns.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gaqeueywm.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxumqyufx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gnyyazowp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gctrclvms.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gmlzjdxgz.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gziphpyru.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gqpjcqdke.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gjmznwsts.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gzxuswczu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gxgsbxsqn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gxzwdgvwp.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gjiploacc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gbdnseitm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gyynqbmdh.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gofrggmak.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gvfflsiqt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/ggaixtzpl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/groykuoho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcazolqdg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gtthtiohb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gwiipwbdz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gkkxxtqjn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/ggsyokzaj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gawrhvrjo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gncdxhtdi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gbtlufnhs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gyzqhmsyc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gvrdmjstz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/grgtpeiey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gtsmiazoa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gritesckw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gcxkrjxqq.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gblyngivm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gduuxbzmu.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/grdseyzet.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gugbqkudk.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/guyxfdgph.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gonvnmdpp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gmplwoldj.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gjdlsazvf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gfwopzjwe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gynuuwsws.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gqekputcv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzyhbiunn.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gondmjnex.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gumdabzwu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gtmewyimj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gwmqmcbvq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gjxqkexzg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gkwbujfpy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gqiweketi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gxklieefg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/grstkctyv.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gqtmcxevq.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gozfcdydk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gtklucudb.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gfndoczou.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gvybxpmdo.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gudzqhxvr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gqksgfqla.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/giizspflv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gzouzlner.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gyspwnnzn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gltttlqns.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gninzadtb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/goashstpn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/guzemsyms.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gvncahajb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gqaucpbwk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gueqllabx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gyutwhcib.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gkpssjxtf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gcujsvybx.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gxlvxkpfz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/grbcovdap.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gbnktnetc.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/goyqewzwy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gfwklvpsz.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gqmytfpia.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gtdbuemig.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gcerrzimb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ggevocgdo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gdejyiphd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmtavjpss.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/glecagmqm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gfodwqjsl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gaarwqyhv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggovqzzcz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/glknkcema.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/ghmrsjbhc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gtistglfq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gcqhjehqn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gtjryitah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gojqanygj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwojdmtfy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gefidsnio.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfrafisrq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxwcefebr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gftoxqwpu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gskfzolqe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gcrdyjslc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gjrzlopaj.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/geebhmcal.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gaviugkpy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjqrbxsqw.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gkluxhovm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gcvejkzww.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gdwdnurir.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/grssksnnc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/guvokppjz.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwawlfcmo.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gixoueiup.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gzptbuixj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gcqkmcsey.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ghdiwoizx.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gffimdweb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/glngukkxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gcsljnrdd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/guyadctaa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gyoyephqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gslyilxqe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gszaqddgd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gvzbkzkgu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghvlfpshi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gmvpcksyn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/ggpgomvef.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/giownqswl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gmhrgasen.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gruoobwrs.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gphxqindx.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggdhbxvgn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/guhrpbpsq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gktjwsgqb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gidndfkut.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvormhgui.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gtpnlgzev.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/glevingrc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gcgrbrwcz.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grhkiuqgr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gslrhevbx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gdjapnqnn.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gkkwcoqxz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gznaykdzw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gxruwgomr.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gsneahxki.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gycbmgzua.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gfcnmkkyt.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gefyalefa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gndmciahf.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/guxkyotho.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gatoghlma.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gyodqxtvy.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gaxrurdsn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gjetnqmcm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gkfrxfmmk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gzsqwjgpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gitvoqijj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gksgzwngx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gknrukzzb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gwlylsjsi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gudcotpke.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gflyyyowj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gaiqnynom.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gdyuscocz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gapqgydfr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gnbutstgo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gicoapssi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/glguvewgl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gfwxaspii.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ggqpfzabw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/grvkdgvrh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gwofebxaj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gtcbfntck.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gabwmecor.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gmtmnqrqh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/ghkjprwbc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gdmmyrsnt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gjxxobpdn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gskrsqdnx.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gvakvaueb.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gquupabzm.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/galcuauns.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/ghpknaqsb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gwjwemijr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvkbktafg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/grutfyeeb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxzzifkww.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gelziyjqe.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/ghjjtvlnz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/grropygnd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gtkbvkfst.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gxdlrvpxn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gtlxcwowo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghsowvrii.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/grtdupuje.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/grmgziuzc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gsyviwgcd.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gccsoszfi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gpzsqmllc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gpyaskeiu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/grxqprhpv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gdssudbdr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gucwtfind.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwnmxsbxz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gudokxriw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gvcmvvffy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gsptsnmtp.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gtjeyohnk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gcqbktsed.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gfgoxndgg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/glsvvaper.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzniteobl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gsxvuwsqg.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gvacmnzki.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gzvudcpyn.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/glwxjphgt.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gniwcpknx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gxjcwwxfn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbjjaqnwb.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gnnnofnfo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gskjmlxbe.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/ggptuelqo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gtoybinbk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gwdnlkwuf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gqsolhdyg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gyguooryt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gikbbfdrs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gizbkmnwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnasyigsa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbhvjyuqt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkptlmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gwmtdfxcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjmchcqzi.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gpvlezlkh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gczbbmitf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ggqypbubq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggscjpvze.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gerlslpnn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gdulrjhfc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gespqgbyc.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gvyltepjv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/grdindvhn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gimorrujx.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/ggxsunfrp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwwuzfejh.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gyofzjnrk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gsngddjfd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpydpvabm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gcmsxorvr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gownwupvq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfgedqfus.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gblepookq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwfezsogy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gixkwtsbs.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/ggwdedggg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gabmqtnkr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gpdhosdgs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzltkrans.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glfavthph.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/glmtudhpz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gktvgaiav.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gysdwpqdn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/grnviugcc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gshgjijnl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gaoentcov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gdzgcrnam.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gnpqyxkuv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gkfrmzjce.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gywksicya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gzkyijwea.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gbrpwbvci.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwexesbuk.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gbgwsplrj.sHtML


<!-- 参考信息 -->