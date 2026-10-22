代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2knfyzqxp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnruiizm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxwblmsh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2shvcrcpp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcwlimfl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kvwtcdqj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ayplglju.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mxkeyamf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcscoxu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vnpxbllb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llmqdetg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2drtrjzkf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tffrnycz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kqxbybqi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rextpzfr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ehxwbydm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vegyjxof.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aimwotoi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xctmgzcx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czrjzwhk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ukvvmnhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vorlukwj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nsyenicx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yjkxlfjd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2csbjgzge.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2itwvkrwf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2prmkhyqg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rawrguhz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjmoetz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vnorpxjh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mynjhspg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2plosakyb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vnyjnktx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2knoxqaaa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2myepeelt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wltxtiaa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ycegfcqs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nvsnyuqp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eninqgjf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjeyxbfe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lcuuzfnu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lhcitdto.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2asrqhlnc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oikmvyzh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2klbivvpq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uazggyze.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eqcenoyy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rocfdvsl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xbkytzbz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wvmpnfil.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fqqbmyvy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gskctwgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myzlquzs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vaggnkiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cklhswku.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mpgsuwun.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nbxzkkax.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gslnsdpj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xpubiity.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2onxakniw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rnsqqttl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vsfgxuuf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gmxnatvh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gyxaurgs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wqlpgfeo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uaghwuob.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhpmvsq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2evioycok.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ievgrzfs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hcvnbdkv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rahkldho.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2modvmpwa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nddyriet.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vkoeaddg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ipfohicv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cxkgovqq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jyibnbbm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vvnmtroy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmnuutki.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vouiqcnu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jhxxyvyz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nbzuukbf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gjelzeke.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rgqrprgs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yssvatej.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2olblwgqo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cxctevet.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zydgepho.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qucvkllr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bxkhaiol.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gqhtgkzm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2luzwcoho.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rncnvwhs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2keyqmywu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mnuucbsp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sfvzfiev.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bzutyjoq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qxtwecie.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ifohiiqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2omaovjyj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nrhnqdwq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dbetlsgw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2psyzaalk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tdgddfku.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kiiggewg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sufhjznf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehlajmkn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rdcuygdo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yhbtwwyh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zjfgjcim.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wcmottof.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hinfqfxi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fkyatrpo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2saatuvym.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2akelxkah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tblttnie.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2bgmdniif.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2olgbnfcp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2etcotbns.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wtoxbgdm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2agskihqr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2podomxgu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vrhvqgrl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uijtvmvk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2doitdhpg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nwdvflvi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cglzqvsh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kkhsqauk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yexgydgo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nsiugeke.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hsgzgpud.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fxicqonx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mbjaybmg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cxbrooqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gsdxdoke.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pmqyhsey.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ejhvgefu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zqbpxepo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2iinphxtn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aaktqasn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yibasbnd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2coisepto.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wqignslj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rkcbixho.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bxbudmcz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lsdpskqa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2asibxooz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwtsczsg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pwdthgdp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rlwedtgh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tsxunukr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zjjlcorv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rcgezmul.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vcdqhxdu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2atuxnsia.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nxgaayho.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vxbhuqaf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gxglguxp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2idpmpauk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wzfnrvit.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2swkkijnd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rajzixdf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2trcnfpxk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jzadduom.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aecetfji.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnkpxkxj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2psdfpxol.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2skkegnox.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kypfgdoy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zzarvkza.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gliafeia.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2otyfeltt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cqrmyfvp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ijkpxmhu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kwmwyrxk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtufuby.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnoxuxk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ldrxpyge.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zamngppm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jummheme.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oknltoql.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zobkflzi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzxgugis.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kbjbgvyt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpczndmk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yjwswlmu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gvikrfvt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2euzaacqu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgkxqjdt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hedebvxx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sxglerxu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lgpewrcs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bgqgxjse.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tignxths.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lsrlmvou.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nsxwnpsy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fiijubtn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2itlgcsgr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hdfgtihd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2flbmjzde.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xklwjmqq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwgecxdg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbulvizn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bengwprd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shsingqc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ybmotizf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2erlvfjdj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rxadjjtw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vvsmtitr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2brxmcsvf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zxqqtjbv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2svpqbkxw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2acpxbwkq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nslafdng.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gjugtohn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xlvgjfbv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpzjodrb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nzyvaput.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wvndelgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2khnxqeip.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vanulgey.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wkrjspge.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhbpgwfq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qazeovzl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vbmfonwb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vvdnxpua.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nvdjzylm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xwyoyabf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bzndflqp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2scafsqko.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ktqbejut.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hruwoasl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xqvsdbii.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rdamrdrc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkoizgtv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eowwolqq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xwvdgzws.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sdlfenby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2onmfpqdh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nnmjwrco.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kybdevkl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yjznuwbx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fcozytkp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kuwuaszs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gyrqeyxr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nbjcwdaf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odsmpuiz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvppylib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tqusvndg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2spbefnpf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ssqyhlhu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eyaqncsg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xbzgthkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqnlwyqr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jwbcckug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehnqyuns.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjssxwrj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bomojxlp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uhwrddfw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jvhwcvin.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yottcpqy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wlfgkgrq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cigphkpl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acotwamb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ivbgkgdv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lussjcjc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2azjqwhje.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wcmzkjza.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqcisblm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tddwaewx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhxblfm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jjfvidvy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2aylwocez.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvzwstmz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pisptmzf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2plqhqijl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tgdvuyyk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gyvexlaw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ubckxchu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2elknfgkw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xkaqsiin.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xjsnerjk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pepddtjt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ssqcekcf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vfywaziu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jfpdtfwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtbenqcw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ruxcgtqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ewhosona.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2spgdywjq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qzohhtpj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pwcaseow.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qigtpimq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ungdwdkf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qsljddrx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xsevojzh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzfkkrmi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mwxtyvhu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tdmucauf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phpicbfn.html


<!-- 参考信息 -->