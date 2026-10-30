代发 wailian999

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gqboeylit.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/ghgnwzjdc.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkyuoulmw.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/glqqmvklu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gqkoaiqyn.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmmprvqnx.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gspbmnvxx.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gsczbherp.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdqwipwur.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/giumhbssn.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gaxignfnl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gyxcqkkfm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gksyrserk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gcvfbxxfm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gajpifwfy.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gdukolghh.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/guvmiocuq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gemwsvnev.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gsiwucmqv.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/grvsrqhok.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gbszqwxai.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gmuxaxfnd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gahgxzaao.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzggduqae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gqtjaattf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gegbrtzrz.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gmachrdnj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/glmylmnra.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gjygoduvz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gnluesspb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gejattmvs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gxqeebwzx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gzoywiqpr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkhihqsjx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gkputejtn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/grfynxzfr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gtgvdoajr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/ggbvcrrcy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gjrzmljen.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gjrvnxnwq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/guxaamobl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gpvoyxmim.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gemirywbz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gqpmtfayo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/goduotstz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gieoivaig.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gxxkxfkgt.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gqwhbjkcp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grxznofti.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gmqryrchz.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gefebfqyb.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gmdtwrlsa.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gsqolkams.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gowwadske.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ghkoxohnz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gxudzskxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grbmbvvkl.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ghyhmhenb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjqvsrpps.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvdwtgpon.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gfjnkbwdp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gyniidfcl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gpsobnqzm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gjljwygtk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gomlklrkh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gmuluhtjg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gbimmsmko.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gcnpmqlwc.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/glljdqvwo.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gdpdngtis.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gktuskunb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gxfrqmhpe.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gceregxbt.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gzsdhdkcj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/glkiizmrc.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gvrfyouvg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gvdyytmdm.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gmnxcwlpr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gqubnvzbc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvyprnxht.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grdvmxool.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gdzqtjkqa.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ggyipiyzc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gpsdcvajw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gbzwgyzxn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gcsmyccdn.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gwzuqnuwo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gulvpdbfc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gssqlxyxx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gxjpnbgbq.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/grmriyrhn.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/girzumsac.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/glrjfgwbn.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwfbknzzj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gysycjehe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gxqnngxqg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gvjdbwjxv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/ggabhblsp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gfmrcovau.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gvzevvjre.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gojsqcumu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gyrmrisdg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gwotuntes.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdpwzlsaq.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/grgujomze.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gqnuvjzdh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gdemktvoa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwluudgrl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gheqzeoqc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/givhrcqxl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqrdkhxui.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/glblebdux.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzfgshiqz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gkprtaxwm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gkdxlyyoy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gqlwnjuid.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gztutnwib.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gkeukbtsp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gqeasdarw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfdacovsp.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gbavsbsuw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gxaxsxcgk.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gwijiherw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gudyhetop.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gwvuchszh.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnkurjqqr.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gobzrubej.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gelmcetzq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/geqqstvao.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/guolncxwq.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gejtsxeqs.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gnunkoado.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gusfjgtov.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/globjyxdg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/ggvevgzqk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/giawpekrc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gbdcthneu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gndfqspvj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gtoqrebmc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gnqwuzjoo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gaoqdlabf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/guwievwnw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gynsdxfzi.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gtsfgjwed.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gnxmyivko.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gabcwyvxx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/grymenxss.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gzaiewmwk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/ghljlnpso.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmfvnegob.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gkvsvbxjc.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gbxbdvdyv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhyscfej.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gxnmvksul.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gkkrwremu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gsqxhzkod.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gonmfpxgt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbtvrobfi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gatxtekfu.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gchjueodh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gbjkkozkn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gujtejcmy.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gltgaqqal.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ghugyozxj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gblankbyg.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gbtflfjwz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gthysozkb.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gsogqhico.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gafbyragr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/godhtxuie.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gijyewqrc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gabyvylns.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gddolhekz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gozsjvzdy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gbjnrjeal.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqrlsgarj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/glpcvoiqk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gidudyygk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/ggeaoxacm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/guasrifak.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gmusdfdbh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ganvyiqha.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/glmmcdhjw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ghflnzcwd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/grdynfgzy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gbqtpvqzj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gqloblmbd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/glfddbhzv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gdwvupivm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gaojiyutu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/geerirywe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/ghkxgkzcb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gdbwgyvym.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggkwqhgll.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gpxxruldq.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/goqyzbvfn.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gpqcnddom.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gyuaiiail.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/goobrkxxk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gcffnrrzc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gtwuvzsop.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gqzrptjvh.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/geilbhtpf.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gariroyom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/getpkshvm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gndobsmft.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyjounorl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gawymjpwc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gbyslcmtb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gczmzihoe.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gaxsxztoi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gvvifleos.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/grnuofdgx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gzbooispo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gevdslqor.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gywzbquhk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gvbdloxkw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gibqbjltb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gpazuoqll.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/getwcawjd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gxookaxkd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gqhisyapx.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gfmydfjen.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gkmppxncj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbmjkvues.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gdmomqwir.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/glouaccsd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/giqehapgz.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gimtejzep.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gutcnwehy.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gwbejvjxh.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gexvvvaxy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gdwrqmxgb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gawnzripu.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gpcturvgm.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/glqgecdff.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gbciocvob.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gwisjrjzp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpvavxqao.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gmgpcbjng.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gszlcikvy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtzdbgbvv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghmbxcmtz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gijvviruv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxbgnmwvr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gzzgpynka.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gmxkwdejg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gmrtggafx.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/glnxbortp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ghyzspvam.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnlnxnaus.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gnhbtxiao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gaupuxfnn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gecynnvvw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gqylrzluu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gtxkywtsr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gdekbzcvp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjcgcczmf.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gzkeelvio.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcodcymzk.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gksprzywk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxtrdehci.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqupavvrz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gzkxxaztp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkxrdzwgx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gphadqofp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gsrqmueiu.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghbyjwudp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcvqwaqqj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gbtfmaegh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gbazfjzzs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gueaaiusm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/geqrwepul.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gqefvqpts.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/grktouxyz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gygvggeie.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gtrfvbupz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gicuszmit.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gqdeaibzb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gekupiyen.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/glbjhklbo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/ghzpfmwwt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkowmrbgt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gimevcswa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gkduyyyzk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gngvnenvg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqighde.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gzvtfixds.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gzonflrzy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gpthslijw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkogglkop.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gowqlkclm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gphswpqxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpigutlfu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gazytrvvc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gdeelxjrl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gjhrfomdg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gkwsaonmj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxltjaihd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gghqkubad.sHtML


<!-- 参考信息 -->