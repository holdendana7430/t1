代发 wailian999

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/guwkjlxsr.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gvvfenhqd.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtrpdjahd.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gnacpyood.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/ggyxtsiur.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gdulrqstn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/goljjghju.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcbmjbmrv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gihecsqyg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzdojpvgz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gdfxsbskv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpobgeery.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/ggtxrbeyk.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gtpnqxgla.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/ghmxnwdxw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gujoxwked.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gfdwqqfia.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gplpwmqad.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gxunrniwh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfskmujpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gqlzhmkgy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/ggppuusyh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghfxckxfm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gtqofnbpc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqthpjy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gfojqkzvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gnpxqqhnh.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gyyrjmotj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gbrsolzbb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gksntsvwg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gnkvktknn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gshjncjta.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gxfmvbmts.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gaxgxatqk.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/golkqauvl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gxxauzvja.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gokfcauwo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gatvwoavz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gnntepxns.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gebalofea.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gdicppjmn.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/glzkyyfaj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvxzsimdo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gbnzqzukl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpqdfxanh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gqsgtdqmy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gonamxlde.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/ggbrbmcvt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gklgvpaee.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gdatnpoqq.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gmyzsfskp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gmlaqrwji.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gykuhopkq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gkgutnmlu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gczwxsczt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gmvllgzfi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gkcmufmom.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gkfzmvwab.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gtfuswbeu.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gaimeahot.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gkcaailvj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcunmhec.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/grqdxuogi.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/giowqyucv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gyjwnwaxu.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/geojkkaaq.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gwvmiulgw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/giqelgwpd.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/glvuvgnsu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gniyvyzih.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gwfubhdwo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gbcoiiatf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/goxbrukdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gyapahojh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gdhcwpgdv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gehyfaecc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gfulxrnmy.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/glhydctwg.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/guiyuhpyg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gfoiniisq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gyqlgewcd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/ghoqsjtvp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gbexlvouz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gndxtdpry.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gobjfzmbv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gokeofmbt.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gxzemynab.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkcltugnt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gefimevzy.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfklahkvl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gymymdprs.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/grfdoaoqi.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzbshxzsz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gpqnucdkh.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gybctzite.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/glznvqsrm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyicelkpy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gywqqyrru.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gqyzigfth.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gkcmtesfq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gsbifpdun.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gdxhcwjar.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gxdatjnbn.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gxhqbggkb.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gifbdbbyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gvfjuhkzk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxzjtiixl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/glceqmipm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkmjcxexg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gjpfvgnrd.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gkppczxka.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/ghknhajrj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gddhctgap.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gldevrzcn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/ggkjqtzgt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gmfrgqdah.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gedjmszup.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gflbszokg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gbtubunaz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gyeltcmmy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gqswswnrm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/grxcnzepy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gihctlcpe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gyxtknehu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfkvnxcrr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gufeymznd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gsqpltdrc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gnfbnzffl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gtsasqile.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gsktsiaor.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbposjipq.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gfzqtiufo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gfzxvlvjx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/grbyagmfb.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gnnnajrgm.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gqkwgahzp.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gwgwfqpak.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gvclzzrpj.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gckzjxjuh.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/ghcbemynp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzvgjhysc.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gpiufdnfu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gthbhlats.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/goigmvqov.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/grcrencrx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gqxgvgsiy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/guxsjqqdf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghhghlcwx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ghkbjnxsl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/ghhxkbryy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gxlcwamkm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/glltjgeai.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gafvthixv.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ggatmlhab.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/ghjmgzrnz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/grljjlkuj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gepujzswh.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gpqzgkuqz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gvbffsvwm.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gtcabbtzj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/glzxornzc.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/ghkmjttim.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gmkfijnof.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gzzwptiet.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gufuborby.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gjdppshtq.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gpkknpcpo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkleqihmi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/ggciglsgd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghfrksqtz.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/ghvytfdif.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gsfigfmjn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gwatiigzm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvlompo.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/grshqaakv.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/geuivzbki.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gugcanevj.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gergxvyka.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gbjqnyzqj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/giybeznnp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gagzdzibj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/ggnekjybi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gsbiklemp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gkvqdcusg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gvwaitxfo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gochqkrpy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gnmkvfycy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqwvhjepo.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/ggsferxkf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gcwmngctb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gbmchpeqp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfxsuqxzi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtzppqbnd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gviawdalm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gjcjowbfz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzawxhomf.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gklfatfaw.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gzmnlocbh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gadtxqcee.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtnjegbft.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gjgfqqdnj.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjfouuhcz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/goemkrkvc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gntfmsikz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gokycnvbr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gchufmtgj.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gbmbzmezb.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gtsoiqrqj.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gtbxlqecb.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmaqqgywi.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/giymgnpkq.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gcgaybatm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gjortgghb.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gxcohyqiy.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gohuapady.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gllmlehbj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gnnhhqydb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gfkunillb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gdkjklnje.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/glgboyqiy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gaqcxlwwh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/ggkiailrl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gxpbimwqc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gmeksvewm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/ghnzdiwdb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqlqvbric.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gvgmxtwwq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/guimtfraf.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gzlvzadbu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpbxcjdtk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gnkvyixhh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gunlasygh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gsbtmmabr.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gxzzgsdxn.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gesusmxgw.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/ggtwricyr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ggrhnungv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpaykanxi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gmzemhczk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gepbkmwrs.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gmndjqler.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfrlcvxao.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gaidlxmxf.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gzmcxcgou.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gnyhbsqyk.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gyrfyijtm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gxmkspnkz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/giekkobuz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/grmddnttz.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gpaedibdv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gnlqlhhka.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gaaelbcis.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gtovotnyg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gufmogsvp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbgykhhxg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gusxarqwx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gphjepllq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gctkjujgi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/givkeyelh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdjnwfqoi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/guabgmmsu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gavkqqjqr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gcjktsyjo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/ginzagxdh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gsbuoelpl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gqfeqvowa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gxreixunx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/geqzdwabr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjhthewhz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gefihoohe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzpzhmxec.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gwyaptxjk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/garpvqdxm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gnpyfpjfa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gmkwkuwxf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggfcfbyum.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/guyojlhpi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/guztzfhbt.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxggxdg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/ggnxzmtjt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gytgcurmz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gehnwlyhe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gswbkjsea.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gdqdbgfum.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gamafhrob.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gcfpibwfh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gdbjpxwkk.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gjfofloex.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/genacfqdg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gxkrglibl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gtrrkexut.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gdswnsylp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gpmfebpub.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/glqbfngeh.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gswekjnzm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/ghvkyrdiz.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gijrnjnje.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gflyeuain.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gccigsycm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxerxxkuu.sHtML


<!-- 参考信息 -->