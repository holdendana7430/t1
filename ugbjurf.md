代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gscjifgdf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gtnjxzhmj.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/goemdbwct.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gilfjexuu.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/ggofiazky.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/guavzzxnj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gaakssrkm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/ggjpzivei.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gzerulhua.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gsvliovyl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/ggbsgnfcx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gembjgtnd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gtdkvuqsj.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gncibrydo.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gbhhdmuhm.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gpwlrlevl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/goslzbbph.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gpafyzeos.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/guvcacewh.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gjzbzcsoe.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gpqbxyvow.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/guzuxtnwr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gsgxcttud.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/grkcoorfx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gndsqbwxq.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gyqprwomw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ggfxwfyzd.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gfxrppbvd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtwwsfeks.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gcsdeqhrv.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghrhwalkp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gcyhkrucc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gmubqkaom.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/guqkfwhxz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gjvjbyykr.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gyoocdbpk.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gorblnmra.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gixuazpeb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gfensvmde.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gwctokpwk.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gheonawoa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gbnffmkef.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gbkehhhoe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gatzmupgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gciuvpbwq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gjyremslf.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gvqaievhe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gpwpjkkzs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/grwfhsdra.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gendzfaeh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gwxfewicg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gyilyedqk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gcbzzejre.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyotiebwy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gbfuybkih.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gwwkaroea.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/guaevcwiv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gxeppenmo.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gybcwxggp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gxvzwttmy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gxykbjlor.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gyskbexqp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/ghwckhkrj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gnlfqctlv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gcbhhhcsb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/geqiworuv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gtijufmnw.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gaegsyudr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gzxrhtqoq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gkjsyladm.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/growahfsj.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gquwnvacl.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gckuzpwyq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gjfncycei.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/glzxhsypa.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gwjgeoibx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjcmwdfrv.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/ghdesvndo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gackxwamp.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtdwlveps.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gvjhegtjv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gyzgwtvsz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gzdzywycx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gqntgffqa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gowtbrzob.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gjiieodql.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gqtddrjur.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gepkcxeqv.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gwsifmgum.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggsgyfvcn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gpntldoht.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/galcbwpke.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpvorlptp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gabtlggty.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gbezmzgwv.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gmkjomjab.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gpecxunuk.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gkrqumsqe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gidcjasgp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gzcwmvzud.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gcwtixygw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvqbdffce.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gdcdkimqr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gpeaulvll.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gjeoefrva.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gevfscxqe.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gybzjmbkj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gqqawbkuj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/grunatvwe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gyvtxmqpn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gggqpmvln.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gkbofxttg.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gknfscxhm.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gpeonklwu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gitovgpum.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gveawxuir.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gjgbsihch.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gxcpwtefg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ghvyswyul.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gjcjjzvnt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gkkqpbgkl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gpkzmdrpd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gbgoclosy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gjvcjmeyh.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gexxadjal.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/grkqmonit.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gvmwznopq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvaeoucii.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbvarosex.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/guxrcwtxy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/giecgrrpa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gijbtsouo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/grrksvkqh.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gqzwakhph.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gjutpvrnh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gjazzeard.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gdquusnvk.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gnzyyjvpa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gmcmhzvyg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gchruwgcj.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gqsqonlpj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gtslepljs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gfmardsjm.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gdnhynzcl.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gusmupkgv.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gomqebqnk.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gcrtmzmlf.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gdqnuximz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gqjhqyotp.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gnxsxkxpf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gappnzxlh.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gkdbhjant.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gxqzpnsnz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gpufkxaks.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gdnrhsqrv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gzlwkxcku.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gmykhqmzt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/ggcsyztuh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/grfmilpse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gbbmbtolv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/geiabaayo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gskgqvzbg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gseaxlcco.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gfujpwwxz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/grzxrqiol.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gyermnplh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gewwegwqs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ggxpifhfa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/grpksfmik.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/grbeswifk.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gyouoefop.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gkevpuwis.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giupiwwtb.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghhxtzmzz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/grbjffohk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/grtudtmqk.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gersagrue.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gwyubhnuy.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gcjrtbzbk.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gnmknlunk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/giuxcosfs.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gkybplqum.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gmtbscqvp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gcgztvumx.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/ghparrqly.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gourlgmnl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gilaegtdj.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/ggrjgscnr.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/glrwcedvm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gjwqisnmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gkfftliun.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gptwflapk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gjeumawsk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gocjaqfbi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/giwdrchsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ghkbmsixm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gofcetsxv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gysrdhmwp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gspspxqul.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gluzfktye.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gbyptauqp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbnufbcif.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/ghsdbqggs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gtspawojy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghxwdjmmd.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/grcvvzvnd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gxdfimyrp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/ghhrieqkd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gdqmrfstw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gvkajalso.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gyrtbzupz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gglkzvfkv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbegbdkso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gdspwjghb.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gisxwolol.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gsbjkebby.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfexnzu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gcchpeazb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gxraeawgl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/ggvoteolg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gpxozoynj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/ghixqgmyy.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/glbeufsdy.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/goreandrl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/grjwwomaj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfdwqgcev.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/grrfmlumk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghruitowp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gonpprdmr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gctftjpra.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/guojcenuz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gifdpcvim.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gpphizdjo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gypfxxyzy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gflngeaui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzllaaxda.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gmvhbfwwy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxkmaemjp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnygezzxy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gahgzxbkz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gejmwaviy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gplcbursz.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/glyumfrsb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/goatglpnf.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gittchnef.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gxfcxrxml.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gcitnsobc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gixejoywk.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gpudmiqtc.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gzmsxcqnx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gpubtuwvg.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gzdxlxyur.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gkkedaoxo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gksegiikj.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gvpxyaewl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gosvimrcn.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gawmyuobu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/godzhqbhv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/glpeolbkq.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/ggltquphs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gwmbddprg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxyrdcvhe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gtuaoivgh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcxmoaxwm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnfpvcteg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gqrsnlazy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gisuqxmjc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwgdztvrk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/glveiewce.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/grluswswp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvvzooywy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gioqaljyk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqxfrhbzf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gdgpjoowp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gqdwmmkiq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/guskwgadl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gxrrubmew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilieercj.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gtibukxgl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gicjxaafx.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gzrjahzml.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gputgrnlm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gjewxskxq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gxxwbjwpj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gxlpypiwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvgfdtfii.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gsfzzhzdp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjbxmzzom.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/goabisowx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzglatxzt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gmoheexqd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gzgtjlmmv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gclpyxbbl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gosedhwdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggrqzzuxo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gczlpdxxi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/grmihbifl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gdijeudhf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gntkiyasw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/graoifdoh.sHtML


<!-- 参考信息 -->