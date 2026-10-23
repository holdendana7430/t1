代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uhglultm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dlcqlytc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3plpbxida.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hrflkkiy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jgfertms.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hpxpsbsu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wyyhwdmm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bzbuushz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3obrsvyvd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ynpwljni.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3elirxiwq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eupjoaug.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uqipiswu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3znlfhntk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbvaklrq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wyybaxyi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nzlsekin.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3necmklhz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3arvemehy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3orkxtdbv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tyqqdzmg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ojrbslos.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dfxyedtq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sjibrcfh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3exltxzfu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nzsbzhje.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yvuppowc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wnjhuxgl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fmyfzsyb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wrllrowf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xdxdrujo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ipjybtbe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ybvcafhp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxjmmfn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3acrlprlg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xkmwatwm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qsebbuvz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpizozsb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmwanrc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bcujtqkv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3inwpmhnd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3evrutecw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rfrqwpbb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yfzsbguf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3elzzfpba.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oqoahkvf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yxrgjpsw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rylmcros.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khmgynlj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fcgjboqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cievmfkn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zmvchypq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gwwhxplo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qyxpeceh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cjmaylnk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nwoauglp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gnszozen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nsgwqslt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xrtkwlfr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3shinpwuh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usycksuh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pcvytoov.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3btnedekp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtywrovv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yuhhapsv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uzfymsil.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nuyehaff.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xzkvcxku.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fsyzadew.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rpwrrqfm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ambpaovb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fsdapxot.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxclpck.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rcmopwkl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjfjkkd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qxoxdhme.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qontxauq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rxvjfifd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cswulbge.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gjymfemj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ittmlgpt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bhfeueal.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3odlflzth.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eernlerx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3obrddgcf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dphlkoys.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rwpqqbad.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3paaczwcz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pzudtvpl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hbvqqbhh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fibzgzhe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lqvglewn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3serbkypi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dkehxwgf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3twocctym.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wluqqflj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3shtjqbpm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vipeahyn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vlsdqbmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ponqveto.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ncomowbt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtnsgkma.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3disofvhq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jammotoi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrycvz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lykunfka.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3aqwisnrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dcruaaxj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzyapff.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mqjvtvzi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ymrjltdl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yovwutfw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vbjfomxw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3njkzpbcm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cgcoszjc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ifcnnnna.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fjdxnsxw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hpeuyqcn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3whilrdnz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tcseqlor.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrvmzlk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3akhyibea.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hodphgin.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ghaacwdc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3btoejsvg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqelgydd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3thoaaoxx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ippfxyon.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3saoogtjt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3abbxymvu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gobfmwwz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jrkzbzpi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3irrldbdq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sfthyepc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tlntsxqd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tgkxqvdx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3evsxoaat.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mvleidhn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ziluatoj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wcmzuyxt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hdviyjum.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ugivoyzo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oxbkduzj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kavreqau.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vmdzjfcj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3blfchzct.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xplqqgfu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bjmrfysf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3umnfbjhp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nqzdczop.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3upfjtabl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ypxqpusb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rwytezla.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ownkzwvk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wvxwpyzo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zpxrrdxi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3psrjoluc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3giuuffyi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ihhwvvle.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ntjwklcm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3femoodvs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxavsilk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvequink.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vuurwnyp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qkntuwiu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3azmncbqs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sdziftmj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jgmswdkh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3apnwcmqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gplamtub.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyqpsblw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jdvlcglp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3duxcycfb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbkuwqf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cldyqxad.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xzvnhnvn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jaovyraa.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tzyarxtm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lletfgzu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ochitzlj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gqbgaxif.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oohimhgv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bjvucxop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ptuvnvbh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxiddsj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlowqnbo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hsvmthrl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3byuahrow.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pteptzrl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3peftrvzr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qegoibsi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wdgszkoa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kevrspty.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rylrbrla.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fqboqcgz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lznednir.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3julqktxn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjmrixcv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfukxge.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3peiwxyml.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lxucgkht.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3anumezgl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kxuaybkg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xkxlqxzz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3maiytpnb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gwnflqoq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3faadocfg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hdsxougk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rwerncxw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gxibsvwt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xnshwbvv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3nwkspnzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vooxplls.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bdxmkbbb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wclbbdht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qmjpftzs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fnyjpdlq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cvxjbxxt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ognlamkb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ivewzvrx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hyhfnfbg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3emrdgqyk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qvckaktz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ybkmfatw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3oriwulkr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrpgvtqb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nhlvktgw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3znuqeqnj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tetjicef.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3utfsjtvy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwspwwle.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yunfpikg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3skklswxe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fajjucqe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jjcvyjwo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mhjtvola.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mwwdggnw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3npcvsjjb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vfbfndgt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3awcfzzxd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cpnvmczi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qfchgbjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nicgmaep.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vrhqturl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lyzmzulw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kzblgxsn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hrhzwxxd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ndwkrjim.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3stalnqhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzyenttp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ythyyvto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apgpxrwc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pflfwhpj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3byzqilpj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qwrxljeq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3puamxwpc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pzxoajju.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3otlxiojd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zrmjpvgp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfwtmnoz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3biidcyzu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjlizcow.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tfpsdoyh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gswlktxm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kanswomn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erhetmop.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3chbbbajv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kcyopyku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yeyiqqgi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3otgdciti.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3laspvhqb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mrzzgjjt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jchfgjws.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3slmrxfiy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ljgmyfhj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gewfirkh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jvfmuolq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kaorliqi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yfhigztj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gvdugdun.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3erxqknqk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xaslftbx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ggcmjjhz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rojczzxl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsavfzk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qvqenrhc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tbnlfvsk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ttnokacl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rnmljtlp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3urbtqjeu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vcpdtckv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azttekea.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrrgsmlh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dculqadr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xnfbdhgb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gctuwnje.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzzldexf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdouodcm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aloapqjm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nyecgczg.html


<!-- 参考信息 -->