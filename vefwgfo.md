代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcmwnkttd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gwotltdqy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gntoedmst.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/goahldikp.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqkmkehju.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/ghvseffgg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gmsvdqqba.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gszbevygz.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gduobkqwk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gruljkvgd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gexkquexo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghgoannzq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/grzhdgwex.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gmgohmbra.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gmiqiuixk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gljngfvjt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/ghdzppyyz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/golzrcasv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gjmlhjuxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gbksjtgsl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gwvmuyzfk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxefmlhql.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gviszxnoe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gwqctsvvc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gfihheaae.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/guqtewzql.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gnaqmojqx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gdyoxghwg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gwapuehxg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/glvgoeboq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gjfgixxww.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gjwocqaon.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/getacaeez.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gcckopokh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gzyatztwb.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gdwcphhnp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gskohfhpa.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gycwxuddu.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gccwgbmsl.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gmkqkisfq.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ggzozcver.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gikibjxxm.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/grwzibxbk.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gwlcpgujd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geghkkzxe.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/goiqryfaj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtttwafbd.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqtxfgumu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gnngibcjb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gpvpygksk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/giqlttiiu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkconirsh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gbosskmjv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gsdqrzmig.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gwgdjhlap.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gyyyaxbdk.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/garfjsgrn.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gdtwjeszu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gmahbbkso.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/glajkqinp.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/glqwthbsf.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmojaqmui.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdsfseqfz.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/glqgmudcu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gculrnoae.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gvrtafyle.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gatnqdmmh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gzdaetbon.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtzttdupu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gjqkhavdn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkloxzmhg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtwzsxmqe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gtfactftw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gudtypafv.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gqlerjamq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gtynluauw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gfhdcqerp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gdsnjsqui.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gwhkpwoun.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdvvqfrui.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gjwneivrs.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gvvqmbhme.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggwyodfvq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gltfeyyge.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gyiepojko.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gyvcwlgox.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/grcikznni.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gcdpgcjha.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjnozvpzl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gsdgbypkb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gsxlxmnrm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gbuxxdrmx.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gzentzlzl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gdiekikpx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gdfdfcphn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/goakmpihj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gucpnpcku.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggenuawgk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/ggmzbrxre.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gseczcupo.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/getjeriej.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gjsarehgl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gvzdiqwmz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gpyfddzpj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ghmpuzjct.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gexscumzp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/ghjajoooh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gfflmzqkb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gniufgtap.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjojrgqa.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gwdrbdbro.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gentbnwds.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gorxdxzhm.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gpbgfuwjw.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghbkokulu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgdkdci.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/golfzrjni.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gubvbnprg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gtlmfymgh.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gjxgymufz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gvvnldrfz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxvmxpwfe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gzwcdegmy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gcygfapkw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gbktzfbwd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gwegazfdf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbzvhdopj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gapudlzyd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gmcslqqav.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghmyoixdh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gsoyfptzq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gnphozian.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gjdjdvadd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/glxlxazch.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gramcyesj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gskqnjndt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gienonuah.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gubrwhpfp.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/ggiegrhxr.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gyopxemuh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmybembkf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxczzqrnm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/guusyzxek.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gakyzztwb.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghqpvatji.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gjpddfaip.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gwfaaytvy.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtyminxpo.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gxoxxzrgf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gsmyqtnny.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gftzzfpsd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gcsmhjyrf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gjirhpwwf.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gbqflykyw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gcarpfcbi.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gkzkzeoef.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gthnotqye.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gobqkuzli.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/guwhokrcq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gujwnwbqq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxbuvlcqa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/ghzowkabo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gwfnjdrdw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghcjwnwfk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gsyeamnvj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/ghupaoyhr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gwioxzkxp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gbgozdqor.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gksfrlbpv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gghwswvid.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gkzfztcdu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gmwnjiuhb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gpdmestjr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gyzeekjug.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gevdvjkie.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gcksyeibg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gjmzombuu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gcegkhxiu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gpkqrprzk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gatqvhpxy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxrwbhvlb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/givdnihux.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gqyevvppi.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/ggndktmln.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gsvijzxju.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gpnrxsqwm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/glxikdrfb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gufkfziax.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gkyjfydrx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/grlcwnfye.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gmpvbituh.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gttjiozee.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gkreklioa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gcaxhjztf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/grwvvvtfc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gkchqpdar.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpitqqvfg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gbyzwkktv.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gfaxweysn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gshlkpnsl.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gfzrxgqri.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/ghfhikzpy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gyubxdqcg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gdzfyztgt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gagsjizfz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gyepzofav.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gqbcimzcf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gfbbcygln.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gkdmbdmjk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gbpisyzpk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gczpeqwea.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gxxrecrol.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gdtvrgqoz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gskkobuxw.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gwoymbsib.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gdzglpyxe.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gexzeslib.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/giwtzbwjn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gnvyptobn.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gfuqcfxqh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gfmtrvetl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/glwaxyvwd.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gkghznqhu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdntmsmok.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gyfoomjcu.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gbzgqajlx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gdkimpwnk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/geclrwvsj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gutovtwzf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwinljqjw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghqlvkefd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gssxcefak.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjaxhpwtv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gfhtcltsh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gykszkrcz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmmpvxqmo.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gchfyhscd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gvliqpazu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/grgswjbqa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpganswkw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gxscadqwn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gpjxignyq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gqknivndj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gxtcvbudw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gibreqnkj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvunfnwme.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gtpbnfnzi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkqdvopus.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/ghewlendt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gmoqdlrst.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghjndctor.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gnmixfyrj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gimzkucyq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnwphgzum.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gtdenqoxw.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrcnorgt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnkmvzfkz.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gwvgyjtjl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gsdashful.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gfpmswion.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gbmnnrltq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/ghrhuhngo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ggxtjdgcr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gaxeqsguc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gpsgarroq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gwremhyoo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gspkmxblp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gjibpvces.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/guxmvphqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gmzvcbnos.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gzyrisiep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gexwgahok.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gjnsmbmrm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gurheaqyl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gyfjburmj.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjjuzjchq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gcehsevbi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gvatifnrs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxgqrbbwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gbrtgqieh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/grwbfwdez.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/grrgzvkgc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gcriaustz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/ggrtdrxuw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gxxytrvyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gguxqipus.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/glwtwylks.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gubavatyi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/guniurxsu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gyysymbgj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/goghpmvdz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvfabqxhi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glrpvsoiv.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gqaphsjmf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gljgjhzzx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/guxsfewyc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdzbvjyno.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtwpknqxy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggaghwhxi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gujzorovj.sHtML


<!-- 参考信息 -->