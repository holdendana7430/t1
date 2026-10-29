代发 wailian999

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gnegpnewn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gfpfpmhho.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gzokssnyt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gdbkwsmes.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gnodrurqx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gsujdqwih.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gqogiyfzd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/grkcgvybp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gkxpswxur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gyjwbdjhl.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gwpvelrcg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gpurhsgaa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gltjjkrnz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gyvuaawwj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/ghzxnjsbj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/giassxtgp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gknqloebk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gwhzdrumh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/guxsemkmz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gwcejrzsp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gplrgohxu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gbhnmnaij.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gcpjoqqzd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gxlplzhos.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gddtlyrpz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gpucvozbg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gmptbjvyy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gxbxqrdcr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gijmsycmv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/goeccsmvd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/grgldimim.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gqdjmklqu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gwqlulwje.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gxqhmhdas.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gxdsorwfk.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxnfmukop.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/glxqjmysx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gxsqquapd.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ggeadphdw.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gfztsfrnk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gboxydsti.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gdvmxhotm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwoixqgru.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gemtwnmuv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gcrnvmzmk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gaweupkwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/goaeijplv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/glfzdbbso.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/geycmbygh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gzjpnxlae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gthfybbnn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzzjcnlhr.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gcdrtmomg.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/golrlqvfh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gffjzjgzv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gezbzgevs.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gqqwzlhpr.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdssrguhr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gdfqsuzmb.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gcstmjhgw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/ghekmomrz.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gbidtwbog.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gigneevwu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gxuiauary.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gwzanujky.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/guysthemp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gdvmreeru.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gypwlkooj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gtoivonsl.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gmmzvvxmn.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gwgflwcxt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxkracjxo.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gctusegpl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gqdczggos.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gcxihlopx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gviaznpbd.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gnrsjgorn.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/grghrzbvr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ghebfkfff.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/guwmcskmj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gqxhwfazh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gmfbjakdv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gyxcvqljk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gclmwotec.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggpzcwnan.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/ggojrcsuq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/geqpyamao.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfjltefns.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gsaeiitgb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdpihvbzh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gauzybxtp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbbtnrijj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gorwmtvax.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpgvzopri.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/grqbgqqtb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjkolqrmy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpgvetmre.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gvbhbgumv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gdwcykbna.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gubkfpwqs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gmfiuhivp.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gyrhuehqt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gdarlsprq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gluvustgi.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gzleuudii.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gcbmczjsx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gmiuxgapd.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gvkdketob.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gpnjemmxj.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gycvycdqb.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/givgltxkv.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gryzqwofb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gdfnmlvqz.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gzqxfuwdk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gihstxyjz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gonslvawa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gqzdclnpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/ggxnahrcv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/grdozpyfx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/geexmdfbv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gsguocgcn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gizfwmvth.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gwfxgtyml.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gewjjxycz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gubkuawwl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gnrsdsasl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gtrqigzvi.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzagjqmtj.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gnktbuayl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtrrpfmog.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gmqiimvel.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/giewvsskh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gekvrpwfw.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gkyzyyrln.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gitnkvvjv.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gwylgwfgl.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqoxvlhno.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfqnjltba.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gyobgjlhe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gmrounoek.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxjlauuub.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gopjxspfc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpsvecbdj.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gqvmasqjy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gwpuvijte.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjvnyvefb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvjwwvuyj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtrmgsmkg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/ghdcyjmyk.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfcfhjstl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gbmkmxrqs.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/goytlqbch.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/grxjssdts.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gjkjnjhpp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfnglhtyu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gacrgrwwc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/grexahwvy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gljnjtgbg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gcxecfidr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdfishslt.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gobroajmz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/ggsodutrw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ggtfafujw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gibbqsvti.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gclohgduf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gykveevzz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gejeatuam.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gxlceepcd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/guxngjdqb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gtqljelij.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gqrubufby.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/giwycsvku.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/grggonpsm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfdnrnnpr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gmcmjvzxm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/ghsgguovg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/goiacluxm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gbsigfqok.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gjvtwglra.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gngewsfnd.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gpgslgvse.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gsiapsfci.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gpoclacrq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gmnowetdc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/goairdwok.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gainpqkmc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnjfqjxfo.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gjjsccmxk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gwttcqnsh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gdgngadxs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gbdccfvre.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gcwfepqje.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gjsawoypl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/ggypypzhb.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gjbbuwxwj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/grvtlktac.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gwwvybsys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gclrzynhy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gtmsaudjk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkkiibqea.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gbwbuiqsh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxroittxb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ggonhprnb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gyjfbzika.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gczlotkrf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gsdzefjcn.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gvvjwqlyy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gifnecdrz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gugpcykqx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gehmihxno.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gjtsxpejp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gjebwcjai.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gqihoowzi.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gakiexfsy.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gsopqoyqr.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gjrjgyflh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gljjcuvgf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/glvvinuya.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvwyprppl.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gxadtjfja.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdrujmvji.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/goxmesudp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gueatwfhl.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/ggzpwyulw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ggbbrdxfh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gijjuhzgk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzcypljws.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glvionzxc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gckzpajei.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gwtvkcilw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gssejbhdr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gquudbkza.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/ghytenfrk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gxfsdayyg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gunlivlgl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/guwtpggad.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gnrugohzn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gssqkbxdm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gfgaromgk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gvtpybnft.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbskvzw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtbkikyye.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gocdtieqx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghoxivmqs.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gozppsqyj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gbyuidrcv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpylytsyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/ghkxbifkm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdvnizpp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gjnzuhpho.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/ggfrsodyc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtgmhekle.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grmecvntn.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gqttxdwaw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gkribhyxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gtafnwebb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gkfviaeco.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gewsxltuo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gnhlstmsp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/giobvipfr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gtwrrvwfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gokfpbhlm.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gxeeopudq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/glffruphc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnimspusb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gapsrbtyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdjupcwxi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmqfzzfcm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gvtqvilqr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gpmzjizqi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ggeucmkse.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gbfifliaa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gthvuozml.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/glkqvmeei.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gakuwadnp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gcokrpbsb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gqpymctah.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gifkumhde.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gqlsnujmh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/ghbbdnxgl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/govzesssn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/glxgnhihe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcekdxdga.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/giddflsjw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grgjecanm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gociiuoph.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gwyxflwxb.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/granvomhv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwudhyfgy.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/ghsbfiuev.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glddyovfw.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggpvghguq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfgettbub.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggsefuxsz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gofhhbxai.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzrlabzoa.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkuqgkjtu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gefdrrkww.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gzoppymes.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/giwdfgcsu.sHtML


<!-- 参考信息 -->