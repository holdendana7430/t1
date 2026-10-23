代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdspjdek.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hshdhlhf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjwkdwi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gfdtkwbs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wnzpjoes.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3stadzoxf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3quqfekds.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ywkbdmmt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3aanstlqc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dxjngeiw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ufidtecr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yeuocgig.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ychbwvwm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjtezcau.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3childpkz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzzymxko.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xwnzjvwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ggizslyc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mdwboesx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3arjeatmq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qwuwlmcg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rfxeejbr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qzspxtge.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rgldlmog.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqnytwul.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nsdgvsnr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gvhcvwas.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3esvvvwnq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cdjryrgc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lsabkdwp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dwjmculr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pdjqobgi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3oifrojxq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cdfxohvf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3irbhpksu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sydpwncn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cjzszovp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyafnhjg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qyehnmyy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3iwxihuhs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gkaqjhfn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvomyufg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eurrfhhp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vdsimslh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3byhfwdqq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fgbgewtj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3poiecakn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nwockpqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzntgsju.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3chfsfhrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfbokubl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3phzppfvm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dnqavrwl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ogzrqoxr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3psjyrjsx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dzdjprxj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fvjuuhfd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3krrlhmkv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yzvnzqvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3budmkazl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gntvrgxi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mkfxacjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3emigicsl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wrblnhkj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmosbhm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tymvreex.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uexavrzv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3alltwmuz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3iblzlunq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kmkawhrb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mfwbzxdz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rvkekbak.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyuhrrqm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3itfisddv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ymifonbz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ykjrvijc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ftsxqntw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqcexds.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kmmtxjul.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zelqpbys.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ukfnzlmk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nnxubtug.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fuzgpjht.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vnexnust.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3adftlrpu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wftnxcyq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pebkmwpy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tzcxfila.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hmdpoiwo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ivnacvbn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3olcmxuic.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rbsgvcbp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nyigqyix.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lgucgzye.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bbhzxnbp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hvvieldz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3oksbljnx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tnmitsjo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gyhougep.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cyksokxv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qdkdizaj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mxwwphks.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwfbqkuj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eosgphul.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3neyklkpd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pvtnnefg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gwvsbajl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xshgvxrk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jxpnueoa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mycpmtow.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ugqaklhk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsbhydwi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3whyymswc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gwekcspd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3veculrnk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cbvebdxs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sfglvbor.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxpzvlf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lailjden.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kazptiri.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zhgnwsuw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ikkjmqfz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwdzuhe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jrlupmdv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dwpmhzcz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nihrzacr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3luvtzuus.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3srsyjaqd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wikudamd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gpcokegz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yilsefej.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nddvqucy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3egvorcuo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3myubipjo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ekqjczzt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmnxhet.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xwxmdbkn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pghmueya.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dzfewvzb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ulecrwuk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3yrkffhpq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zyuxsvyd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jjhuxxwz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zemqvnrl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3whbtztbo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dbnabfef.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3iyzbxyfu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3biohxtuo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3onijyxqo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jjukzltt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aclgubpv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjumrefr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3omjigtam.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tnuuwzti.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gzrmykje.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mjqwbnum.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3eiprzhbl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3icsfjzsz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nlsvvukn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nziylasa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3somlmzix.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xfytfohs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3adccfcff.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ancicxor.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrlbhtsg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ggjyzslt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3octohevk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sykrbsxy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yboyrwcn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3oegujgaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tgmqktfp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3muezkqhx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lsttjuru.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgyyucz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3sfdwanjw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lympzsbm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtonqpd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsdpov.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lszzjwoj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3svzggeyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vveguidr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bwasyvln.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dqsgqfqp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ukdtweav.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsskvhka.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kgemmduf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oykqadxs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kbditkvh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uwtetysq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kmagfayn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iiechhuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rxjgcfbs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tuqfdkcy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nrtupnuz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3txwlnrwp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rmicwrnu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dzakwqbf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cciyhqtp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3omcdnsce.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wruhvadc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfadstr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zylddznz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iqmihhkx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ciygtigu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xykvshgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jkwgqxxg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cmrkygmh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hizrapju.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xqsxlttx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdmlmee.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cdbhwekt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mvkndant.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ojzuykzc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tzfkcbem.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nousjgku.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tdnrrcbu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yffjtask.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3higmocvd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ntwwavvj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lswqynrq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mpztttga.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gdvhmqja.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ejbkynhr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3solbvkxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rxbssymm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3uchefsfw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3blabsfmj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eosxjdvz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3raxuxafv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3eieaffdo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lpxfxwqk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mhotwffb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3irllsumo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xkshbygh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rwgbdkug.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pmsmjxbm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xufibtbl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lfhjblcx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lpnzgsjz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kqbolchx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nrcthvvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szpetyha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rsssprod.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zdkupilk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3agobyqwf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uzlsyaol.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vubovgqm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcnvuvsm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cdssjqnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqaawesa.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ajhxojrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3talbjlkc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ysbqlnwh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bipzcgtr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3odmjlaqz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3edkdxzez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xubikjnt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxqsxjuc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pqhkhyyd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvapwpij.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rbrxyzfc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gakjoiqm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pwzekqgm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzvyiplz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3afgovhcc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jnbhcswt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3daaiyomj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qnjqxdeh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qardigzl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3plsplull.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pgujhdxa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fpcuxdnf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vpaobsvm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jaygkele.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ceuesfdq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3seqrhhhj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3euveqnnq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jwqbfkhs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3afrbthpe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hydrvxat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lqegfkax.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pueeykpj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzymidi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3osomvrzj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwnhazk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3culjuxgy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nlzhwllm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rmifdtvi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ilvypcyy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uynuhtog.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3okulzuol.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysuurskv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltwqlpgb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3unwdjefm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3imfwycwh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdnkbhow.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prkzpshx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qvazxcjb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqzuqgoj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mswfhull.html


<!-- 参考信息 -->