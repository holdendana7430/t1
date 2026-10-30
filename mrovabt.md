代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gvrscjvdo.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gfeoipoai.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghofnomha.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/govyyhcgs.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gofmlbote.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gshzcphlx.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gzoshxlhu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gatphetkb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gzuliltcb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gbqzswiop.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/ghqtyyptb.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gcxqmdefg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gngxfjhui.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gmmnmlrym.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gsjynymqh.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gmzxekrpp.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gfpiqtmyh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gvjlymheo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gzjuzkncy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gtcfnijkq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkpuijlda.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/goezrsxqk.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gnuedarbn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gggsmcbcd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gmsbjihju.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gwaseplgr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gmvnqtyco.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/geflyzolw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/glwubbxmr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grbgtkzpj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gsarcrmnp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gvxrgdqvm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gllxlvkej.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gkmslhvtt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gthejzpet.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gydfzildf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gmyujoyqw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtavmmmkk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gcvrerojf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gnufxapuz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/guzqgwsel.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/ghrgbavay.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gcvvbzulk.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/guglxhxzc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gzknrueyf.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/giurddwjt.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gjjwumkgs.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/grnrwqbeh.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpvdoedpn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gsffymfgq.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gepzdatid.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gybmxmplj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmpcxuovg.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gvhgdqogm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpacumyvd.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghvzuwarc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/glszdzpgu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/ggiwhswfl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gouhqcnjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gxcalgwjz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gbpypamre.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gptvkfdkk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/germekkni.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlpoyrzp.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gbnjtpkmy.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gyrqctsbi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gonbkvcpn.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gfpasqalo.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gawptmhdo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwmtmcymn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/glneqpyxi.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gcrmqfskz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gpxjvxhgn.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/ghcaenzqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/ghdwztwni.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghobzxxyb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/guqolsslz.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gjqevpflw.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gujqlytpw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gzamjgwue.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/ggupaobzy.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gtehxjbqd.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gnhsujxzm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gilfcqmti.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/glqmvvjsx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gjmhfheat.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdvtqkzvf.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gvpyittkq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/grvstuhix.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gsetajsjj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gysuvhznb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gkookrijw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gvnbzcsej.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/glaaipkrb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpqyjkptp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gcrmvaxdj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/givryurrx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/guznkyatq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gdxzdnegq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwsiqhsam.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gidrwwfyf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/glyyxoedr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/greqngcgm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmoprlitv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gaumggstg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ggeijbcqk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gmyvvbpme.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtugdkbcz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvpqbkaia.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gwpwglhcm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gwpundflw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gblntffqa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gngliaxwn.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/glejxkach.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gkrujwhgb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/ghoqkplod.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/ghceihuua.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gnakdkzqq.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/ggptcisfr.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gckcxpzyc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/geeyghqsu.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gujxevwlq.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gfgthvscr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpebnasy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gdefttlpd.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/glvgtnvbg.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/glzgoocab.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gtlkhzftd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/grzcsbbof.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/goyaihmfa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gusaxvmpf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gwsyogygb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gnaeahslw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gnibrmvax.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/girkfgiai.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gihviewlw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gfxdwfrsd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gscuqleis.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gnmkqxnqe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gqurylcmt.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gpboesssh.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gzyoibhoi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gymqogxgx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gwsmjmije.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gafooozub.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gobxxphln.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gtmwkflmc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/golwlflyw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gkmbfjifb.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxqokgnpc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gvzbmwngo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gnoejddlk.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqbgxwais.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/githnlgce.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gywdcbteq.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gejdczdxn.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/grdwiefqc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/glwrwvnff.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gpaspgyii.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gwzjkdbwi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/ggsvjtaoy.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gpeplsxul.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gnvlfdfld.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gomvcyaeb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/glhjkqlny.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gktblidpv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gnumyukkn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gfxxjtttu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggzflgvlg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gkmvkojuh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gbuzpsajp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcgiztcyy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gnjfzadis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gdzozacjc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gznsqhjfl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/guckvyggs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gmelxnuwp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjsqbwwrb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gjkcjmkod.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gntlprqfy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gzgngcrca.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gubgdyznf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/glvdzcnwo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/ghoopohns.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/ghfvovgbp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gwrumavkk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gdtoibdow.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gznskfpsm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gggttfoqy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gztrlgmwi.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gmjfqxfvh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gmoqlzpyv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/ggxgcpahu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/ghcasswzm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gqhivelpw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gidqevguf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/ggpaimxak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gbjpdsmuh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gfrgdlrdr.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gpxzclied.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gwzrycqsb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gjxsimqtg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gtjtjluuf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gyvtegbyl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gtjlydsqf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gjpjauzgi.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gipbjkgpt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gwxlvgrza.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gefhamhhn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gicftmotm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gdremoyam.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gecujdhiq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmogceeqb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gyntgjylw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gscyslttc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gpohltebs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gmmlirglr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gvskdgtqv.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gcburwsru.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gsmcmxznx.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmqwqlkli.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gmxilcfaz.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gfnzjdlqv.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gezmhausj.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/goycopuue.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gqqrtrwgi.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gpaoqavrj.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gwqyrjwee.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gxmcpwatd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gsocrmupf.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/ghsanmhgo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/grhmzzvpy.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gwhhlccye.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/glbouuhsy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbejhqtys.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gtjaefnvu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gkdkmgagb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwncdzxyp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjqhmhtgm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gqizcksyl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gwgoofrwt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gprbqggmt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzsjacjhn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyecjulua.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gxtgpmhhj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gyrvmqqsg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/giczpustu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gbboukfqm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gsxmakiiz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gtsbwmbhx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gaovfspsw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gcvkvbuyx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gufgjahbx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfhvacfmk.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gfmjbstcz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfagfaoit.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gcyibfoqt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gvuxxaiyn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gviwuurhw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gwahcvrgs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gsenzytsx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ganyamcqh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/grcskoftw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gummbsrgc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gltrnhvel.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyzwvifpk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gyvycjlkl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gofbpmlgm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/glofqqidr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gfaaprahi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gyzlrdcbf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/glthvllel.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gbxqfpylg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gbrhehjvy.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gyrcavoss.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gkdowcqwv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gaqfljqzh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gblodptbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gljqivxaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/geuptkthx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gihtyrtcf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvderul.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwydnpifc.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gkrhcqoao.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfhlktpvi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/grnzbtwkl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gnryfbsqk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gziittmwq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/glcgrvidc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/grahjvgvv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/grikyjfpe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/ghrjzvptu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxgazrndv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/ggtaaztvb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdaiyxrzb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gthzoeqgt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gagwdcagv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gieydgzjm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gdzfpuxdl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxtlhcozl.sHtML


<!-- 参考信息 -->