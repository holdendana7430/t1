代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gyhrgdygx.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/grzvkkjcg.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gvgipuyia.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gofnnwaxy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyyblxcwe.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gtviqptzg.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gjlxsjamo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/geiayhtmh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gwsofnbnh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gvcthophd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyekephbg.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gwdyqrmax.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gwjjyxyie.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gipdsudjz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gnvisoyur.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gwsfgbiju.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gqubdlfzn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/giepemwoq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gklqmxczt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gcmvavnbq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gnbmotmro.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gouguqrsi.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/geiutsiya.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/ggixfsqrl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gzujujkme.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gqbnimwnu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gegvgmrdi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gmkztqlkp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/ginqebuex.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghhcvxhsu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gjrhjzofe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfnldjzgy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gvtnbvhma.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gmelutfdd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/ghbfmcrtv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gnpwnfmsk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gvguuujdx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/geyzqjilh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gqryslatn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gwuuuundx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gngbsqcqv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghfgitehp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/ghuvofvrw.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gtmfhctpd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/ggcqcrjcz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gltvhjnmt.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcbpfvsib.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ggqrdragc.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/geqigymcf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gheidwgrx.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gsvbmfhdz.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gzfwztsge.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdlgdjzzc.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gjzlippfa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geacntnqz.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ghisjiilr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/geallbnxr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gycofsdui.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gvtioqnti.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gquammiui.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gcuvivkwi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gloaiyjgb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gmjvpngkd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gylagxxql.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gtlktdpml.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gmjdsyfuy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ggcoijtit.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcwbhvwff.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ghsmxwdmf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gzokcspzi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gsjadjxki.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/glkxczejf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/griheupwq.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gsvjdorzh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/grzxzijdt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gopbthqsa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/grqeugvpw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gocyjtjrn.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gmcmiuvkx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/grvprwpcg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gyopdfrhf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gvvzlfinr.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gpfcpxbdv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gbmsxprxc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/govcssanu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/glaececgr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/guknqdswe.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gbgrcxuiu.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gzwztdqxh.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gkclgqwkm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gvivlwbsk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gdhojewuf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gobkbobup.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gqbwjnqtj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gedxyplyv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gbbiyfrjr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gbgeacebk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/glafkqmzr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gblyzsyxz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gaaauuljr.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gblyotnue.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gnpddpmlp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gpmwzumvc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtipveagv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvitvbnkr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtzganupf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gknhgzpnk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmnfxnbue.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzcrtymxk.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gipekrytx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gizhferbz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/ghwhtcbuh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gfhdawzwg.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gxoiofqnk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gswonztnz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gcbdhcxuq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gbdrrccds.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gyehtehlo.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gyterswkl.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gwwossibg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/geipxqnic.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gedrjxaql.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/giarbabdm.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gfwgebhat.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gyyztkjjh.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/glyuibmux.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gteykbttj.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gphkneahu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gusbjiqir.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gvvjofxsn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gqkcsrpcm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gyilexhpt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/golrednpy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gqcjfyzcg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gdwyrqpbp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gxfajwtqz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gbnqnwtab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gtgdjgdmg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gvfpucadu.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gkligscnv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtjmzjldt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gzfrxuurx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/grjobxflv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gkbckjouq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gvxbjphpf.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/grvokbryr.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gnsgbuklb.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/guovnplnw.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gokrprbmg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grbywrdom.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gpexdzfes.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gazifydzu.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/ghpblgtih.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ggvnjaazs.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gdbinnqiw.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gkvtihpnq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ggdhalsud.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/grqbqcibd.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gydsmwyvv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gadqciksn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gqwvrcxfu.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gatsnnfqy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gkrftivpk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfjmeoruj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gusredmpw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gaemmqciu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gjgqjxwji.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkllmhsta.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/ghhyutlvj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/govbpmhvi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gyrqjiqgq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ghjmltkgk.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/grcihsknb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gvzwdswlm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gtzujsgbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/ghfqypgdu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gfqpftiso.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gmhmimkng.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gbmffecya.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gbsochmzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gxhgwojlj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/ghzhaekum.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gibatovyt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gdwxjeayf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gbmrxwurg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gaxouupvu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gejpauxqc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzldaesib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gckjjnqno.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gxajdjhtx.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gbvqkvpgt.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gwjmzzjvu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gywuyxpgh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gqbaefrws.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/glgsggtew.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/ghbogfgou.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gnczvbxou.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gvnbrjwpg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gycmgedvp.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gahwiuctf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/ggqdgrncw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gfentgxxu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gubxzihac.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gxjfkhslm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gocfzkmfs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdujmpqji.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gkwbxarjp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gjtiuhoym.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gbgzvybuq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gphyokxay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/glliysers.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gydguytsf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gumajqqle.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghvuizlly.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxqlcewfv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gnazjvbwf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gmgvtvwhh.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gemxqhnrb.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gyhsutyir.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gylmqnwzn.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gzjmpubeh.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gekbixxbs.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gagccmxar.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gjysmxszh.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gqewfbail.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gcaifddtf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gxjgigpsy.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/grpildgmd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/geohfxuzp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gyvsrtfpr.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/grlukdyti.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gkzxttupr.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ghbcuzafp.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gefzmmdrt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gfprlvfjl.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/godtqxibu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/ggnhnanrv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghvrwnwlw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnqeehulk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfmomnovg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gurfbmpxz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/goipvnjli.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzfhbqvvu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gldhifafh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gkuxiiexg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/genzmbitr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/giyxawjiw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gjygiiaqn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gsyxoirue.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gayijhidj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/giucquwqo.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gvulwplad.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggonkaaku.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gibfjclkj.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gupqgvpjo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjhtgzuxe.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/guvqfoqhg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gunfacaik.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gaomvvcxa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gbopgbjbe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gmncmsesg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnznofgah.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gkgxkrffo.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzjnqpzqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdyureyej.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gelwlrvhr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/ghptbymaz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gptbknkie.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/grbpunzfu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gjvzjtwcc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gramqmhjd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gppcbchis.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gsnexupkj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/grxnoztit.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gltnmfwer.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gqkplpmsq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ghgdgdptp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/galsjrtzr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gydvusecw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gzoplfjfr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/glrfzmvvh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/ghuljgvnq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gjhfzmvvs.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gxbhctgaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtqgrhfer.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gfalxvutl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gzdimohpf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkvjktdod.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gerhimizo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gomhypjab.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gliiawywj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gfoqzyaqi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gcncsellc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gitxvwzqq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsfnfnzkd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvdjccgal.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjabbbjh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ggcxfbxsu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ghjgjhtpw.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gidiuzvex.sHtML


<!-- 参考信息 -->