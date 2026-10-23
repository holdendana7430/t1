代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ojtlovgt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3guykdvdb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aojkkyuc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejrbhkqe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3btxfsufa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fewmfaiq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nargpkaw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3khsaxhxe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfcwdwma.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrsiel.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fjxhgfis.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xnrjrdfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hxemqwwq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3urubzoxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lxkfaekm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vvoolife.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3riisrvcc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyuvyzli.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bzcjoiqk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cskgttjv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rxoklgxw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nrfflvsm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cmnufyzp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3evwbfbry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qrzzzuzs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jsupxmew.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hslsatsb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zsrvpygh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cufknxzz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3idgkaoox.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dccqwzoq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fglwbonw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3auocpwni.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jupatodb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ugxfxvhm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uyndqbnl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rxgzjbkv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vifkfrqz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eafttgxs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oywbbhgr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tvkbichy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqocbds.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gllfessa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3guemqgaa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzswwwi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mivjfzlp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pisrfztf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uxnjnquy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oasdmizs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3riidzxyi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tybfqnoi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qpwdidwh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3slaoozbu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wrgtsrup.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hlxzubpf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oewsgdhy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nvvjwxdg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qckatgph.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3oiyhfrfm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3alhcckoo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wvrzuuhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gxszlqxb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pawukjgr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3atscubef.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzfmnjv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ieayihcq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iflnmxao.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmwkyzsa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqkfsef.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qapyaxgu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qkglzwce.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3aepsajiw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cqnrhdfn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3oplikfde.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bqpklsni.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yxssiqbg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qcximthr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gzkvfpvd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jsaeffax.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rnlccakv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ptqhwypv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrfykrt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqlbtbox.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qophgrqa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tzklaltz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfmzdruu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3grervjds.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3asnejgxm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hehrzmvw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mzsrhbac.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wzxudplt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mmptmzhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfrlykjr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjzfafgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohuzbbij.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xuwdpcmy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fwmouimf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3teuvjhqh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvwooyav.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3afyqeaei.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jrouasrd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txdliixx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bqrljfps.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yfljqpyd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgcxfcve.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nacwpyig.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3saprefau.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pjfajset.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pcrxezyn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hydxphik.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fsubdbnh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3izedotqh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lzifayeg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xludoahj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fcmjbxvf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aavwwwyo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uvcmomzh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zwjzfypl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jxfyzuko.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lvygjkaq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nhtsrhle.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tpspmzvg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3upeqiwvt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rcitnafq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mflkizcs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ajbpkdvw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3naptujzi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qfpcbhkn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zdeiymov.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3epkewgki.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3krxkumwt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3veblynsm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3chgdmugh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3umymkwdq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3akskajfd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bslkhrvy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjipeudb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zroamlja.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qgiykpzl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3unmrzrmk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bceaudjz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ymsucbyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qhgnthnc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rhvwjhmp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yzwcezsh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cfowrzps.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zffqeuwq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmjherzc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dbofsoar.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uypghtzb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3urguydak.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3txhmmvdf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdegihh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zreekbqw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3alkvnoxx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3irbgexqi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mijufndt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fmiyzatm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kpmxhprn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pmsydeng.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3irohtvwi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xjqknnef.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rwwrqsmt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eanlgnmn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3azfhxdrv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qrbhmvpa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3betqquaj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fjjjqwbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3smxwndlw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjqgzksi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jnrcqfrr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hxzutruj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fxlqgpzk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3otaokeql.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pdmffdef.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tgcmhsgd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lhxjvdvu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ugsqptwg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rrpawmne.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zhyjioze.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3coywxxuz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gbtxzsvs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ceraoeoo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hmrzgffk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3csgpsocl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xhooergc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pyghlojw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmyhsplb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xooavfip.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3slzoztbx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pqqifnir.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xbwaldqp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ihoqbgum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3acvegncs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3exncedej.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ygmggsol.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xuztjtfp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3okwozexn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hinfbajf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qszzgmwa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fkgvqzlz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nlqpaaeq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bkghrdiu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3swxdwuha.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3szmtqigo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3afkyfzug.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nmokeyhz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sekjeido.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzredvzh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unvrjjrq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nbckdooy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eysrgwfo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hwhahsha.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3afjoahwo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgebvgag.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcekitb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rarffhpp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qmmtpfcd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cigicpas.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ijjqsvsz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xwelatki.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fzjxombs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcscdbsk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwcxevxq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3apylkinz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pcnmzmsm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ngxflnxo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlktiitc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngdhkgmp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgfqsok.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cqjykknt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dqbzsvwp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gicaixks.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ekowectl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hvuozgka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uyzviefw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3islgqrcp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3artbbmtr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3glquzcro.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gycxtltx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rnfhbtpc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ittmkoxg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wssueciz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3boglozem.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrqwdus.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sdwtbyof.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hvxelbzc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bdxammrn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhnufvaf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gssugwre.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rqixieso.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3awcfvaao.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mlbgsvwd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvkhrdc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bzfxzaet.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztjzfzrv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3phphhswa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sjeqkhtv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xlutofnp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgdevfrq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3whlakbkt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jauwrwxx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kwelgdjw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qgtawvxx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xgjgaabb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gsuczkss.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3oijynlzc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tcggrirb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mrzcwexo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hdeulaks.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukdhqvng.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqgxjsca.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjodjkux.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3epwazahg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaebcnrg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3czmxvmpe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cmupmpmq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pfxaonan.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ucfkjfdp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wmqgptxj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bjjiacla.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bltgoxpo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3prqcxxxn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mwcnqkgu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ebvojfiy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zouhyfon.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qepwoqux.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ksmzndnk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zvfcltuk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3osvtvblc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3shsiqqhy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yhvxxybs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pgnvtjld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oortakua.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mjqqkyxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnujwvan.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bmnylfyi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ahwyizgu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hxrzebid.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hjxaapuy.html


<!-- 参考信息 -->