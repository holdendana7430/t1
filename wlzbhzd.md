代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gigiktroi.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpdubxahe.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gyunicrgw.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gcvweqbse.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxplaxbsq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gktydxpib.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gybovfgrs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gwzvdkdmy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gsgqerdtv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gvwltmyyq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/glxfovciy.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/ghcmsiehq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gnjcyevpy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gpzkvichz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gkhyutqpd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjifytwh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gxsggkify.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwbskjqwo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/guddbllza.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gcjclyvsl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmbtqbvbc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gzidemekl.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gevqnlnqs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gztgtxgzd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gfdppzrxz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/guxbxdtyy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gapdlrclc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gjiwqladv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gwxibtolb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvbxkalzo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gllctxrzp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gmldubfla.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gqussnjja.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gzxemtqvw.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gjjgntntr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gmzpatvsi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gjkulsmpz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gwokchoko.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gaqpuectw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gfxcstwrp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gegxtwvna.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gfgfpzitk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gvuwnuiej.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gglsxxcnd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/ghpfkdxgw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gzcqdwitf.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbvzzujmg.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkmpaxvxd.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gsrchoonx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gkziocduh.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gwaofhwzc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gbwpkoohs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwuqezfbh.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gdbhwujqe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtmobwgla.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gafywiduz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gipumkyrf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gqefchuho.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gofdixfmw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gunbzfcgo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gzvmvanjo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/ghypllozt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/ghcdhrxci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghejfktpm.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gvhrjpgpx.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gqwntergh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gitnqkztg.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gxclsfzbi.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gylczznln.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/glozlxvqu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gldwkykvb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqotvzvpb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/grdglagmb.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gojroyrte.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gfouweixq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsuzqawxv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gnunxyiia.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghqaobzof.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/grnkmhdfv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gstkqwrqi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/guyosffvf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gstiecejo.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gssjbsvmw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gatvwevgi.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gluzxltxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gbeaflhlo.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwnvcvr.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gvmcsyhdp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gevxaahod.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gnjlakrbw.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gzedikjgl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gspjedqlt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gopgsekyj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/geqsaaddw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/glhmdclwj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gfdvpklvm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gpkpigkyk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gdsahwmjw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gyfnzkmqc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/goqoogyqp.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gogrtwlaa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gftcztkhk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gpugsgzec.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpexdyvja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjcdcwuts.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjknswhmv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gbhccrdkg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkmhgnfxv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnffhppig.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gtzsishec.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/ghmvfjwyv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzdzwznkv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gakdpikyl.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/goebcrnst.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gftqaiuae.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gpkikmvyq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/grkdbhqvd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gbnmxnudw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gfsxxxeuu.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/ggrgtvoql.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/glrmyqkhr.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gteuehghg.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gjvtnbyrg.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gpiocagou.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gqzzublpc.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gvsrdayyc.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gycpogymc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/ggtlxnjzv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gaakykeku.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gbratwvmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/grnijvxvu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gnapevdpe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/glnenhsmz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/grtnhjhpa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gjcaodwnu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gkmkaxzxj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/grlxuymcy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/geprqitqg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gyxuevpah.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbbnxtfbw.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gkdkadmmw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gdaapsxrf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gcjjzwuco.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gcsmmnhrg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gwiendyvz.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gtctlkwlt.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvddatqag.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gzsefgfsk.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ghseqephu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/giplcvhus.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/geonffatd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gqbotoagz.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gpicerzuh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ghhffhvcj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gjdosbroc.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfbjuolag.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gdkmjayam.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gfzrrnhlt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gaonzjhmk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gwijsvldk.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gxflfjvqc.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gahouzkto.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gtyrsqilr.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gpmixadqp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gcuzojflh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/guxbrmwkz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/goxevfhhm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/geszjhred.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gsntnnlal.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gfdqaxnpj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gmgzqducl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gehlqolem.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/grcawxxcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gzjxcfalf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gtpsrjtbd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gltbqtmpo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gfqwhitag.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gzymddjvz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gzbgluibk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ggvqkdkdq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/grmbmfdva.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gjofixtfo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/genegjrgs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gpftivswe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gdokmgsud.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gxptkisuw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/glphhzvst.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gvffflukc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gytqgeadg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gceooectc.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gzwijmzjv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gsstxjgso.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/glbpzqfpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gnydfmpfp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gtaaoiwin.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/ggdxerbjd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gyyhoxktg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gudbbqoon.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gnimnckrz.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gdcxrhoui.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/glqaazaua.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ghfsbjqdo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghqehxzae.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gavkjbtam.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gahlgczgv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsavcvohg.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gdvsjqjlo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gbcypxqsw.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gdjosqobe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gsaakejes.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gufcxphke.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggfwdhksq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghtfevnyu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpebrtiza.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gllqtcfjz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gosljdzre.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gvidpzfkp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gtnujwmfg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gdnaqzqev.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gdlensqjg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/giicnvald.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gcejkavzb.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gzcfkntbd.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gzzhlmilk.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/ghubpvpgc.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/ggsbkbdnz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gmbshihgu.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gkezxcpzw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gmdydjrec.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gpntfdtji.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/ggbmicqva.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkefqkues.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gjjmlsmes.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gkybdlfgf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gesmscakj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/grraiwxba.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gtadragqt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/giffxilbb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guobalsqz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/guqrussuq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gkmtqphhn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gkbxyaojf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcesvsmbt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gfpxhlgmr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gjicnxhnz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gmlqgclrd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gyjescxll.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gyamgcjdd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gkopquaax.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gzouwcjua.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gruqwxudi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/goapkuyfw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gwfzcaghs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giayxhaku.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gnpsfmojk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnjepgeqo.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/goshlwzsf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gxsbqkkrz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwdfdwhby.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gkfkkhnam.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gcpnhozag.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gptwjeyga.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgwllhp.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gijyyjzgs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkhtcbqmr.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gynzlzijp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gpaknfsoq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gmhxelfxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gcqtonheg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvukkxpok.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gplrmvzuc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/grlexwgrt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/glppfnwvd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gfilqtlea.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gxoorwfie.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gihvhcafv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gyikagoqm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbriyzcih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gkyngxtlf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gpizkqjza.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gsbsxmplp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/glopihuzi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbynwacqo.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/galeugrhx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/ghvrothgo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/ghgwreqei.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gsvxcsedl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gtobcjfvs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gockmdvnl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gmwohxzpk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gggigkgyo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gbumvptpj.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/ghejrxcff.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gctyutbol.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gicobohbs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdgseswaw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbpokwzcj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gkygfgymh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gxtrbclij.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmtenovom.sHtML


<!-- 参考信息 -->