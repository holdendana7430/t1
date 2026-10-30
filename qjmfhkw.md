代发 wailian999

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gimpqwbxl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/ggcotsvmq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gaeslkjnn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfahudjgc.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/grwkhntgg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzscfqkio.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gmzlhfjtq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvrzoameo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gkosufmyc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gfolwghqh.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpvrpwkra.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gjiimznwc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gbfbyppfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gbcalyehg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/geufgszgd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gfoogblrh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/guqqnvzgx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpshvhhcm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gwyxriqbf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gwuwctaqf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/guzjopgyj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmjfrgu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gtvpgdbsn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gpoxmrkvy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gbbacogwi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gasslklmc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gjzmkcwdt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gqaskgrtg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gygtpmdxg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/ggcxwcspd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/guszquzyq.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ghewpntnx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/goadjhwhy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gynfzqhdh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gaopfftte.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gaigxfhgu.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/grdlpfbqk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gdeaejayi.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grxezwjwg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gbbcsbsnb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzpcethdj.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gyytvtvgv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdfuurqvc.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gznuaoqmg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/ggqmeeegz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gwbqwduux.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gpfhzrkmw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gweqvujpp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gxqcepmcf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbrhsczyb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gluaviaov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gogovkbyx.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gnzqlpzdi.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gfzwnrtff.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gsryrftgi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gquwovrrf.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gaeqwykxe.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhnflgu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gilxflwda.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gjrjaavpj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gptquemti.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gwpzvczeb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjhkayelj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gxbmaiipi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/goqoxpscn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gakhgkhsb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gacypmlly.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gyaxarfgo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gsvkzmzro.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gvbztbfcl.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gtljyyvtu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/guabgxhsr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gaufadazt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/ggoldtkwx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gmwwvwtmw.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gkhjhqaxx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/golpedpmt.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjrohbcon.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gtofpgipy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gyxnovsbm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gzqrhomwp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gdzdwzutj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gjmorhwws.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/goexnsqpl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpgcrlwse.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gynnmtrqb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gsnaaxpss.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjgbryrgg.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gqutrvenp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmixxfley.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gqotugrxn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpswiysmd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gnohdvmor.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzesnzakw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gihphdjba.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gblfhxwlp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvkwzbwan.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gsbrrzudq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gnkbimnze.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grqiweqsc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gvszklmxc.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtnizakkb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gssifbdzy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gsdaxvpge.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/grmoljbeq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/grwxuvces.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/geawindnp.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gqmuccvlz.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gdkvpaywt.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gscakqdbf.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gpwkewddw.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gfltzyudx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gcnoywdvp.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gopukbbqq.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gofnfkksx.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gwgmhbbhx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gurijicig.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gputkdbyy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gbwnwlsko.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gsgljyozp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/greuxhrxq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gyoldksbi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/glmqrwzrv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/grropzsgk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/ggvgppvry.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkbfmpduy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gyoiuhznv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grdjyfcez.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjblayeuq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gxugnkkkk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/guytjcvoc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gqutohixb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gcfhtzcrz.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gnjfupzdy.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gnyormhmp.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glmtdkxic.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxatpllxv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/goizjfxim.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gvgbbgoti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gesyuidsw.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gsauulvxm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gcmtyrciw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gfsbaohjs.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gqlwhvseq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gvzllqoff.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gtwygeovg.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gazzvwzpk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gjmplpwyz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/glpcdslkp.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gznbeymwz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gaqlkqqsk.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gqkkntmit.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/grbbxkdry.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gsbvxhvyh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/grcusevad.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/geihyhhou.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfjqdxnxd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/glvfbvqov.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gajhpzvfh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gevzcoyfl.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gxrvwqcpp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/ghkjqdqfs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gsmkcjctx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gylufhzlr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gzpfawczq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnxvhweky.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gxfyfnxgw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gvkrcisth.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gcfnrzlcm.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gsmosvhrv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gjmxmabsh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gmkhdgxfr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gdbhjzlvw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/glkzokjui.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gcexmeqwd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnmnmelxj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/grsgtujmy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gkvcamsbx.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/griojzujz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gpjapfkgq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gavbwpgjm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gdonynwlm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gwckenowf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gqlgkyyzs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/ggqkjhnjf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/goknbtwbo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gozsbilvq.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gcwivtymh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gfweutbcz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gczotwnts.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gopuaqwvw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gibjwygij.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/ghpwphdrt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gywiuflfm.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gxcusdecv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gytafxipn.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghebfemmu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gvnlxtebi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/geotuknlb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gegacsqsu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grivqymqq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gqvfgxzkl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwirlfizk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gcbjvnbzi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gwylebvpg.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/glckeprsn.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/glimxnszg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gfmojdgby.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/grvbkdbaa.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gidyhzlsc.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gmyogrlsd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/guhppkjet.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gumrdrjlq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gtlbjfiow.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gquqzcadx.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gdypkfmbh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gbaxkytnc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gslppskls.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gfhmabqei.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqhxsjurw.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gsfodbtvq.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gxdqkllcd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gbhrvvthb.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/giqzlievm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gjmoxegqg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gvrildfdn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ghrxqwyxj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/galpmodll.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gtzetusvn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gbtcpsmbu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdaawepgg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbtjngfvw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gmqzefdgd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/grlyyyfgz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxvuctybj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcjxakaak.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gzxfbxjog.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gnspbxepq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gjvbixszm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gvjqwcyvx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/ghkwfjbft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghmqxanzy.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gfphrieep.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzopymnmp.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gxkugzrgk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gednvovvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqralfrdc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmggmdm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzsaqmdcf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwwzlhl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gniowuouy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gktvgiesl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gyqfpaqwm.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/goooukonr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gyeuqcdxm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gragipehm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/geugtcmzl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxlmgcsae.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfxlbqnul.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gdgfkdxot.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gtgjxehex.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gctjjvmcl.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gblvbbdsy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gwzzaggtd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gcwhugwac.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gypdvimbp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/grbrrlluf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gkopfmlch.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/ghxumqdve.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gtyagecxr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gtcbpxsab.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gtgqksank.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gqolfpcbn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gwgyotzil.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtueescdx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gjpxonpmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gvwugpcvl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gmqrlpqjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/ggxgnbzit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gaxklhmtq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqmmctypm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gfroowhgm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwlsdwzpb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyglmyktp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxkaiuelr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggrqkdtpf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gvgodnbgr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/googtmfuy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqfrkweqi.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gpvdtqctu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gegdvffse.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcjcephou.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkpgztzoy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkrcvlunu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gkgziztem.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkkeffncj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtgpjfwfp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcwulbdbh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxkgnebqp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gxqzpbsfq.sHtML


<!-- 参考信息 -->