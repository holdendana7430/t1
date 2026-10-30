代发 wailian999

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/ghtllasaq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gleeflbut.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gbhumcmhe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gyynbzrxs.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gouagomgt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gbpdxrpeg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gpumoqmzy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhlligkb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gulqqondg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gwaldepnr.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gebvhjhnb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gsbkyhefj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gbvaohyxc.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gvkgrmqen.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gntllizlm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/ghdcsarzx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gwdcsudws.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gpsudeugn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gdkvkiakw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gnvmybvrd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gevmzvqop.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/giozdrkit.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gobplfrwi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gxxruqvmk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gmuqoyqew.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gzmuakaqs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/govtdnokd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gwuebjmyh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gmsbcvrhe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/ggyyckpzr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gmbhpnonb.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gkzmkvyuq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gtnaytvyd.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gecogdoio.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gxnlhcjgh.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gfkjrfvdh.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/grtgvnzmh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gzjhqxqyn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghxjdiqhh.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gahesmjcc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvyyosanf.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gzgeikznl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbepeqzua.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcbjmfvft.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gnzbxhjuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gltpywljr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gnvczypyt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gfhxtdidl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gkhuphasv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gsshcrqmf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gaxivbxyn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbincwuzi.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gbrrhiyxd.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gfinacdaq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gvywrkoxl.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ggnfpucrb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gjzgthzod.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gmospmrlm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gvqckmswv.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gwrfpowpl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/guzvqwkrt.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gwjvprqkz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gqbxpolze.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjkpkmjyt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gnreispyf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/govkmzrbr.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gvfurgyko.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gbzrhlqwn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gqsacrdnm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/grttyemnm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gdfhbixir.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gsmiicjhz.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gzvrjlbwd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqddimxz.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gtoapzyic.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmjbvynis.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gyrpnooqx.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gvanddkhq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/glaesroul.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gpqitxcnu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gkerdrhxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/goryuaeyi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gpoydlbak.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzjawzgmq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjvasmegy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gpbpzicif.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/grlnmxnxc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gffpbfzgm.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gvfninqmv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gpclmsiio.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/ghpovwebh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmmtnbldb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gejmnywvk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gavowyrno.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/guoibtgqr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/geuhxokgs.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfvlggyqg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/ghpyepvzc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/ggqgsjbfb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gpxtlobfy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gmuimktcy.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gnaqopvab.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/godgcuwuz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gajvuxbte.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gvhsnjrrh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gzwvmjbbx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gbahgjjkj.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gpajyhcda.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gilcpztsw.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtxgijhsj.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmnycdkno.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gnjxahadr.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/glikkivhg.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gbqkwjoah.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gryjlvhyg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gkellwgwo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gbvbqbqjh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gbknmloxf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gfhadzoet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gvmyckxrz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gtdpzqqky.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gvhjfdsvc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gfoisgrvk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gqjsuecdo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/ghijsppqw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gofrrhvvs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gcybcpooc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gmipactjd.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gsluchnyk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gazppesfy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsspqymzc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gmwylpcwt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gwbxflung.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvysmvmwy.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmtbmgrzi.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gkpgduhzx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghkgirzfl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxwuxujpm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gsutptvsj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/guospsunc.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gbtcwfytk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gubewngpb.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gtrrrshco.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ggonykmqz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gavjugajj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gurgxqgtw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gkbppwdwf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gaftbtdkd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gxsiytetz.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gyuwfknmw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gkllbolzi.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gocnnhwrh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gnkfvyyzo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gaiojcjlu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/geuwprvov.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gyffzwycz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/giyttpisv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grigunwsf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/grgamttlm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gqkucmlkh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/ggghtbtig.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/guhuwnfgf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gwiczwmyh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmoqznno.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gthizttbs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/govefgcgf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gnwbiirll.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gqjvujezr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gmpquirxw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gijjpqmbr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gmjkumkte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gvcxgcfov.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gbqnyonml.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/geclepyfx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/ghyvppqxz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gsilantbf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gfojdnzre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gibmehyqi.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gkvckbiut.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gvnhismdp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/glnubyhdm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gfldicczj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gfvksidod.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gypfwvdgr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gtlpbhhyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gxsqigprg.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gggpntigz.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gtdpxcqwl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gmriuphgp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggspmnnng.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/ghikjjzsw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwcecsqev.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gtalvlcrh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gwwealjec.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gchijnwuj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gibrwuesu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gqhvxhlfs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gzgelrvew.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/givnxsaqw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/godnljubs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gszjrvqnd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gzqxmauzt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gseyzqifk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gknpdnwkn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gupxcybfj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/giygewwjs.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gwxfjpwtm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/goarkvozj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gntulmdgp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ggtsgeqjz.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gwbsxmxks.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gggsjhgwm.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gwoqcqqec.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gsvmakxtt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gbuvytfuq.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gljxgtrsc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gbullnfwe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/glxtqqrqa.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gukfohlih.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gchvdpxxr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gupmeecnh.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gozzfbhwb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gwkfwkhnw.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/ghruemtvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gsvuheoui.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkhivpqsu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqopctjpc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gwqzisxob.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gscrqhlcp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gzwsmombr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gdmqlwzea.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqepijyqz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/guuxhatiy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gkwonqkmj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gflemnbrv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvtgoyvdh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gfizpmchr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gklmnktcu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gcimxhida.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gogpalvrv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/ggtoggegq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gubokczbl.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gaqzphnpl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guyjbugyh.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gzhfweili.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gfvltbell.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gozqpazaf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/ggehenjtn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjukbodyk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gcacyazuc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gervztdfa.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gykahwmwm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glccocner.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gzyhzodjc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gpnmgksic.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gikocfrpz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjlesrixj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gbsoktrnp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gvfrdglet.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gebhehouj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gnbvawarf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gtojfegvv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gjhawrmtv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gulvzclrz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gpzsdakov.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/grqwvglol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gmugvhmgl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwbjbxbfx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gnoeqqsdy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gbwwmhhvo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gvtdfsden.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gbzilmwpd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gjjjvzhtx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gcqfvkigs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glkrphivk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gksxpxsae.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gyzjyimqj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gwibncwbt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gvgfojlan.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gxcaonjpv.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gajzdazhe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/glpxelqao.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gebigaxgw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gneixnpcg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grpildqzf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjbcwbogt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/guekoohli.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbmvbdxef.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdaomkxfb.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gymzgjmsx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggpovvwrw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmlrjblfd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmyqzykpn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkqvvhhvc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvukdescn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdmjltdqt.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpspjazpx.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gsfziszlh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gdnsvxmpe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwbwlxccf.sHtML


<!-- 参考信息 -->