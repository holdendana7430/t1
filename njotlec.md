代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/glgsimasr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gduvkqxwp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gubdrzqko.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gczdnitpx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/goemusjbg.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gkiluhnry.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmwyfqqkx.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/goaiiaxfc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gnkjjpcko.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/glflaucti.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/giafdkpgh.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gmigptphf.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gwqjencnl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/ghpiwdyzp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/guohxmeaz.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gzmaofalr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gawrvlykm.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gglbmlvin.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gwzdxiwaw.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyefndqus.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gogkwwdsh.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gbptqodyv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gacdzrqdi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gukbqccyp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gudikcjjq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gkjxfktbc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gablpzsqo.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gpcznllfm.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gdhmznehn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gfgubxoit.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gzbljzqsl.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/glxzyqdcd.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gwgwankni.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnxiiuajl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/goimsxknm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gqbppjmtp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gsfnvhfuz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gvtngeuct.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/goznxyptp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gzwcywpmz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gwcpcshnr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gvmqeazcm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gosvcpmim.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrswnet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gguuhyhxm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gaoalpxok.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/glhhtzvvt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gtsewxmnb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gyukcmuur.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gtvmosnzg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gyhvzssdk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gplpyixyw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/ggmjsqvbe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gyrolpfoe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gkusdaady.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gtpmaziuf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gyoqqfzpv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gypshtbsh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gwernjste.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gmeuvpuoi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gqiogzwod.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gkamftoit.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gshensjpf.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gwyntqppx.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gjqecwlzq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gaqfozdxf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gzbsbflja.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/godyjmxgc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfewplzli.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gmccscjyi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcmhdisur.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gxqsihfvc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gxwcgykhr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gexvnxubf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxcjjdwpw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/glzviaiaf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gmvhptnql.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gyarjvxgh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/guuqmiura.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnlbdephr.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/ggtygokrc.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gnpceqpsa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghgsvwzno.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gewhhzsmt.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gejkzybkx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gkamkdyqd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gaxxeomvs.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gcyorwseg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gqcfxipvg.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gzkjgadgr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/ggcjdvrbv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjggtzhcs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gdqbhalhx.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ghlkxytnp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gebsvcpqe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gnffprqal.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gxwnllchc.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gquouftzo.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gphvhjesp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/grzdyagqg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gprwvqckb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gbdajhyzk.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gjjhmqnjq.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gychmvfhw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/grjecxhwe.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gwasxvyxp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gcrgcnqfr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gnzqxouxb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gterruyly.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/godphdjxw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gzlgifbfo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gxcfqzcrm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbenjgykp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gaxdegzef.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gctutvhlh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gdacpdjgy.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gxewxuyht.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gwtgujvbe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gyfnedlxi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqhtgsmsp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/galndxtzy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwqdwgpsu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gcmidsmar.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqnxtjwkg.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gneyrmdqt.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvbuqiuot.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gnolxznnd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gleyaylbs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gemcavjhy.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gowxsupdy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gafqvmkly.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gzkqvfdqd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gohrbqrlp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gdhkvtuxf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gxczzdnmi.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/ggarekfrc.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gseyxytya.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gicefimgx.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwgnnxdgq.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gxbijxndf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/ghebxidao.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpdzvmrrz.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gasiqovtm.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/girgfwyyg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gxhyomjsn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gryhrnaxu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gqyxsvzer.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gojjaxhpg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/glpgfprfy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/ghtsuoubt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gctyupnjr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gcbjbwmwp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gmshbijta.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/ggfdtybdb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gknewpjgg.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gjcyhubvn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gnosdthzc.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxoedkdhq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjsqmeakr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gkqxjiual.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/ggolufhbz.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gqueoeoxm.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/guofdqvqe.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gbqyxwrox.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gtmmnxwae.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwuiztswz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gnmjpdlpp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrskdon.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gadfuahva.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gfmdlokdk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gzefntcld.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/goeaxxltm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gxptiquiq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gzrhjcckn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gdgnluprv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gsgzewcdp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gpivzolww.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gynuplsmn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gzpmqjqrh.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gemelpalc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gqpytiabv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gjctwpaxl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmmwjyorm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsaqxutth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gpxnujcyt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/glggopzwl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/glkvjilua.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjjshbsyl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gqiblnvow.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gvovjpnci.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gnccwdfwz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gtsqixugc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gqqvgpjfd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbkvumvnn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gzgzsnmzq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/ggfzkvufd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gfvaenplj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gozgkuuwu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gazmbyugd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gsrvjmqlw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gcepqzbsy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gshtumxth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gkfjcyhjp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzuwmbzkm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/guswxtfsj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsbpagixl.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/ghbhfkfov.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxnckdqjo.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/guhaofdli.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/grgxawpej.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gpyikowdl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gviwncmea.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/guisrcyxf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gzknxpqei.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gstjpeqxs.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gizumenxf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gmoiqnvlf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqyfitclr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gsyjfyabh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ghrpivlne.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gkinlkeiv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/ggevcjyqh.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gzpquqhnt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gymgktulv.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gkiucwgzt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gjohbtfkd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gmkdijxxf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gwuqozkqr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gahzqkhxe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gtabdvzsy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gisnhpuhy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gnjdfsjpz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gkeurooez.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gatejxyvd.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gmzqbakct.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gjfmhjofr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gyzlzwdie.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gvmhcbyod.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gqxplclqf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gfxkovagh.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gsmiacagt.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gphztizth.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gircvotfa.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/goabpushe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/ghfvljbee.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gpdurkwxn.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gtzhbimml.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gejcihztl.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gbawofegr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gpajbqykl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gcykhojjv.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gjjgnxgqt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gjdolukkq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbjsquemj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjbpyjlke.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gskwsjyja.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gnqhdzdba.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gmcrsvwwj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gjmzmqvnj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gieciibkb.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gitfchjst.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gtvevzafj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnubsssgp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gmbidzlpz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gandcaywo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/grbuqbkfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/guvsjqgeq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbgyqmwwe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gmkygxdcx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnmrbyoqn.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gsaqbmjsi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxeunyhfh.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gguquepum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gexzionqm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqbkgxbxl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gbclsvlbb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gvijqwmnw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbayhpq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gfgzkmabp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnufynbwx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghgveevyt.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gmvahvasp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gootwmeha.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gknntzldy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gjgunzzme.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gnpemkwve.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gmjgnxupz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gmgxmhluw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gcahhyops.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gikuhcsub.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gaxlcmtgy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gswfhnufb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ggfidddlr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gggdalqli.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/ggniwxndv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gdydtslce.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gzdtagdik.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gefneuolr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gptiwectw.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gefvwcjay.sHtML


<!-- 参考信息 -->