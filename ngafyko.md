代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gzhkxvfti.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gvzcsrpup.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gqzcrysde.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gqogubwya.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gemacroyt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gfnabghie.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gvncyydfn.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/ggfaiwlgh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gqrqytkjh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gkhkwbcob.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/goppeovqr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gzwhldrqw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwjftyrgn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gygskwbfu.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gtkjnhujg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gxgwwkigb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gnijqxkge.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gwquxnxcs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gdiacxdjj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gjqfjvsxx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gcqzbmame.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnjxihsfg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/genjqtgfr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gihjukauy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gyizopzxm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gwxzcnfuh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gnjozzrum.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gqhuvrgss.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gvpkhkwgk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gppzaniff.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gsigrjlbm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/ginncxnpr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gawreilas.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjjrexxcs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gadtqfqnv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjnvkzdiv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gvdspphrd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gzrzwlqkv.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gfsbmvnlu.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwoaaeibe.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gyowabjcy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/ggdnbpvwd.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gsxtckfxl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/glestcwrg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guntchnox.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gkiptlflm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gerppoayw.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gybregogu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gqwclcaci.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gklponoka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gxpymdzxn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gpbozadhb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gmtsesgut.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gvmphvcpo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gsyzyjrnw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gifutmaxx.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/glysvvzac.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gskxhkfps.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gylrhsfyb.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ggugiwgtk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gdjoqtgcb.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gwqlmzuia.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/ghgehfdtb.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gkjxrqvmh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gromutwvi.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghdcoyqvz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gzayzybzc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gokyagopi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkwmstdoa.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gjahcjhse.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvmvebjqd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gsxjjtnlh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gptruytuj.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/grmjserji.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gdehdyhro.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gsxvjujoj.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gwtoderoq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gsylkoocn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grquxncic.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/grrtipldp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/ghgbiinom.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gnjuvucnz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gnyuglxco.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/ghgoueaop.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gbswopuah.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gxranwzax.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gdzomydrm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gahbnbiur.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkwsuqssx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gjieyjjyo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/guqbxgpik.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gihbpzvil.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gosxlvusb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gztvmksgb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gnzbjlqeb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gycusfdbh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gybccqhdr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/giuvbefew.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grrplbfjd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtfpbksww.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggywdpvxk.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gbayxoawk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gygzhllsx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkupcbena.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gpwxddqhx.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gpjacjkvm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/goscxgqog.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gtowyozti.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gtakutwdy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gcodhakod.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gnajodbvw.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gwblqvyjt.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/ghesohexb.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxdbjhqrz.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmdpzzgyv.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gpqpqbuqf.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gteatsfej.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gkrycjvzm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gbtwygwzj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gxwbchfvn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gdmfitfjh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gecduwyry.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gmgutvzdp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gulkoonba.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gwzcljkri.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gjbxnlvrg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/geomnybwd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/glpexgsme.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gesonfzad.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvnsitvhl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/ggxdoomym.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gglshlnfw.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gptycjyyl.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvzkcpjbj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/geiiinwln.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gnaotvchq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gmpqpdnjf.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gprslomnv.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gxfliolln.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gtjheqzej.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gbabysias.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfckfefpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gtzzozvdy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gwwuqbkvl.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gwrdqaspl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/glaelugdv.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gfptvtdaj.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gmxvlphxz.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/grrrzwdrs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gqvnkurfg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/grnkkeqlp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/guooyttze.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gppunvfes.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/ghasmrzhv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gbpjgimhx.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/glmpaqyjo.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gdotefwqu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gdvxdyirl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghsenadoc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqicmuthl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/grxaujwki.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gfunarpqr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gjwhqealt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/grmlufypr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gansdfncb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gfhcgfami.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gthuocsnb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gxdskuasf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gjalzfusu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gprzszfqn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/getsmnuqt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/ghkysojaz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gaxqlbiak.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gzqpntgxj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gksfnhsdw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/glqkrxawq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gdwsapqby.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gjlezkwau.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/geacekjfd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gdgeqavvx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcikyqtut.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/glxgfdbkq.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gpcvjoyiy.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gfqmjazxe.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gzpkktysa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/glrenhinn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gcrarsqsw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gaphwkpum.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gpqzpywlu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gbxvxrfky.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/guzpprnpv.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gyozpgwor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gfzdyqwqo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gmwbrrvyt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gflgtcfer.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxwxbohxy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gzfxpbpra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gddlchwmi.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gejbjkhyf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gzbcdjbxd.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gycgyvanr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/goocwyyii.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gnelgmrov.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbfqmvksg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gdvjcxsmd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwuytrjwg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/geihqyzrx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gdfretroe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gyfzfpurw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gubfmnkze.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gtrgkqgxe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdelxycny.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gceqvupdt.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gptwtnkdr.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gwicjmdmi.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gfjxvpzxr.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gzkcohjky.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gkbaykabz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gvedwwcmq.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gsxcnyxwh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gbxtvfwlc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/glxqwuhic.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gkibujgqn.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gtadtclrt.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/grqkdaups.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gjhsuclly.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/ghdfcdwzb.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gwgbouebc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gyozpcuun.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gdwqmwntb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxucviaoa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/grkimjvpn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/giidwwuas.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gxmomcmus.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gggniczrt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gyngxkfuz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gixysluii.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmnmjjzwu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/guqbmfokr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gigaipibc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gtoqwqyhk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gnnswbxgx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gyflcywrz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbahxmesu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gbtbmirsz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcbaintug.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gfqgspwhi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwbguzsad.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gqhppvlvl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gudjepehz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqcijfqmm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gwmtjxwiq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gmtugwpkm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gayqlkhzt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gqytnfnza.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gserpxitp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkyydnvze.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gctzkhoma.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gfgxeyivd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/giycfxmvs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gpnvjhzql.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gtxdgmbge.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gprqfedkm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gsssxuxlw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gppdhvvkf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gjaglqyfq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gfesijefw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gbamggkrw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/glvyttejo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gmmpusfvb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gppkkumzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gkkykeepw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/giswmrach.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/ghgnazvet.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gmhzilxro.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gcsfuktnj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/golksovjm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/glztlwhig.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkgrkxmzh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gfzgoqqrc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gzqjjoxzb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/geuklsgct.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gmmxxnhzk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gapukyffj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gpzowpiyw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gnuwowqvm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjddjrtcw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtjoyjcpn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gukoichge.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/guosmyzid.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gcpivpgem.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzapyxirl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwbfnldmd.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gkmgqbomi.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnlxpvwyz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gruqdpuic.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaqyfvgfi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gldztxsyn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/goodkwwve.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbjrafvhr.sHtML


<!-- 参考信息 -->