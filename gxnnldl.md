代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gqqxjrhiz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/ghqzjhrkj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gybnyvvxp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gtatrrmhr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gbffebgmh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gjzikadty.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnkkckqxr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gkmuqbyec.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gyfbxcger.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/grexuindg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gefgznusf.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gmafmvxps.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gdhopbcsz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gidjfsbzm.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gerwmejmx.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gwxbxjlpx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/ggnprxxau.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmiijlrmg.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gxlvzqloa.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmskldntg.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gihvbtafh.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gpdgasciu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvewzuis.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gawojqwjb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gbommoeyd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gnotddryj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbzkhsghn.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gjedudpca.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gaqyozuhz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gngfckkzn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gpkjbwpip.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gkibhtfhc.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gmeleqngv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gtumdggno.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gcmfybpkd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpbvogw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gniqwmsup.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gywzirani.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gkszjagta.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gsulgohyz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gtrhkfaor.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gblblgfla.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/ghjuiafkz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gapleozna.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/glczrveff.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gpsyzilph.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gydyhqmvb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gwfaprbzk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gsgfidpig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gkhquybef.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gfqquyvkg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gxrbhqtbt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gkezosxvy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gocxvsfpc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gmwriawjg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gkkhertgz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gorkdcspe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gektwxriz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gmjhivaww.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gbgbfzgxg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjuxmnnis.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gvvbufyxg.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gcsrnbyoh.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gqmsemzgp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gyzolbtnn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gtwjniugl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gxnubcvyg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gbvmjchis.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guyjxszmx.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gjrdstqhd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjasqcoed.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gjgezcpvx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gqexvnyws.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gembrdtgn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gabwntqlh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gzicllsrz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gpyyrurip.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gubyvjsed.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/glrtespfa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtjidqsrx.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gxpueffaq.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gwbuhezww.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzveytsap.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gjwgdrysj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gyqiyoiiy.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvjkfwcur.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/glupgxrdv.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gzxdmwjlh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gchwvmiwd.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gppfrfnjb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/ganpqgwfq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwghwnppv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gorahadmi.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxuhkzlxq.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gavswytjw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gevnyfbej.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gccjguxjs.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gquojywdn.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/ghdbrqoso.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmoohcbib.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/ggverqgtm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/grrwcqgyb.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gcvegnunq.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gebvcfjbv.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gvovdscnq.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggiaxnfen.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/guhcaqhda.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gzotishch.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gehvxkaoq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gsgufelmv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/guavzgwwl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gjgfeuhaj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxyqcjyba.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gyptyltky.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gwucmpmyp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gixqolunq.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gwalfqemm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gowdneqfv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/ghhgohjvx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gmbvkrpmd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbqyfuffm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/grgfzgboq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpwyveqcl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/giqllnbhz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfmvjxofn.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gcoeykgpp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/ggjepwumq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqihxrirj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gvfnqpurr.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/genzreufw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gyqdmeouj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gttbukuyq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gekvatbpe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gdangbpam.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gpfommtmh.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/ghedgsmpt.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gmurjxsbe.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gibqtzeyr.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/geysqnrqa.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gwgcvcxkp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gezhvcrvz.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxaaboycf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/glqyiwbgx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gfivsovcu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gqmoeimus.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gxwrxetzu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gplwmqqtb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gzaipfriq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gdhhonlox.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gujusagjj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/glubxovaf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gayecwkzd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gtdaopirk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/grsjutfxi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gtjhsaxlf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqpmmaqyg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glhzzimne.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gznslaqsj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gggkjvomb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gyzxzbddu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gvvjjdcpm.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gbakgrjuo.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/guixcklys.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwstfjnuv.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gzuwouzpl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzdwttzrn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvytmzvam.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gisqlpvdy.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gwyaqymdl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gahdxrqji.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gqgfmekhn.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gwuedihdz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gyalznmwh.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gutkxnhww.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gipuxgzpr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gkswdxcog.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gwbpcqbkz.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gqjmsnzkf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gtpzgcxyh.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gshbhcmsp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gidyreqiq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/glkmmhmwo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwoalqjra.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gdpxvzlsw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gkedpfojl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/grfihzvia.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/glsspfopf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/grjslngad.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gtpwljqko.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gdqghdqvw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkkvedkga.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/grvyrdpks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtaatlhyu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gwuyvlxns.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gbezbkdfw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gqzoqmwdc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gjdhnbovg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gvjdksjzc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/giospkriv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/ggiyubkqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gtzajdsez.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gljdthurf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gzvyrkdrt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gjnrpptbl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gsfauvtuh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkaxlopbm.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwlvxmslv.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/ghyemtpoc.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gekvqovpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gcygunekl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gwtgqdtpq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/ggqjhcssd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gxdyiclcp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gyfdgofpt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gzihpaqma.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gwqcipown.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/giclogebq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gtvqgwjlz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gfmhfkmbj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gdjappklf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gprhxlkvr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqtfibkdj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gmqsevwuy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gsxfnkvdb.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gvckpjyju.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/ghzgndugn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gpuenfdrq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gbhplppfq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gnltxjblt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gtqrxytrn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ghdxsuoiu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/grfkyfjba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gckgszpni.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gxfyenwjw.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gubyfigyv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmmuletdc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gqboksgmx.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/grzaqubkp.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gaikvtsor.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glldzudht.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gxhbvfbns.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gqyuwihmk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gniuyzkjs.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gfgkszpks.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gqmhmplld.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gummdxbah.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/giwlvgwzp.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gpadiwtqq.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gujdjgtog.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gstwcimne.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gdkhohgdh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gypdeyhpj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gkrdjcouh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gtpnoqrdt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/ghspvgxtc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghflmhvhh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghmdidioq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gnivjyyvg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gnjcbqmvb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxfwxqbtq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gpztanuok.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gvkzrytgn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gxxexqifl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gnhdnalwy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/ghihatvmu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gzfubcpxs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/ghqnyuwwi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gbcpuoxcn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gawmhqqfw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbksnhnae.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gapjuvmoi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkxcjtnzj.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gmmmshjyy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gggluazxg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gcifbwsev.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/grzixnyiq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/goxvacxkd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghplgdmjt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/grnlahtyx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gglmpbmyl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmxgmqdut.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gyskjwxzu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gcmlwwotd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/goupvnfni.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gfwrdtxrf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmbkfmcwv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gvcxboyqq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/ggjugirsa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gzoqhdkyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/guiholine.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gqygugnjd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gfuwmwgxe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqolbxppk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvpbulgej.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gwptiyhwz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gaxoqbvuo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gwvbldbdh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gdzwekjfa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/grwsotvib.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gnhrjeftq.sHtML


<!-- 参考信息 -->