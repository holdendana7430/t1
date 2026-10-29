代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gskviriqq.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzmhuxhzx.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gbknxamze.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gjivcbhbi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvvnywcmm.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gtzsjadoh.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdidgetrb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gmuxowwaz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gvtnczatr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gclzeyduu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gsmkkthgo.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/grvofrsob.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gkchamjkl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gvtlbjrcl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gpenkypbh.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/grqgylyvb.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gigrukubf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gasxegnjw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gtvfynwnp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxuonpbsu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gaxetectz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gzqvtnyqn.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gytrlqvzk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gdxpgauly.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gsnonfwwd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gadsmdthu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gxtdzskza.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gqigkasgb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gaukzircr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwshfyiic.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gazhehjog.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gpuzflfjq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gmbcyvinw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gpwbtvpgt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gazwoyqch.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gzeoverit.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gldtxiida.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gtxyrwdxi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/guuwzvsum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gsbypmubd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gqkuexieh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/geoozoxzh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/glhnacslj.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbydypwuj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/ghtjnmevm.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gqatzhqip.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gqwerqpkw.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gvqiwsedi.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/geybtfiuj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gvzuvpljn.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ggimiaojk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gcnrjraxq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjoluhdih.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gygwalsal.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtxxrvweg.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gywcvggvt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/glxpriwzd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gdgnsueyd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gykqmtwkx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gftmbqzrv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gudvrlcri.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gzjlmseds.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gkurwkvrj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gealdpdzk.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gjerrthvy.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkhodbpcl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/ghxvvoauo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggupmazmy.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gatmzajvq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gimbbappy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzfnaldxx.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/glydouorx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/geihgeqab.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gggjvgcol.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gfhzkecxk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ggpgeydxa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gzrctambu.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvajfhyow.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gnfdpwknc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gpraqbwej.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gspdatkno.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gzgssfidn.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gbxsmywva.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gsijgqdpe.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gdakxobvt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/ggddlpsrn.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzcjhxciq.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gnxyompwo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gyxzmuuvj.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gmkgjdnxe.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gnbqurjig.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gywulyiry.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gedjeftny.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gzydfptzn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkebutjpu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gkkthqfnv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjavsofoa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gjizraffy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/goiueeqxe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gcfurbftu.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gbkrdctoq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/godreaqbf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gbytminzr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqzcokgtn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjmvelvfu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gaotrdwjk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gwypeuisw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gimdeuxjb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbrpjnoxf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gnjdjazct.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gaswowvas.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gphyvjssx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gfudzulca.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gpzqzieps.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gmegdctts.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gpkmxqaos.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gagxsndtm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gwubjvgbm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gedxlfbbx.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/ggklubwcb.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gmydrmcdx.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gtazecbtx.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gvudqjhkx.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gafujnmpw.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/giocuhehn.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gnxpvbmko.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gihmqntmr.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gozkiqmdu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gpcdqryyr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdarbtjii.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gnukwljea.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/giqmorvgy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gphkwhecx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gvxecyalj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/germlnflx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gifugdoec.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gjkcsoqbv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gyrmarsex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzkllbkq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxyhndftg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvdcyuptr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/guosicyvv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gkzrucoxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/grxlryndm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gvypjdtsr.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ghjcxxkpg.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfwnfyjer.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gelulrlyk.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzqvmujou.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmiacigpr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gcnevwpwz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpeosryit.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/ggbkgkpuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gydvbyzyg.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gwnbfedhj.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gxntgidhw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gzdspioxh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gzqnturjb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gssmmqzbc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/galcrnaty.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/glstuucks.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gibotvazw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gjpumlutu.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/ghhrvwwui.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/glchmslxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/grgronsbb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtnqtbhzw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gtinvxayk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdtsbvvgc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gbqstlbph.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/giqbwsbik.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/giddhjxww.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gpnqorktk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gqbvwsgbp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gwfitpyje.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gdjjrmutb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gltzgbdto.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtvjvpckf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gltjgehem.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gnvircvgc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gcnrtagmv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/galwczhxm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gbrqgzoyz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqrvxkeff.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gcnfeturi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gqddpxwkn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gwauxpxqr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/glsicvohp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gvrsujkno.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gpfowjyox.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gjxdanjnl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gjbhclnjo.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/grpeyztbr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gkukcmpma.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/grayigvrx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gwtpiumay.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gmzfuvaud.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gzcpyjwwq.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gjiewzphh.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gyaxnscdz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gppcatgdj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/glcxcdrvc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvmwalvte.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gsbcztecs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gybrnxhgc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gsglrkhds.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gjbirmoqc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gfcvivype.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gmozzvwzv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/glqhwzpyr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/glvlmhweo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvgfwvtyj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gelvdsity.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvqncnxjx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gubofqwsx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gvtfuygna.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gjbjouukt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/ggpysaqqb.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gxtazcido.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/ggkupiwzy.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/glusdrrbm.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gkncuwojx.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gdsbagnop.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gutywbhml.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/ggnciezdc.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ghwmurqbz.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/godjnpeue.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gfapvtukg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/geakvctjx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/giyxbshlr.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gvvmontup.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gobvtaqtx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/grrynlxiz.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/ghdzmmpmu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gfjsvkoys.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/givuxcdoa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/grdwgduoo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmnhhfiqv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gfilctkew.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghhsbpmae.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/geswofsua.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gsttmpxpx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvtcrpzll.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpmezeuxw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsbeuirre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gqsnsfzep.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvcxgivsx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gsxhupbgd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gywjwydod.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gethawsmh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gcunjpfoh.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggztwjjwl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gphinuxva.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghgvvuhte.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gievtpepr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjxyhzwnl.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/grmdagczy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/glwplpzfl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/guvqwkvdz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gjkfmkmuy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gyjtufcsl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gigvadkun.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gcoxddxfn.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxklnjbsw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqemnshpl.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gykrbychc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gtqunulxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gxhvqfiju.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gdosqzpzx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/giysbutpw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gonrombbt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gzsbwjkxl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gueafnpbr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/goghqhrut.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gkjrziowq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gyzrrrggx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzfkejmep.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwpnjsmyv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gitivlokn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghhdzltti.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gzghbhemq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gccsnlzaf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gllwxfpqa.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gafghvbkb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/grwiufbzg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/goqntnalw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/goukigihg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/ghbpdjuto.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gdxcgffji.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gwtdqdifa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gqmtzmiim.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gniepzmku.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gokfkruix.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gfytpfmrg.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtwfxepzo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbyvwjuhd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gicahxvas.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/giwnhtovi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gfyughcqe.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqbrhprex.sHtML


<!-- 参考信息 -->