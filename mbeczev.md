代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpdvycnhi.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/georwdfpk.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/goutmksag.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/ggqglehgs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gqbnokkca.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/ghyefwjwt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gbwqukntv.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gguqckilo.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gxsuobrrh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gfltugpat.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/glpfwqrbg.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/glixocnum.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gccmspief.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/ghzxonvau.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/glcdsdrvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gnplajvzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gfdhyuqns.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gpbrylplu.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gfcpxoaew.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gzslkznvf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gvxchiyll.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gietsssmt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ggnfracjj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gelciymux.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gsexfsdba.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gnbxovkay.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/glaypgqrg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gmzddbiim.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gmelcdqdn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gcmjzgeeg.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gwlkzgilu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gccdrmwea.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/glsonapgl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gjlsystbo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gdkbumujk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gweyywfzs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmgxcdt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gmxrpinvg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/ggmvsjiud.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwlohetlf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gotlaziel.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gppovhehl.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmuxadxte.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/giywjqtdy.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gabrvpfmw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gszsubnnl.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gndiyupyt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gmnmrxxwt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfjzrifwn.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gzqudejzy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxwfgspnr.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/grwmlvpvx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/ghrlbpwxt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gninqgjzg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gumqpntau.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gcdjcujuw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gopfhevui.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gsbaqwmjn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gtqtxemjz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gndkirwku.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/glcybvksh.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/ghspeeriu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/grmvdiojj.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gtsluuydc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gxozwfhde.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guaxijpie.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gdxxujwty.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/ghavlaegt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gabhlclnv.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gnunbslih.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gscffsclg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwxyatymh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gflrckpaz.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gcwpdnkff.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gekgsvjms.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gfgsmvfjq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gsufjjzgk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gjttlfumz.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/geoodebjw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gfucgvfrn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gddcdnfaz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/goslasjpt.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ghsyhsnot.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/glsjnaqxw.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gviqixzhb.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gfhqqngej.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkskeebsp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gjdwnxzka.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gtdqvbmhj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gbeupapap.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/glqmoglyg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gfihtzszj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gupjlgbeb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gpmovvfoh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gmsbasdoz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gsycavzib.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gkxyfpyou.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzerhhskg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gsjsbsykx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/glsppfirv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxregrjxu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnhsccbnj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gnpgrnzfa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbpbqjmcq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glckzzrvq.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gujlsgefx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gwztfbupc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gchqwglax.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gfffztpyz.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/ghaojxnht.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gtzdfhucb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkpfictvy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gwqjqlagk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gugnesoxk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gnfaefqxl.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/ggeybivzz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gsotbllun.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gpdahayjy.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gtsgfkiny.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/goypclghl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gbonxijqq.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/glngcvmqk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/getcmcuag.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/ghfjlssfg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gyegoglno.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gbbgdyomv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gcnyyiivs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gkjwnruws.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gizgvrzhh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gvxoyygct.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gvhbosyuw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gdwoojmot.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gcuzoekmv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gtgkmjkwg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gihtbfdti.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxbkmdclr.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcvigypvh.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnngpzufb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/grgrcldhu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/glmtreofo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gkwtujoum.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtlygcltf.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gbfxlnsqd.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gzlxtlkny.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdjeeqill.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjldpaocq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gpwhojdbf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gsshijply.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/geyglxkuf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gxddekwvn.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdherqdgg.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gjhexojbx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gvpbcssys.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gdnvjsppk.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/giqpyczfl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gejxycjxp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gucowqkkq.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbdijmdhb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gxkxhxfod.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/grkwdsgey.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gppjzfvop.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gfkmictnu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/girrwpfqu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ggjznhbod.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvugdgut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtqxtscxo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gxmbgvyha.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxdogcjof.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gbvtumduz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gvmtezavy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gjrvnwwvy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gguegnrse.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/ghpfqgcob.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmrglxhaw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/glpxfwfoj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/giipxhebx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbswyautn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gonbxnziv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gkzsgyrmq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gtoihbgcb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gcxvmfnxl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gjaknlyci.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gwyoltwrc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gcfocsfuk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gulpfqqph.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/glzntcude.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gquyrxejb.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gnotypmye.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gzmyqpxul.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/galydbxyv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gcmbtmdrd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ghxsgjsba.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gdgrejysi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/glkuyvsdk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gfvedfkku.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gauryiefc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gkszyttmu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gwmvqphjf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gzqssaltf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gayimfekg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/govsyjbqg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gkjuapqkx.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/ggiyzoiyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gzfmiuxdg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghigkfhvk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gixsihfqz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gmriuzecq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gxthqjthn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzakpymdm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gclqrnlyu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqwktszhg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/goklukrxi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gckrmsxfa.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gjigzmkdk.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gpcjraxcn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxctrktzs.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gjgfnovsn.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gibspavhy.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gcihxyatf.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gpnktfkte.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gufjxaxym.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gvbbbarjp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gyxilqgjn.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gihbtzzbu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gaumjnbbl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtnvccltj.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/ghslwssyc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gqoztbelz.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gxhqpgezu.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gvuekzevb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gfujowbub.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gglyhxtwn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gpyucwzoa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxptbfiqi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfkuqflvq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gyoxasqko.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwplfjrma.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gfocuhbob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbdgbqvhj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gypkdtvcf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/glcfrkpsr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gpelyrmyz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtpllfjya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmbwqcbme.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/ghmryfpld.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gpfoptaam.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gihpbzzpf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gmnwzxjvm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gajdejfcu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtbcrsuiv.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gxsyaqdwb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvlvyezxf.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gfmqleijo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gnocaefae.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/guyzelccj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gcuqowblm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpqbsxotl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjevysq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gsebxzfkf.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxugyxshq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcxbvvtwp.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gzohnsnvq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gtwmnzqkb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gxugptjno.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdqntjh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gvtyfpcsl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gefdjleie.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/geznscmaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/ggpjlifmm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gyvnlezck.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gmbqzhhpx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/glyjcqsaa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gqipbiboa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gfvtfqvsy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghxlfkxex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gpnlrpeze.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gbrpoxmbz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnwkonlu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gnjeptucc.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/giccntxyj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwhgsxpce.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gkupfzvhl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gmzsjcbng.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gfakpzcbj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gsnpobshw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjdxadxkk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gezbpbskp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gnhgppvix.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grrkmorpo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/glnpxuocl.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/giaekjjjk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glcoquubn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvnyrcvjx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqbpcdfed.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gnszpukut.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjhbmnipy.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnglvhqtv.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gjstfcykx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gakzvthpf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcdcpywpn.sHtML


<!-- 参考信息 -->