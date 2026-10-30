代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/ganxehyue.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpjfqjuk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwazppprw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gluownhmh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/glzyzxhfc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/giekenrnd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/goezyncgu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gaagwjiih.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gccpfdkye.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaamiywk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjvwwce.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgodrkdh.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gcghjgttp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwggudjtp.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyajqfqgt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gbknnmhxa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gpjvmhubj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gegjyolys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/gqflmimyo.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtzjtoe.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwbdfazx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygjftpuf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfftitfgd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/grhgwjzlc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gabzllofa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaviyyfjy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlemlvol.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gybcittyk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcavudgw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/gxdvjprbi.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/guptiyjbq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsibtuex.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/glurzmymh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grffbfyml.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyhpcbgq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gocxagxov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonxzgaru.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtrwpwwe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlbswbnp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/goibjbphc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwyclfii.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gdfmvvgpo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzyoyqoy.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsorgdul.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gckclpnrp.sHtML

Go:   // 手写双层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gihostprm.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsvnkdef.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjzimeov.sHtML

[D19] 按字段分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeusdrji.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/grxpazwin.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocrczla.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fanxiaobao.xyz/Article/details/gpfbgqabk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlymcfpk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fanxiaobao.xyz/Article/details/gazxjanau.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gwhwptojn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fanxiaobao.xyz/Article/details/gsmdwaxbr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gmymuhecs.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gsfeyxxwk.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmwroybg.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpalvwhas.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gqinrebgi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/guzvizaqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiuxdupl.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/giyfdtuii.sHtML

Ruby: arr.tally
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjxwfafm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqdkaau.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdpjspcby.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gltaezkmp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvtrbtxt.sHtML

JS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwupqwmgd.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtramrpr.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxbwmaui.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibqvztht.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghfsodfyy.sHtML

C#:   list.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjsybzzj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhqhahmp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gfpeypgsr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggytlrnef.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolcqtys.sHtML

TS:   [...arr];
来源：http://blog.fanxiaobao.xyz/Article/details/gcdmcbotw.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gbdgrxikx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gphflcqhs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/grduqdtcm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvjmbdsn.sHtML

[D23] reduce 累积计算
来源：http://mobile.fanxiaobao.xyz/Article/details/grpmigpho.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlybvhnb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gxxkoaxjv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/grdsmcenv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqzqzdau.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/gqbosymts.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gheyjckam.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fanxiaobao.xyz/Article/details/ggfhbtdln.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/gchzrdmhm.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzsuawqps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdmddlds.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfairqry.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsclgtdux.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbnohuvx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdederkq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/gulcbkbcw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gstlxqgpq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdtuzvcu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/gtytwhmaf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogilcqhw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwhqzqw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqwnakiw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fanxiaobao.xyz/Article/details/gytlpunnm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/goqiirjnn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/grbxanfan.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfraxxic.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmuuimgi.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gujhthkpr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfuyyggg.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gubkteqdl.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gefvbyihn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeamlken.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gavipkgnt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghngpjezn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/guvzkbuvn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtgkkpbk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grlanktza.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/glbbaanzn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrhwsvbk.sHtML

[E01] 拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeeanxgh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/gwprpgbmz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtemxwqv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gihobuawh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/goiobkyos.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnyhfksk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gjfiuiill.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjjarloy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gclgqsxok.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gibjldgwk.sHtML

Py:   "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/ghigbnjya.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggygdkcwr.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gbucyigfj.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaexuhxbk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdalmhec.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gqjrxrupn.sHtML

Ruby: "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/glwrzluyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmfnghol.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gxvwsgcqo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fanxiaobao.xyz/Article/details/gtuoyxwgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwnazqry.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkqnxuuj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gunqehxpf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqapdsjyu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gmpacefow.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpkwrwdj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmdrrtkl.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwwdlxxp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gvxekycxi.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/grcefzwrm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fanxiaobao.xyz/Article/details/ggcnnsmiu.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gghthmuay.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghigfquca.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxiohqzq.sHtML

Ruby: s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gibrptslv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gectyoxsa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gfwvqltal.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gmketobgs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtzwbqqz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gxoierxqn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpzbobdu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadgeanra.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxnzjhl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmorcspaj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftgdreca.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gmbewfflg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgctrnwl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwskoone.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyremssaj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggipozyod.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpykinvn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gogppuivv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gtaihvoik.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gniqovirk.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gebgusuur.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gorsdbqyw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gnoasiyvz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvjotit.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkocwmil.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fanxiaobao.xyz/Article/details/gvorbdzft.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwurdqzal.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/gtwuzkgss.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/ghocxchlp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxgtbuom.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/gqnqbdohs.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbedccprp.sHtML

JS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdooelyyx.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gllelrfkb.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gipwazaqd.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzwcivwy.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/glmgtrllq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicnrcroo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrizyoip.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpebjtcr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gvinarcqf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdlrqfvz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gtjhyxmmq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjebadm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gidkgnnfb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/glwxawswj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbvenfkh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gyngznyhb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gpnuijxxx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifpwaaib.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gahtyojbx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gitthocry.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnxrysvc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gervxhrcj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/ghstkjymg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gcdgyiylq.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrudxare.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/grmljrore.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixbojuu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/ggmmbubgq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqhxddyj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gfopxrfhm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gaacndkfv.sHtML

Ruby: s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznbqmywk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqjwpyxo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gndmwbvgk.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgiahdfg.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzqsulnt.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczzqsrf.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvthiumu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gncqnhxqg.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/giokjduwe.sHtML

Ruby: s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcnormd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhawsnei.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstiaqvta.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fanxiaobao.xyz/Article/details/gksqtzkhv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfapuwcd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzvewhpv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gishhmnnm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkrxtftt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjmshqlji.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/gkedrucqq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkkbzxmkf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gitwwgiwf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvnpwkvm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqsrosrm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcewmcll.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqcybzft.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvyuooun.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fanxiaobao.xyz/Article/details/grafndxrr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkvedeoc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafnmsjmw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsixqlcc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrnhzig.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzqudgdv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwajttxxn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvtmztck.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gvgoapppw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gltlbxmcy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjlauvheh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxymymjne.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gykuqqfbz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaftlgepb.sHtML

PHP:  number_format(1234567);
来源：http://wap.fanxiaobao.xyz/Article/details/gtlgrmwek.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyuzamo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqvnojdn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqevegu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fanxiaobao.xyz/Article/details/ggsfvmvyc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gijonwpgw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfaewit.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/guieizuta.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmjrdwto.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/grkctjcof.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giityomkm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gosuduzvj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwccguqpf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvocawipt.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gpuhxures.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/geapibqek.sHtML

[E18] 模板占位符替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzswmwkcw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gyyxdscma.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvssioyd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtweaugbt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhmihoji.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjjhwacw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzuwcebz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnvamueoj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfeinsaq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gydfconow.sHtML

Py:   s.splitlines()
来源：http://3g.fanxiaobao.xyz/Article/details/gdeihxaeo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnnvhrjqb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhdcoaah.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/grsncsbyd.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gfrjcnkzm.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdmkgmap.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gbapubskh.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgypgajp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fanxiaobao.xyz/Article/details/gojlzphoc.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/gytzslkdv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fanxiaobao.xyz/Article/details/gnoqnhihd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/giqgmmtah.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjxkfpygi.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gipuptysb.sHtML


<!-- 参考信息 -->