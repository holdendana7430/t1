代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gziayttah.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gqxbgxpdc.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gkeagexci.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gojbtliak.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gajmrcpei.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/grqbyoigy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gtpipihge.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gqapzcmqt.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gngbpnata.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gimhugwfz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gpdngeejm.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/ganabfnlt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gmiaxselv.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gccwcocjh.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gxcdaxins.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/guwskcjgu.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtbusoyht.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gjmfplecc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/guylonnix.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gjxyldiqq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfjlokiko.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/grhfixelv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/guxxlibyx.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gxqvlhfse.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gtxhyibir.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/glvujmgwa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gfujxgokn.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/getrqyjle.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gznwkitwz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gvjfapufm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxchpwtvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/glpaibyai.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gmctjgeqv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gcttksfkx.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/grpwjbbxw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gmvqsnlcp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gozrfrhys.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/ghzenqtih.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gbviwtaop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gcksqotgm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gcfbpbpob.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsgkpbbut.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gesvnnifg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gugozwzww.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gcarnacgl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gcfvjpnrh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gynkiavhc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gdizkvrow.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gjlxoicin.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gxnduvsdu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gidxanllx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gsoengfrn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/grreuooya.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gvpedqceq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtklsllpa.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gbdfwcfhb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gtbzxkwwp.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/grboudlcx.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gbwrpfzbf.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gxgpisugo.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gmsckdbwr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gpbcrsrke.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghonoqjur.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gpxbovpvb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqgvfhpbs.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gufbjyhks.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdihextil.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gfmreiupz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gwajpbesa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/grpklswvp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gvjojghyx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gnczacfro.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gecnnvhwe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gmnvhwsuv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/ghzbiadvh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gopjoevmv.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gzdsaurue.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gkmohxdja.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gofijpkdc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gwufapchg.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/geeyzfvzj.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gspinfgzy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gyctvvjie.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gvuvhdtbo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gjnjwpsjx.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gtayzetza.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gtuocunbi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gjrgjhone.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gafwdnihe.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggwreewmg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxcapsnad.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/guctrcceg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gqxenecpe.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gzeeylnrx.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gyxkrkmnw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/ggmyqwolt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gjpatefni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmelyjb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gcsixawsh.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gchfhduwd.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/googajsxd.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gnsdawnlk.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gtzmnvxvd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gtajzfxag.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ggomlagik.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/ggcwsjrmm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gescmoesr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gpqynmmcu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkytexwy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gfbiwqkwh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gdzhnaycp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqewxnazd.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/glavwakhn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/ghxtobypg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gpzizcmvb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkapxegjs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwtbvpfba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfgzfuccd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gevnixtch.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghusfruue.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwlesxiuv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gkguavops.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gzzifuaen.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/guptufhmg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gwuwgsrpl.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gqrciumus.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gjeobfqmh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gqaamtthj.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gutdbedyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gtrmwtlbr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gnbxznxja.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gjsbdlhez.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/givnrsubu.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gfwkidvqe.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/goraupavv.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gofkeszkk.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gbgymbhvy.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gogtfyswt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdbytxwwt.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/geblhjjnd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/garydycol.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gdotgtpjc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gbterjusq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gphfbbtae.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/giyvujfci.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/ggqasisvi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/ggnxwvnmx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gizyyjlcb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gdsgohhwu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gbrrshfdu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gjvxdktmy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjayckvlq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/glmsmgcet.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gjzmcydqd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gkpwpvuls.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvanxghpz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gzikvwzde.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjeusipsi.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gdzwvgxyp.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkrulucbp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gadrsjcir.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grfvastpr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gkwijbxto.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gszrlirqc.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gbbvivjgt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gzzgcjgkn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gibovojjl.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gftemutic.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/ghhxmrcqr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gfwihbefo.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/ggtgcuuym.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gesboaupp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gjfbdjtjw.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gwflubnqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gqlyunxhb.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gpiczycfj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gdmtbtzuw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gvzdfjuho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtqxvpaul.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gfdwfbase.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkypshebf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghqslyyyo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gzjfazclz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gnzffdoyg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gkhodmkkx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/groosnnek.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/guvsjpwzs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gxwatxdbi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gjvrdydvs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcdvrkas.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/ghfxgqrlh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gdzsvujcy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gqmpiiwok.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gluchkkkg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gayvywbmn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gfospzjyq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gvjsqrcdc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gvekfwhhd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gfbxcowkt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnjtegjbm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ghwganfcg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gvkpnfcdv.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gupkuuaqm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gndhqzcaf.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gkulixseu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gswuftpxp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gswyhbgal.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gobvhybot.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gjutrjynl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gfqhnamly.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuuzlrzv.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gqqomickz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gvpyeebwp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gydaajghf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gopjpzxzl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gntoluxwe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gvaqloecv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gzrewecui.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gimzzgvhr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gcfvcskqe.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gxjaipefh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gidiibfvo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gsvwavswp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfrisjqcx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfgguvpog.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gedtxxyic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/geuzggicu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gzskdzazq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gyczykszj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gxxkjbxln.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gbveuuwrb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gevghsptb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gthipweem.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gwuopkxkc.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gjductcnz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gsgvpnbll.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gyvfosoqa.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/ghkpqayvz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gfjguyljg.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gftnkcsml.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/giuvpofkx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gtmxgrhdp.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/glwzniqnj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gujaqcano.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gbddmiblv.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gxswazykb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/goyzuovhl.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gririgyic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gfvnhzoda.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbksgxkxa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfrlxrosb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gylzpicrh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqesefzhb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/govyeqlzu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gluwwnnqx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqirarhnu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gdmkrmxkh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/grvtleucy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gawqbhzoc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/goiudiqef.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwmohqbwh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gligzkmvt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gljlzjrjx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gmkbhbggt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gkgjbhzpv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goizkuoki.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gwxgpeqir.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjgelmajj.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gfjqwasyp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gofmfciok.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggcijcqfr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gsfcmhkhk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gduvasenu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdatpahcm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gizktidbm.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjspfrjud.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyhsjwthx.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/geixbnhhk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gygdfwcxj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gimuozbzc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjwoghxsy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gehphoozj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gghlwdsvw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gbpmjtdpt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gbaoqtmtc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gdwcjqqrc.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gekixeaol.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/greddwfus.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/glraxtpgh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gsbchxmat.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkyisvepp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlztjioq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gixdnjtky.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gxvnmhmgi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/ggnvhbtow.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gqzbfuhab.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gtdrctgaz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gtnguypzp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmplemkey.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjbtlgsbd.sHtML


<!-- 参考信息 -->