代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fzommwte.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yxskipqc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eulitsfe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qpzirumb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hhjtpbde.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3msasfbbl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3luylsbvj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wchzuczc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fbnnosuj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bvrlqjml.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ymuwfivd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xhhcwvbg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jndjulfe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ypjyfrcx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jaqzhsjl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lsavqewo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3brfndkxg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3adbomfer.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrbssbf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybjuvaqf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nucgsimc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bsxndshv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3prufghqq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aqgdujap.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzuxyzna.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nonnvbwx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yivfsurk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ynpfrvew.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zezrkfik.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rqslpcff.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zmulgutc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vftimixf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wnycisca.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhwenrma.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xrksicya.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pannwtvs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wihgzvkk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mgsiqfxw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bejaqbte.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dxofansd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlnpsldy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cgcvebfi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mnoyekgk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ztzrnteh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjgpdcj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mdlzaavw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3revfhjol.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fsiybhxx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jdwjcnjv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tuqsxwvj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kuqzmenr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3euzpjkmu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3czotsyzr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wekdciod.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ueuxtmgf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twckuroj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vhskzorp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3adyqnsfx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tzkdjwro.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehdkyqar.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ysklitfw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ixzrfovz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hcysoopi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cdtyvgtj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vwurrupy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jhsmtlom.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3miuxikdc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qccwsjrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrpslzae.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uufhpxsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npunectv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3grlrrtmq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rxugqclk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwleobgs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3szyboxhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tvoharch.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jqppvpvs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hurqzrhw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nigjrlyf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gcasecax.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnyhhivh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ovfqlqzk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aeqcwtrw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dttxkgej.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3etctvjmz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aeghajuh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3glquavjr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bmnxalso.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kklbhizn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eyxyqzay.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fwakkzyb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3slhktyte.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vzvrevpd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ocvrkesk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zwdxwglb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ryxubiew.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3roetkngl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3abrwygps.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jltilotr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3quoajaqa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rgijtnht.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhtxjkk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3taljhedd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vwfeypaa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mjwbctdn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vqlnjwha.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3smyrxqhz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dfydwjjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmemsya.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3drcgkclc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eksmgpuh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qvohqajw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kotozmah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3szwitgzi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yikogxxl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pbiaeqgj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hekbnjhs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eiittuqo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ulllehqr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwmvqfxl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mztrrhsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dqrlrmcl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kaajwmry.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3izafrvda.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kqnruwth.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3trdcfxdf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3feacyrtn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3olppbtin.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkezifr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3blndwptu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mujhxhpr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzevwlf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vkjentqs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tcfjrqrk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3orixfqmv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3irieugcx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mmjaxjsn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bhdbikqp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yviebyrq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cofqjiel.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nynfeatm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xywmrwom.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3imsefcpo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fzypmgsc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvyndqwg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvgsibqi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hllbhcgf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pucvvllw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pfmbdabi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zegeqwcn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kruidhpz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lgpgxxrk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rberbkxb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qnziqgce.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dneotrhl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nucbbbdf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rlkcofqe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrkhbfd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cddpbxkw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zinufnse.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vaewttwl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lphvtrvz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nibdrtsj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mbtqvbyg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ursxyjch.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tpietwbx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cszawmhl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rxxsazas.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vguoabdd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wmvrkigw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3buykxgdb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3seoysjng.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3siqmgbxg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpddnsmd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygikulxq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3oqoufcrs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qcufdeqt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tmlmllfy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3easipveg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nmtyxtxw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3sxkkxcrh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nrctilja.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmsjjhr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdcjxuly.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mjecfqvt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3abhnlbkw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mnniwtsg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zviqqnxn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ettthydr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pkjxmtly.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bangkkgy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3enkhspsc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qdpkemtj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cifcwcdn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tphyzraz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bvxidqxu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uubpnxoy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ndgrqrqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwkrntx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwwmlszj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvdgcxw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uyefhfae.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3axsyfhfd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evchewjj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gixhmfun.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3aubkdhtz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vyjwgpdr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yogihzss.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gsaytofm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ceasbyvv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3brwngyhx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3awdjyocl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3expolvfp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wnrgxzta.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3iqpfwgyh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mrfjkcsx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ffgojbpz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3umysttnh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3coapoojk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ftrtlgwo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgcolufe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3axxesfhp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3snztbkpk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3eimbakgq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3unvubqap.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hdivybns.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ocuuhtvc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fhlnpblb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kwlxbald.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tcthsclw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ythmiorc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qqjjnjxx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcdkndyh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nbxbaelg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3krekvyro.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofmibxbj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmjhvge.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cvtolbpi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rmevcbqv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3azkpkukn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hurvsqwe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hoxnkfzh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qvuyirkh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qgfdrtlc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3udvqvpxq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsyxkyyj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyufahty.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wjaxxnvb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dvfwpjns.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lisdzsqv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqznccpe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3odkqslky.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wqsoavph.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cpwbehpc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dwtikyoj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mcakdnha.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wusvxefx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ymwqrksl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3szxmqgfh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rlrktpgz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3catwoomh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3seefrjvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvtwdbit.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ehkflmes.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nwdqcxjk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gqhvogpn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3atlsnayl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ebhtykvu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zzwwdvcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhwtahgw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uimzwwaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppmbvskq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ujjpxoyv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nucsnnkh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hswojqua.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uwdqglvr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ouswsnax.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptppvrkc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xkcgpfdc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewhlndet.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fykyozkf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xqjzwwdh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mzhrxgim.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfcqsmgz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gnutpmtg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnsnyqzq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ygtcngdz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3snsoobuz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lqiqcxiz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdxmlqaw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iueqthpi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vlblkpiy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hekuluyw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tpjtieml.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qqjrjmks.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sppabwxs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3oswkyvtq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tyrsiwjt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vwnukrbu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbazpcua.html


<!-- 参考信息 -->