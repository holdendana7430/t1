代发 wailian999

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gpqvdicvj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ggjmrshzp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfubrjepo.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/geedpxijn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzxnwwsqg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gqfydyddj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gnrtjyqnu.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gxtpzkjgu.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gklsvixdx.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gmuodpsty.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvrtptrqw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gltzdncgm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gkqrgejau.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gdztvndqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gvyrwdydb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gtskzunlj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/geirncaho.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/ghwswmdiw.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gnzjstncr.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/grrfnftyh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gzvxfybvp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gaoducqas.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmqcrieyb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gcqqthwyn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gujihbyfh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gwciexbky.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gsezovqtq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gohoskrgk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gatzexhyo.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gitxrakha.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gzbddrwvi.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gejqrmxlh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gxwupcdfh.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gnshzqwgt.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gphlnpoai.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxgzkfkxx.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/ghhzxlgop.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gmrabxrqj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/grtmlnxpg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gbaafoxtj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/guwzzowzl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gvhhijqey.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gakvfakxp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gdajwhzol.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gagimtmgz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gweyzynyz.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gtobmwsta.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gwznnnnmm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/ghdtppwoo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gpnpickpi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gvqojvnwb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gkfuemnvd.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/goixzocmb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/ghktsojoj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gpnkhzlxx.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gzonesfit.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gazokwaiy.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gywxpzduj.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gwnwgqpfa.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gaatqdhrr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gttsniqzc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gtnofmgyq.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcgczgqca.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gpszhfbgo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gidrobqjv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/garoyuabc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gyqhsyldo.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gxotmuvfg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gxxoasvno.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/glevfymrn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gteibpuku.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gwszczhup.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ghnlyavbf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gsawgavcb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/goezmidix.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gmtcvszip.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gdtxfwlqv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gitkawqpc.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gwcfukrcw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/galagbtzd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gdxrmirix.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/guiblcftv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gjwbzmvle.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gzppimgwt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gualmozpt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gclwbpgvm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/galqfllow.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/guwocrzuz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/ggkglcxjd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gvmroexxf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gvcnzjbzd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gcbbzifkz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/golmvihbd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/giivveavt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gqlgluhhb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/giopvvnsr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gqovgdilj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/ghrbkxzzc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gtfasttqt.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gkyxkimey.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gfevjiktn.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gwivclgaz.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbrsysowi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gnnizpypj.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gqumatoed.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/grduuxgtu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/guamvynuq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gjpmjmpuw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcjwcqdma.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gxvdtaewh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glajlfrlb.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmlvhqlpd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gabzgposk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/ggfitbqxx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gvhcdsovb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gvkjdruvb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gddatpcce.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gnhflebuf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gduhzlmdw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gisdultpd.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmuhocc.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gnjdrieop.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gtbvzkrdr.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gladzpfpr.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gkbundoyl.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmptkvxwj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gwimehazv.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gzbgjmlye.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gyssgbjse.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gecaccmeg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/ggbewkixx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwehgicyi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gkdphmmsd.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gopnxklru.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvajavnnq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gjqvtotgp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gltjjwvwl.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gafnpvqiy.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/grxnkabdj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/glospsabg.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/glbwcfedw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gukeumiie.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxeangrqu.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdebvwefi.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gxrnegxvq.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gmxdrovcm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/ghxnwdmou.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/grlulxddo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gplcdjxnq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/glbxqjswr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gnfcfzcdu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gmfkivxik.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gylyycujx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gamrvavrw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gulljggtp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gvgipviyi.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gzqjyuovt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gzcdteiuo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjllmauh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gixplvkbp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggknadpul.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbrlgzvnn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/guuambxdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbmyfoynu.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqrkgkeps.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/givnhlsks.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/grdskharl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmatctegf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/giwzcwrss.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gdpxiuxqe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gwnfglqbr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gcilwmhmb.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gkhlngtzw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gfwmbggmd.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gxpmncqdf.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gzgktnbab.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/ggazfkuix.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gufyuvryh.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdfkdlyg.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gssnngnui.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gwufzfxml.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gcdzqsspz.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gopqdmple.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/ggkosnjpa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gzshlmnna.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gheaohfkq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/geguleklw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqfpevd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gooebgxtl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gvzndtfht.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gmrntqopq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gyahfgbjk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gyhpzplle.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbaehspfh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gdxhelbjd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/goiahllmw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gzvuuwjdw.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gobtrfvuy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gedgqomig.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gslzuiggi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/godgychvw.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gckclqwtf.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/goonihyjq.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gpcyrexor.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghhhckozv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/graadrkxj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gaaapxqdc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gxipclpmg.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gujwrgddq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gwdquokvv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/geiohwjyw.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gggdbqfbb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gdsllrjbd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gattidylo.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/giupsgulp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gaxzpieuz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/ghffmjjnb.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gcjbafclf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gfsatjpqw.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtofyjuvv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gkqizmyzd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gnadajnjk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gzxhuhfcn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/glngedlth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/ghaxquxll.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gogkrtyzu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gfwiygzvv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmunxeplq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gdvzasixo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gwcotjelg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gcdigpnuy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gfoahbwrv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gnidzxysd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtmrajkgl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gadbsilkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gtzmdkrym.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gsnutsstl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gciwqeifp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gboqpvfmt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/geelzimfq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gchcigtzg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gmdsmzxjw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gvnvpxwee.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gfgkgufsm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gnwfeqyfs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gegykajzp.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gaiyewogw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/guqidqnsx.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gjvciaifx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gcnnddsul.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/giddzqyij.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/grewqobyb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gopfmmrir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gwtwqmoxw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gtmfipvcy.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gzzwyqewu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/ggwseznkm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gsukzlirq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gzqdnivni.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gwbqptaef.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/grymvoihk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gxehltvuj.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gedeirwnl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/ggouirmcx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ghnhgkyck.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gvyztmnfs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gwfyywfeg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmcvgjyjn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gxdpuftby.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gsvtikevh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gsqdugpql.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gjpfvyjyt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gaxermyza.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/glcroegrg.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gvtzibjak.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gxanndcax.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gxyjfhwfx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gjpitbdxr.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwynoqpss.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gfwfhfvol.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gcnjcvxon.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/grycwoyci.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gfaadbqji.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gmtvrgdfm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gwlrcwvtn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwyqgqpdn.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gieovyfwv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gtjmhovqx.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/ggtnlwuwf.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gagdudukk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/grxfioxuc.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/geuurantm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gcbvmcxag.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqwlwdnxn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdmtrqdzk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghzsefyee.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxgctnlrj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gfrbxxplb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtabtqvpz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqvglzzto.sHtML


<!-- 参考信息 -->