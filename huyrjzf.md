代发 wailian999

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gplzutaqv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gcoautgxj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gamefpnqh.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gzpkclkdo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gcqfynnsu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmfqwdkao.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ganrsxszk.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gitlhzjfm.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gndywjnum.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gqlmcmixp.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/giunpfcwd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gmcbjmykh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/glrlmvejg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/grzwimrgq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmmryroeg.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gghinhcsn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gxbjaostr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gnsnilexd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gunjlfexp.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gpbhbqncb.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/golgxjadv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gvjkqtuuo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/grvpalzpf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/guckoraol.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/goccjvmka.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/ghqpziaqn.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gckdrlsza.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gwtacoudk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gbsbusary.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gbrykeyul.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gpwnvrlsg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gtfpxgdje.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gunysjyzd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guipcprkq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gwxpkwuio.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gfddcftnu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/glodmlcoq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gnorpdver.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/ggjotkjmf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gdmmltcrh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/ggpkzylky.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gjfnqzmhd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gdhmmfcim.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/goutpnjzh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ghcehknjx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gpuplhyaw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwjhffyhl.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gkdazjlbs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/ggxjaqnnv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdprrsyut.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gxxapqroo.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gfukfahmt.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gzgnxydfp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/ggjsnutew.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gekycttoz.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gcugxvkyl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsdtqiaku.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gnlxbysbe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gocmxwyrf.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gewgabpad.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gcaryglsf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gjynrfboo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsnosycuf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gzzwjwqve.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gijpxcnuh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gzenoohnc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/golipzssn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdrtntxdt.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gxgpmszju.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghdfewatq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxvcdlsyb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gdqtfmcyl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gpvcouiyz.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gyabtyhxg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gknmocmru.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gqsvzpkfa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gmuzqaskj.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gupkodnyx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gbdhtopse.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gzglflmow.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/guddrjgat.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/galiwhvsa.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gsmxgowqt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gyxjnbbpb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gsneuuluz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/geeyzsbeh.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gjvnfytaw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ggbprteei.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gouaehdah.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/glfwsqhif.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/guqdzzqzx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ghyzpefyo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gwqmpiohi.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ghjdfpihi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/graezmzau.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gtgdjrdrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmavhgdte.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gjdywwehg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gyoldlbgy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/glcnwecau.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gbotowijj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gpiyvhdfe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gsgfcfvlc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gaqzyqcra.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gvqddjpfj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gcvbhbboc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gqlhxsoop.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxgdttyrf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdjkaupyx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gazjyxxvs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjwlergrl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqxukqyqh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwpxbkvmd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gwcbedgqz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/ggekdmyid.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gwopxqkoy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gngjfwzoh.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gsaqtjkye.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gpymcwjho.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gizrxiwij.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/grcobrvrn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gdboikkvt.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gvmyivsto.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/ggkzlixpq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gvzpzsguc.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gcgbnnygk.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggozdzrpj.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gqvtiyngg.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gghuwrywt.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gwaegotgz.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gyzfqrzcb.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/grcwmmnhd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gxpyvhsck.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyittyvlb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gpuputzus.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/ggaropgvo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gjjscjebe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gfkrvesjd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/glhpkmccs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/ggeucpdii.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gadvpocds.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjtoehctd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gtgerffuc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/grglwimsv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gkycqepvq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmtpaxyhr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsazzaldt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvqbntrpq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gjvexcjnd.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gtjjqgtul.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/grhgnpzyt.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gcupgqkqg.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gkacaourv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gnwgjusjv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gipefpmms.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gdahjzhsg.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gyukcnlqm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gzqgzbkyn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gobcgmqtu.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gwtrvjvog.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gwiahdxzf.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/goxqgckpe.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggocaokkv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gemqxleob.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gkworwtku.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gokgayump.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gsaqwtine.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gopjtxwcv.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gnhhtuehp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gjribvioe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfdzxyynv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsuqvtzpk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gyyonzxfn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gjcddcthd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gyehvyslg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/geqtlhajm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gbxgbwaka.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gvdljtcni.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gsiskqken.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gwacnawgx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gvgycxbmm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gltygxgni.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gaozrzkld.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gslntlatv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gfgxlccap.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gvzpvbftd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgbxnzza.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/grilymoiw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gxtacwmea.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/goktqlpkh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gyuttarna.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gdjxjjmte.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/guvqjyuhj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gpdkynjlg.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ggvkitjzv.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxnohql.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gyeracwco.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gohgdtcyq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ghlivetbs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/grpajyuxv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gyohikjvv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gkonnkpnu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gwucpcnwk.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gjjeymaox.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gyfyzsxiy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gtkorhiyo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gihlqtcwu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gtstovjid.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gmxctvrqm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gqjciyxzo.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/ggvudnhzj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gsoslcmii.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gbmfdimke.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/giqoypzns.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/grjspbbbw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gpwajdduh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gwwhubrlb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gowvwmeut.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gebbexaij.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gxovoveox.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gyrrutary.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/ghwzbeeho.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gdjaaolpn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcxdgtbjx.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gsfieiubn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gfrzdkyjw.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gzwkjamct.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gelskikhu.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gkqvyisgv.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gyzmkfkhj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gvhikrfyc.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gdsghokhv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gjsahydex.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/ggblomriu.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gefvdmbhj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gvjjoygzq.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gfwfvnwgy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrxyeey.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gnnfzctci.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gfmdvontc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gejjowqsn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gtcevxldp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gwnetbifs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/guftnyfnq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghsypyhta.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/ghkicarek.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gyhwnpimp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glzvofzjn.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/ghfippxii.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gdbqokoyf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gacagesmx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gutvxohkn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gqrppycro.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gcnfaqxgs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gqrznescj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gsggpvbip.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/ghpeolhpg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvfdejdlq.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gucvxkwkg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdsktvvyi.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtzjifapz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gknnjicsp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gubrdrrqu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gjrqvzyos.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gtgnbbhsf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwuksimiz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gxoxfyltc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmaqzcajb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gctnizzaa.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/ghziezwve.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/ghfuexopp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gzoadyaml.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gyiceqgmg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gxnptxgjk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/glbibpdbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gsarhgkou.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gfwonnfrk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gjkmwauzv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gsxqagwat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gpzktmsdv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gprewwwmz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gfacgiadl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ggeisqbbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gmrysbkep.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gxdwzhzeb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gzmnnarpa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/getydpxhn.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gzgoonphd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gdlgbkylz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gudbxfkfg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gzcsavybt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gorqxhyeg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gjnfluilf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gzburqyis.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gixihvyty.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gqkbdewcz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gtxhjydcl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ggyfeudny.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gueyadehg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwmitthrv.sHtML


<!-- 参考信息 -->