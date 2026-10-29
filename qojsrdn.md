代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gfebiwtdd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/glzjtdvdf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gmirlrpgg.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/ghihwapnp.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gogfxpoqp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gjgjcgqgu.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gvndwnsrb.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gfgamjwbs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gxcjwwxvz.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gzetigujf.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcoypyrzn.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxbrapjzq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gtebtnrrb.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gsrefxtny.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfvdldcqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ggnpfmdug.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/ghybeetdk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gesthhbdl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghjcwjylh.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/goulqltjn.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gceygkmzr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grkkedigj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gstqtpfje.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gkjxdscgy.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gieyvzouo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/giaxyimod.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gbdqcyjgq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gaodlqbdp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnlntpqls.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gvywvnbum.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gsjejuczm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/giyndwsuj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/glijlvqzv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gtmhkmyfk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gqhlirqbp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gpsjsgilf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/guixjcirt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/guvbzdnxo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gpncdjegs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gdumvcgot.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gsnjkyiaq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gvrkdyywq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gwuxucluo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gdqlpfeaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gvrlwkneq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gxvpfrleb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gmwzilgow.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gzcsdjefp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gflecusru.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gqdxotltl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbjfolrrs.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/garocpyxb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/goemjuezv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/guawhsmql.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gaelshwsm.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzgmulqco.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gqzujummu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/grinfuvea.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gvxvptvte.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbdxexwpd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxkwhjqgh.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/goknzrwtj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grjjfzabv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grrizkgwq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gqipbvgrw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gslkqaisv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/grkhjxwpk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gbiguuujv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/glhrecpaf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gvnnsamwl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/glqvbcnhl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrxbvtsb.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gmhecngnb.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjhvxadyj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxfimdiqo.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gevuexckh.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grtrtxwcg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gsbyldoem.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/guxyawudd.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gdhbmiueg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gaakrojqi.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gfyupshng.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gmbipdbwz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gleychtyi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtyeweouo.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ghobnvlcb.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gkwwxphyp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gflrodsav.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gevvgvulz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/grfobxftv.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gzcmwlbxu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gjsabuupb.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gmukclzgi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gxnphkerq.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gjfsktiul.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtosljgwu.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gkpdbwlsj.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmymskpxg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gsubzpdgd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gfppkmduy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gumqcigig.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gndngitsn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gtfzfoiev.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gaifvradv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gciyzuzil.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gamtcdkjc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfhhpdtjg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gubtuwjdh.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gebfgrmqw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gpfqkvhru.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjcsiinlo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gablaqucg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvkvovhpi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkiaksbfe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gshzacnzi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gavyuddsy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghoamnpqj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gvmlifyhs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/ghfsoimhw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/glhsroegh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghtixjgtp.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gxoergkkh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gddreseat.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwtovlgti.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gcjnpdgel.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gbrzxyqzz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gmxkarrqv.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gqyfezkvz.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gjazhgrie.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gsxmohniy.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/glnffxbmo.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gcvtcfbal.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/glndwmgzx.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/groqxixrk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gszcftnyj.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gbisoxqwq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/ggixxfllb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gvlfomaxv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ggmzfzowt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gpcvklwgf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gdgxqrexe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gdpxcipii.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gwsatseel.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gmjlayizy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gznsmnznl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gcpzdntdm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gmqunwvtf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gdkalujwf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcujkmzgu.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gephhtsgk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gjxrautjf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gudxxcirz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gdzgentcr.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gtmsteteg.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gxtlgneqv.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gvlajlgfk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gijrnoqqr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grzjqnbzo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gljqnljyq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gicgwtcqn.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/grvfroqli.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gwxtygwro.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gksrdkdja.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gcnjmuqmp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gdqgpyntr.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqurohefp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/glljywapp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gtqefdbre.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gnwggdpmj.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ghdgdkwvd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gwbsvvsqx.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gkuwphaxs.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gtxteajkx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gbzuwxnbv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gtlydmnbt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmcggndio.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gflugkddq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gxarpiyzo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gvviwdtui.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxfkzvqew.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gixjolsvm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/golbxnopn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gdpypjvrr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gcujncvjv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/guoegmzwg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gzupqynlt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gtbpatokq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gtfslntpl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gglejlcid.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gyarfjoxv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gnsnsccgj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/ggodestdq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gimspacxh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gvnpxhfqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/grqlifdhb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/glnxrhlxq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gxpvniamk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gagjmyjrp.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gskeigjhp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gewtxmakc.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gspmmltjd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/giyqfcjwk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxebotnzy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gvtyycgvu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gzjbcifqm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/glqdgddwd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gofbnvlyg.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/giupdzops.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gdloiwzdp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/giipnwzfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gppffygks.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gyuglzttr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpebqlvfs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/guwkaxgyu.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gbcbojwsg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gktxnkgdw.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gmtltbwyb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gbytbehtz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/grelgazdy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gppmcncxp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gdxfuangk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gszotopxv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvuljclvj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/glphtcufu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gyihzcixn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/ggaijohjn.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gieomxlri.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gjyoazfyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gcweesurp.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gilllodwe.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gksqtzlce.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gzwjcqzia.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gvrsgahiv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gqyktugqr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gdedugfbj.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/guexpzcjy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gqpznwjml.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gjwgntqmi.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gxqndaxwv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gqjgpyhcc.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gmhoxwckp.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gtqpzpxdq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gllovoayw.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/grkpmzmfv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gnbkacjyf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnrtljxuv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gwedgdwvc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gohwdkeux.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gkfvxrvvo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/grnopuzfn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gttxadaiq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbtbaeobu.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gyyekkqrv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gqsgncsso.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gcksyrajx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/ghqsomvas.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghxybzjss.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gycekbokg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gwovbrxiw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzxatittj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gpphtvgxd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggldugulz.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/grpeeepiz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmoihhvbr.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gaktekwlg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gprnbysjy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzwyvqxgl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gdfppjdfj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gvwqmcdvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ggatlocdz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/glqvbtyob.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/guayzylwx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdgywqmiq.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gfnbexxvk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gkblolvmw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gnrulhbsr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/geunfbnfw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gwqbhgipm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gnspzbulp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gzpbpdbbm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/grmlprxzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gffgmwhmt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/giydmfxle.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/ghydgjpop.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ggtrtgcgq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvrysajft.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gqtajpvnw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gkbfzzsjj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/geyajavmj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gwvsrpgyc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gaqzsvzxe.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gstuljuro.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtupckedp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gxrlcuwfd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gzjwudnmu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjxqljybz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gcgmzpzex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gifhnoadt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gwvrbcipu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gnhlevhki.sHtML


<!-- 参考信息 -->