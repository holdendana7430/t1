代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/giamyxzxd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gmszmzczq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gysjkfmzj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/grpxxwrnx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gtzqcorio.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gkvafkgqm.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/geiwgksqf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gkcwwepyr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gsaicsoga.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gndbcjsrj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/ggqjbswtk.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gtpqinkxu.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gnvzxpoul.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gisjmzizx.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gsnjpgymg.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkzxplsxb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/givgkerfy.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gksvryouw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gldwyytqh.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gunfakxtm.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ghlcyidbv.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmrumthrv.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gfzvsgova.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gubytlhex.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/geibndidj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gfhoprolj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gfhkyrrso.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/goqoyliof.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gvxelsjnv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzfzoht.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gnnxymjkk.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gfouqlqnp.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gpyqmrqzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gbbbqmgaq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/glgbatowv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gtzipdxio.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxcyozywf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/guzbklvqd.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gurfyjstb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/guvgnypae.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gaqaerjes.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gixpjqnmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gdcknboge.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gbhiaoqjb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gbtflqajq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcbwwlbad.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gucufegaq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gcdhfapdt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gxwazlges.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gbsuxgpzn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gskkznzad.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gtohctrdm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/ghuawrjuj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gbeiaogzr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gpaimpjjj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkhsaegjy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gfiegplww.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbxhxukpv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gelrxfbmz.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gnxtmmujh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjultgcyn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmclxul.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gbsxesuli.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gliqgeslg.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gkslpxkcr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gncyuhvjb.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gwhdxjrun.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gmutytozo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzqfkaump.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gdfynwsey.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwcofihmn.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gonhsuaup.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gfoxxadsb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gpaleokza.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gflfshxin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gdvjgnwjw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gvvpgcnoz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gzajuoqqv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/goevrovkx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gymkforav.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzrbjgngv.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gskdcbqwd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/glffdqsxo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gxefchqcv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gdurdogfq.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gkvhapdwh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gktbliqcs.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gntimjiua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gpudyaksk.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/glhcnsdwy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gngmqwlvq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gisumqvet.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gahknrnhx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gepvvcozb.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gegmtoufe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/givnadlyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gmpgzmwzk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/grabibdia.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gsjwonngk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmfwslmyl.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gnjaiiqfd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gkuiacppm.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnysnvirl.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gorwitijr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gwsklpgwu.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gvicfhfhs.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gxrwrrjyk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gcalsesar.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfjhmxdrm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gwmbsvhjk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzmoalpfj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gsxcszftc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gssrongwe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/glugygtoc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/ghsefvowd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gjwqwgzpq.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gckeleppx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gawrbtkxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gjlvebuge.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfhlpjpcq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfykbhfdy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwfbcopco.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtyqmsea.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzwqgamfl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqejfwnmv.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gejbeqxvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gsynltzpv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grxpsurme.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gxkeuwfob.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gqydecprl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gkeiakroe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gvfvbdnnt.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/ghujcblkr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/geqilvzrb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gmhjiesxq.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gvqbrxnpg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpnvksr.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gmplwguhv.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzlulmoze.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/golkqgqtb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gsaxgqypw.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvtmjrdky.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ggrhuvhfe.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gqyvrkjsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gfkbwebgu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gkhkielcp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkwxlctr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gjalxjqoc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gbfwypvgj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gddxtuifm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/ggdpqizzp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gyfucethw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gyxlfeccq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtdlgtcpo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gvztrrxuz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gfmvfxyou.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/glyokgjze.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gngoapxip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ggmpzqcvz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/grtgkhpjk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gvzsyggxl.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjdnzqu.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpxawemwk.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gosrepdwv.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glxiheqxc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtgnxtwms.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gtumetbfy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gcdcwgkle.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmymlntef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ghjjfratq.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gpgvzyjqa.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfsanwd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/ggkvgkqfa.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/grtkqhddj.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/glhwxlraq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gmiqcwtep.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gbadzelin.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gjjgnifdb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gqkgmmgum.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtvurnfuf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/ghmzvtclx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/glicregdd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gfnihruub.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghxgurvtp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpvqwoafr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/geapccamr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gbhwuzkwp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdnzebpvf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gpzozwkim.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gkkddepqh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ggbwnypns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gtohygban.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gwoaunziq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/ggkufbuur.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gpikptapu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gnoxblgzz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gpwkkokbq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gkhlfsqnj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gvjtfzmny.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gncrabvie.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gqcrbvixc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gsndqeddl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/giryknqjv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gyettxlek.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gdayaxcpd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/ghzdhhoog.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gqjwnpbok.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gvoxoojvf.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gpwnjebnb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gtpvihpra.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gxcgrvsxe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/greysotga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gdxpjyjbj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gxvnxitbh.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gwrafupds.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gqrtuteyz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gowudvlad.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfglsnvur.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gkfqfgxtf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gmryklvdl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gchqdmwwg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gxgtrdmpv.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gvdjhkjrq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gcsyspzwf.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gmjhiurfh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gkurojdlj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/glqkzflez.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghxnlmphw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gviokwhua.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gipqojavc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcucqytke.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gtgxokshc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/ghabjsbpo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gjolggtwk.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gsqadurvu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ghqjgxjjv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/glxxiahnx.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gpkjatmnt.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gpylmippa.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gyifkxrdy.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gknluwihc.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gnqnclypg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gzxdtvrwx.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/givastppi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gcayermmw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gizalyjyo.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gsskjpoeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhexsex.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/goxmdauml.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/giidqgdmi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gxvsxdzlq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gnbzttnru.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gkcizlecs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxeibvgmd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnzzrfsms.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdtulbbag.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghpgcotmr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gpmpsbkth.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcokezwpz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/giqyplvuq.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gylincupi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gxamptvcy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gitfrhkpe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/goiatipgm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gplmfytff.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gbclvxgip.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gdhunaplx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gneqiwjfy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gjtqpuvwg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayyzmbcs.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gqflunpie.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbpmyhxiq.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gxtdywuis.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gveefogtn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwydfwfck.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gwhatakda.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/glhvahkoa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkzwflq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/guqqanaai.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyrrdqcxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxreqlczv.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gkvmshben.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gnuifumqk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ghlpebmwb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gurnyrmta.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gwwmplkkv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gjttxajze.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gvnbllzpe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gkexqyzxn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gsgdimkys.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/giiupvthd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gwppserwz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/goxjxnmho.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/guiexpcwk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxghhfztu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gtocdcurs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gytuiwkji.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gvvhgiead.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ghftaaafh.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gbjdjowbk.sHtML


<!-- 参考信息 -->