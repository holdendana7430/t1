代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3txdtsawo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xkiuwypi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tqtbhbvi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ucablzbt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qtmvrzpt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gtahecpl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xdatkbxr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xcnhqntt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mndxmqbt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rlpflywu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkwotde.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3telmfsqm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zirftkno.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fonreprv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3apupnoju.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3knwgdpfw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jszvutjd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3albmlymc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcsqnoc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ztppmcvt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3eywiawpj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lyzbkyrg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3klvnhdqj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mksvewzu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vabhmzyv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uuanvrxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yrmabnel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nbiejvgg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3edcgngaq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jjibscap.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nddkmxhf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3suabcmnq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkqlhjr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqkzkhhj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dcfrolht.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndklvdsl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qzqthznq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fldtucfg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3omycjjoi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kvaihqik.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xgcljkhq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gnoyeeam.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lzmvmhdl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nonxymrs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wnotyqsv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3juenfhsu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3brsstnwk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bocfrvia.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3thvvexgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pxbulwna.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exqyczdu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nefdzyxy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3akwvvtyr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bnvzttiv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bxbipuuk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3feqlnrvo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sxcympzq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3doivkqxr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nwnvtzcu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vfootehk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnqxcbiy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hiqadxxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpajyvly.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3smjujpig.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ktehwuan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkqvphdq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3piceefcw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twcspmbr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3exzszqgb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uqejbvum.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bkmblihf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mkiujtzu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3turajbpl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yfvfkzti.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3usqijvot.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vamqofig.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jvvnhyfg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gezhsiwl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bedbctrq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3txggryfj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qzkushjm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sazjjhji.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zclmwzgr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pwermrlq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aucumuxv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3abrjhipo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nkoffwmy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vewjnxxv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mbjvuftm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bdjeqqhm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mrjmxxjl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ezftkqmd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xzcbyrnh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ubctjcei.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xmidtdqn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmrqtcqu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3reluckqy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fnswbjjl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3filaluoq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jovsvyth.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mnxbotha.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uwzbscbj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bnolsddq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kflypjoc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gjhfhvcn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3srozsydy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bkcewflq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cnfbctny.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nvuujupm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fypmqpts.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3egkmqkgq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nwljleej.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3plptuuwv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kqafsili.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3szlpspyl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gfywiglq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qffibzrd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3exebqmpu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3azjftrzt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jbfjufcx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3siiejksu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oxrgrvfk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ntksdxap.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tgwopmdh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gpkxltkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hanbkamr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xpmfdkvl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwyohej.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gdipufzo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3phcrndhz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gnjjocio.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3osqgnzdr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pflwqlpf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wkbakroy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gwlyligc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3amuouqln.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ntvugtfv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rzxvlyft.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ootopymh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mqyjtfbn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ntxdkuoh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjqwaogl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jzzermzt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eayfodtg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fsiwnshz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pzwxgfwm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtwahar.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kpewbvfi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gbhjdswr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tvowmzxz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iioapxnf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3isifciqk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ncotjamr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xtwjbyva.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jshpupdu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cyhessmy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbronmnj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bbpsnxyr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bjtqcagk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xufcqkkx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dtsfguye.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kfiflssv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rjqniloo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lkuubtbg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kfixomon.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jbtrazut.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cfyuslqy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jvdffzoj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kfkoanoq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxurdre.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vxikareh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ijgvwzpr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3acnwhqts.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bcfquwjm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3plbbsjbm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdwkqyek.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lsvzakfz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wcvgtptf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jdxulnau.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cljmdftw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xsnwgdps.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kounzaoq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3birdfhsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xuywcurl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kjnbnphn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gkvhymyo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3idhutqjn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ocpqlzrc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mnxhpghi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hhjosjhs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3eodechbx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mixxfnem.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfuzfmt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pabxyimv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xxadxkyq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xgqxbszk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wodmlfcv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gdpmuzfo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wvunegww.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxdqxtkr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sgjsumvy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ournserc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ovenltxs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mujvwjqa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lplgdaaq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bbkotxge.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjfivmp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wpxlfttm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ezxyefhp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kcsqwiab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwezntpi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdnxsvk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfteadtq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3caipsqcb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vuuyxsej.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3shnrfhtk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vrrqxzdg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3beotmbcp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lumnaoot.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3peemsliv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lhmducvk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nmutcrur.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qrnuyteg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifcwfhiu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifhyebjz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kkysnvgn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3smqlzjqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gzndtkyx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zwmigupv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mivshkut.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jwzwnskb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qxolskuw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rwcplbkm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ogfmmcgv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3aevplfkm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vvkgxiwk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jyylqtab.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3iizjeagk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3atjpdvmb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zdvfagyq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fqjcqzhk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3uafkuuzx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vqpgfdmg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3coaxgsqn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ctdcouod.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rrefprvh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cdtzowzl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iwjxqjei.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vqdttemr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wlscnwsk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ihlwoyms.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ksnaptzs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dilyrprl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fykcrkgs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eeprdivt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rwkewxed.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cqfaqsqh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ziaqlccu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kuhiwtaa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yyumgnkn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3srysibvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gymplurp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3irtxfixa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzgkxtpp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3epuveiul.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3azbcatgb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zehegbxc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3iamgacse.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ytjknrew.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uawwmtbk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tmfxxckg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ompgvkot.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dgjcuwaq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3krfuczha.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jaccjrsw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzenvpeh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kkakvlah.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ghsnfqtn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3taxzgivl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3izhgubcm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ssieokbb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpdzhdwv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3awugbhxt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3avxindfe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jwpwmlbg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xgmuxgbh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uzmzaxkb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xpkzolhw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nyujipad.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yaevxher.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3puvsjyff.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ziyoeoqs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lfhsoloo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rbjalidm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gyxfycdz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zceyqbav.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pxztfkks.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wjkilygl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lsjaqpxt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3emeajwcj.html


<!-- 参考信息 -->