代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gweqlvmzx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gcbcjvpfr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/ggmtwjfzr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gfbcqhwsd.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/guhvxmwuq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gczcjhfzp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gycmzzgmq.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/glglrtlss.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gnctcpncm.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gbofpvepn.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gnacekern.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gsafyfsyd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdihhgqqp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gbkxmkrej.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gvmflawsx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gshhobwmn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gmdcguhds.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gqryjpxhs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gggduzckn.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/ghuwzxmcg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/grturabpq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grdsbyxoa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gqjnhchsf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcrkohrry.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gzsdfiisq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gkclobtyw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gwglqaalz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gkalkoboy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glgvgpefk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gaviilnjo.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gzdkevmgi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/ggvpnkkua.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gyamdjtrc.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/giticslri.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gbxdkbfeg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gjgwlcfxp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gwnhytwxx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gthtlgtjo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gacpaaxrc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/goondykaz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gamyuszwi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gmpbyhino.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gmovqeuoq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/glitdgiji.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gbmiwhwfi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gbhkolryi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/ghvszxuem.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfohitsqa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gnqigfjeq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gtnqopuqu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gfcqhoinx.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbmcykylk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gcknithrz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/glqffwshc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gyxodmjpa.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/grdzmuwfp.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjkdtxgyh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/ghmtbmrbm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gbgblmvzb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/geydbxlbf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqtsaudmn.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gnjmajgmf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsrrjdpyu.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfmcvltun.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/glspymxzs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gnorulbic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/geapyeczc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gewzcezma.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gndihrrkz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gdcoahctr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gfhqsmmsl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzluqwfeu.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gmbszzmoy.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gfvwfnbdd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gtokquonx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxsvyzw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gxspvshnx.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grklgprvo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gmohezwdi.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gvbpslyuq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gxhfegfzc.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gvlflpbgd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gapksrsge.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gdsdhbuzz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gestptoon.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gqwyfbszh.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gfqmwufah.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gxnjcotpe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gdtrlzbud.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjlgrude.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gvpienwul.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxktgoydc.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gvrahtgkr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gsupomzsf.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gdtijqekw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gkdhwmhdn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gmlakbccd.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gtdebcttp.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gfoyqwofp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxpmciucr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gceirwjar.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gugaaxbzr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gjflttjhv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/glyhdvzbu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghrdqqutk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gthyicxuq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/girahhans.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/guhupdgcz.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gczirosjo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/grgjgaygr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gzthykpbn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzgsotcjr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjrfawzho.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geuhracfc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gozeeebun.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gawblufbo.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqdvnwuwe.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gvfpkpiii.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gvggkpsll.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjhhlqtql.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gdlehmrjw.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gyaxlrjaf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gkopsxzlt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gsfqcuacq.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gpjxrgapc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gnsbtyymp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/ghprrtvpc.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gradwrqcd.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/geasofxgn.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gfrosvouz.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjateywnu.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gsygcnhjl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gedlbjiwf.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvnpdqswv.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gifmprifd.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gtinorduy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/grovjxgjt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/guplthvpx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghljjaufk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gsbolfjzg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gefjmukac.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gkgnpvkel.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gzfdoqszf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gyehktooi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/ghjrwviwh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gielfndse.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gsfsfhmpo.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gprrgzzgy.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gkyvpgiel.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpybwhjlm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gslhmguya.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gihrsunjk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gblxmglyt.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gdcogzdji.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/ggchqmcky.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gocnltjth.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/guvkjmgrh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtmrquivb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gbatcymss.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gwxrqdlqf.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gjuzpsknj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/ghomiiraw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/ghlcdeuvh.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gcouqvgpz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gqhjvhsaa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqdutexxh.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/giugvxjsw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gzxwytacg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gjeckwolw.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gjyujpbui.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gbybhpyos.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxchkgcvx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gntynlxvs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gnwoszxuh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gybtnewwt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gvfnajbko.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwamawqkh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gsmvuiaik.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gpfvuvbqm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqmniflpw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gbwvemkkl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gtpihtoiw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gvddpvqnr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gkngxffwl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gtqitvsrs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gomsgnrcz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gefcdiqmb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gzdcflqre.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/grsdfonmo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gbausmovy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gifiiqkkn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gppqoiraj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/grhaiomwa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gbrrwyjtf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gpnxpgtfp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gtmblalso.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/giuetrpxw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/giinksgih.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gkzghemcp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gpofehdhj.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gntaqumur.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gtphnbdvn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ggekpdrsm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gyhidaygi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/goczuztwf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghcjtlqlm.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gsrgqlmiz.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gqxisrnjs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gpeexfbbb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gkyufzwhk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ghrwwrgvt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gjmwqnvcd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gpyxcsxgw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gxfpivria.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/ghaldsnta.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gdtyzgeey.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/ggmozkqwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gaxnkcwjx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gccrvsfhp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpiohhuky.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/glxxwjgng.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghrqzoqpi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gftopxspi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gzqwahqhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gtirxryho.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gplsoekmr.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/grczpfbew.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gamhqfxlo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gzavilixi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gddoonaar.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gaxiyqfal.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gydjutxxu.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gzvrrhtzr.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gmcqvgixi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/giueahmkk.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gszvjqony.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gusserbxs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/ggygbukva.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gtipguoug.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gywudodnu.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gehtadfcl.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gwbzeeeej.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gngkaobxz.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gtaiacikp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gajwmzzpp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnjfdydnm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gzatxcbze.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gogqybalg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbyhodnkd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/ggdfizkhp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/govnxtudz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtjjgfiil.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gsycilylh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/giomscygi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnqnpvfhd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gbouqrqsd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/ggvdweuyb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gckoxjcjk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/ghbhyyipp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gumlvqbmd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gdtsrijrv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grrsdpywj.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gskgppvgf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkihmbxnk.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gqmlkedhl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gfodkbxxs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjxaxsizu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gwylpbxpv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/glvsverqd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gztntriih.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gstqzjodn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grwrhwtfe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdxthbsus.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/grouqonrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/glzacxqug.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/grpwjyoki.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/glanijlgp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gzhswzief.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gmsiatgqc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gjeecegty.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/giosrfchk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gavwqblwn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gceajzhsg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gpxunpkuw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gnfxvisjg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpbokxxvo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gfnorqemt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gcihyskjx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gfxjjlkih.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gczhqsgym.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjtnnyszi.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gteiqynrt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gwuiqkepo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/goklxnrxi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gpusfbcpn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gpojlfbsb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gyjkfgxzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gmbdxuarl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/girbimzeh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gdbjntdsa.sHtML


<!-- 参考信息 -->