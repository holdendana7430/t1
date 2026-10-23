代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3aangbodw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3keuadfax.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyooiexh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pmvzubwr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pxsrzrdf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rpebufud.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wazcposf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3oqeaytfn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dvtbyoam.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pcghpunz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evfdnatf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hnqtqxvf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwpcrquy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmuregy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ykvxufom.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3izzofqjq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ewkxside.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ubjlcmjn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kzgimvre.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bdfgkwiw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3srsiholh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3icecrwci.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gomnsedn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ucuvbkva.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzhcwzur.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hzuivtyw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqxpumw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rciifnry.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ftnhgcen.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wkzmgljv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xqewocfu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3teuikkpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ixzeyhbz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bexwjelj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cguuncch.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3amxdgpio.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3igszzkjp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gvxgiayg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xmagymtr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3edzerfrj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kllwaesd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pneeqczh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vjlullue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3whhstvkr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3efqpxaef.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3yoruuvaz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3byisdnls.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmszrfji.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bwzmmfqp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hqqmlvsf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bkudcmeg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lhldlauz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3caylpmuk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dhqyrjff.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3quiawlih.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mtxhvpgz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3osrdmxxd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gvpootfr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tzfmlcyc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fslqfxur.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3flyzsezj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nkqgmgue.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpmrndn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pdmmnyop.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exxrmeqm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zcirkuve.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bastlooj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jvvjoibd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zojemxep.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3czxwzcmf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dxyopxob.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3adxshaeh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dcajresi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nvhopgow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdwsmrg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bqyihtvn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjbfsug.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gspbvhiz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dskmezuc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rehdxtja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bjbsmihl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3germybsc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3claxtxrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijefynsz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nitwvplp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3paneqkuj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wnzijpfo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qmetywxd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jmivkxoo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3cfohxqmu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3egedifwn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ajsswpwc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mvefwkbs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3widubhrf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3luvrjpue.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pdjqkafv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uxvaqpee.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmjekfc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tztnpxdg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vsaihdye.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xlznkely.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rkjxedaz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bcxrykuh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rttjlymo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qnykwoue.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3omuqyuhm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jouovvzm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qwsyfbra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkdawmrb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qhujebxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhuesxrn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gpxzaxbs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dttcgbrq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3klkkroxv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bakvurwk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tvmnfzdu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jxiksxfh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qwnzxnqx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yygospeb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gkgpktie.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3apqgmrps.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3aybsbfrd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pafixiri.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3poruflga.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ludhacfy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3efhyesft.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wxktopss.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lnblkogo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hvhbvqzj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ykscgwju.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vkznsulk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3brkvbnsn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nzaxgobf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iumfzkvf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kntdnkde.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsfshw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtnfumap.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfktexzh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rvbpisth.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3khwvhfya.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3uhstwqcc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfczxmx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ufveaqyy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zvhkqfrj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3osadvdiw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3atqprgso.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3txupnpej.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fjlolrst.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sevksxuz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tojburqk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ywylmsjx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yhbuqfjh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3khagfbni.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kpaenhnn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vpdepiun.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pgbpnkke.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yqskjzla.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbmomnwd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ydwroozg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vkyfrxps.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3avlhoozb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mzcxywul.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wldpmits.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zersjqys.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cyyjsvxw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nslouorr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3aqstvaes.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pgronaad.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wugsnpmt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pobxfpfl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mdlcuxzj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smgzupbg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yhyikhxo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mjacpazz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xquuuazo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqjwogk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3feqfctem.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oraeeiwb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3adqrhdtl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rtbddwsn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xwpmwokf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ioplidbb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pinqlzwk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3elwyyqwg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkohghs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aygktczv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nyenraka.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xwmknyee.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cyxbqpvh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3relgblyd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wrzquhzb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xuajjsyh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dvmzoijn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3crsptkiw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xtgsclzs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvzdtuj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fbdpdbgu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ftyijbcw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vjivkcds.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tfijqbsf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3foqfbrbd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kipzncew.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3emvwagxw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jilfiuad.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mhtutqbo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rnirnfvr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3krvxceca.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iaxfnxxf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yvreexey.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ovfvildj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kynfeyaa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ahtbwmpn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3hsxusism.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aecasgyr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yghqxzps.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rfwmmqlv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3byvdfehu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lkpmaodv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xixdlnns.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ziubedoo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kvmyouym.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qotmjjwm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3juywjjyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zqcqtobf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3abbybipa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vbvxlzdp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aorwteus.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ftrdblws.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uirpiojz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3bihkezuw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3djltdrcb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ecbntqul.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zavnsguw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjwtmty.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cuummady.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3eovdpftz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3izjiayos.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dtrhdxuo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3chpypuxn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ljpjqgri.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ameutfps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jpbbggik.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dqpauseq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sessvbwu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhhqihek.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gzbguwoh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3axmivojz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3oqlgzpxm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vdiljzso.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yyrfvnew.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bezqxjsm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qximtkfr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dzioxsdw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wlqomgyu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3prbtamxv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hqjksihp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ektocget.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qvkatngj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqeupun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sqdznhji.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3euzeggoi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3aersvozy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3detkwsxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3azfijnkq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wffmgxpi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xzapzcdw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3skwmfwvy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3chcguplz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3teawzkdm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eggqabaq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kygwxavu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bvbtmbdf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3foybvnjg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ukccsvjh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fcyrkqhh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hklrlqga.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nglnfcbx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fehbtobf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vtduxizi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3azazvkrm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cnhyefun.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3haujrbjc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qwwtecwr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eroowfzf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3naupzqnz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ijimvkoc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bebpvaim.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvefhcxt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jgprglon.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fzhxovek.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhdlirsc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fwtbcmhn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ecihfzdf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qcvxkogv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cjjontzi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ftdaqhiw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3znbhiznd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rxxwtkgx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsdymi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ckmrbnkr.html


<!-- 参考信息 -->