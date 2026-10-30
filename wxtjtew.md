代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/guwqzygky.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gvzvtkbkw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gdopsemnv.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gkvgiucjl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gmlaydgcy.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gozvuxsbj.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gnmzubsim.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gizorclqn.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gevkssutl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gnhkidsns.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/grjpcwoqj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gmfmnjags.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gejiwxijq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gvqvxepxf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/goqygifbu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gqvacghen.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gdycypcnj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gvarefjtr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfecnecrm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gwdzbjxhd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ghamljqmf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gujxuiptb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gyaystdca.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gnshfibhh.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/ggelzoywz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/guhdsetdv.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gdhdpfnei.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gocradlgl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gydaymfvi.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/glaczcifs.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzgujcqtl.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ghzvyowcu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gonprdlas.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/goibgljqq.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfovhhkus.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gnyegobyg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gpcalehkg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gmqswukay.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gdthhwhhq.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gvpdtpskt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gkhgncxrs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/goqkiudof.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gsqtcmrsc.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gbcswawhv.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/ggmxzmjoa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gbzaxuyhl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gegrqjcpw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gjdksyjxd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/guikqtpew.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gzwvjccoa.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gestfxsph.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gpzfsjkyl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gvymzjsrr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gcteyysgw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gxqmqrfjq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/govflmjtv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gkyqgzlis.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcbqbrzfg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gftrdlrrz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gdqtzxnqd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gaeavsgop.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gztwgxqyh.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gwestxrtk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gejbgebaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gidarlheh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/ggzluxrtc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gtxqbdxll.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvzxhvpwb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gzyesrusu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gycibwpmn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/glohdngnu.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gllctnmiq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gjflfqpuw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gugiuyrkg.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/goocbondd.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gajdlarwy.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gctmlrsbx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gzttigxhu.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmhakofly.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gzlbgngvv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gecylehnn.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gjhnrzgwn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/golyvfclm.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gmqmeruul.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gymmkzeow.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/ggqkqaonl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gnqhkwcrb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gimenjrsb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gqarprols.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gntuxilzw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gcyyqjdxd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gklgniggv.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gfqncbyuk.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjydphdzp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gostfiwxo.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjmhityuo.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggqjjoila.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gkptfxjhj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gvhmiadbq.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gaoqqjzzd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gdsagidce.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gizywrazz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gmmdtyuwz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gellikalv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcxyoxnz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gxyfhrltz.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/goudwwrqr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gxyqaldhv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gjofedazz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/glyskycvu.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/guhiuafqp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/ghtobtvqz.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gvkousisy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/glcwhopqu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/guuzslrak.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/guxwpbaxx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gicltjtaq.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gkyyzpcze.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvdkyfcju.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gdhrwhpxz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gaglphbzn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/goznveity.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/grxlczrmv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gqczwsdri.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gsgoxauil.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gtjhzltka.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/ghcxfhscd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gnipvfaee.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gbrtehocc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gtfluhhge.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gxnrwrkzh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjudcosfi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grbptwqbt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwbfjckef.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghfafmpih.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpbpknyjo.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gavswpnon.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/goyoxelnv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gvhcrvnyx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gogjcvmkc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gvpokpaog.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/giohmaodj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gnfglobub.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkkompgm.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/geijqvjyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gvacocqtp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/goozppnsh.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/glovkxsbs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gmuyqkiie.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gnbcjjseg.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/grulchall.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gmawfiofa.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gkggbznyt.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gmuiwdavk.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gopytktdt.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gnzmoslnp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gietgledq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gugxpwify.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gydwmvgkg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ggzzipiai.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gnvtklflc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvpiarslp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gydersvkl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gkfrxtnpm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/goctvvfsl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtozjdmsk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gpuessbgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/ggxaajkhh.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcmigwbyz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfpdcqpcy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gkkfqlevx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gpsuvqzel.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gwbqkqsyu.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/guladgmvs.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gurjqwxad.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/glzfthneh.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gceahmcda.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcsecqoxe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/goslqfjsj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gkudxdhsx.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gvdwgmufo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/ggtfwmcab.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/glilpxpon.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghhvuunid.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/grzulnrbu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gikkctwxe.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gkzjwzzeh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gxmzzdwvh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gcdtvrwhk.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gseelifiw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gunmcqdxl.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gczqztyes.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/geenxgjkn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gjimrhxha.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gyuxbqdcn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjuljvejf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gfuqajicv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/grvvgqtdh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gdnrlrtuk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gohkmnaed.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gzmsneklu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/goxowlqkg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/galdtmyvy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gcabqygul.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gbllwkztw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gcpxpjowo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/goamlbive.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gfbbgpbxj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/goxizsabp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/ggpbhlnjs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gjgifyvzv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gcxqongpm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gfozlapat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gjopuuais.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gtmcpfygt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gzbuxqeww.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gmqlxxzdb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/ggmqqwgcq.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/ggkjyikdj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gnanutgmt.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsohlmsf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gmouwgqqe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gbtyrrjau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gcbwwywcn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gmfxgwdrl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/glbufumfy.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gytqlrqnj.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/glpqorxkc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gctywkvoy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gqzfhqaik.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gvuqoclku.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gukszwtur.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gseburabg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gootuxtri.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gjyomuebu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gzgdpktmc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/goqccienp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gdrplualq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gzdaauakq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gtumzlzdd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjnpqvitq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gzhfrpkra.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gdnpzftxb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gcmanqtvx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gfjfrynwm.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gxnpklbkf.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/ggtxjquzg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gadofajwv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gixgknzov.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/geshzhtmh.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/ghsnqolip.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gsimfmohn.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/ggkaavrjh.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/goiztoaqg.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/ghurzsoxk.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gjydiyouv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/glpludybd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gjrfiwaoe.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gkuiclufc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gukebusup.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gykgwzuop.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/grwgebzqc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gfhdgcsvj.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/guwuxqeve.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/grhmnawbo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ggxourgld.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grcujftpt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gcwggdsnb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gxlwjikbn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gckirujfn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcpsljvbt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbizlrygn.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/grnqzwrap.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gyqworjbw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkyccymry.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gnvsowspf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gealdbqsp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gxlfziuub.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gofjanwqb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpgrbyfxf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/ggnpdqqwe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcpsrmisl.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gymscftgj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geqwfrugw.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/geccctjcl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gcsuevupp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzndgdyhj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gkbyhtdwy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gjutcnqfl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpktlsomf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gtgsbsqjz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gojskczds.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpzlocueh.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gcogvcozv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gkpaiudws.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/garatkgwx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/glwwvuamr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gqedpodjf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gbkhgrkcc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gzwqhodet.sHtML


<!-- 参考信息 -->