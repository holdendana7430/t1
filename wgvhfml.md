代发 wailian999

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gookusnvd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfpknrikh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gzmhcdizn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzzkzrqgl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glfchnhlu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gizmptpey.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/genbscoca.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gpnawomsv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gjmveetox.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gllgkmlzy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gxptziuqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gelifedhp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmqrgjkpy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjdhahxuq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gmabkkzur.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gflfvgsaq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gtotauycb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gpldahfxh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gzpsxpgpe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gspnnqegu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gtilabwft.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gfqxwxajv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gipngwrsw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqavorkuo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gvoptkewu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gjgojzqhy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gkozvzlxe.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtodidwwz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gknbrkili.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gtspglknj.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gstoolzeg.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/grmgwqpdv.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmqqnlwma.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/goofwpbgk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gegccwaze.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gojbhnigf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcbfzqecr.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gpncuxpax.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghllabpby.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gnnxwlgcd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/ghhdmtwbk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gdfznwryh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/grubsgrzw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gpxmricii.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/ghigpypgg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gpzoxcyfy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gbasauppe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzgbanhef.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gdpfkdspl.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/glhrxfjkk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gazhncgrl.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/glcnjrnpw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/ghdroofna.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gojwlidhz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkqtyvebk.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gwtmpghcv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gsdqrjfow.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gwfokuuys.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqmghghum.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gluzjegyf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gwyqdvfgs.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkothdpmj.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grfmjvysi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gafoqaaoy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gnahcypjj.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gwbbczvds.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gthgbkpjp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gcqkmstkq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gdeswxsqk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gfzuhswue.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqughmhvw.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/geytsbnac.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gekvdfxcz.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gsbhqqtmg.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gevpeyzpx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/ggbaciblo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/ghjbsagei.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/glvluhmly.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxcbfammm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gzcyicmqj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gtzdnizqu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gyszmupuj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/glefnlndk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gajoxofyg.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/ginhfelri.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/galdmbgzx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gbirkvyyh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gyegeccjb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gltimwfvi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/geayfxwub.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gpjjacugc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbuwfaolq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkrqtbfdo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gtmjldcim.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gklfzryub.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwlbmukja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gdkrgrhls.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gznjjqgmz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/glvanixvx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gltlchbia.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gjnnvmmqw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gysxeuegc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gnifaxgwp.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gtphmkdkv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gsltnwgik.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ggasesdtw.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gilfoywxb.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gqslabtvv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/grxmovmdn.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gxvohgjfg.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gvqilualj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gxucgtbkg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gioyxnrmh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/giuhsgxme.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gokslofin.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/glcxzmuqp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqscorjau.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gqjhbcezs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gdszdofnt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/guosstrkm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gmdchncje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gxnznlpid.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/ggjiwzueu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gaeqfecin.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gyboeurde.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gxbppylqj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrgndbao.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gjoepwakn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gilmlkwib.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gjblhwpxt.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/guaqwomtx.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gxaosfcjw.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwqbxethr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gourvigml.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/glfiedprn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gcczkycbf.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gpxeazbaj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gwubapjrv.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gccmbxzqv.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gjlihlvvo.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gldikthtb.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gwzitohsn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gtunebowf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gycjafhgj.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/grcrssjsx.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gvqyvssie.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gzatkqcls.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/groognyyu.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gegqnemml.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gehrynzyu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ggiecquhl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvwjhoams.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gchhgypmq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gopgeifbt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gopvjgkjl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gzrglwhls.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gfrocpjqz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gaqsovdvj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gvvmaqqlh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gudyuzyzq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gaitbsfzz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmaehkryi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbjkrdk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gnkhxkmzr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gbobuvjga.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gulgawtmr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/grxngbsli.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gzvwssxkq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gfqibehif.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gglsbomrq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gkojymttf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/ggxoqpfdc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/ggjkxqtvk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/ghfscvwgt.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gwdmmqead.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gttkmtufz.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gttdddrvt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gfhjyhyuv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gnmqtwikf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ghadhxawg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gkoflhxcx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gbtwlzcmk.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gsicfzeaj.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gijmizllk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gptepgamf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/grunaymvh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gcmixlgav.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbthwaqdu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gotvtbvei.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gqkpsmkcl.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gjwmgecla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/ghojauhoy.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gyeggdsjr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gxundxczn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gdpqdueis.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbfcwfwaz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmjfbinxt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdqcapskb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/geueysgsj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gncooejaj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/ggmqhhtur.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gtgkhmxic.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/grnpiycxa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gypeibysh.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gcgmozgor.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gmvwelmcz.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/guhbebexz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/guujsdune.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gclkljryr.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gqzlvfkvu.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gfknblyux.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gsuypepvp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gujnpgohd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/ghurcjuoz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/glokedaov.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gmzlqmftw.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gzyvdxsyd.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gmxerefbs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gmcvcgcrr.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gplckbrvy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gpjcugkoh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/giljeljdr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gcxwpiqph.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvfyhzvhp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gggbyaxjo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gwcbmbydi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gtgqcuwnk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkjtzkgcj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gzhhltnmc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gewpsfhyn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gufispiua.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gvjuqxevh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gipdtrwds.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gomqxfskk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gsfsuiwpf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gmxynowmt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/glipddzsp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glsyttbrr.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/glozecglj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvhxjllcv.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gulxzdcme.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gbcqjjlgv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvugrqzyd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gcihfnsjd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gqoqihpvc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gccjfcjqo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gpqmmcygh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjogjvqki.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjesaxppz.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/goilikjxz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gbugrnajn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gpjdnfnux.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gruibwhxc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gslikoufo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gdppneefw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gbazwvgde.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gexnjppvq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gmyfcmjwm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/ghijhlauh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/grvppznna.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gjvhfzniy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gxrafefoi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwoaasfkt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gfarqhxuf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gniawcncn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gpqopfzpm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gtpnditgc.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gzaorqzks.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gffmjcegj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gndxtelcy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/grwtjzwos.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/geeerojqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/ggplixtdx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gueztqfwt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gdhvwdbnn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gbwsoloha.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ggzmsrvku.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gcjuymvrv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpbnajcnv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtkhkjmsa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqymaxsmh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/grthnkdgg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gfgwkngfn.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghzgeuxic.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guxrlzmrh.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gafuinrup.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gijsgctkw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsuzjbpzf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsjmvacjz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmkmulbdv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggcxszaxr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gufolfgsv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/grjhgyrjw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxkhktp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gmdetfeau.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/ghbnmmzos.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ganhqfdrl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gjnfzagrg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/geetuthmg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/glihuoscb.sHtML


<!-- 参考信息 -->