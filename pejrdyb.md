代发 wailian999

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gwxgihjlt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gnwpjxevs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gwxtloszj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gqykefnwt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gwfodaapb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gqynkimcv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gclbogftj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gnkroyizd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gmtceaksr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gamcnvyyu.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/ghywqglfy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmizvkxwu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gtqusporr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gexntdrdd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/ghzcprmeq.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/goranjikp.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/grwbpksfw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gpcsdlzqq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gkeuzreaz.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gxksrzqqw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gczuvmpof.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gtmjzhiom.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/getwpmnzm.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzifdwlcz.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsydkorvx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gobzlxurv.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzejkapij.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/grlypykwy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gsmttyniw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gqyrcbwev.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjlzyhhwf.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gzhfwdtnz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gnmuyzvtx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gtuwbbvjs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gynojriyn.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gzlgyctrr.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gjeptvylm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdlcfiw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gpyrbqjeh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gcxiewltj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gxyfdqgss.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/ghvhaohyu.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gucpjtscl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/goeuckxzj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/givfmccdp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gtlwyedmu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gwxnrhzst.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gftjymshc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gzrzbmied.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzenwalav.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gdrtktwwm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/garinjyma.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/ggkdrunan.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gsoldkxfo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/glihuqlei.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gardknnji.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gxsycqtgs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghrhmtapu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gnqwweedu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gejijppjb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gvgouekgj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gbhcjyswb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gdhriyvlh.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/guwwojwqc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gglwqwbjf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqnmuooyk.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/glhcriqij.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gkaizogkd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gzkxivbwg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gipbkldwo.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gglsktles.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gyzknngis.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggqqcokvv.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gszsvlfxe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gggeozqfi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gclqxhire.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/ggvezsvws.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gqelfjiar.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gmektmrhd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gcyuleluy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gwdgdmkzz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gbxcjauhp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gbxnfaszk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqbeuqnvy.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gahbdaomu.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxehecx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gpenidtsa.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gknmvknie.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gftbpxdtg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gobnqtqhc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdscfzupl.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gxsabimnm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/giukxgelo.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/grtbwlrwz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gdnpcizhp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxloezhnj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gathnbtfb.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gprinmhtt.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/glavrnarl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gktapfqnp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/geqpijbsy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gihboukoo.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gniuaqzdi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/grxvyncmc.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gghiqpacz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gkevnmbpb.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gpbvfldgj.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gwsmzfhya.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gvylaqvmt.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gqfhblabt.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gfzkctooa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gtlmeikvw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gjmjqgdoo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gqkwxndxj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gwyrcutfl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gdzzjbepq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gazilolkc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gosxbzxbz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/grnqyquyf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gptjfqrxw.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gsrbgnhdt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/glkidngsw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/ghvaoecij.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/goqovkgdd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grbtauayh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glmqvzicx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gfriyqnbr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkptvgrfe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggjwjspyp.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gjvoinajg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gbcuimzhb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gbeqfeqex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gjgbyoeys.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gwexqqbjv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gfvoluljp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gwxmroris.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gmnpeewst.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwxxveug.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gvfsklkzo.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxupivdc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gkbwdmplp.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gscpfyazp.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gepnlyhbv.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gvrremtpr.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gduakzgvl.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gfymjgzgq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gezyyrnus.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/grqqurfzi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gtvfemqxd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gwjlccgli.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gvbevrfka.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gaplganre.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gqbsbnzxg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gfgyqtgmd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gmaqalgqc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ggdvxekfp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gbvgrfkbs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqxqzhxyx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/ggnzcizvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/grubypkei.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvfmzgpgn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/grjzhozce.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gzsclsigl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gpodeaewz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gvtosxkau.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/glncujosg.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gexzyvzzi.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gkacaiqju.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcqqfbqch.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gonvvbglc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gxbzoaads.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gnoyzqvwp.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqnpudgtj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gvpraproc.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gxkoesits.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gmtlvtkwh.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gejrifgtf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gmxiuvbtb.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gbeggqktw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gvqcritki.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/ghxsuqtpd.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gbplnmgut.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gyhlniqmm.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gjpmfwjja.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gsabidtwy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gsziaidaw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gjpvvtadn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/ggrrsxelg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbxdewiqc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/grzgwjqax.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gbyyyiwae.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gjhpyexma.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gnimmrwus.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gjoxujahw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gmlmruoxe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gmnlczmrs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/ghmtylhsp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/grvzvmadn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gdhfnxloi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gupsnvujb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gbqzqoyzm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gvurxfbxc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/ggtvvuqmz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gdkylapzh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gjihmwrun.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gzozeexpi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gdtlndzpg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghpvztfqg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gzahoukgm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gizboaanr.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gsdiissuw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gtppfkwhu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gdmkwvzzn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gkyghrure.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gvrvbptrt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gksypqrzl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gtywnhnpw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gvuorvzpf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/ggfznpmdw.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/ggtzehdez.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gattaopcq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmqvachji.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/guvyktopa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gwsrgipga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkailwpas.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gvuwbitav.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gfnoahsle.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gogxmlsjq.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/grzrtosvt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gdvdwevrk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gtxwgqlux.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gdafzirgb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gamrcclzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gpnlqjryp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gvixmdhhw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/glkhwnyeg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gzxidmnzb.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gtdiogcuh.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gunprfown.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gigbthssc.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gxzjjsbfw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/genszbptw.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gdiuzcnub.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gxjqohhhf.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gfwvzlzan.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gztbdjsbw.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/goxyetazq.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gowpbczzo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gkfjsqpdp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gbmtacpdy.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/grlrmfoic.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gzejlrbpm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gjvvqzbjn.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gprtkevgl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnyqxskkz.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gtthpuagy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gqknkmjwo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/grznlgxnp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyofyrwtt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/goaevrntx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gprfjnjts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gpnifrdif.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggexspbsi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glwqlvapn.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gbxjgrtob.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/garuvxnep.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grdqwuyqe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzyjssnqy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gpueuuksn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gqqbdueck.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gqnzapewv.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/geuajhfwv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gigbqwzom.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giueyjiis.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gkbrcodsh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmjlgana.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gpwwdiwrg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gabhwanmc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxlfltquk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gzmrgkmbc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gktbanerz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gndsqxmzy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gkczsloyd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdlfyezfj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtrsutnuj.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gwbmlsyfc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/guzdzpjes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gewkqxjtx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gxmftjcdg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsagxrohw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gnsyjxpii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gazkuzfio.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gwtghzpeh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gmcobarwz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gdibbugxw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/ghezebfnk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdafvbwna.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwxemwjxb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghqeqmajh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gofzsruzr.sHtML


<!-- 参考信息 -->