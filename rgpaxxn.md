代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gnmpmcdyr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/guzusbhnn.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/godromwia.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gkscsnxyn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gwpbdrgtj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gtnsvmjqp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gocpratkz.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gpnnanrhh.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gqqsafbix.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gdopzgnjk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gzglfilcv.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gvjihntub.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gwqwbrqdl.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjncmohjm.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gleufdcun.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/grfgfbxlu.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gejyxemnt.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gyzrfdrtk.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gsfzuuvpe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/grgucqzvn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/givlnsqhq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gcaxmzpiy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxitbkdtj.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gsfjalvas.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gdpjjjyjy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gkpsiptln.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfmxbxk.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gixrhlrjf.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gijfvciqk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gjspjzeub.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gugaxdusb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gayvxubzz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcnllyxbt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gdvxkviif.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gznfayxtn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gzvvtboms.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/grnwxojqb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/ggshlfejm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/goiguktto.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/galvdrqmq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gwcijvfgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpwofvqsd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gnnioimyi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gonhsdeax.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gylluvcho.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gvvdemfkz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gxderuneq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gfvuedjde.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gwmtvsqlh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/glfaxrcgi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/ghyenrkch.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gvwljmmfk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gpcytsshr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gfbqwwjxx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gvfjhtqwi.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gywokzaff.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gerohbevn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gshnyfxxj.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gbtwoqmic.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/grfkebult.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gglivipcj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gpqyllupb.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcusoffrj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gqrodgeqh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyxwrugfl.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gljbpdcer.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glaafsrec.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/grlxduanq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gevwqlggx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvdgejx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gjkrqogxc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gtiqphsdp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gezpcbqtb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gmbulagtn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gyhpgtofu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtxjacyjt.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gxnkiukyj.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gejjgdmoo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gztbuexdh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqezukhvf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gptkpmwwq.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ghltqzods.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gvxalfsfw.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gacybyzpp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gomgabjat.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ghaozilma.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gbjjaenvv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gypnilzjz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gwbqbdddn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ghtruvkyo.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gmrjtdkvw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/guyqobzcj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gghrhulje.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gaonomanv.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gosvaztab.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/goymrfras.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/glijowfzv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gwgwaaugq.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gczaxynhy.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gjwuohdci.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gpupzkrht.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/glrmzwguq.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gxihuhsnr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gmqnvqdwr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gktewklrq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gvihicikl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gaesdukiq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gcztwrtgq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gniumtune.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gbgspsebx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gniqyuwcg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gyllgsqvi.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gdthgkvkv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/grounofhm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gybjqtyot.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtnlusqsu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grailxffv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkxmkyrob.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/geaniztvb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/geoczzqqb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbcqanchq.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gpjfntjkj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gwvwolcff.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gessdbfmr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gotogfzgf.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gmcgqsjne.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gpzihjgsv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/grneevrzo.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gibctfhvb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/glhwsyuwr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gzaaqekce.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gfhvyphmh.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ggiljwfuu.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gokpxsxus.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gvqbzabxq.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/grcbiynnr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gfufbjmha.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gkgmjpdqt.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gpoutlrcc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gflpbkhum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gtsgqqwfw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/geqxovmsr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvbquleqm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gdunkgbjf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gniijpfxp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gkbpeelis.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gnrnjycno.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gmryizdiy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gnhyphkxy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gkoklvied.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gtlirlhqt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gypsqanho.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvrsrpulz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsxggdcvy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grmsmbaom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ghkjnbenh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjtweqths.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsusiedkb.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnldcuegg.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gezskkekv.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gndiczhzr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzyyivlsp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/ghtsgibtb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/ghzkqyhtj.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gtdlsomcl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gsnbrywqv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/ggtuvndzc.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/guxipnqsw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/giwkbescq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gxtjtgyjq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ggzbrwpbw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gagwrwtqg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gomzkcxqx.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glydabhtp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gselkjcgy.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ghtqyaxnn.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/ggijhojbd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ghgfitmrd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdhwbgbgq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gkleptkee.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjlqqxjwu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gczxajcts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gchwxjneu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ghenxqgaz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gdzqkdoud.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gldpydwih.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glwruxmke.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gohilmxfw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gedwkhslb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gvkhxwfqh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/ghraqkplw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gqqvkusdy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gkwqnanhj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/goavsbgzb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gqdderbio.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gnvoedogq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/glggzhtbl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/guntydhuh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gnzphlrum.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ginrvydgn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gnhzojnio.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gpksgekeb.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/glgkygkrx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/ggfxadefm.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gdtpabdcu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gxqpsfjkb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gkqlcfmir.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/grwwukduc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/ghfcizsec.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gzterfmqp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gvlvtiwch.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gtynipefz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gdwwqimty.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkifqfrw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzuabzdyk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/geqjqvlwz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gojuhrcbo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gyrmqooxq.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gsjrblocy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gzmkkbcte.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gqkahtzhy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gvliwbulf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/glevmnmgy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqwgtqgok.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqclixxfx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/guunnrjdf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gemomysnl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gnfobevhm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsnsxsq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ghtagshyf.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gedixicra.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggzyetmmy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/guveyymuq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gukcgdsdg.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gobpudxer.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gkisjkqzx.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gwpuhjahz.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gnsayqhqo.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gjdfibxox.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gnictfbcs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gehwypflh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/ghvchykrm.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gjnuohilx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqzpqnffp.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gdzfmlocw.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gawonptxc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gwjzapnja.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gjmfemtpb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gajibmywm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfqvizmsv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/glgweaswq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxskrvuso.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggwvdfsmp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gdwjfnldd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfwewkupe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gaofkuoad.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gpxeewdbk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gdkawmvrb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gljlmmiss.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjhjxtbrh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gagxnpmbg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gkoevrcmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gcmokkowm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gbbudlmez.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gdqjmgufk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gehjvfifc.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/ghzynkkbs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggonoatyd.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gwldzthke.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/geqvyzzug.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxaayshnt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gdtmeoiah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdlvpaitw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gurqtjvgo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gwftkpzex.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaahhrlbv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmfsyrtoe.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gpmvttmir.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gfrkafiry.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gbayiwulj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gokxoloku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gtyotwrgk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/guhtsojmq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gseyfnwkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/grwzdfexo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwglffjfo.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gbzpoatqi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/guuaclkad.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ggvveuavs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gqlcibdjw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gnnxqbqfc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gavcathpd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/ggydkwroj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gicgmlyem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gwrhepdbn.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gcbhbwztp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gycyfyeun.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gsvurrzqt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpmocsvyr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gxxunrqnd.sHtML


<!-- 参考信息 -->