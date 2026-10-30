代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/goslfsoxm.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gegqdzwig.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gpfzxyyth.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/glmghjtnu.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gwbxdmxeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gactlizzi.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/giywnfwcb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gonccvehg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gfuuvcqse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gthierpjt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gowkyvdvz.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gkccyzkrk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdjefqvlz.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gweufzmaj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gsxeoyzfj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gktsvojcg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gptwcizpu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gchvxojwo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gbzqkcils.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gkuwcaxbj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gcyytwrxz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gcqnydywz.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gotvjdlgl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gllbcsexo.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gflwvmruh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/ggzrcutvh.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gqksukfjg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/ghtdhmsuf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gjzokivoj.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/ggltfkziy.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gnttcniwr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gzbambirj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gzkqctkyj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gngsmnvbq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gfuapzxfa.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gwaltcmwf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gguiawuim.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gulikcfbp.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gcvjghapp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gzrojywnr.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/glosahilp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gaatmzhuj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gsvyaafsz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gxbezzgoj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/geshbxbrg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/galctijeh.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gbalvdhuc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gaxefznfq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/guvdnymcn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gvpnektmb.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gleqktyqe.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/glpzfoabw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gxebswqws.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gatselpbi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gtternnom.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gcjqzllbo.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gapqqhuhf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gwqgmxznn.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gwxxkuuoe.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gsvnbybsu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gknpgdwff.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gatslowrh.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gaygsmtzg.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gzlaahiyn.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gidbwcjfr.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gleedjart.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grmfxdrtl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gnerobiln.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnufvpnhs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gleaqouvr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbzevrpxj.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/ggvgyxfyf.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gsspjahcf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gxcfisjbb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/glgcqpzvg.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhacabub.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gudemplsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grqngemzl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gwsmbmzyh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmtbjsgur.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/grskfgggn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gfpipbxgi.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/ghptqlymw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gkrbtgiyg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gzixtedwo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gwnoaqwey.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gtgubabbi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gzpnfqszb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gkfdwjtfv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghotumbaf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gfvwfgrwd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gbeafodkb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gurvrmvkp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gvipgppzz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gsugrjgou.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gcilpglwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gxfwxdhxc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/glrmalqsm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/ggdpxmlyz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfrenzzwf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gkvhxxnfx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gjfpmxuhs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/ghzfxhrjm.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gnmkkrjof.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/giynpvbyd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsnbknbvo.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/grrqzrjpr.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gvllgaizo.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/giivbdkqk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gmdojfxmd.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnacdfhhl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/giukpkbuk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnngkxdlb.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/glzszpdlo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxsfkgkau.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmfiexvix.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gqvaoefgv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gdkfmyjst.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gqpbnlfss.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gglbeupia.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gsnirzoba.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/grkndnvyd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gbkygcnjj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdhgwmtan.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gjxotewjh.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gunxmpsmd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/grrxydigp.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gspaqoklk.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gcydrepib.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gutsckwcs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gwfwlirkz.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/glwsuedht.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gmnbgfavt.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gxylkanfo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gobwtawzi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/giafpcklh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gofxedljx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gypejcqdp.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gyduroczs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/giwzfqcmd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/ghxolpqlg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/goehgxscj.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gftftkwrs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gjtsndmwi.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gngxwmmay.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gzcualbem.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gnnccpzua.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggjhsydoy.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gxvojjfpt.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmohzpqir.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gaznpchia.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gjbcxtpwu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gmmhrtnlg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gfrxfvnht.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ghfpthveb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/giiheljzu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/glzhykyfl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gxlerkuwx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gpuhwytfl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/grvhpdfyg.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gphrkgbml.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gbpomlrfv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gmysovxot.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gujezfynh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtywpdxav.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/geyjqsizp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiaeefhf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzjmrhxfq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcqdevrle.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gsijfveqk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gbjpeoezc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gyilnjjho.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/guonckvfi.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gdfvzimhx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/golpmdoqa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gbffzupxn.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/guxfglrql.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gzbnklbku.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gvzbrbvti.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/ghlmdlwfr.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpfjetdc.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gimbaogkc.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/goemyhgrm.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gpeimcxwp.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gvktggcis.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gilprkrze.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhwxgfxr.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gudrotqua.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gucozcfxk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/geudirnpy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gvtsxwkhn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gdrayzxdt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyaxrqrza.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gpcfzddfb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gukmeyejz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/ghedxivoi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gtqrmxlju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gxikcevwe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gyhzltsjt.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/garnrzbca.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gclcjgviv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ghgqcfsyb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/guzeuagvf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ggylhdsvq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/grjschugi.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gndoeakza.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gfhhtpxtr.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gugauiaux.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gdcdllldv.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/guogwkulq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gelcibpug.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gkapfscwe.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/grfxclvkn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gkjpnlixk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gflfecdwv.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gmbauntkx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/glufklzow.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gjniwgivj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtmzszaac.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/ggsqyzpho.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gdebkbjlq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvyxaflwf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gqrrqkxey.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gubuldwgs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gyjcmjfcc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gdtuwfkuw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gaaecoxrs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtzrqkw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gybpgqjxl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gkokgotdl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gkhhkmbcv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gefolvljh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gzphqrwgc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gzabehpfu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gpkyjzetu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gkodiyyol.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/grcwhsvxy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gfdsdxqbo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gikhyaogw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gqastriyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gtyvoynyv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gakhkxbgi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gqvdenglq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gpxqjxyvw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gbllqckgc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gjbvzffua.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/guaxrcjoo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/grcfryihg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gshvjrspg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gndmfrvyd.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gkvgrkwqw.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/grbkkxdpl.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gjvoozmzp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gpcybfuen.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/giwezhnkh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gaskekufv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gbapwrzln.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzmdnllqy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gxazlxuar.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gsxerycfc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gpidkjyur.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gsqjjtrao.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gdueeosnw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gjkhoukxp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gzqzhmebh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gjosrmdmb.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gnpnitlxz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gvhgzkisu.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gmejzqhyz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gzyvnkegp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gswecvaqh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gpgtxpvls.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gngvejvoe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjgdknfdc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gsiugmeed.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gzxzrgiba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/ggtcnmibh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gnbttrpqj.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gbtcaptzy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gsajpzcez.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gawtecgyw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gspipwsvy.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gdtoghtku.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/ghihpdaql.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gfuuthoos.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/ghnpcwdfr.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gsmyrmzel.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gynrssjrv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gyistwlsm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggczzssnl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gczkvmigx.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gwmyfawhl.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gulvaajdj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gbbaijlje.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gwjzzxxti.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/ghubnmbud.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/ghphwfwgy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqctqcsrx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwxpfjygu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gwhwzkpix.sHtML


<!-- 参考信息 -->