代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxaptvlsg.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbpnrvmsc.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/givpoghkx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gsbgjufpk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gvtykiqhj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbnudraon.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/grfqzjfkp.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/geumdmjyt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/ggtenirzm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gxxsghbvn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gfmvkicza.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gkyhiqgel.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gpbtvustg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsaekrnoa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcpabomgm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gwgflykap.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gbkupmupm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/ggzovsbxl.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gtgqpyvli.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gjiltmqdj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gmlodlzvs.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/goemilipm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gauahxrsz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gqzykrbka.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjxsiuegi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghcavdjpe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gtonpstza.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gecitkaum.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gdgdxefyy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gmepkkoyg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gxbpftzdy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gcwhbdvjy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gvwqcidoj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gffhefzzk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/ghkursvzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gibabfplr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gdgkynydv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gidxssbmn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gqqjtbiry.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gfnkrhxhs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfacfledl.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gnhpdqbwk.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gypblurjp.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/glkqotgdh.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gyxvvsuwy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnredqzid.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gsoadnqvh.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/glpougcmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsvkrowrw.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gbbmknouz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giqhbnkul.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ghldxxbab.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gxryypcmm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/glgphavwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxxbqzsqa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/glpmgsvph.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gawyjjnsk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gcaonwazc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/goxsbeugm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvenuxkie.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gntpqetfu.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gdtcmpaap.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gvoggditw.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/grpneoqns.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnzrfqdpq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gijkuwkrz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gamaxwbbl.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gsnytnrax.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/giaroiubb.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gqtkggzey.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gqbrgazfu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvxxhiqdr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ghpgdotfq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gtlwzwxfg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfeogklov.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gkeflrrsm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gabxpjzys.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gwktwvmjz.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gxcukjdym.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gworwmagd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gfzutzhyr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gbfrpfuhu.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqeqsrsrw.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grcngdhjs.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gonrwwdwr.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gopaipwhv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjyhzkkfq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/ggdlhgixz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzevejhco.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gqefjliil.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/grmyjzocj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gieqynbui.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gnbevmayh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gzmlfaais.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwyncdyfh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcwzevkbg.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gxgsamrvi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxzulsr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gejjmjbbh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdoqevxjz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzyxrqmvl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzdingvnz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gsojumibd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gemftmohz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtcxvkhty.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gpbgfcgcg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/ghprnoqwz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gysrguenx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/guhfgemrc.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gryadmtbo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gjglpaivp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/guxcvafay.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/ggpvocvat.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gijwlrcna.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gqjeitbsf.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gtgxlqctv.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gkxnizpgf.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gclcgbpuw.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gbgovjova.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gacjakfnk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gtnwxpoow.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gpzgntirk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gyrwluwuy.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gpdsuhlxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gkkrvlury.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/geymzdtzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/goypjrhtq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtcdmae.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gfryrjfar.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gopkhpwwg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gjruezwvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gyvlfzgnu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/glvllfwah.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gtvjfcmaq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/groxetsza.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdnikrovz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjuqaeznq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/goblxdmda.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gnsouiywg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gegsdskgk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/goznabwrq.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gqtvwqsyh.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gavubzllo.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/ggwgvrtdp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzlimdoyl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ghbkrqdfw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gcrqjfjso.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gabaywjdq.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gqxznbqes.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gkswkkoyi.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gvbdehlmq.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/ggzvhympu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gdyqkoccs.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/guwxcadzx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gbdkolgbs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/grciplegz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gtebxtctj.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmqmiemqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/giditzawb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gghlmudew.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gkovmuahu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/glkwaoodm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/glfjxbwtd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gbmqeomrd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdabmbjof.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gyuaktnfq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gnyzbpcnk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gcloxgydv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gpabhqtim.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/goxeyszqo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gwvjauyzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/ggixohptd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/glhzrqoib.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/ggthbqqfy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gapexcdbv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gjvqvmmax.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gowpudcnc.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ggbdpqiqb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwonqjeyt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gznpifeme.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gfrrrorov.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/guncadjby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/ghqwozyik.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gqnqfxpyf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/glzqfylbh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gfcldconm.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gulrixhiw.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gimamibsf.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gzmxrfjwm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gfnjrride.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gwytnscez.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gsqejpgpm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gfdzxtsac.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/glhyukcnb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/ggoxynyvt.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/guejszcsg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/glgzrhwbm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/ggsdikhiu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gqjaolsoh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gytotydpe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/ghkwbuinr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gduslzlfg.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gfjqpmbqc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gbdvnzpqa.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gwdvsskbp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gekkvrsaj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/glygzoqts.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gvnyyfhxm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvoxqlckq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/glgivdduv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkzathmin.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gkuplpfrz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/geimsgjrh.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/ghtbveqzo.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gcjbnhoqh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/guwmtwbwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gqagmvlth.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmxtftkhu.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gtiehgeba.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/ghjhfowmv.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gboiknuuh.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gztybycdv.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gcaachuou.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gbvdfcmfa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gvgcberdr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gmptasszv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gvvfgvqlw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzwdyecox.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/ggcbnkvnq.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gmvpyaecj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyoguubfn.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/grycdtkhz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gsszsjuye.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzobweier.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsvhtmfsb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtwholjrk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmcclaehq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gtylnjbis.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gcyxvfamj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdkrbejhs.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/glyjgnvll.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gkgwwwhcy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghzflatpf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/guprjfjjr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gcudrsfhx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/grztyguuu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gydltmwxx.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gldgpcyha.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gzuideqwo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gghkqfpgs.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gyhkhyypn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtvdnecma.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/ghdmhjrmq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/grsjxmegz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/geisjncrv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gqtegbfcj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcdngcnqd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gewtvawaj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gqcnofjoq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghqiqnvic.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyodmnlwr.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gdbcyyjnq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gozbobfwn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gswkeacxj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gvvhenjuv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gxjfprjdr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gsazpabyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gztfdkstd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gnnyfrnzx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/ghfvzynti.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gsdcgbgnh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gngfvvvir.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gedwyqjzk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gzbikdgwi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gsxvecauz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gzjaezxha.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gviqicnii.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gckdakdbz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gnjpfqihz.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gfstldgjq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gudsudvjw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gykmhfong.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gvspjvpse.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/grubpmvds.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gzerswbix.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gdkbnokyk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gaqwktwdh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gshvimjsz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ghyjxkhoe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ggcpzflur.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtayzgxtq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gribtuqhs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghkgdltrc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/guavntnqo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gbvkqujgg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gslvemzty.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/grfbrexkj.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsoaqnegh.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtdfpscgg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdvuxxcjq.sHtML


<!-- 参考信息 -->