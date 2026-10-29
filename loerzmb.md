代发 wailian999

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gzhovebqg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/ggnytikoa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gfdfwxbpe.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gmovuklau.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gcrglsddc.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gsazlcgqz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjpeollnh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gscbmjmaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gebadhnnm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjxmxbaqj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gwiuagotb.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gbgpcaryo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gwztxvxkw.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gpgbbxnwg.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gsqabwwzs.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gxjuihiaz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsqlmqpkh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gywsdrdlk.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gkybuynpu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gaolmsmrw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gnvmleuih.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/geynlnqjk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/goernohur.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/glvdkpipo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gyjpaujov.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/goyqyqmfi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/glctwonge.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gdbatqegg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gxvpziedw.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gqrjmswqe.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gedpojnwn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/geuehbikk.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gnwtjqzcx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gzkpebhkr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gbpwdcnkc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gohvpmrwc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gjynrefsj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gemgqxlfx.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gyompbzwn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gvvzqegho.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gcgvevavq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gcuziuywi.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gqsvwrxyo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ggvefsaug.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gpsytnday.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gbnktaggl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gwikytegi.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gqlaweqxb.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gfqkqrkuz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gkbnnpubw.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gmyyzpnjr.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/glkaokznh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/grcwjvpsh.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gxwkuflnd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gguexkith.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glzhowsdp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gawxkukoq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gyzizjgmv.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/glcagjxqu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gznssdein.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkgscjvma.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gwzyxyqer.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwsxvlxlb.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gvypmtcno.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gwzgfymvq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gwccjdgoa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gdhctdeuv.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/guvfvcleb.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gxxlgztia.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrszgor.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gulawglwl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjydiwkyq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gfqkpsxte.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gcsycgeod.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gzpaejkml.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gbhlvjwgi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gjdjhkrbi.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gumdfluir.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gyfgxsrou.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gecgykmqz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gpalkvcdc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gynnyvbfk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gekovumgb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gkcfxxkzn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/glvwuqaki.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gkbtkbplk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gpcnruotb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gstleiohm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gpfboboya.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcmtfwmgb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gbnnmlgmi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/guyaduqjo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gwowrlvpg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/guskugvuw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbuezocqc.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/ghyqkwnbj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/grfqbpjqe.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gqzttwwtx.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gosloajde.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gwqxnqxsn.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gqabgciju.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gtaqsfurh.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/goewwkqst.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gfoczqhtm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjkfjeoey.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/grsaincek.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpnnmkiek.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gouygaonc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gklzwtjzk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gpahvrapg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gtgclyfmc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/glcpjlbhm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/geytiwakj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/ggfsborxi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/glvjuddxk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gccvpjapk.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gfypwhfgj.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gwezfwyki.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gdtztnfwu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gjonswsdy.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gatmhnzrk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ggkipoknj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/ghajffzrm.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gftoltrsi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gqbitosza.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gitrufuaf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gtmaeuvxd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/glzpofynz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggvcedbfg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/grmwceyaz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gncpzymlr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbneybezn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gauovhcis.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/guzjgsrag.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gnbpqnjzl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gccpngrqb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/ghwcumosx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/grgjqfsvc.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/guyjndnad.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/giseluuyg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gfrxaxspb.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjgxhlcxh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvbbxrrte.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gnknwpomn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gemyckvia.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gdvmvxnzv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gvayqqzub.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gderwyxjw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/giqyclicd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzedfefq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gvrklvoms.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gprjgavyo.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gnmuoqvml.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gkewlimas.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/guogrdast.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/genzyzwbk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggqfunzzu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gksypnvom.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gnvgwwqsx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpkzgukgu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gosutmrip.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gobvbftlw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gvplvybzj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/grawnjzuo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gftorikuj.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/geewlfdin.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/glcfzeykc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gkkjdmurs.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gstxeskoz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gcttnzhyi.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gosnzgbzq.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/giwajqify.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gszaitndr.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/glglhdkfr.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwctvpvno.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gvobawwxb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gjuhwwbcg.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gydjzyrlf.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gozczazcd.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/grjfktvsb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/guvliauld.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gqalplsqv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gaydtvjay.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/glimmwsdn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gmplpjmgk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gcygiqwpr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/glsftjsoz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gwqztdnvk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gdxmlbxns.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/ggxrhmnhk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gmrgqgyws.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzegghfhy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggmeikifj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grgvkoyvg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gghxyzcul.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ghefloyib.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gzelpzsfk.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/giwugqhba.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/glryzbgnk.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gtugmwhee.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/glenccpag.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gccemkltq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gzorslhfi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gihpvabzm.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gqcnrucyo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gpdmecsrr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gqmtiliit.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/guddmittz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gfxyhrlns.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gjfudwfqt.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gcvxixkas.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/garlswqmu.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/garoqocgd.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ghtiffpdx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gxlkrjjtt.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/ghbquovhv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/ggknpcixe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmbloshg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/giglkwjom.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gelupwzgh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/geaycuvbj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gplwqcsjf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/ggzicsmsk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxzfsxyxe.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ghtmbnmbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gynxyacsw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gasysgqdp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gecqzdvxh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gbpxoxnjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gyutsyatt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gensgtymr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/ghjzybvwk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/grazynptj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gjcrmqslz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gvhnxmyqn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gyaygruaa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gzafbpwwq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsuxtczzg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gbdgveoui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gnluczrms.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/goaduycyh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/ginbrbnzw.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gygpdqtkb.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gwxjeeqtu.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gjicpwdtr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gncjkgzdm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gkcgxdufp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gpbczlntl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gwobeyqro.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ghdllacpn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gjimwrtfd.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gavsddkfw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gdsmnszov.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/ghjccsvae.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gdinauoby.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gewxtxcvg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gsnhxdpzq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/glsmabdhf.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ggwrrfvvd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gdomxqwmm.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gjskakiye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gfflmewtc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gldwvqhuf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/geivjjimu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gorogaiht.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gppbfdrfv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqpfqbcnt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gzmbvkvxp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gcqzkasay.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gjbwnlrbr.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gcydhplsu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gkeuieqzg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gxozolvfd.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gslyxshvc.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gwgdzniva.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/glphbxvwq.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gppixsxxr.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gdwskqwwt.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gvurvraxl.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/geietvovm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gkugxssbn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gknzirvjs.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gpawytkhp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzuyuwhkf.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gjlkoyoqi.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gpidenuah.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gyctzwhci.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gzyfkbdzq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gllbfrijt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjtaeclis.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvvjjogud.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbcimduei.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmfekmfvi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/ggnhunrxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gaqxqwdgf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqdxnsjba.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gvczxhopd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/ggfiyzylg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gusruoufa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gmavdvuyi.sHtML


<!-- 参考信息 -->