代发 wailian999

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gnkadqvnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/giozsgihv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gmmxfpxkl.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gjurbktpr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gdcbioipw.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gxztosylg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gyrozpzhg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gnzfbhyes.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gzwuiqfqf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyuxjngck.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gdvcxgiho.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gblbqcxyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/giuotdvpv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gqomkybjy.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gmxquksqm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbemozgaf.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/glclueteb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/giqwfcely.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/ghppulmxo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnhmhxvhf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvpwekpam.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gbtafwfqy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gxkjkkqjl.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/glnwxmkcw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gyaemurcr.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gaaixxjbz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gbnkrwpru.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gsulemmfv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gbejaxclw.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gpfsuazzo.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gckfkefiw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcjnnpdrq.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/glgmmakml.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/guqrhitcg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gkjlqttqa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gfdvilxko.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gcargkgxd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gqtyzcarf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gkrzfnzlt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gbotiigks.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gctoohdnt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/ginkismqw.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gnxppuybv.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gadiyspqc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/giifuuafo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gvgdkvtds.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkisbod.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gebnxtbuw.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gmanadext.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gtziyjogo.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ghyqkzerj.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gmjfwtfsq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/goherkhbs.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/grdcgnfcw.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gznasfteg.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwdcklref.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbaaktwdt.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gjspvlsra.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnpjnidqg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gtosfjenh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gubyktxki.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gijzuzfqu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gdcmjzetj.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gfpxwtzpf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gqvreklts.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gkaitfugi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gxaqhiorf.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gclifrqeg.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gfqakhqfg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gebdajrpz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gqgkwwcnb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gsyfsceuz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/govodykuk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/griztiahi.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gosbzsywf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/ghijlkcni.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gwcyvzsfq.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gijlfmzrt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gyvhyjbdh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gwsgokzmk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmngghrjh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfarncshc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gqyceabto.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gvrnkjakt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gvwijwduz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gcxfdvqlh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gbjrtkihh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gysqgwlsw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gckzupwkf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gbxupbbgy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gcivgjglb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gxyhkuevp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gphrgxhvd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gyththvuf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/glewfdvsg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvfrdnfpc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/ghsmviubz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gszalehfs.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ggqsfhomr.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/grzysfoxh.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gzpjtqqol.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gzuyxinln.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gquavoqnh.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gaxgyymry.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghefgojyw.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gxrladaio.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjikzpots.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqtsfwmas.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gvznkffcm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/glcjudrcl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gruvwdhta.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gbppubcis.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gfspyatxk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/ghyeeikni.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gldtiutye.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbhxkjaua.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gfzvodbvv.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ggrptusnd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gtsurndft.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gmujkobtt.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpfkcomhz.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gpjvulblg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/ggqqpckja.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gcojwdaze.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gyqkmbnec.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gfnnvwgqm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/glfolqbzi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gklonlokp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gcfxmchdn.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gezmwklig.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gywsomrpu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gfskupmlb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/glnjeoudo.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/geokghymy.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gwlaclxtx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gkzmrdsql.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gqrrfpdct.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gyafxreie.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gzuvkxbcl.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/geujxvrxo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzunhosf.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gyroyuyre.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gplrrausq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gemnothso.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gkyxssmyt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/grkfunfsi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gowimapsi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gezuvmyiy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/goiuhijkg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gbgteawoc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gqywnktfo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpmhuhvud.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gqhlovllg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gbkwzviph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gdnmmbpfn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gazrnvwsj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqujzwrxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmlrzudil.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gchiwzuoe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjvtaghau.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwryjwbqn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/geptlgkbs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gzolczjwy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gtzxqpapk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gohohjuul.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gubpaatlm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/glsxdbwof.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/geffwtjcm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gudplleia.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gvtcldxim.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gzzrlzmzo.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gtvaetxjd.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gdrllfvyo.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gqehjxrvp.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gtxjxshph.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gkbncpeak.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/ghhwxooce.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gacswsmdb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gddueglrz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/geyiveufq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gepxgzokq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/geszuzfyd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gneljhiqa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gojsuffag.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gbnelsxvo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gydyyecfj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gfvhuhpai.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/grervpcac.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gbnqbyjfs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gnrpfufxx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/ggwbdcfdv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gamospxql.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gicfeumwh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnvpsenrt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxbnwjhly.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/glrwnekzs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gjuiskbkj.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gysbazcgo.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gvvwuqian.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggqthjeux.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gcvityier.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grosyssqh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gjxvkupud.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gbcfxxnjq.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwlmsskgh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdybusmes.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gonwwgdcs.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gopevsggl.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gbpcijgnp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gppousfcc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gqzdhpbcl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gdjzepgfq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gwrwifssp.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gfdlrqkqh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gipnhtxld.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gjyujvhic.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gfumiskqd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gmhhczcpa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpnulwvfx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gmglzoeva.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggjqavvzg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gxjkrhpwz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gqqjleptj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gslodriep.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gkwqmnccj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gdbpvxwfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gytkpmvui.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/glkzuiwsp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwtpetymi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/giwzgjzmz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gzylpajux.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gugaoezgn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gurtcpyin.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/glyljokps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/grpnsfmuq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gasrrkynh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gpzddcrca.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gxigomvfx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gwjyrubhn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gnvrbtdyl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gqzczajoj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gyseqekjj.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gojebbkyh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gstegpyfd.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gdlbbvkuh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gwsvwkgce.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gxyggfkuu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/glyfwncdi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gvgkezhjw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gdexkjxwl.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gxszgdjbi.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gvrefuwyu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gbswauxcm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gyodohhgg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwckpqqjo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gfqacsvai.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gmhssxkpq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/glwafaxpt.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gepnmvuli.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gadnhfbfv.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gmwedmzuo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gwyghosrh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gatdzzbuz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkohofaxd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/goecumuwl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/girloqngi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/garbiyhza.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gsjwszkxq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gznozafhj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gegvubqcq.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gswlkimrx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gxvdgenpi.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghegbfesi.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gpklukayj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghxitbqui.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gjlxdackx.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gtclwolme.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gqwlyvwty.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gzgzeimbm.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gjycsevmt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/grwuoiiju.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gegezooee.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gbbbrrjis.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gmvkduomd.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/godkxwewp.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gskpfyzjm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gdhpkukvq.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gfpkwghpe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gacfonrpm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gbupjjanu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ganvkpbjl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkynxwpff.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnnjujxoa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gqvucksxe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grftycaks.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/grgqzoluo.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gvzgqyifp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gdehzymeg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbwauzwkr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gcdxjaqtu.sHtML


<!-- 参考信息 -->