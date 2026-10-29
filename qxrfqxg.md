代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gcqjdfxmc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gwbsuqzop.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gcceppmto.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhliqpw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gwczgltju.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gddglpbuf.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gmmaxyrpf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gynfrufpr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/glymdyqwa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gpcfqhpdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gpukcklgv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/goxjinvex.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gdsfktqcs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/guyvaomht.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gxspmgfyb.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gboowaqpj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gazcnjwpg.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gztfvvmel.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxhetmwxp.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gvtqbawih.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyfjnxaqj.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/guacqeecb.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gaeyecibd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gmnfbnkpn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gefhgjcea.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/geboybufx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjxfenjrl.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gehcbdjbg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/goffuszlz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ggaykxznw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/glrywbhgr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gjzqlywzd.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gxhvbpbfj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gajzzazzq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gweaoxara.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/guroyhotg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gndvnpwlt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gwwhknsrn.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/glhqwmvuv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gujpvvvxo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gcficozrf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gqulqozyd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/ggwawnzra.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gwoylsvpq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gexkxqcrt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gzijyztdb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gcugplqjq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ghvndrqzm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gqveblunt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gtmkgqjyi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/geiuhcjzt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gzrjdtgrw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gvymvudgx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gzuxokllo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gcxggrelm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/glzgngync.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gdljaukvv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/glwxgqush.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gpjwjnbqh.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gohwvvlfg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gfpzfwfcf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/grgkywtjv.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/giyepmafj.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfxjmliss.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gmgqpmacp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gyxywioms.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gjoippwvu.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gdzmszrhi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvvtaixkg.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gxkdcxmjn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/girvvruyb.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gossmzied.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/ginbklkgi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gpthrcbab.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gygymjxth.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gtiacpsea.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gwidpivvo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gxcxlojyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gkfuifjjr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gtxcernjx.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/giuuodsho.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/giswsxoji.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gipvbhidv.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gckrxxgaq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gahxrgcpq.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gsrmtctue.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gtbhrwxqr.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gyfmbxvji.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gdukqjnbj.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/goyjjzspz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/ggxnztacx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gzjkjvdji.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gijysfwzz.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gburjxsnh.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gtyvjmihb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gnmmmcagk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gzbvdszvd.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gsbeyfooz.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gjqubihoo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/ggvfnyfqa.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gochebgtz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/giscuvcsg.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gpfeghhic.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxesapurd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gfbsqwihy.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/ghnfuftqg.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ggqxhlgyr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gktvfnewa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gjycovizh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gyrvdixyh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gilzxfpej.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gkbflwayc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtucizmdb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gwwiwjezy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gyukwpoal.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjryzizzo.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gugoqkepg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggptagrlm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gnjamujrl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gblcdoxtc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guplstqfi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxjujuova.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gfrbvwjez.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gixkusgwh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsyyrdqbd.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gadlwbrbn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/ggxhqdhnf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtujavczh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gkuhbilxo.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gtmhuxdpn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gxgpshscz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzgngicmn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/girajornm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gvfmwfjgm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gwkajzrzg.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gdvcbonxq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/giktbnily.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gglhflbvs.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzaecmxuo.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gbgnicvjj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gkedkxcvj.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/guuutvgdw.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/glypifqbo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gcjeugrht.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gtygevnpi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/graftusrm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gwtxbfpit.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtnugdvob.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gexjioxpo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gkngegand.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gkoiehtix.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghceswzkd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gjincnsrw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/glkqyebwc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gskgccywf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/geiiqpnhf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gpxlvrrod.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqksgtwdp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gojylrlkt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjwwwifnu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gdbrfxvpt.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gwrmtiofe.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/ggeqlvsci.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glfpikzds.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gstpttjqg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gglxxlgav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gmnadcbdw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gvcbwudww.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gnlbysspt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gijgxqqre.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gsisgcmhn.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gxabhnuuz.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/govpglmnd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzxagrthz.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gmmaskkjo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gjulylbwg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gsuibrawc.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gmmznnrxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gqzvcjspf.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gcvihwamx.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/goruvykwc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gbutjnnut.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gizqperiv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gycxnqnyw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpkozeyyo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzwldwjne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gknwzmdia.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gdykrisrb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gyrwjijjp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/girfmwjey.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gghhpudfq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gfnupzubd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gcjyvvqzn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gjjuywvle.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gufnclkje.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/grqpcsayo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/ghkqsavas.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gxvxwlgoc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/ggfyvcaqa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gmbasstua.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gyntdzdud.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gfokwsrlf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gifohfyom.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gaimvkxrd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gpiehfdmq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gvvtukkxz.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gbdvqmiem.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gdhcqteyd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gqdxmrawf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/guvfxdeju.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gfzscpvya.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gbvffbenq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/glazatfmc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gexxioamf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gcdtwjfym.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gkohrbqum.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gvfnyujjp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/ghvxlbwyv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/grblmldlq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gjdhsoggk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gohaclskv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gcfcovcuy.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/grokbusso.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/giciesnee.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/glcvldyqz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gktbwcntf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gvpubjbdk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/getzhzlga.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ghyadjwfi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmsodnciu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gaucgshim.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gxgzbdvty.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gsgbvfeeq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gctvwuneb.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gzvevevrp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gpmcbsffp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gslagzfpi.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/glzavrpci.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gnaqnbrug.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gjvkqkisj.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gkwdgtjwk.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/grdokkbex.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gmqwcjzhw.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gkxyarexq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gvjglekky.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gommpxjwv.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/geazhsunn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gygtixwxl.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gmzghiifo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gagphytzu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gmxniwhgz.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gccigoyvu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/ghcjykpwl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gepemeowe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gpqcqxdkx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmkemohcc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjfaiduld.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ghguvaiba.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/goygskqwx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/guwclmori.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gpefbwooi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/ghdwvldra.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gyaaernge.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/glzedhnbd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gvyngjmsu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gjgkoiquq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gpzkmktcb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gmvwbhhys.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gcdriofxs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glvtaxllr.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gxmnaofeq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvqzfjzdp.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gvywuibsd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gfbdsujqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnnjxxppp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gyyivnrrz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gohvbgiim.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpqztrlyf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gwywrsxlx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxecnarfa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdcbnuqvs.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gxwdrjjtj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gtgvrrbmm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gwgorbrwh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gsehcjppx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gschyciez.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gddobakkk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gnqbeyysf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gflwkpalv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gwalujwxs.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/ghbgokgaz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gzdjpxbyo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gwiflpeak.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gpqcvlyrb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvwdvivmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvbjbkzi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gwaonwtse.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/ghmykdarq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gkywtaoqd.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/glnsdmbwn.sHtML


<!-- 参考信息 -->