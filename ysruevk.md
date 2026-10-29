代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gnishngqr.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gnljumkgs.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gudwpjrec.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/ghmszukkj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfctghjln.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gxfetnsfc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gagfkyjhn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gzbafiecc.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gkcqhszyt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/grkcakays.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gbempthvq.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gzqraykmj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/goptxktrn.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gprcbwtte.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghaoojsda.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/guhusblpi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gflbwhqse.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/geitajekm.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gdqjbhzyc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gteppzesy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/giukttdrx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gxydxmzkc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvetxszbd.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gvliawboh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gdabigfre.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/golaelaog.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gxcieaqaa.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gdbjtyhqz.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gtxazojzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gvsxnljbz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gihghfwwf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gsjzezgkv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gedtpmsxh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/ghtejuacp.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/ghgwdzqev.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gjnmxnxks.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gsyleucwh.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gfvzklayi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gumaevphu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/glqrgafxw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gqjbwnpkf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtfreirka.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gfcggekve.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/geqdctecw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gddxhuywp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gbsowvhrc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gdbjfdhup.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gzdrgyllx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gtwpdmyrp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/ghonslslj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gyohzbdag.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gzhebdxvo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gxipeecas.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gvzmerobs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/grnmlksya.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gberbnxtu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/goeldkkse.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gmoqtogzs.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzzhlolch.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvqpjmjtc.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/glwiltisc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/grrsexqym.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gltuuftve.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gnhbxarhp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqkpsgeje.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/grfddowpw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grnvihggd.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ggigpuuut.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gufxalbut.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gqatisqde.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwxtiaemq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gmtuspsuh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/ghcmemqha.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gwjchpoha.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gjzlbdowb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwhqhhgtv.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcijdqygz.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gvwrudplt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gvwixckbt.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfjqjzdhj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsgubktxc.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwudezxcb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gfzfuxwfh.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/guyoxhoym.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gwbdyagka.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gukkxnjql.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gjznqiwnv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gudkceprg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjjwrchdw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/guywjitsf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gygthgbcu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/goqgudbhe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gkfdiorhv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/ghdixvhwq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gdqaydlti.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/girmjqovj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gifyxgnds.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gwguxpndx.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gbfmntcdx.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gddkzhzak.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gydlfabdy.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gglcytdmz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gfuoyhfov.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/giclzgedc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjzcehiru.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gqymxcmae.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/ggejisrcr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/grpmfldcc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gicktpazw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/glkxyxdcf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/geyzzgevk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gvsmmczzp.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gynjvdbpx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/genoytkol.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gyomahisn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghsrbdavv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gsjmtwasu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcjnzvpsd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdcnubwzw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gswwuighq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpoqxraob.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gtecezpyx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/guqvwttjg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/glmzrahlu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gjlpoitny.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gldktmycx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gckrojhcw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gaurosxfn.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gzbvwefnx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gniafndzt.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gvvberkil.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gviwdslsw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gfhwexxst.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ghepwgawy.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvqagwmsb.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gcdtdnnev.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gvdydpbrl.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gobcgwhxl.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gddmjhmnd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gxgzexylz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gusuwebwv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gympwtwvl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvtzmwdfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ggtjjzdmj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gbghepxlw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gunshxpbo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/ghdlxlhhe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gcdrelogs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/goervlvfk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/galocmsap.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gumrgopmx.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/giaudvojy.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/glxipdwvp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpaslccpq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcpmbzhti.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gujknsgfr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvcqnhv.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gsklzesad.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gsxrjqjaa.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gwhddqtsg.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnoampwec.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtczapmif.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gmtbubamx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gbkvohwby.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/ghdzfvyud.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gjgrajdmc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gxwladoch.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvvhlezs.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gowdygshj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/glyqoyihp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gaqkhwbmy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gwdwxbiat.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gvoppkzqt.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gptgfravl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gdqntyuyt.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gyjbccscx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gmpsaherr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/guxvqoekc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gvhpryzta.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gvmigkfpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghhmqtuee.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/glekhiouz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/grejkblpu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkkcufnxu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/glkmwwndl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gmbwntxik.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gdpvgukzm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gmqwdjvrx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gxfhyavsg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/glidqapfp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gqknfnsqc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gdwhcjtcx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/glyzhxqab.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gsxhvghlv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gxvtcqtwo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gzmrsfzzi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gnrcjibek.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/ghzeboeid.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gkjcirzph.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gcafyybip.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gglngdtni.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gjfrpntbn.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gfxmrvaku.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gvzxrmjdb.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gwzohoisg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gayafhxol.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gpbkzsmij.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/guqtthnqb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gtghrmndf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/githbvjdn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gkfhsdkve.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gaetcscfo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gxtltnhsa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/ggwbhqnsm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gdbdkjswc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gjflymxuw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqntetnbe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/glqcyozuk.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gjoawovag.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gaotczboo.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gtpctnphb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gtlzyaizc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gdaloqofd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzbaikymi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gknbwzmpm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gfzabntsz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqnwlllpw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gxonjmqux.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/grfvqmqme.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gqfwezzht.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gaxitnncd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gsuevoyyy.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gidsuoklu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gpmngzbuu.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gnesmsfob.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gbtfmhhok.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/ggwkispco.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gbcfcztpn.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gwdeixmss.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gpkxwxwut.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gtrlzpebs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjtopvpty.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gyarnnfos.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gihfindij.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gfsyovdoq.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/ghwnfogra.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gebdmrqsc.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gfcjbwjym.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/guifeqyab.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/genztdwgk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvrduyllw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwwzlpoxo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gnnbnahop.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrhtmgi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqxbewelb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwakuwarr.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gnlacejni.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gybiqedvp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gftzebree.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gozlvqxfp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ghokcuyan.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gtbwolgrc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/ghhmcvewv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnkirzbdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gmgtlrecq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjtsifyin.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gwifujolt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gahhukurx.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gzfjurvtw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gatnmqbqg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gleeiacbj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gsxonjrfz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/garackkxs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gamyzxsgy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gzgduakgb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/giedyhnwa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gakxlcqie.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gedkulbbt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/ghvuvwkwf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/goahlrxwc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gigknrosz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnedqffes.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gqpwckuhc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/grlsfxwva.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/grdfixnds.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gutktsdsd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gnquaeqbt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gztcertsi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gwcixunsd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gsaoqjqwj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/grqssimzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gvbdrhhzx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/goxlefxax.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gnqzqaplg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghrjautxd.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gxomwpuak.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gecybschv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gohfpcxak.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gvhekaffi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gapfizglb.sHtML


<!-- 参考信息 -->