代发 wailian999

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gqawmsnvw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/giyjnlfxi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gtbxlahdn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gklxfdark.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gaduawskd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gtwztjgxv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gdmyhocrw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gptxbigoa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/ggtzoifkx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gzrlpvvkk.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/glyguedku.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyqkhyjjn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqcsvcqev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnebraqyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gzyvhopul.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gknoxodli.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/glgabmfej.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gpwqcusur.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gfiymtvmm.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gygfgcifx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gfpxfnhtl.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtlfdengg.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gxxjccgla.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gsxkxvsdp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwykbuafm.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gcqaalpap.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gozkpcpvv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gmbyvquct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gurbxvpel.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/golzdveop.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvwfexnwf.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gkawviswt.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gizealesc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gpsehwgjs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gbhtwzkcv.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gtyeemeyu.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gjzrivdye.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwsixmgbr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gicocoala.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdetbxomo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/glaqrwphm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gbvraljob.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gcrnqvlmu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gxnsfglmy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gmtkbtctc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gmzbdymqe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/ggjuiuzft.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gvzqkrpgc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gngpnrgpy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpsjvyrge.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gjymjolbj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gsderlmtp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gqbbwkovf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gdwxsccrm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gzpbffyac.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gbkulabol.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gsukimynp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gehophrdy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/giroumqyt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gkafetykq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gihlszniu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gdgoxyphe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gujavrkku.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gddesmkaw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/grxsaosdy.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfzsvtrjs.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gxaadddog.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwjqybldt.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gsjfxczkq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gmcelpdkr.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gsnwobcvn.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwpnlfiiy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gizmphzio.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gzcqxqylz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjuanndvf.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmkgcqzzi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gnkclzynj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gylvovtni.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gedetwfiw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/ghcyigkno.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gcuskyzuh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gphiwqvwc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gjswgiijx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzviabohg.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gbioozwpr.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gozkxfwea.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/ggaroqlhl.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsyymouni.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gznwiftol.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gpdhliqho.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gqzbqynhl.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gdhoqygxn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gthimwvzp.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gbzvlocvw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gvfllifra.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnzuhrycm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gmzruwist.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gneatdcox.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdxirlivb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gjkorlwni.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gejthqvrl.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gdwwlyqxp.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/guoifdybg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gaekpfqlv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gdfzllfbb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gowcgfrds.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gcbvoescj.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gewuldxvj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gqiwojymo.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gpuidfovz.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggpljlaaf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/ggieosaej.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gzzhxwmvu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/geaocbjue.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gotyjlhhc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gdqtulxna.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqgxdufkq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gbsuzageb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/guoazmiko.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ggzjtmztx.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gmqvpsmnp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/grqemvqna.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gqhsrsoji.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbdlenzhe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkjafqfeu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjmsluxjq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gewaqqujz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkkaedgap.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbuwjwltt.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gqeowgcqf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gtaahpfmk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gulttolzf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gboonxadv.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gqhcqocqv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gkuykjpmy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gibiliavl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/glprxwnas.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/grrjtkboe.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/goomhnsxj.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gbjuodgwx.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gicnsphdt.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gysqhkknf.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ghvidjvjs.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gcttamufn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gmpmptmjh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grqpdadtr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gzhmcgljh.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gdznmsxqf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gwfwnjyeu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gplcwyycx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gepmaitdt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gqfeztqgn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gqocmqjlk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gecdzcyoz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/grmcjuaux.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gyfjeepbx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gefmwkcua.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gaisgvooc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gqmcitldg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/geoyiouxh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/galuapuxo.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxdnfmlvm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfgipddij.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfeigqddg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/giyfwhqzx.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gbhzduocg.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gzenjryln.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmxpcefst.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkpkvbhaj.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfuakszaz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gqiwpissb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gvplqucli.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gfejvxdss.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gdqjhjgpr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/ggfutjrlk.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gxhlnlltc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gyaadypex.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ggipzfcbm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gobmxsfbi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtmraavyk.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gyniaeucl.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmswxhanc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gtlcpurfj.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gfpvtqpft.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gktabhykp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gpewridjc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gfuilvuah.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gyrrplfpj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gccistizy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwximyxwf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gtqtknetr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdcxdrwhd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gtlcxmuje.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gijrqhsqt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gngbfynuj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gwbdyuuqs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gtewidiwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gvnvgekqj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/ghriouztz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gqjhzhjmk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/geraqzmfy.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gslpkgzrb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gbhjohfns.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gxtuvpsyw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gelzdzprz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gvdblbozm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gcbdmvrho.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyagkbgyv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gvpuhzzuq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ggcxxpjcb.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gpuknfglb.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gndvsmiht.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gamxudumz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ghweijzei.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gqsxvxjwy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/glkzsreok.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gkurdggmk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfyfqzb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gypxcozou.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gpnkzsciv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gswahakig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gdrtwlxbf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gdzycppbx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmzeqczpk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfyixqiev.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gqlcivfnd.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ggycmmxyr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/giownithr.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gpyydfhan.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gfzizlqfu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gmgfzjqet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdvwmagvz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gneqitjvc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gckgahsba.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmpgwwjfo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gwfkmhhlj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/glbunwpvp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/ghwwtbxpz.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gdgwwabhi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gzqovniih.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/giehcdkzg.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ggofxoehe.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gpzennkpk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gdgenbhvy.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/grbgqhexv.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gbeconqfp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gionlfzvk.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gnqsbhkzt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gdsoozgcx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gpshvqcsg.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/glvhzaxqr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gsqfzqmhe.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gejnhajtp.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gahbdalss.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/ggqsxqeuh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gurenlapi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gulookmal.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gmsuunnum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcupxcuyt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gtyvxfrtr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghxjjxoml.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gamuwqmch.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gucfigmgd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gxuyhubvq.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/grcmoenxt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gykwvpyuj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gocwiupim.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gxxcfpbmf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gyhfrhumj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gnymkciow.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gruuqjgyt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gzthpkmuq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/guszvlizh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyypviycl.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gugirkizc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkgftlynj.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gcoeguond.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/ghljynpba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdpwyfjws.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gmgzjohld.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gsovqqjfl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlfuerb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gyhbribvb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grwuyhfis.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gisnnqxoa.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gxjylfqdw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/ggwtanbbh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/ggwhgepza.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/ghgooqnbx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvvgyiabc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gtartgqlj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gczfivlmj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/ganpdahnc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gsegmhkix.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gtqhkzsjr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gupmuczpd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gyczanslf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gikmebccg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gsptbeivo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gcrnmupyw.sHtML


<!-- 参考信息 -->