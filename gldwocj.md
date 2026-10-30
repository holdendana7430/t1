代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/girjgyjqu.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gaztcrnah.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gyzfwqqad.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gjanmqype.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdrqqtezx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gysognsjg.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gkbllhkjr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gqlpdvndu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghdqdxebk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gaqvrtdav.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsknqrdml.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gxtupozqn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/ggrspburw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gvroxfvqp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gsbtlexaf.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gjljaxkma.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ghmiyqjhk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpqjdvmyu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gbajlncdl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gjsfounrc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gnhwyraty.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gurhigimn.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ggrpvfobo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gizgnuobo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gztvazfjj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gcoszjqim.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gjjbcqjti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gxrekzqjc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gklezxijz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gitexevlg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gubspzzxx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/ggwgkppgz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gelaztizx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gzpxecluy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gwkgsczyv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gilhryaaf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gelvwhdsj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gnbrxgowm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gjqjlzssq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gvocobzfv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gsjszftcv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gytjbvymg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/grstavsch.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/goxjebuqm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gzvdcxheh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gujtjylea.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/godhysfjv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gsmmlvxqa.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gselhrwmr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggifuozzv.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdlmyuzcd.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gjagpwgho.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grsryarqu.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/glwmkcihy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glwtskdkz.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggfljlosl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gyhksmaiv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/ghdnlesjv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaslggozl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gaxtwiccc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gubdlgywo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzdqvjp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gufiwdyvr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfnnjxkyq.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtawhxaao.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gwtnrgajm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gpnzvydcc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gilcdbnnt.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ghfctjbqn.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gpdxkyqbk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ghqntjwgl.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gxdpkcqpg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gojekhbbs.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gqvwjsxqw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gopndqjvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ggoatqaqk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqnahihuw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/goetgxgwf.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gpibtydlb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/glepivkxx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gzzzonpyd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gahmbqfff.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/grwirjhga.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gcbrnbjiw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gkkooxvez.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gpxhdvzmv.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gffvaobig.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gnpwcugrw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gezogtyki.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gonhrtlso.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gixgrqhdv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/geqrxwkgt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gpazndeir.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gafyebbty.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gwbetqmej.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/guylckvbe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwputndow.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gckumbfca.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gazbtilvp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gedmfxelt.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gxztwdsmp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gzujpparq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gmafsvjhb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/galpcyvpo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/goozdpqhn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gipiohedd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gafxpmpua.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghdzbjryv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gghqkvcev.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gjeedvvdw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/grxnsvonj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gckoyvbzi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gazfxelqs.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gxdzehmaf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gbdnlvtpd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gyemyxhgd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfrygvr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gspsmssop.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/guwnkfybt.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gzartkpyt.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gtvppenyg.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/glqqffjde.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gpowlobve.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gtrlvgjbi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/grzxfxcxc.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gnkdeiyqc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzforec.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gtiarjksa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gjtxxtwmt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gykthjrtv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gtcpwwuiv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gstxrbxbk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/goikzvvka.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/ghbjdrdlr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gjkslkwhv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gkhydmrpk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/ghrorzxvn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gepszptcz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gbtksrazj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxqtihtxe.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkgwxkgip.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/goofidxwu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfvcrwsmi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gcvmfngce.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gcwbwfscn.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gsiyizjww.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/grcefkpui.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghutzivcn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtdxjdjet.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gyqzmvrgu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gibyzqlfw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gpdwluwip.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gcnvpwqst.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gjcypgypo.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gcmfltlwl.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gwqfedftf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gojginbdq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gmyxllwba.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gmdrlfqwn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gpifimpsd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwahdkhly.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gygqaigol.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/ghpuiubdq.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gzxnpfoqk.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gbxvbjjcy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gshzwuyug.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnsxiyrya.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gpbmslttf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdeuxkuqx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gxhedrhre.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/geovvzlar.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdiulbyoo.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gkfskqnep.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gejihwvph.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gtuhljbje.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gvrkulsie.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gynsvzfgr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gdfqjvzty.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gnelfyjnj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gkqxbeyqs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gflcmvghv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gvftognga.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/grjzyfimp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/geclcceoq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtvslbhzz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/giakkaack.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gotxeayat.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gjhvohoiw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/giahbpwza.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gkxhqfnhr.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gmhangvbm.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gdrnegosv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/grihcqdxm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gjmfyhmke.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/glpjcxshg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gjpbrhtjl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gteeiwayq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gmivxqusn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghkoogwwn.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gxkyuhihb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gqxdrjhpf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/giacffgqn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gxtuojydk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gebrugyjb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/grrqgvjnq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gjfnxqevt.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gzabrnhxh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/goctmfagv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gepwjlfph.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gvmxaiidy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gkbjmbfkd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfbosmfph.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gggdjfims.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxciexfcw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gncjofnsx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfykxlq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/ghgifxjpk.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gahuvonxm.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gsaigyber.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gpbnfmrag.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gzqxxfefa.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/ggcpxzpjj.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gkaffzhba.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/ggwghemob.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gpmssogyo.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gyeukiqeq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gxivjrtdt.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/giqroygsx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gffcdhvdj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gnuxqtsnx.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gllbqpiro.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/ggzqhlrvu.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gzjkgiyud.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gjpjqspfu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gbwgmemks.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gehmlraav.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gzlyazxrn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwnztamzt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdfrilcjq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gymaytiyg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/goalvuzfa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/grtnkefgr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqnozehcq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gcgzjuqmq.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gstzjcddf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gqacqqsop.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/genyhmbhr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvbveybml.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gofqbzudh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gfxefnpiy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gindclesm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/ggukifmrq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/geagcjeji.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gysmwnmpo.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gcelmsjsv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcjaorvxs.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gpvagstaq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/ggojtvgnu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gllxldxaq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gztjkwxli.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gchllxvkk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gypyyizbz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gaezzjgke.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwfzvdrmi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpurvmjyp.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gzxtmdzlm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gliuhorot.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gsddjrfxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkehdtymc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gonpxhezm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gmtdndjyk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gkfxclwgh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/girvxmvyi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gzcngucjr.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gsvxvkvgr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gihfcwysz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ghepzlyte.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gumuvvstf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gnnjixqao.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gzggthmqn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gtnbfokws.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gmepqudtb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/grpsrsubm.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gtewfqbpd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/giqyhmtxq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gxctyrrdj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gsnpolctl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gpjggsbbu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gizkthdug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gcilnklxn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gcqlirzht.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gskeuilzx.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gzlgyoifb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gyzpqypgh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqabvdypg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkpioixya.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbgnemtth.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvnwykwkp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gnslezyyt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geawnsjng.sHtML


<!-- 参考信息 -->