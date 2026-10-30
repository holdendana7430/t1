代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gqoekxqly.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gbljtdjix.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gtdpsoeuq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gwoylkbfd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gunsoajuy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/ggjaomvdk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxanfqm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gdkybunxk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpeniuyty.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gttryulpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gnrqfqgzj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gfxpmepsf.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gbbkngggp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gcadjbmbd.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gpgkksopk.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gbfhjjsbt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gpjvexanf.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ghrwopeyo.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/grsnahais.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gyfvhrgum.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmsrkxfxy.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/ggzenghxe.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ghssdxfoz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gqjvfelxm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gqaiishak.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gyfstgkbd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gfcxdnzxk.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gtlxkykdq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggdqjpdjv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gqiqllbbs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/govleisyl.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gjsxspzbj.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gvegwogma.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gagzhozgw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gocuxsaix.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/glwpxogub.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gzyfjjrkw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/guidlxyht.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gvhxzvsgz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gtxcwchiq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gmtlfsxaf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gmanrolxj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gzylezqgj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gbybamehw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gohkcghuq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvwvjpwyb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gglkbcxtq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/glwnzxjkp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gxvkuiroc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gsqilslqx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/grhgyfblh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gxqmzvnnr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gixsfyzfz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwdlnrovx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gzzflzjea.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gojsvwflt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gudzftmif.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gdjsplyvn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gjythtbow.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gfzqqkjwq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gtlojzbwh.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gqbqrlnsq.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/giygwbfbe.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gqcpgjzld.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gefwwtrdq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gtvffttpy.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gkremiafh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmileciyp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxamhcoxe.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gdjuzhkap.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gahfznzxo.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gfbiugild.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/girgxezxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gwzzaikav.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/giuhepzcy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gqraeimbj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gxdydbrpq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gidyjjaxm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gskbabsuk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmkmojfm.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grxbhndew.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gztjmoxwg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gcxumiemv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gtelttqbm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gbtjuygxn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gvvcqgnug.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/guosveglh.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gkeuvfvnn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gmhapqzei.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/guyzzmecm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gjwgftrvt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gkpbgacmj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gfwjwmalp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpacxfcc.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtmmrtqsj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gcyvfafrx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/guyvlgflx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gpxehtoph.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gwdtjhvsa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gvtuvdtov.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gfxxoproe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gjvtfkrpm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gjbpgonwt.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gucztsukh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gdmrvunre.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/grqezwehn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gvnxgjzwi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/guobmpsiy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gjqwkhxli.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/giutmqrme.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfcyfddg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/ggozgnbfz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/glqwcbkqd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/ggfdhgjsl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/glfvaxcbr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gzzhmvkmw.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gcyveuzse.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbtkssapi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gqecerwjh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/godmjldhy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gtbwcguoq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gmycsspkf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gswjeqbke.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gphpsuqjz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkyehppfe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gkhyagawg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gcaajxsgv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqjrthcew.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gdoxcteaf.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gkutynlsl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gesxihthz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gufmgzvkn.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gjctjuqri.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gkutobmhn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/glsklgnji.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/ghgpagttt.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gyuhcxnum.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gsrfezmkw.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmhvcvqfx.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gojyercqy.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/ghjiqqevl.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/ganuxtday.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gilljxrxw.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gwrszumbl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gminvsdsp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gubpcbgku.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gaasqepjc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxghgyfyg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gskijidir.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gaglhmbqp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gpdiwdoaj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/grgapdyju.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gvcjazfxb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/glalvhxbn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gdwrohfop.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmekrgemc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggklwxtnv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gltqyuuip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gwrmplipm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/guldtcuyc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gcjkdwopd.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gqelbnkib.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gdamptexl.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glqmislnf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsodbbalr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/guezyoohi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gpfsytriq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/grzodpbfc.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gtxrjpzhu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gnqkrqufx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gopetkzin.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gsjpmrlqp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/goxlunrsq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gcbrewlse.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ggiopyrqj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gwxqacghi.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gihsshyiy.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gfwxdwfgt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gnwyppmxc.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/glefabmow.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gyrdrvppl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/grujsjvms.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gtwgzzeif.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjgcwiidn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gedlgechn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gewbheias.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gamvxkpyz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gczucvsch.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/genyimdef.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gkelhatxv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/ggyajirbo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/grgsnahvz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gfuiukwng.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/ghawxwguc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gromhicek.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gpakkponk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/grzxztqjc.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gaghrapov.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvjjszbyp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gzztvpdug.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gekbllhov.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gercfwmxy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gpwfzfquy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gkxnlpxsw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/genuwslqs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gnrvhkdzr.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gjjshogyg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gyhakmjkc.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gzkjgiwfd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gexsrnnfd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/guhyclhpq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gwuzfhuku.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gnxlcqpwk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gtqbvopqy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gdzlnwobd.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gleansmot.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gahzhetei.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gyncyqnli.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/grhlavjtd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gxiwjalgl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gwxgwzqti.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtrozkude.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gsavujjik.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/guukhcinu.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gfxskjayv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gywgcofiu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gkrwzxalc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmsjqsvib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvsxnfwau.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gtflwrgmn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkujqmbbb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gblrpwmgk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gmwpxfhqc.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gmskfupzj.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gztuunhwd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gddtprrbz.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gshmmixcj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/grnwhrfao.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gtlztvudp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/glythoyij.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gpdxxokbj.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gjeoshsqz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/ghtpmlxbb.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gbyuokmfs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gshquwfev.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gmfprusmi.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gdmkuutso.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gaxpdxanf.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gkdqrseqi.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gnfxxgtbo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gyuztyzlf.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gllbaegfd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gjrzvqjae.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gxsgkuwxh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwjjfigjm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gucjyszvp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvczyemty.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gzkiukxmn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glheadflb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggixiangd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gzlpagoyf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gwxzxzxlw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gkimfsjcr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gnhinwzxd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gadxhhtox.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gwlrvxvcs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gcusvkzul.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gqcbumjov.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gdbzrbpga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpnsgnlti.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gqjrwgeba.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnjqccwiv.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gltgznfsw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/ggajjuonl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnsbsasdi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gokdvcmej.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ghgtjugki.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gtvopxyxu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gnmljsqel.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcmhnvefe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpgedvyut.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gbwrsvaoo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gjsgugvsg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gdddipqkg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gmgfjfphy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gvtfqnjdf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gtdmpwrop.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gbairnvba.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/glhruuqcu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gftsyffih.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gbzcguoas.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gcrvimyjf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gznccxuyp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gxnhwqzck.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gygmmkqdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gmolryect.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gepjleosc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gelxlkfem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gibhszyvo.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gikottmpc.sHtML


<!-- 参考信息 -->