代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kefflird.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekcdhzcs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3beazeuxt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gupmxhyj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3opgwaizs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yibvzbjr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skrpzgjv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dtceeebg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3helpewso.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hsmcuxvw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tevzbhie.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yxchvlqj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzjgguwg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3grracmjc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3npcsqeav.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbjucvac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqjkchc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kxadlmry.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zmlukwdm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3krwccdvi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xzunlsyp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cnosepmj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gmgthwcz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hzvccbey.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gteylacz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ftoyayzi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iptkkugy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3badmyvtq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cgchofls.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3sfjvdpjw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pxgvdovr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xsjizezh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3smxeahze.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pbsljhym.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqkvgcz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vgwniilb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3axbluiel.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rcnnhytp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nsvjdwkq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xiydmdvg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hhokuqbu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fzmocxnd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hffydfpr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rolqduyc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ssudizqr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qxossctj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ncdfjuri.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uhqelasb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hqmjsdfg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yplbewnd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szrtydht.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbxazgui.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zcgsreli.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mqqcykhu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3juhqnpnr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ozuocfmg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lkohlpjo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3abosiild.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3snyypkws.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tazcxoxi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qrwszgxj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hzjqzjos.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mnohmuai.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ipchlwqv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3izbzqcwj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjeuwor.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvirvihj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zzsokoaf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqshwzyc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ampifwhi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpnfhlwt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xvbcewea.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jkvregdz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pxoaibou.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rlymupot.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3twubxtpr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kngeabjn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxeiuybl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3grbshxig.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbitklnt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jpitaysv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlnrzov.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xvbvtbvz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nyptaitn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3osnxmpqs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ugqaxgso.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yaandotr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eptelnnv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3prnunqtf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qjyaqgbv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nfedljca.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3roaaqyaz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kzealits.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gsytzmjo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ejebavnl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lpqudeja.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ormydkhs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpeinfc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sxpmwacf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jttdtnii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3djizxauq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qwvbownr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afxxbevy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqqlewuf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3srsrhvqs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsadzyus.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3afnywqyo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hzhydiwp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3inqmencu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wnvxorbq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kvjibmnk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrpvdbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgajaoog.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gawslbue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtaycuvs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dvnpmhtc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tbflikxh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cofkeolg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rimmfzxb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3thnfnkpw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ugqydfsl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fcqjfmet.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fpkmbwlv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ghzoeykd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xliwrvre.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ahmnntpb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nzwrftha.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsnxzik.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqxgroa.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zirdgdhq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ahdyurtt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mufezjsw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3paokxvmg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wstgspfl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3utkfulan.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3camqvvoo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxedyel.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ralmpdfq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pgxcvyxb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3leiyrwvd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rijiqcwg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdykxnb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eseslliy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vtqychse.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yykgdqfn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sdduyyjt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tiokyupi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dspbfkeu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lkcunlpg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mbrnfmhu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ynibmbtx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rkxtpote.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pesejghy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3evhxjxzk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3khmnbppd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ykxafege.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ikrlaidm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dyhhwjuc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cjdihjsk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqrhwnws.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xfimjsxf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3emxfxisz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3udplcemd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gblbsxnj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qcoohevk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ephepvyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qielqamp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3enczniiq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbyjnviw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qfclzoem.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mumjocfb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjzzamls.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mzmekqil.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ojuckuxa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qzrweowm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lprdjpqw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kplxxiar.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cdeapwqs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gyvwhomq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3toykmysx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ujrykfgr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wvotaxfi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ohutfuae.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3swqtlzxw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dwdkaohu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yhzziiwi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ynskgrbu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bqgvqxuj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhimyzic.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nrvpsazb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qvdmbquq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eumzraow.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hxnhydls.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3paouijrx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3boxydkcz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vintbsez.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zgwcymym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kticmsdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kpoeignh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zeuiuejm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ymjljfsr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jjjzwygu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3intheeia.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjziqqgu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3aiyskfig.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3harpekln.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vxidwiqr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wvrndsff.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ijrrpvbk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkkbqgmq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vraubtcu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rspqyrfp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3scqpciwf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zopphhol.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zuibhwob.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jsddpqce.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3astrdysb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbryrcgk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzaunmkr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dymouscc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3umlzzrjn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pkerwonj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fwivvtki.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tcgkajvj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbboyys.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jawrpeuw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3occrwhpz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cidfvymt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgpzjakg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdkmpjwv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3uwwwnzrf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dwcztzxr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3obclackz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3eaqgewrs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wmpdiusz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qasdlvdj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3baxnsbyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3heaptcuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3aabmjiut.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pelhkwey.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dmfmmodl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yxjgqiqc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmzxsmi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3esmxsldu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcrubtd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hytyexen.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ttmzmbdm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3erwdjgjt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vjrunnwt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dhgummkm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3spiaupwx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3btnwyubj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wfiqlxsk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tdhulkih.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dxszdlfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjbnfjp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cisjbjax.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3uyltiobx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vdtoooro.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vdgnpemv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lwhzubnd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3eerhfeay.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itvubrtu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqzrqwzs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzxlgvy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nccshrtj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3needkkmu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gnoyjess.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qydsmnri.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dmcpaqbt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3epqbphkc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gbcumpti.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkkccoa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qfhpcmjm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqhdhzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lhyztkqo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mcsstnci.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jeulehps.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nilsizip.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3havvpxat.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xlputtuz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ylwljtsw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3iaezthoz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zupdtaoc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pgsjcris.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tgzfacbm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kvsiqwcx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3teayslsw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dxtjykeu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zugdynsd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ybtrlcso.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhpmqkal.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lbznkixg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hyusrtyg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pqoyncme.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xzmdirof.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jaqvjzls.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wkaipfvv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qjgpeckr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ztvultjs.html


<!-- 参考信息 -->