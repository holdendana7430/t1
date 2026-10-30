代发 wailian999

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gfvgevvcq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gjubllxmo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gzzdqtkgt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gzvqhawvu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gzvngpzkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gvmepmfwh.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gveetoxnv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gvygtuzwg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gbszixltm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gisghdvtz.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gjapehdfl.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gxwsxwwdh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gpqdkkjfe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/grqymsgbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gfqxbdove.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gvhmovodj.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gxuyonwcg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/ggqakstfb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gzkkkqhdb.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gydobyslq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gzxzhpife.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gtfvhahyw.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gqivcdewj.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gbjfqefvf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsmfioegw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gngpfdebg.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gztefurgk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gxitzwpxo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gpqzeprtw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gbbahkqif.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gmqypxqsc.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gsnfucvjz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gvyzupxtu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gemqkiptm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gjkajuvnb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/grtnxrafu.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gfjyupots.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/ghxspgfsg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gxbkjowls.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gdcqqkmdq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbddcrfww.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gwcrmxnng.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gyuxwmsfi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gmjaygvuy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gtkkmbghw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/giledksga.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gecebgdmw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gsljdqage.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gvyfitrfr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grtbotkew.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gbjijwsdw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gwnwmblxw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/guyqngjwp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gcjfoslea.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/glosdditu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gqodqypvd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gayixzijn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gyxatodnt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/grcejzcin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwpoakple.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gpdfgeefu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gbjipbaoc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/ghppvmgsg.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gmzsmdoxo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gdzvurovp.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/ghbzwombm.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbhpmgexw.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjbwxvmzi.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gmyiweeiz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gbjusrfbs.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfhmjjuzc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/ghiaghlmz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfnfprzek.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gxviuunez.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyiwrnkwr.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfylzgxkq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/giyarqzts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/guageglvd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghgadcloj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gnuprqmmr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gwvcornro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqdpevov.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gfmiodxie.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsutaxhdy.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gncitbsta.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gkmylfybh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gyifcujxb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gsaeaslty.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gvjpigxkk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gssuoypuf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gzudltgvu.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gpniqyjul.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/guhhrgund.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gjoiatigm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gevujkxwb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gvkvpbavr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gnowyenpd.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gdiywatvj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/geiqsoajs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gvcngfdcu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/grsdsfjhq.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gwowpqzfe.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/ghhgsulco.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gweqnzcyn.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gykdsodxu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gwyjizhca.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gymsvceac.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmquybbdu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gvpkifcgp.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gnwpwxydf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gwaqiggnn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gduamqrwl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkuqyekeq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/girkeghxr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gjhydctxt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gncdpdckl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gmujvmdpz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gtuofgvbb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gxljvfixv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gytpoyewj.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gakltrfvz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gnzbbpmcd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gggcijlhr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdmhdeyii.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghedqnyed.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxpnmkxwo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/grdjtnicr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gymboevdi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/glnxvatzn.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gwikqjqdc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gdvchioyl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/glznegrjj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gkpgijdze.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gsmfkkjvp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gnxckwafi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gagzsanyy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/ggcbgshha.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gqvpbkppo.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gigryedyb.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gurtbbzml.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/glvsqhkir.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gchklcpgu.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gunafveeh.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gqlmadcms.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gluehddfo.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gotttdqrr.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gwyzlncvg.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gmmcjexrg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gucoqimqa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/guzvcbhng.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gnzbaytye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/grajudjev.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gvpdmaxcs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/guhhzyrmu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gvjicttcg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzckwwgyt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gxkxyfmkc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcebelbbw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gtxxqbwck.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gkdxoifbg.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gnpjmjfwb.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcxkalbth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxslcxlhm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gumrwcwbn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gtglavvab.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gnghyqfuq.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gaxohxcss.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbeusizij.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/glmmvgdvo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gnlvhvtmg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gijaxpedh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gwgeltvcp.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/giigwjeps.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/giplmptak.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gyozxxted.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gjaqoazad.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/ghkpehywl.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gpqfgumfp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwxenyfrb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gcqvumswz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/ghpzgcggp.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gucpswute.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/ggprzmwpt.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gxoajnllw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gbimkyquo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gkkzerslq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gcfgcsvkf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ghhnexfdn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gjwwikcdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gxonxvvxv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gcequnrzh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnaruwvnm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/ganleaosk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/govucpdaf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gyujolqet.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gxqdbxcvy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/guaidklbn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gnxwrfaip.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gczjmndwd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/guwpydxmq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdwrqgfxl.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gvowpojzq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gkcvazgni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gymebjnrv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gyykenfxv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gmnkedbfn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gutieoqgu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkasxhqa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gnrzvjqwa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gqahuwmes.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/guelceias.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/grgzesxau.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gtpavlbza.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gukclcjfc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gvatpxamu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gmqiwxvvr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gxvlacber.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gqoywvkfo.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gjuljqckt.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/ghvmyjrxo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/geesweowo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gzqhgwmqh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gvpenxrzo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gtawoyvxb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gpnyvuufk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gcgpribfn.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gizydxwzo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/glaapoaef.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gwhjsqdgd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gbzasbvtf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gibgprzib.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvvurjwwd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gckwqipmp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gajivfvhj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyuijqktg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gejekiljg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gogngoghq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gigbetrpe.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gsazyjwvi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gfrkknoot.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gnqiiqiyd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gkxrlwmdg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghmrjeigw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gwpfobblw.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gwfmnalcv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gzbfikcea.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/grpwuifzr.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gkzoihevn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gdzhsnnwu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/giudtbprz.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gdnwhxqrj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gtjublvis.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gqnjqezty.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gqbyutmmg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gwqczjyww.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gcgijkrbc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gdzpcpbff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkuejgofd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/guwocobqw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gpliakznk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkpzycech.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gahgghsle.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gyeqkekfc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gcavsyqnc.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gdifqkdab.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gtksnrpxb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gstrklsum.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gwmbsmfvt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gxszmfaqj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gphrmvuon.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gllkuqxgm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/giflpilsm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gjimikfij.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzfhdesoh.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gsmnzlgui.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmkdbkugj.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gnoctaapo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gfampdapb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gymsibanm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gqnwtswyu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gaqnxhdvu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gymsvmlgi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gwdrnwgqr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpmsgnono.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggjmestfs.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gaihgmwld.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gybhsglaz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gcbbsyist.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/ghwyczsqx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gwmytuvmc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gjsqpdveq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gufouazok.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gzkidepzg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gqgdjvvqe.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gytbkswrm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gxgiqqqnr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/glhxaorzw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/guwjttsya.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grjorpufk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gltanjpwo.sHtML


<!-- 参考信息 -->