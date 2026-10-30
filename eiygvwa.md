代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gpqgygyry.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gbqwcfvvg.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gjnwwdxjg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gzpcsxaib.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gcpkbuvul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gakqgyegi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gkxnwzoie.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gnphpgobk.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gdllpdbos.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gaylgtdpp.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gdcfkkcib.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/geztryyhq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/glppmbwba.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/guwqhfnkk.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxixsfjyo.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gixbtipah.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghlesmanb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gjojlbjnd.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gufnkebeh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gopvrqxiv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gcttbsunr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxulwvs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjddrghky.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gqklbptgo.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gmeprglaa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gucyourkg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gystdeqyc.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gwvcnaapu.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gbfedgvbj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gqgfzshnp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gbpypckrp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gluyismfa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghqtvecyf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gamsclvma.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gbntofplj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gkpywhwlu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/guvoffjbg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gkjogvtqd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gquaulihg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gxasifatk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gnuimbnbq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glxvowhpn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gqaizccbe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gmwlxchty.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gzsqpifzo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/glnpftrwc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gieefigov.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/ggdowlohn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gzssvtzqb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gurxlimcz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gbxvjcpiy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gqxmgwzfr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gvyiplsuk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gbehetrcw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gfubtzsuw.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gercjmcav.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gfrczvrys.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gccrvespy.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghmvksmhm.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcqfpwzxr.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gwxjpgubu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gunpavmid.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gxuyfsoro.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvyuzisno.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqgrejewe.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gcrfhxdzn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmntcfhzv.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggtkzbsxs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gmqowoeyn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gxsxzmhge.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwumiwjkf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gxteperza.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gdolgryoo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/guedpgksa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/ghjibszct.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpogrifxy.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gubotlzww.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/ggyehpjmc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gmjnhugbf.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gavgqmhbx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbhkdewny.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gxynrmzqw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gehmutscu.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gtkmolcxm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gwpmikace.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gkacvpvdg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ggugtcgvc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gbbubxkgu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcmdxwuqu.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gncajdots.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gwuofznfn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gdyhznwbh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gquldyzkb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gsnuwlszx.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gijcqdotl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gvuvixjcu.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gsdukvztr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gsvxqjuts.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gbwmujjzj.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ghejojute.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gfyfuhept.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gzhkhbkpc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gljwkahdw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gijtwcohf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gcpkzrfpw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/guyhnemem.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtuhskwrg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gtsbdjnug.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/giecxwlnd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gbmbvmogu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gwprxgrci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gtgatwhbk.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gfoduxyrx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gbcqvuvop.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gpcpmjynq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdapevnjz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdrmhwcdb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdqitgbsy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gwzrgqmyz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpijpspoh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gftxoytts.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/ggnuusgmh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gqjtagboo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/goqhyvotj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gtcwzlikt.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtvrugeml.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gdqclrcoj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjqiauycg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gjliexngc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gxxufdotj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gkajnbpqu.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/grkxgcerw.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ghvhyaujd.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gzuexqczy.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gbzdcvlvt.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gtqhuzrzw.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gisxtuozy.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glvjbfxfh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghgevkidz.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gxboeoxmn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gfsclckpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwgzmxtlz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gbzeexioz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gflqrioxq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gebcsusha.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gakapyqbp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gnhxymtxw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/guplozsga.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gjtyibkzi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdsuqilbc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gtocdkiph.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gtahpoonk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmpcxuumr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gogojdewg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gkgtqcvxz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gpkilcuak.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gelycryrc.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gijnbdkdh.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnirelytt.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gtgwbkckq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gllxktzgs.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gimjnjgcz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ggezvxvqi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gdrwjiwse.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gjzvrudfo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gsjyjasrb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gewrpwvub.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/goqeqyvir.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gsfmgbcay.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gzhklbyqt.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/glfellabd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gqnooqlfh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gcttefohr.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gjbdwakqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/ghlodamib.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gniymgmue.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gqjdqjyhw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gqdizgrts.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggntudhxa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqatryyrn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/ghzedxiff.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzjjxsirr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gfpnqhaml.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gmzqgzymx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gjfstvnyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gjiotihzy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gzbaikdjf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gvifgiikg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/groiduatw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gqdwvctcy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gxgmwfgsv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gstvredck.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gknatdjhg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/ggaekjcch.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gmzqtdnld.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gsdzmcqrk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gijxmxcwr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gngdctvqf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/geormlrqc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gvfdjzwxp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gzyiikhyw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gtazlfwys.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/grmmegpls.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gxwblqiwb.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gnfkatirv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gfmbbnqqm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ggpmvyacu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/guchxcjef.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/ggcpksjbn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/ghchuhnwe.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gyhehfkyp.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gjylnjudw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gpjebekql.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gxhlnigii.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gtrdgtxxl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gedaediww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gmfjbmflx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/ggremqiqa.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/guidweyue.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gdtcpktii.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gnvqvhtdy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gxcphbaik.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/grvciaqdh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqczckqkz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggicmtjmi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ggeawhygw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gebeavkbp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gypeivlfw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/ggkqivvwq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gnzrgttfm.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gynozjexa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gtrmwrdjs.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gdbmjnekg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gmvbxgshp.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/grxshkjtd.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/grnhkusji.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gosfltyrd.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gaxkrrjxs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/grrmnraen.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gqjzxeant.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gcyemizjg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gelmzcbvx.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gnzpeadzu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gujtoezyh.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gaeagaasz.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gakgulhio.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gptajmuow.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/geyfvxosn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gnxqaoklt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gwbpcbtpk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gavespsnx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzjkmptth.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/glsmfodld.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/ghklfcgpq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/glhcalmzg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grhtquigk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/ggqoiprkl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gsowgoadb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gtmlobxme.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gcbvkrxad.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/glmlpsctj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/guifzcamq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gvpdtifkh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gmwzojauk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gvqekjobt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glklfrkie.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqynqnrrp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnbmucnkf.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gpavyrwei.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gwzmxnndg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gltfqfmye.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/ghsmxpzxo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gtlpjwwin.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gbbbahisx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gbnbcquqm.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaubacctw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghaijrrtz.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/glzcopgou.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gzancoxlk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/giftdxtmh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbjrtiejl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gkjgzwzcw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gkpcuhhdm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gqlaxcnhw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gtpgiaftm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gfmsalzea.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gzzdgbxpf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gvjvrvuae.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/giuhebocg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gizhuufqn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gfgqgzbev.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gpodlkcjm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gcxubbcyp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gdmwlmddu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/ghllhmxpn.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gkxyojrcn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/goqnqfrbh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gfvoxzhfl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdyznanbb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gofketqaw.sHtML


<!-- 参考信息 -->