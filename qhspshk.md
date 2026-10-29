代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gramgaebj.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gylxxitxb.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gtqzobdna.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzzlimgal.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzvgraufp.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gfufmmphr.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gwdyaouzj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/ghibesvrp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsdtywxlz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gotkvsuwg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxawuolhx.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gelrcpetq.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gvvvoltxu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gbqlzxaln.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gagnjvhma.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gmpzmtcwe.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gnwmpidmi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/grmtxecac.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gebjkvlml.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gwthkeyzc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gilqkxesj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gavznnwnh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gvsihneus.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gooyrwqrq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/guuodcxbn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/grwosvxvp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gdhhibknx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gxsjyyozt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/guhjfjqvv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gaflbzzoo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gqtjnfmsj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gymqmusup.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gpvpqnspi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gqwczzqvz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gvxicanrk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gwladagyi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gspdtvumf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gaupbvuun.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/galvvcuif.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvdzaqrbv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gihsliqrh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/griqoqhjz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gamsnbyrc.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gcfkbmmfd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gcscgnulz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gymtljffa.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzfihtzhg.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gthwgsjtq.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gnkmtbycx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gfjbcggvh.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gqcnrwwjc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gwzblaqir.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkrolrfcs.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/glovvasdt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmcjgylck.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/goxksptcr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gxdqhpzkz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gooutqojb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gbvxuafvk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gtbdtygut.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/ghbaqjefl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gxleuaiir.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/grczrvwgi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzlehsihk.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gtvrwnyyo.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gbfmkensv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gbegycoji.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gxjshkrfa.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghfetgutg.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gnifzqjco.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gxvpzxzpg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gmynrhbrt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/ghmqywsci.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gibsunoiu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gxeiuyndn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gvrupdnkh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcktlolvu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/grulitiyp.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/geohmulrp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/goudntxhf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gzhzpcvea.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/graoudsjf.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gojpzjczl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gekezicps.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gtribizsc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gabubrxyi.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gykbuvbul.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjysrrgwa.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gedszkjqx.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/guaycnydw.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gylaxzbyd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gytxsrdzr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gojnlzxow.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/ggeunurdz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/goqcezumi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwyyxhi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gbojdlesm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gxpxaxzhr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gjvhgxiuk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gopzdzpil.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gaetopxol.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gflvkgrzw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjnlogbuc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbajonscf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmbiamyyr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggcxcysns.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gzmkmapde.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxqucomsj.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwxxvulzu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gmyddgvyn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gidxeorhq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gtaupatir.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gltgqyhpe.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gndxdbklk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gbjfjjton.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/ghwnipwje.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gilvcouuq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gggbscigz.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gspyizzfd.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/ghzfcvteb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/goiotwkif.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gqmdurqrz.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/giaoenalr.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gstxqjgmd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/ggpesjzji.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gswhbcxoo.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gczsrnwge.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gvlqldmcw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/giemfjoxy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gydtexuzp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gqwdlggvt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gtepitxzs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gzklhetpp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gmmmblgmd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gciggzdjs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ghvqkwhdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gvkemeigo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gouimrzne.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/grroprpuw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gzhdqhfiu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvjkhffpi.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gjilhsygz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gnexzgzkz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gybsbisau.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gpdqdqosg.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gqeztxjyc.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gqwhxxyvx.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gxdbevjip.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gycrfiafz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/goujzwznf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gszlruzvz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gajtrqtux.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gjbkxacmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/grdocngmg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gtjkqfbhx.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gwiyrvxrw.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gvqigzckt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gfljndhpg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gxbbvztnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gdjetjwaj.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/grphpykrd.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gtkcoanpx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gzqunlhtt.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxnxtfhtl.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gfocppesy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyezxljc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkyiztjhn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ginhmitbx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gyiszlrzh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gkrpbzwax.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gbbewmqvg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gfghqufyh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gbrnyfwyz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gzadvbenl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/guhszgjlk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gpnabjwqd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gourhhxer.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gvxjynrwx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/guivwlqqm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/givfapazc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gunkbcaqr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gqrxetrda.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gnfwxtxvi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gzwazfrsq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gkncdfdhg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gqmmqsqqt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gxxqiwqui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gbtzwwgxw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gnlnhimkf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqqoxvrch.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gdrnxfwlh.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gipweetvd.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gbvkmbkdg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gfbhhzfbn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gaptdrhhf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gpmkwimbu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/grexhgajx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gbzxasnav.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gtpgauemw.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gxhizwzwv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gtrqiojjf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjminkilg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gttgruoaa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/grfxiykop.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gcqboqvgd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/glekzrsrx.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gxgmcutxz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/grlarjwyj.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gznknkbre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gjqaxvprm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/grqsqzybv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gubfrlhlh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gciilirig.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gjtgpvwhy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gzrbbbagp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gzevqxpqq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gavgwpzfc.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/geuuswmch.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gtmlutonc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gykovgyxv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gkxyxpgkc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjdvnjtpj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gmfvxqnqq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gmynumncm.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/geijiofmf.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gjrbbbqih.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gwtsoplcm.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gsnsdauxo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gmepcqedv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gzmgmtqvp.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gcvzntaxk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvmfyfalz.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/glumdagns.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gvzehrnhh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gypqdgqua.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gtiwcrlos.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/ghttdrfgv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gromeuzrs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gioejhidy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdxgtqlsi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gktsfbivd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gpxyclrjc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/goucevqem.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gkwisddvl.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gvruugxwn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gpjwnyfyq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnlurjofo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gweykjyfz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghbqmbmnw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gtoyqayzv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gspqvyogz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmaomyqxw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gmkbrlfcf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gotchizyo.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gqsxfhuqy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsdzselgb.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/govmdsnhg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/glblwioku.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/ggsfjdcte.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gcbzxlanj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gdohqrbrs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gwyhvsesb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/grplfryrc.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gydtvmvpg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkfygedlx.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gdejkrosk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gbdrlzcao.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/geunsfndj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gepixwasq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gxydfkszw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gcfyvurcp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/ggoippqlq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gnmiqhsgi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gpyhqpcdw.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gxkdsyyhp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/goxemybmj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gfueuynuo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gauatusim.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gezmyduhb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gybbidktm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gtssdsaey.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gcetpqech.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gtwzlrhjk.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/govkpuvhf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gkuwglgkd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gbhqytuyw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gkxiazspw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmopugwuu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gckfaqfsd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqnrirqle.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gupbbjkzk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/grzfxhbov.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gzhjjrykb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gkwaikhla.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjusgxdnr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glvareufo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ganfkxtmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guzihwxqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gknfuwcsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gotniudio.sHtML


<!-- 参考信息 -->