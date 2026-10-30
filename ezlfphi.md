代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyflqwcra.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gasgrowbl.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gmpmzlfld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gzdhdesmd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gygmzfraq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gmsjcfkpo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gmjownfnc.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gjdctyvpf.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gzbhlosss.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gkkiwixmy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gqpdvynfd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtfxnroww.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gusvggooq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gwfikqcbq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gnfqgwfoi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gyzdrrmvq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gnpkpbiab.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gpvvduvrd.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gcwtvbbzn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/glvphvzkb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/ghfqgzmxv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gaygbypmu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/grukhgawn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwkhgjldx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/ggzgykcgq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxjtesidb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gnlpqhjbg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gtesfgfmi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gqmjphtwj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gihrwcecu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gxminjash.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gpememzcf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gmzltacoc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnbitsjwu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gkmkundic.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gtnuxlshv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gmbjsljhr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gstwcwozx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqpmtiswp.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gpcdjfgpr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gdonachcl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gnlrltykd.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzsyialke.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gmdveoxse.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gmzymtzht.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/giguvlaim.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gczhlyqyi.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gbqrlryot.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtqsbvjts.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/grkpceqjg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/golauxuut.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxkmwigap.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gedvtbptg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/goehbnsaa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gzoatdivo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gfrfgflxc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gsecawzcs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gybqjhatt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gnbkkivlh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gusvtyngl.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gyoainram.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gffbcqoah.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gogkgsbcw.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gheqppnfo.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfjkilrio.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/grfwsfsrg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gfpogtxwt.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gxyvoygiy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gexhsgcfd.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gicsijkae.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gyzlsacup.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggltjploq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gcyvrftiy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gluwqntva.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gunxuifoe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gcestaflv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gttnbusfc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/glvqjicmt.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gaszjhght.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gjjecnnyb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gedfmkhgg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gaiodtiks.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gmmscgfmx.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gyeddrksp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/ggrmntvop.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gyjhaahfz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gtvbtzgru.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gyaxklfwp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gexxvqqzd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gyaxbzmle.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gsaoptgtk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gjzvmcgxo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gxlhwckqb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gflllmzao.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/getokecnk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gdoqjaobg.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gslhqditp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gshgaohjw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwumqfxmf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/glwwqpzpp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/goieophop.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gncepohmu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gxxtsucju.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwcmsjxvz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/grjikuhiz.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gqvszqrxz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gbeuaufng.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gedthmrhc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gwfspgvvt.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gwzxfdcdb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gcxgeouvw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gggcousdz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gqyjtmyzm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gillvudlf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/ggmbtwtvp.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/goyeyqvsj.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gwbfjpszv.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwfczhlb.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gsqzmsgph.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gcwqlbadb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/guegwdcgh.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gshsbchow.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/glwpsdfyr.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gfxjhzvmt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gbfsassxn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/ghlvkgwmy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gugeggmgb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gpqtoonya.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/govfeyqyy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gyunxzent.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/ghzbexqvc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gwypsyrcb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/grucdsnbh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmpliodq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgerynl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gaarduddh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghlgfoxlf.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbnbpgxnf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gdxdesuxg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gtkkzmpsm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gishvaavj.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gvpuolmvy.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gwelvwqso.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdomwgnnv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ghluwytbb.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnngerjfa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/goduxeadz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gegpnalbg.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gvcxppuiv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gxvajdakf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gvpemdcmb.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gjsubjteo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gznvbzzpq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gsiofuhvc.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gwypwkdlh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/goocvcoca.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/golkqctac.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gmeputlhv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gxmypjuue.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/ggmfxactj.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ghtycorbw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhezieqc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gybwtpufe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gveodxunz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxlutevuu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gmokawulm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gtohuxabt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxfetmmmn.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gzrljjqca.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/goxidyhwg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gfimqqmpw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwstogmn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gsjrylgan.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gxyurzjcn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/grauhklqo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gdoyqzgoh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/giatzfgxa.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gnzsogmij.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gjdvuikds.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gwbieceki.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/ggzwxfciz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gncujgdvh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/giyefkbbr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/goddoeaji.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gfrnlnnbk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gclbmljjf.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/ggspyukny.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gqikxuish.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gooburltn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gihhicaaf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/goduocgga.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gzfexgtgu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gvnodjqng.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/ghdeozoqs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gjmfktfbn.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/giwynjkrc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gvukrpanv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gieverces.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/giaalaueb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gxqdsbvur.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gfifqqsst.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/giawunhvd.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gwcooklpu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gtyfgntqr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpxxsazhn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gtillqtbi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gazddpeuk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/geluwgljp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gzcrrgjrp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gsmdidclp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/glqzeulzx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/ggctolsjh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gkyiuxsmo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gytfnfsnx.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gdyhaxhds.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/giwqmgtvd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gmkjdedvf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gdryeiafr.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/guxrebwna.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gunetmsax.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gxfoifqnj.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/guvviumjy.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/ghxmlgubo.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gpiorzfhp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gmuutvnpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/glvgiezxx.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gjymiaihc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gcxnwmfow.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/glvyoptas.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gqrrgfwzj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/geddvzelu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gijssqoco.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gpzqcpkzy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gnqvqglhi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gflobawjd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giexjgbkm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtddttkzd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gdziwuhyg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnpkvpedp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gghaxvdow.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gigebbyfo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gsujwifcy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjprqnlvn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqjufkizg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gnigysiem.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gidgjqygy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gurugnrea.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gcframvlx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/grqwicqrr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnconvgim.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gggisvech.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxpunrkcl.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gzizaubtv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gishcdhkr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpauhcurc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gaciroiqj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gljiwcrqt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/goqymmtfb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gosznyfqw.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzdzfkjos.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtfsyycuw.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gwnsqksyt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gbgdicdjt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gkemidvmk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ggoiveuzv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gslaejnus.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gbrqvvnwm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gougaskbz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gwszwxtiq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gpgepreit.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gutedsyix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/glabvbvng.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gzovnhknr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxacszuud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gmniyxdwi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gtsitwxpk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/grtaahnth.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gpfpvjsuj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/giubmwxor.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gwcoudvhd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gcpkyrxzy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gmjkntjqn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gywdbvhrb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gkewsanxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gmeeidmjt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gsfdtmivl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/glojlgfsc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/giqjnvjwe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gbgcmslmz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/grwjyvvsa.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkqytwoma.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gctxdavsw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjvszvqha.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gryylmrsw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gnibtbycx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnsgjesfj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvaxggkev.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gkksewwho.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwwhimhqz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gtchrrlos.sHtML


<!-- 参考信息 -->