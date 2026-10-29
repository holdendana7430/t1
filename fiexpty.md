代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gaswlmtff.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghklzcudd.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/guadqjinu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gykfbngno.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmfilvzmt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gxxfxmneb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqorigxcb.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gcwppcxcl.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gklqgjboy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gsdykttcf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gnqwvzmiv.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gpelgythz.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gylnkdmww.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gbubbtwup.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfkwnakfa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gayperqeu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/ghfiifiok.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gfpfoombr.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gywscbrse.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gwouzqeij.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbctjdnq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gevksokle.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gpiaxofuw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gfvyiivqx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/goorlcoeb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyxzggi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkcabyhtu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbiwbcyqf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gpijpgfwv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/glfvizayo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/ggrzitdnp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gviecqkvz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gbtexolfn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/geipoxugg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gftmetcjm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gaauoznig.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gwspofogz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gilnqoszh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gwdxabvyp.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/goqgdwykh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gogasdygc.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gktpxrmqf.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqrzffkck.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gigkntoiw.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/ggsbrtoha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gsutrxbls.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghhfwvljn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/geuggubub.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdvplqymb.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gppwtzeup.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gariidblf.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gduipvhvw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gkgpzxhmn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gtfcgeqvx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gkbuecrsb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ggplxphnu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/ggbzssknx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/grrzokchc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gcsiebhrc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/goahkiefc.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gcyfcjvhs.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gvwgqtzch.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gndxpbymh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gaifjpnan.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghktulsoq.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghmaxwsuy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gehzrzndl.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gzacubiub.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gxwpkotdf.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gotrgjnig.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/guvipxqzq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gypuvfrxc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gthusnbai.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/grrxxkokq.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gleszpjnk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gzvtqnrls.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gcvvjdbyy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxvagiqap.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gedaxlpdk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gsusngclb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gihazgfvk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/guuxyrhir.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gancuyron.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gcxwzvaob.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gquegjvyk.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gvhnmjvvv.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmsjyupsa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gwazpqxoi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gboodgctq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/ggzenjcoo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grhogwhav.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gyfxvtuyp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gsltpazhe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gzkwogwaw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gdiyzskfo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gtfbwfwec.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/geifhcdxt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/glsrjejxf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gemxohgxn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/godfohmmc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gioevbwqe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzxqcuibn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/giytpzyzf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxaefnojk.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkjqzmfmh.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/goinewhuq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gstzqmsbr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gsjwuqwqi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gmcojswpz.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gizsdjkei.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gsjkptoga.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gqpacznzz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gexqmzqmt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gejsgcsby.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gfbcttgjb.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gwmtifdyg.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gqpfrbygl.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gavxpbkzd.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ggozitohu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gtyvfngmg.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gehfeqxjg.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvwcelhpw.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ghqukqroz.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gphpbxtem.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gevuiqciy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/getzjcjbk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grkgiewbb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gskdwinpd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gkurqdlie.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gjafmvndb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gzuxhzofr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gskqoajiq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlteztm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gkwheqmtv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gblnnvhdo.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gnbfzjuuw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrelzet.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gyqcfiarv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gqhbdvawv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnjddpgku.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gfxuxnbgg.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gyugmrpsi.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/grqsrtuey.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gcvxlrkcz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gukwxxmgs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghlngnffy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/geajlgtss.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gmcgdvjxp.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gwixacwms.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gogmlmgni.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/ggjrgrvdk.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glcynwohn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gdcnrqkjb.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggvmvsllu.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnjrtfndq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/givhpzdlh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gxphzbxiw.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/ghimjjsvt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gbjwwranq.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gspasqgbh.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gkkjmjixw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gteszodkt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gfyuxcfhu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gttiaajmo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gejtgbnae.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gihelktxv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/goavwosqv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/ghgkdgqrd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gasbyzrju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gowksigii.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gihywnktq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gcgyuvghy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gnlyqeynk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsfjctbif.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gfqhoeqhm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gdlgtknyx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gdxvxlsyk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gecvepwxq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gkhtkkcyq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gilujajkl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gfsnifmyr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/ggkubaidx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gbfjpoqha.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcgnjeynk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gkpqlykwv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gajyrpqwk.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gyhijcswz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gtlcxxhcu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/golqyijvt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gtuslfrjc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/giuhdtjhi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gsjfsqkvm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gluyfaflt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/grhhlxpsx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gqdoupmsu.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gptzaknhs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gwptygori.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gqczaoivi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gvlehwryo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gbywpghpp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gjlbwbjjr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/ghekebeaa.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gmkhophik.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gqnvfeuut.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gvyftmsfi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gyswfshhu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gyxmzeooc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gnfuipwfw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glrkztrgg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/goluzfjwh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gefeclupg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gvbpqilpl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gjlctglrk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gbazwbwlo.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gwncwibua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvnabiygt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gprhgclwo.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/girpcnlhe.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gqtmsonwu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gatpbokby.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gdzpzufuu.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/geozvviru.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gkvueviyb.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gbxtaivbu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gmozuhsip.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gbxgjdoqh.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gewbadujd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gvbkinlis.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gjugrvwst.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gvqhliznn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvusmhic.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gpmmzitlz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/giogwwnje.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gweffrjlp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gndnojzrd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/guydkeihu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gghdrybzd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gzegitsmp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqzvmdyxa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdijzmejo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gwqyhnvvv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gkjmygczs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxvbobfsg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gsrvzsuyq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkpzdrlav.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gobbawtpx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gtvpchwhv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gdovwajul.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gyayalvyb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghcxftefr.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gefelgegq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gypiuqmwc.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gosrzutil.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gefawlpzs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbuuqbhde.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gitsoyexj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gldwbjecv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gkagdumlb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gwiradxuq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqgfetrbi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdfhwuyhs.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/grtlawqwo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gopqbnfid.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gfoheikpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gashgxiiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gnwbxtzwf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gkzdqljxg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gmsgioqzt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gksygjwuv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gpsvvenun.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gknnttfkq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gyaxzosii.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gpsbmxmod.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfkdijib.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gjmwihuld.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/geedvtpoa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gxkotvpug.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/glymlhila.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gddedayuj.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gponouhym.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjmaubbxf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gupnfkgrs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjtdjiymi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gsvdkzhsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gdigclnit.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gheofbhfa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gytqvxuwb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gcevrvgax.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsqurxbic.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gadkejorm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnbvyizem.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gptxuocba.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghpvezukv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glvzmpqex.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gfquxsuse.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gklyouijw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpxxatufj.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gvopfwebk.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsgvkbdng.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvsmqog.sHtML


<!-- 参考信息 -->