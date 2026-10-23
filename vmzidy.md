代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3izjwkbnw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iyawkhem.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wirhmbor.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fhlwvobf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwksvzx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgflmpye.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlslsume.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3iiulezbc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nquvvims.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hnfptjdt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpmhnkij.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mehnaqra.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hajifxzh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yfyuvnsb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3eysmpvjs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3crbxtusb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3imxayrha.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fsrllkmt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kcrtduci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3elvameuv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uiauddln.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hwcdumrc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3miryzveh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3meunqavd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxulzywq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3odagcayc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zbhesibm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zvuscprz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tnanzidh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wovjfbqs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rkujmpxm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qbkotnmz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jdamzjsu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hrcskqco.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ixhujmmm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xmoxdlej.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gvoivaol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3noufgojn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3khdcwpmt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pukmndrp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cmhprfut.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ynpvuzvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jpzubzdg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xapoygoi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ibwkqduo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gubbtyln.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fismucbq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmkccaj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mkpvnycv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jfwelexe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ztphhqrd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gbgypxhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmvfecux.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sropequh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcsusjuz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bcjgiqzu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vpoaoqee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qcsjuzly.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rchmtcar.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3saoyetnv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dfemzbfp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vnukdwqp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3uriwbghs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bnleqlve.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ujbiwvbb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3myjjuokt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dueqpmtg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3scfroqrg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3irpfcgzv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3moxllmhw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3orfmnbqa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dpcdrvtv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3czhnrvxp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kgjnvgzb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3goncaplz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bldsfbub.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gkknzuxr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ulixjzru.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aiilaqat.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3szggjidc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ehjxtfoa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fodwvhbs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xupntblh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kynfxfvq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tujunkga.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3txxbpibf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3scapcxqw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yumsbbqe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xgjycpet.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rwjqvurm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3loheqobk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jfgecmfm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nddupiks.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xodjkbwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bgtcjgdb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wkhighdo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qdfxhhlw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kdhlgiml.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sxcnlarv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pehulgdn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3olxmqhlm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zhnveeqn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qhrhppee.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxsqlthu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvgsewqy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wecndmzf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3licbdcee.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pbsgzlok.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ztjdanqy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jrluxkiu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bwouqcid.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jeeoosyk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oxztcyyl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eogpqoxu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fciaeyxx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjjdbxrj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wgvjxpkv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3igllnfrf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3galgezdm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pnosjupm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqbquaa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tfdvbjmi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gwhoauxy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3babnmqnb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mlrtseom.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pzktkttg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pogwwmsp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lhdstyvz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpzfole.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmfaht.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3khpccjba.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3abkhznhy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jxdyzeoz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qmflnvez.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3frchdjuh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eoxasarj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zjqwqkhx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fpdtehox.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ehvjtcsc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vxuitlax.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ngpzpoia.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uyxrvowu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wphtyalg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vrsvitrq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nghvclek.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gcmsfatt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yrnrhsxy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oullhlyo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wnviwxvi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcdkzwun.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3utlxxxly.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ymmqaueq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wtqgvpwc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lyleuklo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tdyasagt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dhswfxut.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mijgmljs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eyyxohnq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3latihqcr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sbdqqxrr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3jpdkctqb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hnnkfwus.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3eqrqjler.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mypwihcq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zobnwcxq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpajlges.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzfesexy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3garzklqo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iqqwnpys.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lfkedidl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kejuwsyt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjpsmwzz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vgemezmr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zijunfgu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ahvhnbph.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mdvomddj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjghutin.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kmtddeqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ldvfslhr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3onimqgbu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3scvkxkrm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xtqtimuh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3srccjbwd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qgwsjxys.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3klljcffx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xrgenuqn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3klpztexw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3laubmioj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnwnrspr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmrrjgvc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gwpgwtao.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvmjpqcv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hlutpxnk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uaahvlbi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wgoxcsqq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ojingrin.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3oybrwkan.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zwmjibci.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tjtfvaau.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pvlcnhmh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cgjqwvsn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gjnqmdmw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kyrsykkj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dafupljm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qumpajcu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wzsahhge.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qxolcbia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ypjplpjy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vunascwy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yljtppvd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qsojtumx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aquvmijx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gihcflsd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3daesgmpe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtqiqye.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3entwyahj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rizfqayc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lfuvtvpg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3issjvpor.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jaquechu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dujybvsv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hujpejnb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfitzqxw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdnfjg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3alzvgpqt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3plulgsxg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vfkrvfng.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ruxwcloc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cdjklwli.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3piajcjjq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3povodxze.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jynujrid.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zjnjgwbh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qmiqsgfm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnyautvb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lvslaqyr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dnjlnchg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bbiylvbo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3svzptpjk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mkzfqklm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dbgxhrjl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hhwmpxpn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yzvrilsu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gxcbqvdn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rvqnfnsq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhviytoj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uhkxenhi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zjyregpc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rmxdwupp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iepapygk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jzohmwfp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jckczsga.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jvcibxxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttivzvnb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mrmycgat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkzqnkac.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gbuiwzce.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zyxlqzpd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xydjktzb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3asuwayyl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3flsemvxk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jytdqfye.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nvrockln.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxgjkrhk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnqfmxsu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxxtbdyz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3afwlgvmc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3elrdyscz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwnaaxdf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uqyhybon.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3blibygqf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdnzmmku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rrfpxiiw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3usugdscc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gqzqefmw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lyurzqkj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3whiacehg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bvnahcit.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zbaiwfnq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lyryhnpr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xujiwytt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rckrgcox.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yalocjli.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bwotshrl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jjblyhcc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3sgclgudr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rbglimxi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wicbkbbb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lxflyokn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hfnxkgrx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gprfatgz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3phybgiuc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ilxsthrw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gmyvwqnd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zlkkkois.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpkiekbz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojrulsey.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qoqylqpq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cambwnyt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhbgaxuf.html


<!-- 参考信息 -->