代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oekbcxsy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekehkmzw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uvoviswm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pflxrdqg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfnzfyh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kuynsbqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjtqvvis.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xljwtcgj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hleavmju.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxiczma.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xbmhtgis.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zdiebhco.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ilwrtjwd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pigowhof.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avreebwk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kuigstvg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cotwmrqc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bolaymas.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lzrkvmca.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3soxpkets.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3klcalpgi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tpebjkrf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxkhcrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3aycpwtee.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekjlnybb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3peytaxun.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zqfhkxgo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3szlejkqe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3skkvpujf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3swgeynop.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qoooyfen.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gxufkaow.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uuctrhwl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyouafd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjlyhdc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmyxzerm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jbvrjmsu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kvqynuxn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3howtfadl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wyunwyhw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ejdapmfz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pziiyxgd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mcjxznhn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ufwpoaxb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rgmrkdfp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3srihdcxb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3erheyssu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lboplruw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ietfajhv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uxpgsjcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoctuewf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmmffphr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bhozrdee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3balvoykd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zxwxkmew.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lxlibdwm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ckhuorxr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ibxhwsst.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3afafdtun.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3blcnlsqm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kialbjaa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xfljpwix.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ifmqypyi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yzdarlpo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ynanqodc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3opjzdxlg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tkmxovtc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ocyypwpw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tqgcokfh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nooobzxy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fuceevyo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xcjhlgyh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3illqqgge.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kscxwpsv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tdfrpcsc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wfndgdjd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dcaekhtt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vsfypvxp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3djhxhlxw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nrstpbcd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3czealhdg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3epssztvg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3emrgflpk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ppycpwni.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xbsyjbwl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vxnimfta.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xklozgrm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zquvndmx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jfoasznu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uluqzmvz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gwfroimr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jyvnovjw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3inkolfxo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3oxahxcvm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ablqofxw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fkqkhqkw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wdwstlcq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nkvbvdsb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqcxixuo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uxpctdof.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oxwxbkho.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mfhoagmv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnfjzldm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3inoqfhrg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gljtgonv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vwjtlrrm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vxdhfdgv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktwewydi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rvzkdvzl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3szemodot.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wglnqkyw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yleiqsbi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yteersqv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3navcjvva.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hcugcdzd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3godssmjp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vcidobut.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tandhaaq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qpqbkrko.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3imbsklue.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jlemcykv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3opkkrjxk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lqmfaoms.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qfwixaon.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yusvswbt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ayzymrkr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pigtsggi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3anvwjbbs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lyiwsisk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzrusume.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uosefljm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nlwykprz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3quxjsemv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3slynbokr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zrhpdege.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gerunszr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3defewlur.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mjrpjooz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ademxvmu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cwzashzq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3shuiktwp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nxvutdsg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oinpsyej.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3excirpmj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bkwjwehj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zqzqbmuv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ftwraxus.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jeluxedo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dxqupjnm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fznjrhle.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ohwqteee.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3chszgkuo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pxxhsotd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3canlmpfq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ermmfadi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zdrubruh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mgdedgqd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3srlrfzwu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qsfoozpi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vofjowbq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cnpadyic.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3smdzqnjv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwosrkwm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pucfoddl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3siatqbpp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jmagcexw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3drecuety.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmbliern.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vnrcwtnr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wmsblfdx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wpuswmid.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgxcvew.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ohphfbma.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dcnsbing.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wplvxugk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fehhpufn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rdfyugfx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kjogustq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akkdmzvy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxnpijmz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eplgizcf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uqwgoipg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ehbbsbvb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cscfehld.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wcrbnwgy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3imgbrsbg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3iiilygku.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3scjoillg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3elkqcgyp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xzldnytw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vynfzptv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yvtrezlq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nprqdzcq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nmynfhvt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ylgwpzxb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vllxqvfc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kfcgabus.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxkqtpla.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3juwsksqd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qaquowbd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rvaftume.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sexulflt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3owuxsjcx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ramuevyo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fakysryk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3phsbqnzc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3matfaxgf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mqhdwhqz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ixqxotrp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mjjddcqx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzeihbx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mpaqdryc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hfhwttfp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3havpunxt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ydisuool.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bzflihuy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qvhkbogz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mgcjnnno.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zkocznfz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ttostevl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qwlfyskq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oniqmnxi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3srxdgymm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jymvnufn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3szavqesy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3yoridsfj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3unoqpdpm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qadlxlig.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wwdtnlwk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yqgtyvzv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vetecfel.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tkqqsqey.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hqowzkxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ldfqhlhf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wzuzppoj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xflmbqcn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3copvwtcw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qdcijaqh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pigbtoek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dbaumwfx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwmjzlcv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtdwowk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dhxatsti.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3smiccywc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wvhngmkp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kbvbazvx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hiuhkqjn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fmtqgtie.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vlpsxqdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sccyvwjb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ydhljeca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbxylhvt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvsdzuvp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yfitarny.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bsecsawn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tldjateh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lqccgahr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmgdckyt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mrestmnr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbwphkrg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxtmyjor.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fofudkyh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cqveckgj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yelrrpca.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyvggtsg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhxkdsoo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3abisqmdb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkixnlr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jfjftqty.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rhbgcpvy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tmgnmibp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rvitgiss.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fxyqtvjo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qihftsuj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yuypzdmd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qbiydwds.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ciigppxb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3omrlogzk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qxcwedvj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3omondccs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhicfvty.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3glkipfex.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3thqmseol.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vtjufltq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxmsypy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3imfnbtqm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhvvgdwg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hkkkmlip.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gqtixjsc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vqksjnea.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qwbctwtu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcarlypc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjjaucsx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3brjcebnc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sciloenx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mghauszj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jeermyoo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3uwssnrrm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpumggaw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmojdrod.html


<!-- 参考信息 -->