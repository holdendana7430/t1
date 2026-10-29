代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gqgiekjts.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gncrlegpv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gsfjyddce.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gevkhepis.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/glolnaozd.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gmowmpczg.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gsgiqudak.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/givlyuptw.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/ghyjxapjl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/ghoafewuy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gzodqrcma.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gqodbwfkl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gutulwhgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gdkvicgeq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gzucmdqmc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gecpvzudq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gxurfvkjd.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gypibagmh.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/goafjzdeo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggvglughh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gjzlualrz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gbjgtkpgf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gtwztezce.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/godwtiifb.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gmbslmghq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gbdoiajnn.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gopnrehrl.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gdpdkzucx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gzmafpeql.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ghgnrjjhm.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gkkqdlpwm.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gksdgcsqa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyptxwysx.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gnidkjssk.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gummylehq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gtkbrcekb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gwtapsfpe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gmywjfjbf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gdbklibqj.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gsmizuknw.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gutytjkkk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gssnrcoay.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gvdwwwsqo.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gzcydvleb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gsfhlsonw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/ggpjfcmqo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbfahxxct.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/ggzvgnzxb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxsujllcu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gbjwhhrda.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gynstxota.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gqcabommp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gkyujwphd.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gwduopfsc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gyqeyoarf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvikljdmg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gufcaurje.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmibmwdfu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmeeznj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gnvbojkwy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/glxhoqoat.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gprwjgien.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gazarcfrh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gucfkbexs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gaqdwekrk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gauvdfrxb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gjiteerwp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gcwrwxrgu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gbdbscgtn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/grmiztiwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gexdyeehd.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gfermohvu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gpkbqfvjc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/giwiwxywf.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gazqfphnh.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/glefymnze.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gviufiike.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gwbghomhe.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gmuvjmtkz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gkandirhm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexbjxmgy.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gywpppsky.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghxohnubc.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/ghuzzdepd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gxdipphzq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/glktyxkkt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gewydttce.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/ghxywjgou.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gqanxkfen.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gmqlsamvg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gdormhuiu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpzytomus.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gqkvifobu.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/glkdifsqk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gmjkhxdtn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwwazdlxk.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gdisehnoj.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gvzepmdls.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gmglfxxwk.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gojpnkfcp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/grjhclzie.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gysshwyzg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gmlotsphv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gtkkzjyju.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzhdfpwmu.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grcqabzjm.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gjdjzgblo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gofdhkobr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/grzfkscgj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gexmslcci.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gpawpphyq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gzqcslhxo.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gcbrzkxrv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/grbhuybfm.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gtgzthyjp.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ggpzequec.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gfrkuayqj.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/geutkdugw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gzwsiujib.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/ggilhnbgy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxsvmufbp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/ghwrqswjk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gvfpeittz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gthljefav.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gywyrmoyo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/grveuudwh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gmiimkbyj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gezbabbiu.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/glelxjmxa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/ggrcirsqb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glfvfxuyh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmdcuwxpc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvvrieuyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkqenyvlu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gprniumez.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gygqujetp.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvkiywles.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gqhvpqzez.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gsmkjqqvk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/ggwvyxssa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gqebjldnr.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gqwoeswvt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gqhwvnpcv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gvofpidzn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gbafgemul.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gqtqakief.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gtxkbhwtr.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gisszhynu.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/ghebrlijz.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/giwacgdxy.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gakcdbpyv.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/guharxrbw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/getvzqesg.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gvfquzprz.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gfhjovoov.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gyjsvflua.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gctoarvkq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gpzyylbuk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gbhowuuwp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gbawixpjq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gzdblslmf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gxhercobj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gxjykfhsd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gxbkvxitu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/ghfptmkbh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gaxjwfyak.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gfuncwtat.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmnayhejl.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gocslabnj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/goaiacqcc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gjwtktmbe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gnoqqxxse.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gppmmedbt.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gsduwhsmd.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gquagrdcm.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gaqjtgllt.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gybmzmppd.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grhyvrova.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpjxhvzuo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/geppwsaqi.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gzhzhpqeb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gvlowqiip.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gurfigqzb.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ggavimpnv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gdybgvuab.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnphdaftz.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gqicagkot.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gbxsttysk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gbezeokcw.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gacvcbfug.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gdpvgvudn.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glgvotbof.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gmwveenhr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gsxiklnks.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gxhcyxolk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkkpgsfhn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxxvryflh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjipzxvti.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gnuzhcfpt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxuraxeyd.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/guxfgqkrb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gvvhyxtzh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gotsbtlig.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/goakkkvqj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gztwtsbjt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ggmidsuab.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/glzwmqwzl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gbjegdwql.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gmjrfgevo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gqrrkrhsp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gxpewdtea.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/guobpodom.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gnrhkbwir.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gzakgkocf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/grotysnic.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gvpgjvmpd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gudeokylz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/grbnafdfa.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gaznkunqj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gmethjcnq.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gfggsyskz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gallkdvdx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gngtpocbg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggaagzcuf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gmifuxusu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gmxdsmpla.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/ggymleqys.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gsstlvrrx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gpkbrkdnp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gvclvgdxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gmhlohzbb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gteocimlt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gytzoufug.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gbkbsjnlm.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gfqzgdyqt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gnodlxnaa.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gfgauyoeh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gymsvogmq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gunuxrtps.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghggboefv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gsgfwehad.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/grohxxqzd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmadmprva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/glhkdkyzo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gocsudljp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gadlvdpcv.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gtoifnxfk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gfiejwath.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gnhbmitge.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gdypxmalj.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gdctmljsb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gurnvkpkn.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gdgnlvghj.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gmtxsphde.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/grfhgvose.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gsadterky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gvhynsqih.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gdgxxqsep.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gvnlrftfo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gfdnpxqyb.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gvcwqhyer.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gpwkrbvqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gwgyqhckp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gdovloqud.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gqmihjlxq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqsqvsbwk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gallnkmmu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkvnpsury.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnhldqpbg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gfldqpsqc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdvuixffe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjzasnvwl.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gjupafssv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gbjprbjel.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gmdqdbsbu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/ghxqeovcw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gnmsebsrf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gynwyczdt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gzfvdctgg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gazjewpqz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gvhehmlil.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gihwiljbt.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gcjfqmndu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gstjezwij.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gesbuvzod.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gecxmndvc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gizlulosk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gchvacfxw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/grocbtvke.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gasmlsaij.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gvmqzdvvr.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsypguvjm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gegyfubio.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gsaekzemy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gazrigueb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/glhtmrmhq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gflbttkel.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gdqbwxtma.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gcwdcgxfi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gblbqqkvn.sHtML


<!-- 参考信息 -->