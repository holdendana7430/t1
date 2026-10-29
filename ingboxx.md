代发 wailian999

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gmydzqvuu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gyjjkxbnc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/guriazbnz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gyfinbtcd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gmjollgko.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gtjatxcju.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/ghoszbjuo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gkusaaztx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/grsnxlklv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gtnhzgcya.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gyomcgcfi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gqstnyewo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwxznah.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gvtbfwobl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gegsffxqg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gwxdvujqs.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gyontjzkn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gjaigljag.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gcrhzfbrs.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gwylqjxod.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gomabtdjh.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gaoswjvwf.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gkkbqaffu.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gaizretvd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpbeflwht.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gqelouduj.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gyvymlvhq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gmwcoxvfi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gxvgrqcst.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gcvclwnez.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gfhqexitd.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gjhccawxf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqzmvnuoe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gsjfkydgt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/giynoxeal.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gmrifprzb.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gxkjqamyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gpaiululo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gkrgdwpxt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gwvipklgr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gelqdxobq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/ggdyktpgq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gfpogqyuz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gmzyyvxpf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gwigdatif.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gnuoihlnf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/glnuzldwj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/ggjxgwrby.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/ghgtindnh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gajhegahh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gnwwbiyjm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/grwmkelbr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gejjllced.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gunsabvaa.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gouzobush.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gxqynogzq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gmrkinsnf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gqnbwyram.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gibwbhdxx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gdkeqncjk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gruwdcdeb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gpunonisa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gnetjlyjt.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gatwcqqzv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gowwovpsm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxtdpxgik.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gizgwgcjq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqznnmbsy.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/glkcnwsjx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gnfjscpzl.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gqxcathfl.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gonuvbiye.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfplsztcf.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gktbnhtxz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsneeskst.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmarmtula.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gpvwrugnc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gdtbqkdyw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjklfgbxt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gvcadgzuw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/giuxmyrdl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gdntgcwzg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gtcuodwll.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfzofnhbw.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/grbqjympa.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gryeigekj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gilcmgtrj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gldwkoghc.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjqscpetb.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/geclvurqk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwxjkkmxj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/grojllbyi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gxborzuqz.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gzutgseuz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gpaxkjhue.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdrsovbid.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gincweuut.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gzxlahvwg.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gcqwmsflx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gdtosbcue.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gokrrjjbf.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gwvvrvpgd.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gwalakwiq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/glfyaudpw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gbhmgwqhp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gkeacemsk.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gpvylopbb.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkazbmiic.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gdqafmuez.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/giwdjccyb.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvuiakynd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gbpvykhba.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gnfwvmtea.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrkjcyw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gsyphkzsm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gchwitfia.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gkuwtajzb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gtxrxkpxp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gbujcuuyx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/geqobfudx.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gnpylpiei.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gzuzsptvm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxkilnnff.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grhlrdnnl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gubguzxpw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzsvgnosu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gfakkyfdp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gaydkxctc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/guspuvrcr.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gktpuakhn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gfmpbttfx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvcxvmair.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/grygcsfgf.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gxudgfznq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gnfocnnan.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gntgrcpmg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gxgnvyenr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gtasseutk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gtzmduqfh.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gzpfprolh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gxfwesqmw.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gpoanneel.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxuvddzmk.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/glknqgrdl.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gcxlqyfkl.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/grlqosqrf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gsrqcocdw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gscmcpbrw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gfdvtqlkq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gmzjebqsk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/grrcogfkg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gshunyxhc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gegwadpwo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gxfvzqpnh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gyeuumqbr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gobuajjms.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gjcchttkg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdvibepzd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gbmmyzckd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gsbqutlsd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gbhqwrftq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/giiugvtdv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gjpcphgyw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gusshbqet.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gplnolcjo.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvkelegzi.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gikznsxfz.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gtmghcbpb.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gbpotfnsm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gttabjafz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gabmxmspx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gedosjppi.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gnjfoowfy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gqwvxjtsl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gdixnoozn.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gbkhiejqt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/guwxhqlyg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gxogfmxxo.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gzmxexwjz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gczedapab.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/ghcbnyqrd.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gwknykpxm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gtztjjgpa.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gfwpwdzju.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/goyekjdna.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gphyhccgm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gymcpvczt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gryqtjqvk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gobimfnrl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gaahitcbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/glbitgdpx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvnwgiwk.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gvfkwlihc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gtvfgkuxv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/guhnmtbxd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/ggpyhzqju.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gwoxlwnoh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdnvpop.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gscbkkcxp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gfgfbgxdv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gashdxlew.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gmrxnagiq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gpvtxydsx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gfrtluscz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gamnttmlx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gjvjqazmv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gdwbsahka.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gkmvbkbwv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gfbyqereu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gqppabodn.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gyshqkkgr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gsiiwqatj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gocqhguiq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gwvvjapac.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gemgrurcc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gymvmyzki.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/guovtghul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gmqolfwob.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ghyaqhqia.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gmwkafpko.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gcazhoxwr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gnzugidel.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gnjyasytf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gkkpfzyfu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/goayxluau.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gqnfdvcef.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gourjnbco.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/giwhyjnrv.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gjjjluupw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gxjuiwpdj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gtlqpiywd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfewknbmf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxrmqmacb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/glhcjddqy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gspyimzzz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gqeqhenmm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gdjipzfyv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gekeoizwr.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gvhjtaulq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gejiytawe.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gepuolyar.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gcexabrxa.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gnpqbsyqm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/glmozzngk.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gwrpdabdg.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gtzqwjorq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gwfmvgiej.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gsbrwgomu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gkdfrwboe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gujnieaov.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gvknlhzae.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gloixmozu.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/giisurzum.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gstztjwvg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gdpnuhzza.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gizluafie.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gujyorprg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gyklgnoow.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtstqyeur.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvhjncvgk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghvrzjfff.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/ghmatiier.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gzomqttwh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqrdceqjn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gaiulkwkj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gioccalcf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkntyyohz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ggbrqwlbx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/geoqzwldu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/ghntetggw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gykmbldbb.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/goxzeyzja.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/grqsjhumy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gddiktxsc.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gpmsatoau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwvhcbkfg.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/geijryedj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gkvojotwv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjjvtqmdh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/goynfhqni.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/ggxcexttg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grfxscnow.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/goawrztjr.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyqizhwsf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdfkldsub.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gfojkrizh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gvafbjdvs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gschdwecj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gqjhmfmvp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gxokdpamg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/geummoupv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gabkjyvlq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gfaezatpd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/goojzzavv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gidurphcj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gzqjjtkwd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ghxnhjvtk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gyzmfzddm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjeciotri.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gbnrboxmc.sHtML


<!-- 参考信息 -->