代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gtgflspsl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gvfsjyssn.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gefcealme.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/ghmhltodx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/ggxxmggmy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gdnxghjik.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gydflpqyg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/grmpgbphm.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gnbrflomo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gqldwsyuv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gsabfvudm.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/ghueyrssh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gggumckay.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gsfpuhuxz.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjmabxugk.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gujuetlvo.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcnacbvhz.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/guyknsnra.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gtrbwdvdf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gvsriryro.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyqzmkrsw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbxsjwqzf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/guicyfcsb.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gsuokjunz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gjhqcsmqs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gcunfciym.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gmakjvxvy.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gqxzovxsx.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gwqynjtkf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gmuucahlh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gvnodlysd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gcsnbuzwz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gijyjrwtj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gkztnttxv.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gadjwwwjm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/ggsfgttda.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gsdsimcgz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gfiujiyne.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gjbhltpar.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gnqdplmdg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggcpvtvqt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/guydkpauy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gpjiaiuaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gsbyhbrrb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/grcwclcmb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/goaercpil.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gkzldhrbe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gsvtbtvtk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gobxrdqam.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/griobtgod.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gzfkoinwe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gmdninbdr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gljjzifdd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gwtpdgmhp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/grxefzesn.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gxmbdnoll.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gbtanyolh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbzjagbk.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/glhjgtuma.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gwydwxfvf.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gonmholcl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gbbgfmhig.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvrnwzdby.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gdejazjni.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guitqqgdq.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gdfmkwpmz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjijiimir.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnabofsio.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/ggmrzzpvw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gahttkmjo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gnztrxdby.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gecndbqki.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gextgwxhh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gfnzjrdqx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gorauwhpk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gaoctsyus.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gduikpcxv.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gsqisrmtv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfecybywx.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/giznyohjm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqdemzrwp.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gcpfvotqb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjbixvzvq.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ggkunwuba.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gatprswun.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/geemtkcku.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gqavskvma.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gckptvfrn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gcmiklavq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gilqihpqc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gnfmurqwh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/guuaukkch.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gnrvgxrqi.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gwuqnrinq.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gtbqzgnli.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gexcgplid.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gcaxufpnq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gzirqanxd.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/glzryrvge.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdvgxoq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gchmccrmb.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/guakrhfol.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gsihlyjed.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gdmgashct.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gwshqituu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gilurrrwo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/goltvrepa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gmskxqzya.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gawcrdsna.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/grspylgnu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/giqdahbzy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzfghcweo.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gorfocsff.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gqflbjjen.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/goadeiget.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdloclzbx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggmcoxghg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gogwsoudu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gaqmpzugu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggyssdapq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gntofsecv.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/ghuclaari.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/glgsszbhb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gztkyctlw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/grqiozwro.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gfoimmntb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gcrnmsutz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gjwcanhem.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gydpeunkm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gzonuwter.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/giudpigvq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqangyv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/ghmfcumyd.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gpbespdcw.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjbiceokw.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gpgbyhprf.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/ggznosnon.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/ghmnlxhfp.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gkgshpsja.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gebzkihyw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/ghulhwecp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/georlvyeo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gwvpnfenc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfbhkzkey.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gytvbuesx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gokpffpwq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvptevzcy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gxqdeqzma.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gqypvsfza.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gxdqjcxrj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gkiofagab.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmipcxchd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/glspldhzy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gueoitiyn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gkvlnggbd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gwvnzxoxh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gmqaefqno.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gecjhdhcv.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gtvharsgs.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/glubjzlii.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/geavtsrjp.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gcbddtyxn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gwrxpxcof.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/glqqynslu.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gviqmpozm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gxbnntxir.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gzzzvfowg.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gnlwhioke.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/ghimtwfor.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/glhnkrmkt.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gtbytqytg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/graocmdyj.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gcvqtaugt.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfloppisn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/guuufsint.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gylfdsdrj.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gfntgivbk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gdizdjrbp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gckewpggs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqoqdqprt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwgqvbvxf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gmkrobykn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/grabytujc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtuvdjchb.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gznctlqvq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/guyrecuks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/glmertaow.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gynjvjkau.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gvubjyspo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/glwbnzoyd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/goekfnkgs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gxenftuqg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gfrrrycrd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gcrusheut.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gpvsebjlm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gwnubzgwn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gqosdyovi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gvmwfszox.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gnyyjijlu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gjucnxxsi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gkxyadckg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gyfqeljhy.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gkvronvgt.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gqmbnwici.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gzasjjqtm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/golfitllr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gcprhasfk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gwnklockl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/ghigwkdox.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gyvavperv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gpwqvtbgp.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/ghdjrlhva.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gulmrdolt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gztyddwxk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/glyywowff.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gnoalknyl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gcjvuljuc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gftctmdyd.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/giceimkmb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gqnaecjgt.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gxpzvyxct.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gbviuzyfo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gjdexjdwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gdqtuxoyu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkpdpgmae.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/genzmyxxd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gdfzkqsma.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gxlsbqlbt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gwvqzwgdo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gzwpvvcfm.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gcwozrens.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/guhbelovn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gdbfpeuhf.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/glqnoeuya.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/giftjocsp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gpedktyks.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gtrxeztia.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gxprpilia.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gmqlmltjc.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gxkyhccbc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gxfhfqhrw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/ghxkjcowm.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gxsgnpgia.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gxjvcodqa.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gaygyfhkh.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/ghuoevmqm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqwteyugw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gvapecitn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gnoxkolfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ggijjiznz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gnkjwsnyf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gajcddpne.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gklgyvzls.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gokiwwowk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gswlwmlrv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghsgtaqqx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gnrjiixay.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gyvpoirnh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/guvdwnywt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/grwxdocdj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gfoxwmvcb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/grlmgylio.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmcqtfh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gpgksbqkc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gkilqtous.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdseuabix.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gxezurazz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggqkerkbr.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gkfqbkqth.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gucjgyymt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxqgebsdc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gvsfgqkkf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gughezwtb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gbpjlqrld.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gqsvxoofb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwdpixblx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsvqbmsgb.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gymesvpwr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/ghthpyigt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gdpcmyugw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggcmvxpxc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxmcdiuz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gyprjdyuq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gkxqndatk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gymhqmnba.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/goszsuzpm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gtsduzzeo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gdlvcougw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gzxwhvlmt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdnbjfmfa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gvbvigxew.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gdbttehap.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/glrqocejc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gjznhidbj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gakfcitmq.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gbmkxpqfh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gtqmcvtwo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/ggynumuzj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gaknychzy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gfoxenlab.sHtML


<!-- 参考信息 -->