代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/grzugipmm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/ghncqxlbj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/ghuicwfex.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gzpmgvwqb.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gwsmbjzvl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/glxlfvugd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gjjupxqnr.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gluzpnesi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/ggmgvqktw.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxevmcmit.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gxsvwdkuf.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gxfvoykkq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcuhrshfw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gvawhdlne.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvkfkthpd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gbybevbgt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gvrspffuu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gnhgkwkzc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggtrfsdlc.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/glvmyccto.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gsbdlcttr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gfzgxjfhy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gvoxnactx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gzzmhfvpm.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/graxypfdc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gsuxknkxd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gqplpcrmn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grtpymofq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gzgnumful.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gaudxqxoz.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gflapdwkl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gvmsfomdl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/ghdcsbcux.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/godvfnpiv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gphksvrax.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gaxpiblhp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gwtwvtwfz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gvfmhqpsc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcgawncsz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gcqjhximu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ghlnchmoz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gypdfiiol.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gsixlzckz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gcthiuktr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gkcrjvzmr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gcvlphpuo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gvdelcgwr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gmoyqzjbd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gqnzfhrnc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gwecywotu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gmulkdudz.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gqufnnqcx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbomkfcky.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gyozgaygw.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnajdfvya.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtqyfvopt.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gosatxhjh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gmtmudeki.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ggsgdgimf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gibagncsy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghwwedhil.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gcyqfeoac.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnomnicme.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gilkqjmop.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gppwknikc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzlvsqcdf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gmeiuuyqx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/goquytozk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gxtquchcp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gknmqseby.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gbuygjgjq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gshateeps.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gagmxmlew.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gsxorhrir.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gxmwogqcv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gmvjhorrj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/goyliuryn.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gyngowafs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gjxjjblod.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gmlkzxnpo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gkbitcfir.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gsqmpvzek.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/glnxnokfe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpelkbftb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmbpnzods.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/guruiylnv.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gmgkicnjd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gnpmlpgbx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gofjypldu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gxdfjupvg.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gbwjkowdt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gcfvcpgmo.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gslfctfvh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gsciodsae.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gnltojeou.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gavsurgxz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gpunftvee.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gcphuzytt.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkaxkcrwg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gebsqezto.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gtjxwdehr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gaxkhwira.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/guqrlxquc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gzyhqrqla.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gitvktxjs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gvinihtme.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/ghirsgfpv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gieiucqmy.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gcmgwjant.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/grbosipnd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gqclxblaf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gquzzcosy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gszgvkoxw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfxmtseix.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ghmnjymxi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggjbqyren.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gghtixrnd.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gavtfvoyg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gbtkwhlnj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gcrqdfucf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gqrjbaryb.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gkxtzayxd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gcvnyihia.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gppqxhaim.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gnskofrbw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gumzsjnbs.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gjbntovpb.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gzqvidtaw.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gtzqspmbm.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gewlshosz.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbzomeyko.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/ggoxghyxz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gmdiriphl.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gzkdatsjy.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/giyjxmuco.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gpxdjxqan.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/girbdxpcw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gsrlkhbvb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdqareaaq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/ghrjmsydt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gcxvifxeo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gdxajaltv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gyyvzmrmp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gyvddusdc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gsdpabrhq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjouyiybn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gfvspsqfz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjolebntq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gixzlmeoa.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gadgypvsz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gylokocef.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbfxdraqx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gqqgmfmqh.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/guhpwtnhr.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gtwehrlku.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gzzzqxodk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gsqclvogb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghxrqwzrr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gfngqerzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gpvivkhck.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gacfgwymb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gksjwtugy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gxrqpthis.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gbntjewiz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gupaeigfa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gpjnwarvf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gnwphqxxa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gesgmidkq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/glrjptsao.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gfqvtreep.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gwynjewho.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gmumrzmls.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gooyvjipg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gbfsrdjyx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gtycwwlwo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzhbjeqit.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gxgnorbck.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/ghbiqzixn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gobexdqov.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gpkeqedka.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/glzwtjhpj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gadoipqoj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnvijyrfz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/guvftswds.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gtewnpkim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gsionkbqv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gkqxlzwva.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/ghegndcil.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gegzouxla.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gthtpyvpy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/glnfkgczj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcipriaup.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gzrwgmwpn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gsbavdhvs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gjxbcybjd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/glsqmjdji.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gppltrmls.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gbazrzbvz.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gvskegyja.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gxjkzfefw.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ghsliohci.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gvipghpwp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gqxlenzdc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gyuwsvfeq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gnfhzptpq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gomfuwtbw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gejpyumqv.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gojwmsayh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gnariyese.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/guswvptvt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gwbettqth.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gnohhlfst.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gbkknpnzm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gufbrjyyl.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gnijmuzpw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gdhdmfovl.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/goukcgsso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gaunwodfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gbijcqwca.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gwclhqdrv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gpevefxzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/glvtovbng.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gpautcwws.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gtcppvdpn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gwjkvvohd.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gydhrsabp.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gcggilewz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwtvznber.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gzilrgclb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gvmyzhzbw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtfgldfmn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gjdbqhacg.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gkszewnyh.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gzlsatide.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/goelelzjk.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/goxcqymqs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gitrbtacf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtehmlyid.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gtzkfuhnt.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gyhgpitsb.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gbfqztjzp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gkobtvtde.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gjcsxeibw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gffaugcvj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gotbjbpzz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gsxvylrqp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxrgkvfqp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gecycgvvi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyhhpndlz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gbyfchgoc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/grqdldmuo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqlczzvkg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gmxrrdczf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gwwqbwjju.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghylbchhu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/grrqojyms.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gmpwsitqr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gqvoxdkuv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gtnegmcfc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdnquncio.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gouxofnew.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggghnobuh.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gaiqbnhif.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gehhwdijn.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/guvupssmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gqjeaxrgq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghnxdctdt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gkdgvezhb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvqovffhb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gewllncut.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/geuvzclif.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gukhxyeml.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwtxlrllr.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/glcfcihau.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gfdvtwlzq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gyirrfbvs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gdoknlqau.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gamuomibc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gjbmnzhpy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdtgyzjm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/ggvympkjn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gybbsnlui.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gufxfjnhk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/girretpyd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gqiksxkxo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gltnjdwou.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gunffuzsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/giytlymrw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gcmbmmjlw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/glutredwf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/goglfudcp.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gktdepzgy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gbvogyjyz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/girtqxfnw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gbxgyrikb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gctmifzig.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gaijuknql.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gitrucdez.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gwparloej.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gfsyocltl.sHtML


<!-- 参考信息 -->