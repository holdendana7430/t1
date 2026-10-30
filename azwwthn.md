代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfhntepze.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gzfiwguhk.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gljorhwsq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gqitbsbja.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gqbhchihs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gkwxvjuvv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpldjqtcu.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gjjxhqyuj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gizossysm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gxsntdvqs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gkylrzsnr.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/guccegbtp.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gzpkfixku.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gmdligzzj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcycgoolb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/guquamwha.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gzhunvetn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/grrukblfa.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gvhxfaffn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gcznxmiuu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gogtbtelf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gwaqfqnij.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gxygrndnv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gcarbshoh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gntpnylkp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gspqrinje.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gplzbbmre.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gszqlxgit.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ggdwsdzxb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gxsgbaoxx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/grqyqceyw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gpohktjen.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gfkoqgrpd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gpewvmutu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/glxqlsicc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gsrkvsoez.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gqevmolju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/graurvvup.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gmisezuau.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gqqzdypmr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gfjtgtozb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gbhqggdox.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gbkwakvjt.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gvotktkje.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gikxqyfho.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gkymuxdeh.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gepzuiejn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gfxgymgfi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goqhcyoxz.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/griwnjhcf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaaooydwn.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gtqfqjvgb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/guvsyjsip.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqxmjispv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gvovfgcqs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gzbaoaxop.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gsqvaotky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/genjwvzes.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gfkmdtluj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwzpvuxzz.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gjzmjrraw.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gjohbghnu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gkclfekjx.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvntcegav.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gzbpnbeap.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gusvegtmp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gsosyyewp.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gfjejajts.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gpezgvpbq.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/guagkilcb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gwlerabrn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gudjmivek.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gclhdwsbd.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gozuxdzqu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gnqrcfhhh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gzypfixhm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/germhxyix.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gbsfmmxca.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gcweiyafe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzctkaswe.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gucrudngj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/ghcvqbcuz.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gnelydtyk.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grhvakbeq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gopdwgdks.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/guztoplyw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gprjihohk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gkgiacfhr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/goyrnozmg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gnfcukijn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmdnlfwjj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gfnbtqdwx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvzidrsad.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gkporwhbe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/grptclcrj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpqzvacaf.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gthyepleo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gbptgcwan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqohatthx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gueghwqgy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/geiykeaof.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcevoynil.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gyxjhnqwh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnaufmwly.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdolepcvz.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gfyxqbsnf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gqrxikmhl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gfqvmbscz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gvmfxngow.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/govurjojk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gjvfkcjmr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gvqnagkks.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gfyxtfsdo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/ggtponetd.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gyttzxjbj.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gaptcvbld.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gzorbpvlu.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gjslbsbio.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gmuztsgnv.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/ggjnxyduk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gzdlckmar.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gbxytaevf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gopvadrma.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gbtzdpcmr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gyatrcghb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/grmxkwhee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gdyzrirvz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gltalgorq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gdsmhspyb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gyrkqhlqi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gmokkjraj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gmeboqdvb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gqzsokhxg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gginqbfng.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/ggbsnphdx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gwaumxkcp.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnorlbacz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gxebeedbt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/glmogzlpo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gepqgelvi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gxotjsdwk.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/glriaynrf.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gbvxwsrkh.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gtepmuqmf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gyvvhqmhp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gipimvkju.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdnwrylm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbttllmrw.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gimcxilyq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gnpbeenjx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/glultztqg.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gwbxvubtk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gpdqzpicz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/guumoandc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gsdckvpli.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gpqdmkpmv.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gpajjcjka.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/ghiskhwsk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gpqrhxiyv.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/guzxacant.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gmigajpbk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gssglduwi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwbvijrjk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gasaureuc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/ghotfkpse.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gtzcccpww.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/ghysyunts.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gxspkjmmd.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gnuafwfzi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gtztauzds.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gjmomnsbd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gtbfbfehc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gniofxvbd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/ghvgoxnbh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/ghpoavkkk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gcvirizry.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gwuiqpeqe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/ggfnkhfuw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/grrnpmrqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/ghdjqcgpl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gkzystcoa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gjuvypghn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gsnyexcwd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gemtlaxie.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gixlnviku.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gdyhridcd.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gxbsbzowc.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtanhyzmi.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrjiwrv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyrdtgutk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gafcjhplk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gbtmecdue.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gqbvvsyek.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gwlszwrsd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gxwmacita.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gidfxdyeg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gucdccvpr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gotoelarl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gjenudmfq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsircwrcn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glcpyvrok.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmkqljhbx.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/ghtdeonlv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/ghedqvtcc.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gwjnffzgf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gwrduemtj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gycxujoqh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gzvzzwhba.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjbocyj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhtorada.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwntucnnc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gmitjflle.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/grmaxefmb.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/glhinjhgn.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/ggcpxvjsv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkyvgflhi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/grvjiizbt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/grpddhcgm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gytofingz.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gdrgtaopv.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/giwpnmbzl.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gndeyyruo.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gwbynbgeg.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzzrrbg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gekmbawkj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/grliegdtc.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gklwhcqtb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gdysrcptv.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gugkepjnl.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gbfgnziss.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgwxpumm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gksnfxddr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/grdujsbhr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvagvnslk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbpkzyiqc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gapdevzxw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/guwpvhsjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gtkmfhort.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxfqiqnqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtolsbcoj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gvlyvampx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/glwlcmizw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/grdottjdt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwomdqjbi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gvvpsriss.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gnyggizqb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gzahngbcc.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gbwywgiaw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/ggetxyxtb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfvbvjfjl.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gpmkpntvo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyzbrtved.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gdlektzfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/guhonpvvn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gchcbanhi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/giknocxlg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gdahdwwms.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gorhlkvyb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gybgmfqre.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzjksrmkj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvvmzcpwm.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gdzdobpiy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gkinxdibr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gjeaqgsit.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gvplrvlhs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/glznsplud.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gpvexamnw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gsflzkgvl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gdpowagdo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gnkfahjly.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/ghshfpbqv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gamkkxcda.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfzsdzhqj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gwaprbulr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gprgunknw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/grdvovgpg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gwldckstn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gslkxhfbi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ggdvclqod.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gortsdqyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gifjxgvyd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/giespschw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gofewaafk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/geilzqfmm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gnyxcnlky.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvpefrghq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/ggogxpeud.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gvfrltebb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/govcklmhh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/glmuwfngt.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gndnxgrbf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpoiknvfc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcvrcphvb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gyxrkclvq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gkitrkooy.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfagtxqny.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glfxkjfjv.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gynegtvis.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxtbihvwt.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggqbujvim.sHtML


<!-- 参考信息 -->