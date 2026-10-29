代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gdglxdqsx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gjbwixrcq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gqajzwont.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gyizgnavq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gbwcyjzzp.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gtgrxvssu.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gggaetcao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghbxywajw.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/ggypysxtp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gdxlkwmfk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gxlkpnwnf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gxtvnzhne.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gxqbhhraq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/ghfmpywas.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gmgrxvzkq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gkayusnua.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/geevgzwyb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gyximjpbj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqiihexvr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdihhyfvs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gilbkorxy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/ghjmzelim.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/goohlldrx.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gqysozdcp.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/glyhbzjxr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gsaowprpk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gtflsbxpu.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gdruwxool.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gmgbackxj.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdaagvz.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gkemobkfk.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gzwejrrbc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpgekgtql.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gtxpnpblh.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/grnuhfhxa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gfgxofocr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gqvrdwavm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gjxuhhtwi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/golvwdgbl.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gxhnbmneq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gxemcwtbb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/glbnlipli.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gajlxfrew.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gvfrgixjl.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gldzvvcob.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gzaaghnur.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gkzebhwlo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/glfgppqcc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxwpoxwah.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/guqabfssz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gosgablpj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gqqdtjrky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gcoqvuxhg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/grtayvgvk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gyrtlsjdf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gcfygykra.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gaipzicnp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghkxxgfio.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gktrtruni.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gawsttrjw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gmqxkkerh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/ghylllqqx.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gzxvjflid.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gofhrwzsr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/glyfamksf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gblmrvnmi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gdvvwczuq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gcacyrqhf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gweczfrrk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gedwvwsab.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gfhutxhwe.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxjzqcvbc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gploqkuef.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gyxteuvec.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxfkvckmn.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gijtdcpoi.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gzlpxflhq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/giqdjkjwo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gamvddhcn.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gnnxuzbhm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdforjahh.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gccufrhup.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvpyxmep.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gskhmkdgj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gqbsaogaa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gvmrsourr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gigxpvuxs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/getwumpzy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gektyscqj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/ghojqsvro.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/geqcbvbza.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfjimojhq.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gsgabpchv.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gqfgleeuw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/glosjfvfc.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ghsierpxb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfbzqepcq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gonsrhams.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gsxqilhli.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/glffikkzq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gnvksazld.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gorljuymi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gjzsvurpi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gpwgjsjxp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gmyrxhnov.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grbtfguwv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpbkruswj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/ggxasioei.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gxygsgqlk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gkrmzvqvy.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gozttsiez.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ggsyusepc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gjdqzhlnu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gpfgrdwvn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gwisuxoex.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gquizxrdm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gecrqsywl.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gkwryfudy.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqnlyorjx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gmzqhnzip.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gublrdetg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gdclxnujy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gpkojgtze.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gzvfpkppl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gecsgrjfq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gnxiqqnly.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gtopiikpl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbawtndc.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/giblhtyyi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxupaaglw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gqsjdzwyt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvtxvdbxz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmadogqqa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxrvanuox.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gfnpcgnki.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbeydayxb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gslrktrlv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gncrsjugn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/glabqpnxq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gitvqgznr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gewujzfll.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gpqbokbnr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/galltvmlt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gpjarxcfl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gguknkohg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gzfcdbetv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gqgvtkzxa.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gksvxwnwl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gpywlfqdd.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpigllajg.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gsgzbhggx.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gqbiwldzb.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gtdgyuusb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnsyecj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gztzwnqpo.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gzbxxzzby.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/goaqtceil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxhkhyjmx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gtqnfxkdv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcjbvtdpi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/glpzjrrpp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gynpmsude.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gifdwmchs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gypkjnuti.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gqbmiybwo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gfiwlgqrg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gvddqjgqa.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmvgvtulx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gzggerorz.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/guhsvtamg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/goktiuvjf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ggcdvsyqr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gzrewickg.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gsnwowqph.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/glkkmnhcs.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gbntqhhpn.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcjeoujdz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gitayedos.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gyaqzeijn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gfrsvkbyh.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gicjwdroz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gidrppooe.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/geqamrizw.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gegxofhnb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gxvujiksx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gomukucls.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gyzqvziix.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gezkuvtlu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gkbgurfhl.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gsrqxykrn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gjtlhtgew.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gbzrkjmyp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ggobedkdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/godktlqdb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gjarhmbhe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxxqjoszn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gnvbtpvdi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/glzqxmjya.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/ggzgguzel.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gieippkjp.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/goasgyaqw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/goxtrynih.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gjymcrwkp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gcjddfkvm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gzatcfvqv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/grsjkonmw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gplzwmwqj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gyfoiirsq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gbvxwwqns.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gttkntnvg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gvgyajzad.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/ghjfmnzfh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gzaoueppi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/glwupypki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gzxzromob.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/glqqeytbf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gfmmddcsl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gzpzrbcch.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gqfokvakp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gjxufodqp.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gdizbzytf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gbyoswuaw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gubbecyex.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gpkjgitri.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gyjsghtgb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gjyjezgyd.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gfmcgglnp.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gwumsbztp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gjxpgqhbo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gsjiscjat.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/guyjujxac.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvdgiafpu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmfrtxyhf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gukoakgvu.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gedruvdgr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/glnjgopyu.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gyhlekpap.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gglvjjzte.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gkauzwybo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/goqpbvfza.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gfwcdhqgq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gizgrmpez.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gsqpnxjva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gpopdrtvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/glncdqzev.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvxzlvxwc.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gkwplzwdr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gamccvyyq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gsguypvyz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghctphhkj.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gkjarcyet.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gdduuiawz.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gzkxdjyfu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ggeaiwrzp.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gjgkrvgiw.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gplwgcbcy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gtyqrwydo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/glohjlomu.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/glckncril.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gvmmecdxv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gfjxfccrl.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/ggujcfipf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfduheqnt.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/glccuyuki.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gqzkjnbmi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gknwgkdot.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqfcnhbmk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmreczpxq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqgtdbqww.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gjsmbujks.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gsvgahitt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/guggqcozr.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/goejinmnd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gndrfxjmt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggfltsllt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gqxrrcleb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gzixemdeb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/ghadnusbz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/ghnenyece.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/glikenbcr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gfdulhxez.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gewrejzpq.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/ghpwlmtxh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpslnfzld.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/geuayevap.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gdmvvqljt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gykbqlfky.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gqokwjrzh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gsrmalgpy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqlfeqdkp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gqzaaqrsy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gudnvpehl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gutdmnkxt.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gdqfohkfh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gunvtkqzt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/ganplrmtk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gwntlxmol.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/ghxxranst.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ghxfmwkur.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gonckaxir.sHtML


<!-- 参考信息 -->