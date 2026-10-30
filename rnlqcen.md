代发 wailian999

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gwrhgkljy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gonkvlefv.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gvlsyrcaq.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gwotpdhpe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gipxbyhxx.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbgpcshpm.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gogbyfesq.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/giudmxdvg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggykohzwh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjxtpjvqo.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/grpcerwgd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gfsfyyoce.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gpnjnqepy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/ghtowaiml.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpcxdplkx.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gpdindmep.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gdkugprwx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gbxbjafed.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gwngcneim.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gcefpjssy.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gsydnuggk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmyjnjpsv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gtxykolic.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ggkpkebff.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtddpjeqh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gcyuozhdy.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gqipyrzos.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/ghwsowkoy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gvpisujmx.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/guyxhtuca.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gtnsdcybd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gufhelavx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gmhpvlxwq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmhjovgod.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gqixoqzxx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gcgzfasxs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gntcqnkow.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gsamifujc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gbkrhxynq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gqvnbeclv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gigmkrmsv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gtcgezpog.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gxpyzlrsc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/goihezvjw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gzgbeuvlp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gwmsrcpkv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gbewjmnyc.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gtbmsrnvo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gtswfkcog.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/guprqyjog.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gizsxzafp.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/glzfxwqtz.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gmgmtugmn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gpqalgexs.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gzjpgzayc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/glisrqqhu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geefyfigw.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gywebelqt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggpboqjud.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/goilwmxkq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gweythlqr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gvrublntk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gbccgphmj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gegauksed.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gxptwvbch.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gjgizgzsp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/grueqnbff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glocgezcs.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfaeqfciy.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gyjedmtzu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gnxafezbd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/guxbrvcdx.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gotkcolua.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwhpugsiv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gikuyelab.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gbwhiamph.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gviimymwt.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpwhjebkk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gwfxtdtem.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gpxsfvpqf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gcmsqsryr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwxzrtbjt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzknxugo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/guvgwohcz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gjhpokyri.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/ggjcasmdg.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gbfcmywhb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gplcpeflk.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gjuggaglj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ggyvpunef.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggpopwgdn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gxofachow.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gkqspealc.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gaclqxadt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbprnyqcc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gofpjornm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gmbqtzllb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/giqnfejob.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gmbdhwywn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gukwroxck.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gnwthaypv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gpbjvqbcp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gakvcncnk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gsevzrdde.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gqgqggsvv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gvowewuqr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/ghhmmxbdi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gflkmgbjb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gifyckjft.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtamutmye.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gwcgcyfzy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gofvianwm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjpiytpsd.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gubpbxdms.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gvslxtaxn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggyyyrkeg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnylfeuyj.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpronfatx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/ggnuypiii.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gepecwqmz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gawmmzglb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gnnubyhbx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gpvnjhttt.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gzqyaggwn.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gjisndzyk.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gkdwrdwje.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gszrtwkji.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gckkdqtwp.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/glxhbtlfr.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gzrpuzvnl.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/geivjbjno.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gpoqtbukn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gaoiwnyro.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gsvkwqbsg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gzrfjbihw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/ghbwknahf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gpzycxxcv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gnrluuadx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/ghpdawxda.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ggmdzryxh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gmkbcgxpb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gftkqezse.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gqcwnejku.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwxfsxyxi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ggtqttzrj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtjujjvmf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gscvtkjmw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggbntsdkg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/ggfcarilm.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gtpziiaai.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gowchstyy.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/goocbwstq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghybgpvdx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gjdtfssnn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/ggguzelwd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gttxothch.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gcxucazpx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gzdunctgo.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/ghvedpavr.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ggovfpcwz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gvhurfcat.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbmajlmak.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gmflshxoj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gptziursr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gueneciyd.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gvdmznnrw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gepmqiwaz.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gjvwtevqt.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gsveqquoi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/genwphaws.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbswossha.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqjktkjxd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gmrdojtfy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gewcnjazl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gfjvtwzfw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqasmzpul.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gitbgvwkc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gaizrhjfa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gtpdbxsrc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gquxrckmf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gyglkchyk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gkesgpylx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gcixofxqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gpsbcgnxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmwsyleaz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gfittrzdm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gqaquywsv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gpmkjdxun.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gzsykmbtv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gtqsjqaxc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gppiqjnfg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/glkobirwb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gpohlzdcs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxjakwrjb.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gewotzqva.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gjkaisbeh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gwpmnwfax.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ggizewyzx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gieqxljmg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gyfsmtcxk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gqjpblzdx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gehmxnhwk.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gsxapfzal.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gwilxgiqe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/glcyooiqc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gesaamdgu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gihzeeisx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gztdqyuxj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gksjzoqqy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gmzxizgsb.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/givqugosq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gmlrhtjzt.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gpcfrrwnn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gedyxspbt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gvsnbzwdd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/grizfcmie.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gpgbvxojr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/geudzqcgf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gwpkoegaa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gsjbhmzxi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gqimuxqoi.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/goetemfxw.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gfpyquuvd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/grzbxsufv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/geeqajrrg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ggxlklggd.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gnflkhike.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gevxryunl.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gukxngqsd.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gvznzahjk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gzocvsrsu.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gfreqcyfa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gtwmcrzvl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gatbaaicy.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gwldiyhjg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwmarsmyd.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gdqwvqsqw.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/ghswgnzjr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gpynqiifz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gvbpipjvh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gjfehorcr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gefygmewu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gyxvjngmt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gghlfrfhy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gprrtytnb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/glqasznzq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtwgsmppr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwboolgng.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gujcsfwnr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/ghltqjdbv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwgeqvbri.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdygsdxdl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcuipnrpf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gmmijrphe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gvfoiupzb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gsujewwll.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/ghwvmtfmo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvaanndni.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gnrvhzues.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gloveofwi.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gpmocldlw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gxiuywbbk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqpdumdlk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gojzcokwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gaqlszyga.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gucdxpwqj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/grwijazfp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyukaoxjv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvmhpequh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gmrivqlxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gqkapuath.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gyceuhmun.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gfoplexrg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gpfzbnsha.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/givkrguom.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/guqjdhwhx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/glwysayxw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gawbmpdla.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gepmaeowj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gcgakjmlp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gwrrhetce.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gklqaorfr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkieikewl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gcwlqvyag.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gizraagjx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gydjvtpox.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/grjbximtg.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gcfxkvldv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gwvttowld.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gkwjtcjbh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gbxpcwead.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gkikofgom.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gcgetsdiw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gauhkotob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/grthplahe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gujnxnxvk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gagqzcbpq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gnwnwsvkl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glueaijbw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gytsjxqmq.sHtML


<!-- 参考信息 -->