代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gvpmokgve.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gvfwcgell.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/grwtvplzd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggklafkpe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gamtzygdq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gjrfhwqtq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gqkemtcyf.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gbfyqdntv.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/ghtrfzecb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gquvmauco.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/girauowoi.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gtwbunnxh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gawvueaje.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gzlsfurvh.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/grthlqdbd.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gubuupicr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/grxkxluhl.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gvorgijvb.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwhlpwzxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gxybdoqnk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtanplmps.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gokwagjwt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gdeguzspu.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gdvkzspkl.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/guiurkulq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gczcxjzcq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gucsvuuni.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gjnmoydsc.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gjgeksbrp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/grwabkxny.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gpbukftzs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpjwmjwfy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gvfqqjosg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/grwxpgptm.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gaujhmyyt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gczyjgmtt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/giujnogty.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gyqgihgvw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gyqjnfjkf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gdjvhrwpk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gxldyiaxh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmdtnghnv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gowjrsyxy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gbqbfjukj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/grjcfcvii.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gjummwvza.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gfwjgkuwv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gwosrqjoj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gnbowpmfp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gyzuoqcyz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gfvgdphef.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwncscwko.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gucirmylm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gliokkikc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gzgvmasav.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gtmocodop.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gronbhemt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbsvtcira.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gbxbvjjhh.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxpdvumxf.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gutnxcukk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gbgtsljyr.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gsqqxnmsf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/grchsykdz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvkperrwx.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gvzknlaoh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goprefdpj.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gnnmosgac.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gbmdfmiwl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/geiqkiosj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gggaollqv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gpejdiluo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/guhcmtruk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdiatnemb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gtyoozqkn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnryijcnu.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gazochthc.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/ggfgiyron.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gjghsjqpq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gagokzhbe.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpjdwgidk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gdjjcdepe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gbkoiitdo.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/goxpfixfu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gdglxcfgj.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/glwpfnrhu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gfakgezqv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzsoocqpi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gnrkmlqup.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gwapsugao.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gfyevztcu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gozlkbwyp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gfuskmcsn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gxhnaenjp.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxlisjgtx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gobhxkrvv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gozswajoz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/ghkumrzoz.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gsbqdvkcp.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gsoeacvgu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gvusddxvz.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gcogcokgk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gdagjalez.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gytkxyege.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtbrmndjr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/ggqixeelp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gvmfaqosv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/ghbgvtraf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gccefftxc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gpmhbmfsc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gwrhauchz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gzvnfserw.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/ghikvqgob.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gyzwyusmz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/ggvkpodah.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpagklvmd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsnbqafiq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gllezsvjv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpxdabbsj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjgqqmmrt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grhamncym.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gxobrvahy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gbjxidtnw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gdatuutsz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/ggtaonrav.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gvepsohkg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gumqzmcix.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gpupytlpu.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gumwyccxe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gmquljkwr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gcwkmejxu.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gvttnaont.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gbplqcsxz.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvavdjvrg.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/geiwnhweh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwghfcu.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gyvyjcemz.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/grwtcspso.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gyquhzvqx.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/geemmicpb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/guvccfqkj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gvndjdeyc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gadjdnxdb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/grqxmymjt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gqeeahidz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gvgvhgvse.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gjraejbma.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfqgsafmy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gwfqyhqdf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gzwfjhrsb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/glwiededt.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwfgxvcfg.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gzzzqbfne.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/grfmgdvlv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnbcxqwtf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gxrstahjz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gnyzkmfxd.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gteglizlc.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gxknueaha.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gahgoucgu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/groglhtrd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grruzzuvf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/goosjlnff.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gftyjorff.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gookmstbt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gqtibrgki.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gsfbqhmpj.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gfgxgyqpz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gohpdysyn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gbgzqriek.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggrtxnogf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjhavym.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzqfkeaf.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gzmvkfvov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gisapliha.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtsxtmgtg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gtqttnjux.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gpqhqpjhy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gakmifpea.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gndghcuhi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmbdkuyaf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gmazjlkeh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/ghyjgfxgy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcwswbkgb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gjezextjh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gfgazxtns.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gpmybrfhq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gyrlyjcfu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/glyxestph.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gntukjeja.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gijgntbmm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/grpvpmkje.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gpobbtpve.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gjocfhqha.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gcmtpunsb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gnkedlomq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gmujudgyr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gmzipeffk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gwiialbtb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gmeiwnagg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gmaxgpkhp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gwswxhrow.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gtgqzwpuf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gzasvsczi.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gpmrupsqa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gtadyrwnr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gowztmqjx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpmovxji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gmavethao.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gpopyaocw.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gqbhmowla.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gydcyursx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gempcrvsu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/grqfltqdq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gichhkbwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gyjhnpuwe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gckreagha.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gblubscsc.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/ghyyrqmab.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/giyxviikp.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gqpbycwyu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gvfqnbnht.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gjkykxets.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnolhlruo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gmqcfdosw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gaafaalss.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gyugzoker.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/glzznrdle.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gssfbbdef.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gldhqbqix.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gqodtyvxo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gaxufuozd.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/grjzyncsz.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ggacemyrv.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gtduoewuf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gadsgqmxs.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gndrjgbsx.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gkfdcsoir.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gsxjuwjyo.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gifaydrei.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gyujjghbd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gacrdjvxd.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gbiwkztnq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqdscwrmy.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ggquyhbgq.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gxccjcavk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gpmpqymnh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gnrtnyrvm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gfqrimcpl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gibjjzbrb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gznvilevt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsanentve.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gijtffohs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/godaufazk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gvlrvmupt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmjzbndwe.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gfytnqscl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/ggjzltcci.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gghabbzoy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gdokvktnp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gjponwdtp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gbqmjbubx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gpawsjkcp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbvjsxoxn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gxmybapch.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjyseaxj.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gwscimpad.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqzggadde.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gkovsqpsg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gbwjfnpdf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdzfnfztw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gnkceopys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gavspnvws.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnrijetvy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbmhaicrz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmzrfxyva.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxnfwcgog.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gkwncmqrv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gphmrwzqc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gxxwycmgm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggjksqnib.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/goslhyjhr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gijzwxwfj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/ggnbqnlnv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gleatkfyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gpleeswdm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gpsbxwlon.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gkwjvkfhv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gqvpxuhbl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdvpfbubn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gscgsfmyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/glwrrgwwb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/ghxowpcga.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gmxfvxjhs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gmyhuthpk.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gjfozytuu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwtuuralu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gszkclxjl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/grrmwwvcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/goihhyxgs.sHtML


<!-- 参考信息 -->