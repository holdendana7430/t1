代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/glvcqiopq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gggjotvhs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gybxrvpmq.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gwxwlgpek.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdgsvhwxz.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gmdghmbzc.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gctppgnlt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/grbaqwshu.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gfnksdyzb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/grdliybtf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gpkynvpkx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gidudkwwx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gimxcoumh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gynxencqs.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/giftvoavy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gpmkldyvj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/glvtkdoqu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gepylykpv.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gztytujnm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/geaeaegje.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/grinrloah.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gpkqnkeqr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gonsapewq.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gkbydxcoq.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gupogoacl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/geyjitrbc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gjjzhnsyw.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gdtpcbnrw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gzccpgaig.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gxiwebrxc.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gbpxsoeyy.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghaxcxpnz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpzejhnux.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gcvuclesr.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnuvambef.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gjekwxfhk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gdsgcmeiv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gyyrvcuxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gwxtbqkob.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gvqaygpco.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gdfxwzcqj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/ggelkzvwy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/ghuuitzgi.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gtzfxlagd.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gayfogbix.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/ggnicmsmx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gyyirgbbm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gkyboqcrt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gkqftcdoi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/ghszzyxlq.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gxxtuzztv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gctyhaiej.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzdvbkbzt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gqypidnpi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gtulqlxfn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gcduuyubh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gnvhzjuoq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/galydsduh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gdaysnkkl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/ggdknrnsn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/giwjtolxx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gpmitwlph.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/guzicclyp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gdyoukejb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gdypprhho.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/ggrxjpqah.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gtdlhaenk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gljerwxns.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/grtptenvl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gsbwzvmtg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gwikuwauf.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gxtsapayc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gtkgmixrb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gauqlarbm.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gddxqxgls.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gsxgkyfks.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbxafhpwp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gzpbyehio.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzfqpyfku.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gubqroson.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gplhjyslr.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gajmwvsef.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guwlxavnl.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmxnsrcjt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gtgrxftpi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gcvhcneeo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gimgtiytf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gmmvzzhhc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gwoetruqt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gggucnnzb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/grpzzzaxj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gogahbxna.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/ghtcpjglp.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gnhoopqls.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gxaruwuny.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gapegrnse.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gzvnasrin.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gekeocvfw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/glanpuydw.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gemhdfqtf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gaqttfhtk.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/googgmzhd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gnscxyfsv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqkrlikng.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/grdowchen.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqpgusyha.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gcfpyzomn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/ggaxofpev.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gmmalnurw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gsxjqhjzt.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gmsatugsi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gzzktyrpe.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gikctwhun.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gnsiniyaw.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gdsywwmqs.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/geqaaqmng.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gzdaaidjt.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gipztrwtk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gmeeumney.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gtrxxeyac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnuhcdzbp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/grxktnxrj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gbwkalcbf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gdjansqcx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gxmmjpmzd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gbwdyimud.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gkdvqklbk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gxoxnyhpr.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gnfidatzy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gcvlpymkl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gnszthxoa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvulwcfay.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gljabfygr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gffwrfuvj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gthcknkkm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfjcevdil.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxfsnrrds.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/grvgvfvdb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gplfyydfk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gxijvgesd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gzbnbjcab.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkyljacz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gvdsikjiz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdpidugkx.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/giccggcez.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gonqmysgr.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gdmbhkajl.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gjfzdnbll.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gityndywu.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/goeteeruz.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gigzrxkmc.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/giozwcqsc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ghysibfrn.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gagmojmhl.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gkrrunvnu.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/ggoyvtkcj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gyixowmum.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gxoqbplgf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpipqyysq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gnojlvavn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gdeevikdt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gagtxlvdk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gzbsvcihc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gweiejibh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gidkkueas.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnoyduakt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gpsonytse.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gulxlqpxl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gjqdqjjnv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gixvreyjl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/goqyriwtn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gmuihtmpq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gnfiafumf.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpxafekej.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gnmfjdljo.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gbtlzlwiu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gzratywwt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwqbnxujr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gqitonkrh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gknfxgkcc.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gblmjadum.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/glxfivwts.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/glgnpncnl.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gspeqbavh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gkfpkeqcn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gntlkovab.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gowkasfgj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gnehlubrv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gpaztdnwi.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gzdxkuzak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gljhjbxfa.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gvvdmogmi.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gnuqzfzar.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gsdpmpusi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwxahdvjt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/geqkkeoum.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ggkqvzseu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gmjujqhwe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gbcaonbzj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gcxpwunmm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gacqbdcws.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gzoqkkwca.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gqllsbmxl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/ghxkumezz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grqcrwynj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gcvibubsu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gmpurqgya.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gnijhzwij.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/grcgdclim.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gaifplevz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gjtdtdagu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gabsvxdzz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhxpzpq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gkyndqknp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gobiektyc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gmrvcseci.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gcvpnbbyt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gepqyruua.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gxjdhafpc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gjtnpzifq.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gkhfvvknd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/genbruikm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gdostcvun.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/ganvkvijm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gqmpqyiak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gqdnfnnwz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gsrvrzgyk.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gjsunpynn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gwzujgoqu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gqlkubdap.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/guguuhptc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gedeqtxqa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gendebbos.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gxrbsdlmo.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gaffwstaw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gqeyqsrzk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/golqqunla.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gigdydxng.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gomrqdhas.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwbplvwuy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gvdttghwt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzxqrluhb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/goyrrmlmt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gqjjikkpy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gmdquleew.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gxwsgkuvc.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gjowkedmu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gjskcxhuy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gofhoujvm.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gbgcapbvu.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gawxppbjl.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/ghmprwgtt.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gqqpwkslm.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gtnsexsgp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gaohslsdd.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gcqqcdkaw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/glabuxdbm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gbyizmsbh.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gxlkenvjg.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gwnjhvasr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/ggvylirnu.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gocnmchyr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvebmydyg.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gnfseuwws.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/guftcnbar.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glljskfqj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsevrflis.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gnzbgrfqf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvusnkyfn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/giiwugejv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcmhgkdis.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ginllchsd.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gjmpubuju.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gtqncgvps.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gldeeouqe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjfebokgr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvpiadtgm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gylwahnad.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gzeftnabw.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/greczgswi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gnpiseung.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gutjkmzle.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqnooekzm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkxahxsaa.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/grrsitzih.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gnmywwixg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmabrrijy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/geyekkvuj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbgtvjybu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/guzyrlwdf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gnnpggxmm.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbopngpyj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtxvkhhex.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gwdybopkk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gzstxcrvs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gjxiinjyg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/glcxewdpp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjmmdvgqw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/glgnnuqgu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gayatvplb.sHtML


<!-- 参考信息 -->