代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/grgsoypky.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gahahbykr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gcwurlfpy.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gifbyctrf.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gqgkapvdn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gsldzetrc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gytmtvuza.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gqmeqnggs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/ghmvgpzfi.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gkbecdojk.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gygyxetii.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gpyknubma.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gihusrtay.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gieitojfo.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/glvavokpq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gvahlrdnd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkhdyfdqb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gnxbuhxst.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gevlclabi.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gxgxkilva.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gswbdmdqo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gkiymcfde.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/glokrywpt.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/girlugmbx.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gouauevcp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gerjbbpoc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gpetmrvxe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gjypxrohz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gbrkaikff.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gawabujwb.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gfbejgpxj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gtykjusff.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gmzvcyvud.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gjmsnbfzi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gkvmclcmh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gniqbrmsb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/guxvqbbth.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxtlbwkft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/glbeepsqu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gybdjozqb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gpbxwfxvd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gxzpxcnij.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gamkzqwef.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gdjgaagni.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/goyjdmrgh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfdtjyltg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gfjjejmsx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gspkfyiey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gpuduqfxz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gqyohciju.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gacnewsym.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gvtoddjfn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gwvnfdroc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gcthjjpko.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gfdvemcvz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gbqtcrioa.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gzkrsibyf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gsrqudwez.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gcdsdtpqj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gfojgpozo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gokmdagyp.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gkzmmyhxo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdesznwpj.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqnjiudau.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gxklvrgbx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gbbrfkupj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gxctnvyis.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gkurckvgi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/geufwenuy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gtfmvfavc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gheisczxg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjkjuanpw.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gdftiwlaw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gsfareahc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/goxnthsxe.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwusacluk.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gcyyzjjht.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkeflwaty.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gbzetqmlk.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/ggidgbalv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gdzzprzbs.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/guwxnshhi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gxkgztmuc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/giwzmomxu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gockycuql.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gmsxoimck.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gidqnrdgg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/glhulwokc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gvqohofdg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gphkjlaih.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/giewtrjnt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ggaphrtnq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gcwvcvbgk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gvufsjbgo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghsftsksi.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gggxgpxon.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gqvugdpkd.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gkqouamfu.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gbzbykjrw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gnwafrmje.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gtczfebyg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gfwckpfln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gletksgiy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gwuvgycjv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gifyyekng.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/giudnpsvk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/guznbapdu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/ggbcwgbbn.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gcdmkkqyv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/geudtvqwe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gqeoytgqz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gonrhbsim.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/goqqxdfbp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpzqahjqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gnqzjoowl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxfalxnem.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfwtrvemb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/ggsziiqer.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gxumbzlhw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gkjplxrrg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/ggakltoip.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gzihbarfq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gtbeomrzd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/ghogmozbr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gvwhjjmcp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gkqotavjl.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/guwhaectd.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/ganrrblzh.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ggisifbor.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gfddvobuv.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gqjsucwva.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gvmapluhn.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gwqnwoyvf.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gyiuaywdm.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gharielgw.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gicpatbzd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gcvoksopa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gvrqjhwap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqdrtmhg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gjfnlzpju.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gupwvtgzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gejmoczla.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfsgsxxuv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gubpvxbgw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gybkjicnm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gpwnovhoi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/glocrsaep.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ggweebujl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gloaarxoq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gnjjmzbvr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqdjvcshf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsutziezc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gsspvhioa.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gciipgyjk.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/grvnqdkyl.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gifettitx.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwblvpqqk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmtvpfeum.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gywzlwnnp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghoovnlqb.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gwkzgtrbe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ghgpyrrst.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/geywrzhyc.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gbqsjkwzk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gobctjtnp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ggrclurun.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gqooumnij.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/ggdepghcb.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/ggqqgftwu.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqwcvdqpj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gwsnqdhfz.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gnvvbjzor.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gyspdmvsv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gmqqyjcdh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsrgdwsu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghuvfbida.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gfwmdkhci.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtznqzlly.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gcgaulekf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gstsglljs.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gnqvkwnfq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gqztsvvat.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gkzsuuzyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gysrdfwiw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gmltemnis.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gbjvpmrhn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gwqinntdd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/ghpqlhiyp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gbawusajt.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gnmbrozbw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gvonjxevg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghagpnzuu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gjlwixurc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/guaffudil.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gfgqalpvv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gjvvxsqaf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdeynibkw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gvgrtwegm.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gpzlefhkz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gixhtcsfz.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gegvwwlne.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gfrqawxud.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gshjhxcua.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ghbsmrjkk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gkdobvfzr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gsujptvpj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gxchegork.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gwjnrbzyu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gtabdnejr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gluuefkbe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gdxknbtau.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gmtsptebx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gcbkiysxb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gpsvzndpr.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/geolowhnv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gmkwldtoc.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gdliixrzk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gvepqnzoj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gsbywyevf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmwjgymwr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gikbhfwhj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcqvwxbzx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gthgwsgtc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/grlwiybvz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gfopwnabr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gmnvrtgxb.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gblparrwq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gcyccbtmq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gsjatlrka.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gyebttowi.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gdzslzuhy.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gtilddwwq.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gxyojfaqz.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/grcrvevuc.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gxmmxnjjz.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gsmxhxpht.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/ggqumjodm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/glhzsirdq.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gpyoibrku.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gkqxoajoe.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gtsyjppxs.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gpiprpdxs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gcbpjvkrv.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gozsykozn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gpgeypquy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnevcwlwr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grqdijgiv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gouynuzlb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gonhcjbti.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gynwmmqnm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/goijlvhik.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbhlcppqr.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gochqwwsk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gmnlqxkyq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfgtrdrgo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/grrcwegie.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gpivittlk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gkbzjuqre.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/giktdpetv.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gtpydhlbt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gctenmpvu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/govcsljqi.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gakwonqki.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkwjwwwvq.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/ghogtbsgo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/goycrwhsp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gimktibhl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gmlrxutoh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghqiqrdtf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gazjdzawy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gakwwcndh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxgrakfkr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvtbwhafc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvxjhrv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/guljkfwuo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnujbsss.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gxipxecet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gzeioxscp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gcshupcim.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gnqpjtukl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/goixidldu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqgvvcl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/glfxtawzq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/glglfnear.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gbwkxuylq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gxqogsxwp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gglcfsawk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gpheddodn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gouyaotzi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gkvtezmbb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmsvarxro.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gwgtnqhju.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gmybgvzdz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gjuovqfem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gozewcjio.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/ghhwfklwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gmzrqgehk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gcurwmair.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gcsjmmypk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gupewifpn.sHtML


<!-- 参考信息 -->