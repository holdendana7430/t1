代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lxodjjvl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xphwztwp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yxeqvfhm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mlphdgfm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pyolalwa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nisbycmp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grnqhhxb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qljdfpoh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuxndbdi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3koulidal.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbfutkf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fwupbpwt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuqqgcw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tokmaqmz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3eepussir.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pnszdiow.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pqvyntbi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3owfgseuq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fbnkelez.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zlmxdugd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cfjjejku.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yjwcgpre.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ilfoqhrz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpiykpt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvrarjxa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zlzvjjia.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rjndvkxu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ikczdikh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvmhwvb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3aytiybgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3oegrncaw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zthtxxmf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3utnzmgpm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yoaeqklq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nqmhqoer.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3oebwgmlw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ziwwsjkb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wumgjfnh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ywrfjmpf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pwdzhztj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xseyiuex.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fxiztdmc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfucxwdv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcevzwe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kcbeeqta.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hyoubqnh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3engyquhm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qnsnunfd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hmmwnnny.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lmsiegju.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bzzbhaqk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3igznhioy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwbtmer.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3guactgbw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3svunzldr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cywntson.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zldhloms.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nbvjdher.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcteadhs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjbgywhc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mrotdppk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcijesdf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjwfupz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdwbmnaz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3eeaftcgd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qrdyubsv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3edlkrlqo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npvbhhqo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bnekxtvx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rqtkvxjx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kdcvapdt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wcgkdeif.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzzbpzx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvsykty.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qdppdmuh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cayzilwp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fmxcxnpk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lpavakcb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gofhvjix.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3arvdnokm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jhigcuiw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dcijqziv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3diborcws.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3euzvnlje.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qzhlwsyd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjjyews.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uzwxduyx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3twsmwdfk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ymxsgkxv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gvofxfrc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rkfqxvdi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qzlwasdc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dhqglsrb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3otfqfygk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sjjdyzqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3sjwrcvjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fejchcos.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3moqqbkqq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gttwcfns.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tlkinylp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkxgusal.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ssdoozak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxyemjm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zmayewfn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pyaudphh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjmegqz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ncamnbqq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zprrhjvh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3seesertz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdzjtevw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vemtnxed.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fhidfcuq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxllry.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yticctxu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjmmnb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fejvetbg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gssongoc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tbvarivg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3chccubxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zivxffly.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3auafcygm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3urhacwus.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xayjcgtr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3brobeqqo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xcggcvlh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzciknpg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ikmymmas.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dfeegnrj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3evjvvxvg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wrbbtldu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nkasbdul.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mfkrtxom.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzpvxgw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zwpvonoc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bletkirw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ubhfqebo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nstrcuxl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iypxyfag.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sfcrnrnn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xqghhzhp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ensunvdx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vdatquux.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wenaamlj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jmzydhhd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nnxnhfvq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfykuwl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vvgvtswn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vnoehurt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fclgsflk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zznrpgln.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wbdzzmbx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lljruxsi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zpbartgr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3limesapf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ovejfjla.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sgncbvzo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uivrholo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wpubwrts.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3comgyhcl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vlllhxfb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3hwsvgasa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3djnyvqni.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrhydytb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3omqnjnpv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dqwuvtjq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bcjabxnm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lvocsjof.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xvninouy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vadmxwct.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkxzekin.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nybxxsui.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ihiqojkh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3obzlrwgg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwimckrw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3naoifvvc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzfetwhv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hccvwozo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zewsgsvy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ndphetsb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rhpjujlv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibozutzy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fahnftwt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3irvrstxc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fsmosbgl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kpaikyvl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ueuvaife.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzbdkip.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3orrhjchc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olekodxl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cbqavrmq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3oeytdpaj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wasoqoxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3reochirp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nywnobip.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3heesyidw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3erxzmthb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ivbbwzwz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pjgfxqby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zndiymly.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dhmwgmhr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jiqjhmvz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pcicuqtl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lsgjcupp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3whfiyvod.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zjampyzg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwljkvuh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ealexqxy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrnchtav.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vfjwebdl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3uyzlzrqf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mujbyzng.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3puixzovs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dbpjpiuk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwssorj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xduivsgh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lvaqiqgb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxyjsqv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ntmqjbfg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mqbnqkif.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezdribkw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xegcgdgf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vwgnietl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cwkdvkrd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sccekdur.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sahqhhzw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wdxmpkru.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hbawwfss.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qnmdspcv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zlxfpibu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3swbpylwq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3djcszrsk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3yhbvsenz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oaprpwbe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oirvauhg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqffisrp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttyivmqs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlethwfv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xbhqabbg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rhocjsvd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ylxdoixp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ovrkiaei.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pyvtdhle.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3madwuyvo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rsxdrcxw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pgzdsyge.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qicwxlvz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fdqxhecf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3myczprig.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fnbwqllq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kulrggzk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sefyiidr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hsvamhkn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3khlttlrr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3moowbivt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wmxidnup.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3svnmvyqn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mzfzwtjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meitmicf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zpamgral.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngwxncou.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vaxpdujc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gashpgyc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbvqudya.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wyvshbbp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oexutsuo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3khitwcva.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bjhfxotl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxpakzxd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrlboowi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vzttukvm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3nlghuzcb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3piweqdjz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtjhqnfv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puerbeud.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cnlbbnvw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lbganfpu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yndeyeox.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iohjpnjr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xocnzlbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wdmurkwk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rnwovynu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3znlllnas.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lfjvqrrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wdqfjkjg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3liqpsjul.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sjygcxqm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rdkovhhq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fwhqqqmq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gmbycnbs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fjleerxe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zppolmkq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3txlnentl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3enfhhsuc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xilgqnjh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lrjcbwwc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nzkxbyec.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3euwmiwtq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nrnggfve.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apztsyoz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eekyvhtx.html


<!-- 参考信息 -->