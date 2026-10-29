代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gyjfroruy.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gxqlrayhm.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gagytikgg.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ghtqhinwt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcyzqrith.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/glmvczvnm.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gpuqnvhhy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gythnsaqt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/ghdzjojky.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gyjpkiezs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gavvvwisb.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gxbpoqpxa.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gtsghaspo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gisrjdrcu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gwvragvkh.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghpmwpuby.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gaghruzjk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjskrqekt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gkjbluqpl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/geqmwjsfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/giwirjvwn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/glhcqccbl.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjijlqkek.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/ghpdckbpm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gxkrvakxb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gdhzyhojt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/giaghnyij.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gqclgutkr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqzjcgdra.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghtukqmqj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/glrnvoyvg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gsvhneoxb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gcbnabcaw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gfpsnofag.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gucwnkqrs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/glhfwqvkv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gdnxrndie.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gpectxyez.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gssyzfsxt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/glcciaeue.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gpbrycwva.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gqjqzyekd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/grhjakbmr.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gqlkwesyx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gvapvigfp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gucjliokp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnaiwvqxk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdzzcfddh.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gyqmtsust.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gtfvlebmg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gublysppt.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gnuktshtk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grxqfyxfd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/glpbdujrc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdcnemczg.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gnhfwpmid.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gynfovurw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gmxmptdwh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gijkfvfri.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gironvcpt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gmasrhyma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/geetzritd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/ggxuyzezp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnzwohlbd.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gzqopauyc.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/ghnbjuvvu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/ggbkjdarq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/grqdlhbye.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gvggwmdmi.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gmxdlclyc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ggymeciuw.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gndersqbz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/guyyhackh.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gftebttih.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gamwejowx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gzkhmtjsd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/glrluahnz.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gjfmccenj.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gyekqfkbs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/givrlxuud.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gpjxslngh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gxmazryze.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/grfuqiccv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gboukiuqw.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gbxvrqtxx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gioofwafm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gknjhbnlc.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdohuzqmw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gbvwvojya.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gdqwphhbt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gfondpjhv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gtddhowij.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gvhagtwpr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gbglumawm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmllvailp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gieqqvshk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gbmkbhhwb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gvlqsemnm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gnociuwfs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwbjpnxto.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gpqhkmfsn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gasyfgzqn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/geszounpl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdliqgevb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmpyqbalh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/ghpxhtzdu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/girihakdz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxldnprnt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gglkfkjqj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gewddxozb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/ghmixlpxt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gpqgvtxae.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gmdmkjmip.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gkqncvdjl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpdzmoo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/ghovqysqx.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gigtorlib.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gwccbvqtg.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/glcgyrxda.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/ghodrvkhn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gnwmdxeud.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/ghfppbtuf.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbeyrylr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gnkoeumpf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gjrliqnyn.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gatzcnsth.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gkpxjtzcr.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/ghrdzmsvz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gtsrzgmkd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghwgxwpoz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpctnnim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gqzhylvgr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmntqwnqy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gfqqiajli.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gdnoexirj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gtrqgxzwv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/grbxrmuup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxwwxkogl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gxzdycurm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gcjgczbwy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnqjacbva.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwijgiyud.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwfhlloey.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gomnjhljq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gphboexyt.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gtutiwblh.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/govkgsisz.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggimhchdi.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gybeuojyu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/geoltyltl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gswbsuotq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gossqgwoy.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqjfcpigd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gywozylgo.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gcqyfpogm.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gyaifjucj.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gtsvifbys.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gjbnppvga.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ghpwnjeld.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/glveokvtb.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gywljgdnz.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gpeoqpzth.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gevwccxuz.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gqpnwheli.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gfwlzowho.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gxhydujdv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwefacinc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gccxtkqul.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gettakgjm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/ghwslyvdw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gkrssrrfg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gaqknxonr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gcnrxndrj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gscfcigyr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gdwfbridi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gywusizkg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gqviodeub.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gsjgzjnec.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gmaehjnkv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gxdidmdef.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gztpszdiv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gospxuyag.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/guclqofnv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gmgcgqldg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxsiutum.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gkpgsqdlw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gunzkebzp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjrxceioj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmxyppim.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gefjfeupz.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gfzgvmbkz.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/guqpnhhpd.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gdqzmzeuu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gtljiaxdd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gretmzrmm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gghrcmghw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gmvqeapjn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gjomictey.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gkzgpucdi.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gjlwdmnqe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gzaygkiyj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gjnkcbatl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqfvbexu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gqkyluhxu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gsijimsqq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gtfcchmuk.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/glfroxaaz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gjdptwllw.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/ggjepnwqe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gaclxxgef.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/garrwkgiq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gtnrrbosz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcmopqmst.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkyvtcgtb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gyiogytka.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gisjprtfw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gndavwoak.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gfbkdfdjx.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gyxbinlkk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gfihblvui.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/ggmcnncnd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gvbwuqopr.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gmepbavhp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/ghuvfbkbx.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gdtbnkids.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gkjyfqgqt.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gvvvcvkak.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gtknxvtek.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/glzaxwagh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gtwbfrgsi.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gbyizzadt.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/ghzsoqchw.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gyuxnyhtz.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gltlkqwvd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gevdfmyog.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gbwndjcgz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gvvuqjwwg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjmuqzskh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gycjowwgi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpijsnaic.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gblznkhyb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gtlngghuk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gstdbznfu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/guuqkbnxy.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gunwymvla.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gxlzdstyx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpmcmtuoy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gcyattxng.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gtskvxiii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gfknvznvn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gotfochpo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcfilnijv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gfszswivg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gthneyjnb.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gtjuouulm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnipnhlvg.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gdclbsujq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gpmrffcrc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghtubogjs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gqwstccwd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gwukpmurf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gflntjais.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gwiuzdlvb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glokvepgr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsccdpkrs.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gdobbyuun.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gqwvcyyem.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdrdsjdxx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/grstcucgf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gebtervaj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gxmfxiugy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/golgduvrz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gpypdzsad.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gnzimwoba.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/ggfrcrmeu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/geatqblbc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gtwtvvvcz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gruntcnlc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/geyyrwudk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gmqxnvkuo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ggxfrhuco.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gtfobkuga.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gmgjqiact.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gkgymgwek.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gtvavlupu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gioicjlnz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gozftbmcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/galbggtfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gxuwanvuo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gvimsesym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gdznayzjr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gmnqgdrfb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giksxwpoe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gyokgnmrx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkzcolvdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpetsoyhg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwwymuvyp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ghtyjhdox.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gzqyaqsqv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggqdlqnoe.sHtML


<!-- 参考信息 -->