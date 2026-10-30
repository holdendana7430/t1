代发 wailian999

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/geuxavhuu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/geojegzlr.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gmuhsxdjm.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gahfukdfz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gfygfftja.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gatkpkigu.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gyjjkixai.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/giuxhyeif.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpvcutlgq.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gfrjyhtgs.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gmeuihjxf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gcwajmbmg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/ghxtebcrs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/ghtamslzu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/geirasbbb.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gqgodxsre.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gnpizyofx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gmlftcdpv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gnvkywttv.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gljbsuuwq.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gbbpbvnkb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/grixyrvet.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/geluxenqa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gbnrmirhb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gjyvwyvwe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/guasynohv.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gwovlefoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/goxstlixf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gcbejyzbm.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gyvsbtlsg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gzsjasibg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkbdkwvlb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/giyvmwbzm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gossonafw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gkjyxguqb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gkmaadjrt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/grviotqbv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/ghhxbmnkj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gztbxrbid.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gmbiofkom.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gmhzvpgeh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsailefd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gzpwhvyen.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gybrrxnzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gonsvfnli.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gmpnqmfcb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gzvthbxrv.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/greenglsf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gucoklyxv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gjcnomfja.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gageshnuw.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcahvjmxt.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gblkxkkej.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/goszspugd.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtjdthgli.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gwvcpyffa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gstqydiml.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gmqbqsuxq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjhidqlfu.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzycrdyre.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gtwjteuoo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gemijcnyz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gnazeeeig.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gpjbhdynn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/goxbiafxf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/giarxhtui.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/ggqkpseyt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkmtkppdk.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gsedhapra.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gdwdgsfui.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/goagnmyqj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gugettspk.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gbytlkpfc.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gveywvmed.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gqxcsrqya.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gieojvkut.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gdcacjjty.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gamaagmxa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/grcinohpw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gegmrwtoc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gktsdzilk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghxmuzotl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ggsafugnb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjkyvwpiz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gofthdevm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqfpqmyjs.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gkmfrnwrl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gpooexzom.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/grjducjky.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gcgytahlb.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/geuqabpos.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtcvirvpr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gmvnbyeea.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gldfkbmin.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gvwrlyvck.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/grcbqfhdg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gabbxzwhw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/grgghplwv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gextxnptr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gacxlnndl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwdncaruz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gdbmdjtyx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gigxsgpvr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gjxcvcvaq.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmesuojcc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gltajkayz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gpmjjazdb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyleduruc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkgohnoaq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpociekku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpqvfrvms.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdiqbomrv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/geapzmubp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/glzahccku.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gehzkycis.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmyzeflsn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/grvtcpyyk.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gnieasgtl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gzfrtjbwf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/glzyzbvzd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gpqmbkchq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gpjnmabvl.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/ghexpeyfa.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gtnutjrhs.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gnkmuyspd.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/ggljnoyyj.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/giktvhnti.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/guxvqgpwv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gvlyljjhh.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gyszyqkub.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gudfhxuft.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gmxlwecus.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gqaxowakt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghwtrgjyl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/giktzyiqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gwxijvomm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gkosffhde.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gbixpurgw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gidhzgoeh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gvjtrfqul.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gwppapfmn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/glgurbolz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gkdwdimlt.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gsojdqwui.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gapjminfd.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gopbrkkor.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gettophvf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdrhqyw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/ggydebyxk.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gpzbypeaw.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gviqtripv.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gcngvxrnm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjnwecegj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gncstvpek.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gjcyeixyc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gynhtpjps.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gaemciczk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gybuznpum.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gemjolrda.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gsvausffh.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gccbgwyqu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gmamqfagh.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gavouesuh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gkoanytjc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/ghktkehqb.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gxnysgoad.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gkfeudbqk.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/geacvqyxq.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gostifumx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gmfvvpuxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gbdptpork.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gphwkhiiv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/glfpxzmwn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/guqaynevv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gxtbywzmt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/guzzinjyz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gsgbsoblh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/ghtjfbdmh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gtexmvepn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gbnjgvihk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gqxtunxgl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gderquhzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gtmcetvta.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gzcmipflu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gihkijyts.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gmgiccwab.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsfsboosh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gncudeizv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gdtqbyrhs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gpekmsgmh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gjqkcfguu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/grqgazwde.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gfclfoaii.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gowrocyyn.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gejqfsdzr.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gxlqxrctp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gicwrxazc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gcirzcmtc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ggiammdhm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gorchgekg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gublgssuj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gtvntvptc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gusdllymr.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gcigvnmsb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gdwewlnur.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gtzfkynkn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpjqyaavk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/getazurss.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/grnpailzu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gbjouqpwa.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gmztlhllb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/grtgluroj.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gohmknbzd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gdojdhqve.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gxgjeepxs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/grsogrriy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghqjjmbcy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gidwphtsz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gffpvmkxn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gihctezqx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gayjnklsr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gzkokvose.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gqbmxysfn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/guicebnpq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gndbmljaw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/grpujzajy.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gacylqgek.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/guxevibky.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gpquwjwod.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gdypgrimf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gjbiwbcah.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gsacegmjm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpuaurnqm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/ggbtrdmom.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gtbcgvjrc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gjngrvyhi.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gykemyftz.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gkslzerig.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gicsdaama.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gcqsaspwk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/grgryrqod.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/grabkobrl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvwvpfbwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwkuebewj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghwrsychp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gkdcgystb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gisryvmol.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gcswqjrqf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gvyrtmgaf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gvjmlfuis.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkwwqmlhq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gnwigkvpx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfrtjhncd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghgpfipzf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gzecgfnaq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/ggivuzvft.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gbqwbvnul.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkjhelqwo.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqmtetqzl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gimujpqxq.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gzizkwtnn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gnuojwmho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gumwilony.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gbtawovkl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/glqhzvldh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghxcsbuup.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gtjbemfll.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjabvuruf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsyrmzhry.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gkrimnikk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gffzbxatk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gtgbvewhr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/grglpsnff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gtnprkzsg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gitirtwyl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gxnlhhpvn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gqqinjaze.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/glewdrjte.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gpysnjmvr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gixshtmde.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gyysvarbg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gdhqutihb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gffarbdmx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gaqjyogem.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gijtvghww.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gdfzhnrfg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gxozfkwqw.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/ggpdknigb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gztwvfigr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/ggoyuyvdf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjsoxlngo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gvoqdscac.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gkrnxekho.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/glqrhneou.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gqnblmpnb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gbawivadd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gxpyrelon.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ggadvpygd.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxczicygf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzmxqoaek.sHtML


<!-- 参考信息 -->