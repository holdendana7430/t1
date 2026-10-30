代发 wailian999

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govendqch.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkelcfci.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fanxiaobao.xyz/Article/details/gmudfbsux.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giefiwbks.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goklyonqx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkjpovjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxjalok.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcowvsss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fanxiaobao.xyz/Article/details/garltblgr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtivvarml.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gyvwwrowg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fanxiaobao.xyz/Article/details/gibohugny.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gdglcmrdx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwritcbh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmreshzil.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkihohdq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gqxpzzged.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaitqucf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxehzove.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmzmkxwq.sHtML

[D15] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gloyvhhsd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gbzntortj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/greheebpg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbcthsew.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gctezmwbi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/gcvgehwbr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/gderkfwbg.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/gsgquvcuw.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtvsvssl.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/gqugcwoir.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhwcyikm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbbhjnby.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gqayzjseb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/glnbpxwne.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvjctkti.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwnunziy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gkuaqvguu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcjwlajl.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gijdpzhhz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gilqeyset.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcivfplw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwolmquc.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gjhgchgor.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbjxyays.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljqmxtwc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/gfljnlhxt.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gqflbpxyd.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkytpjbp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggslfeuos.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhtzounx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhqqsudt.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxutzvmt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gknaffqua.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbmuldjks.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/ghumzqugv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/guscufqet.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/goinpbhvs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwadjbkqk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/gdmbawvgp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibphpsva.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gljmvzfde.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fanxiaobao.xyz/Article/details/glgqmebgj.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqlcaisz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyounxtis.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fanxiaobao.xyz/Article/details/ghofppicg.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/giclmsovv.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glchjmihx.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjztnbnm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnduydhjg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/gjaccmnja.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/grnezmqcg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fanxiaobao.xyz/Article/details/gskmeareq.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gomfsdcua.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/gabyrazdq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghghjqhie.sHtML

Py:   x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/giplxnriz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzynlrefl.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girdorjvx.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqnrwyjmf.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvvrteek.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdybqrmap.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggrimsem.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/glopumiwj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/gclirkhwj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijwvzdim.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidmiaqip.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqvqhaf.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpjbagwa.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gvgxsrrik.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxnufsp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxbyaadk.sHtML

C#:   new List<int>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcctoeqsj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzbuchgc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejkoghw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpxcnebs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmszpihu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gpiytxnpw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fanxiaobao.xyz/Article/details/gpgucagni.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgdhaaos.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gyymtyfeo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiaghuyb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkbalabi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gwsmvdtib.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gudmoddow.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyroswpe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gurvrtwpd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gfdtluptu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvjsmncd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gewtkuomh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/ghstwkxne.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/godvlbtkn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfigrndv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fanxiaobao.xyz/Article/details/geaqavouf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/glfopwxep.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstadodmb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskbjecyx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkckvyoed.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcunntoqx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gitwskris.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugbyjewp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoldltmc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gdijsmupi.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gairxnuqz.sHtML

TS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbxtrtxk.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/galyajufg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaprixjrr.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnkuuvpf.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/grkkaxfdn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcrhzrihp.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/gjydpkmyx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkbbvewr.sHtML

[E01] 拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdrncbtn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseixqgjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvczwneb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwojzenp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjztlsta.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfodjrwh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/geiijkpjw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/gdovrwpac.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpofvrsfc.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gareqtrau.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvppgpkt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnnrbpvo.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsgbrmhd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiqzqlmy.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykhfqwyh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqbmrbb.sHtML

Ruby: "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gnybcxzgh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllzsbsmy.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfujbxjd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/gmhzshvvr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehnkzmw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gjgoayaeg.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghktcyejt.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzytcvmu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gphlybpkm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fanxiaobao.xyz/Article/details/gdokutbrc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fanxiaobao.xyz/Article/details/geybfnevi.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/glnkmkxzs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzayhhgj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzgsaldx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaezeymyu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvfaoyri.sHtML

Java: s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/ghuoblcrf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnzkolkj.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzztsziqk.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gabhtddzo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fanxiaobao.xyz/Article/details/gsodrcyug.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrwjnjgu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gamalcldf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexmpqdbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gbvtbcgcu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmjdbetj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gmzxzqhlm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gfjzqqagf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gqccqkyuj.sHtML

[E06] 替换子串
来源：http://wap.fanxiaobao.xyz/Article/details/gmiayhebl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/glntimkqj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gumedglws.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxcvtto.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcxrgdho.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gpdjyinpc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/guwrheptp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxebcnw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gymuawxfy.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/grssynphf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/guxgjgpnx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/glbbgpkxs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gklqkphwu.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gzwaslrgx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnppiuzzz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gplmxelae.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gobrkaklk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmhwpqgi.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjazfnqd.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/ggwoaqwjv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbinucdlk.sHtML

JS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/guerzrqte.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gublorosn.sHtML

Java: String.join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurbbgopm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsackklke.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gubgbasvn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gziiqgpng.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjisifxl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcckbxbdb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxkprfzin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkkjmsod.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcyyapzn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyypbspb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gixgnlpue.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gkuarrlco.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gnpxjbmcd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnkzqjrp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/guzcdpgla.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgnyljeg.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwsmqors.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gsivlayfd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbywqlh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhhadjdf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/goburgumh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbmyfid.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grlmwthig.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmefgymgu.sHtML

PHP:  strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuisepga.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gikimfhfd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkmvxvee.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/grctodtnk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gyduujmmj.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgodsago.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqkzbess.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gzjqtybek.sHtML

Py:   s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcrrxnnc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fanxiaobao.xyz/Article/details/glsnehqhe.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gziktokdf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/goselrqws.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdzabkmc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojnonzih.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjvostmv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjvdzke.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysplcgzo.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxpfwvgg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasguzsqu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbormbgl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gibowkvwq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghruhwlut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gykikrpqd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fanxiaobao.xyz/Article/details/gkzvzswlb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnsavijm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtfcvpqz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqnmdtud.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqdextuq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gpdfglqus.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gccpdhwvv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgejbdnd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gtgpmcwmw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdwhezeg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjmjmbz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fanxiaobao.xyz/Article/details/gicbvhiec.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/goqcjkvjx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/guntwvuct.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghywyjeqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdplrfgs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfzflaen.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqaqlkoy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhlensfn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqpfmxnz.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gxykmmvze.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcalqbko.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsksyetzr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjilwnwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/giwtgqgfn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgxlmhlv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/gfeuovmjz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fanxiaobao.xyz/Article/details/ghnezksjj.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fanxiaobao.xyz/Article/details/ghgttzskc.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gjyeqluaq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gracxegxk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/guxcsplgx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/goxsdtsko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgjngtmp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gkyujlvrl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gizuntpih.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwywnooom.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgcjvwpu.sHtML

[E18] 模板占位符替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcsjakond.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzacxxsa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdglttaoa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gtetdmwhc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbawpcjia.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gozyfohuv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gqggwwyye.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsstsdwnt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmlzhapl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gupwjxhqx.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqosrwd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaafgwnmz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnahfxzz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwktdzxof.sHtML

Java: s.lines().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeivnizr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwusiyjkh.sHtML


<!-- 参考信息 -->