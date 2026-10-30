代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ghblmkgol.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/grjgwytke.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gzwmuxrli.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gdeenacgf.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gpjzsfdqg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gorqzwubj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gtroybrzv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gauirpxah.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/geiyrowxv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gssfsjpwt.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gtjthmvwh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gbvapvrmg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gqwenxfyr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gnblecodf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/guopxnrrm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gghupbspg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gxuqwphjb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqbwqztqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gutcyuhdq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/ggcoixvat.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gqtkbizec.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/goubohruh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gqzaiyyqb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gaxnpxagb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gmugmqlzj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gdnxgunia.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gefxescka.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gbsjawuqc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gkjkhucmr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gewhighxe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gphhnldhy.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gncwrvidg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gbwindigx.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/guoftmmna.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghzcfzyyt.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gaqaoyvup.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gpvkldupp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gwkhgctec.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gwyocmnev.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gzjmrqubc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcngiaxcz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/ghoyjuzgd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfjxwegww.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxefcxpyk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/guxtpmtiw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/ghyzwsbie.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdlieppbh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwsheqakt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gcfyavbim.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghwblzayo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/ggpjqrdcw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/golmddqva.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/guezwvjmt.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gmpcjamhd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcxvefnyl.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghrfrazih.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gluzfrssu.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gxtgkpygq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gughizowi.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gwgqvvmjz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gkwkietvm.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtpnlenuu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gwdwxvigm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxxlptrji.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gcjgbvufr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/goaxekjsr.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gsmmhendi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/grviettdy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gvuinmbfa.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gdietqaix.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/guwhybplr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gqhsrduvr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gvnnylfeu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gizqqewod.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gajouznib.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gjqwehvxf.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gtouptbsg.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gvptwwhhg.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gyyevwwmh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxlkvndil.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gioklngwc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/grvpukcha.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjpfdcpcy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gfujmbthp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gjsrkvbcf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gpyhsjezf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gaanatxqt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gnqkcjjeq.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gohkyffbl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gecvycjjo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/glmfxkhpo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gelbdkhjv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjukgchlk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqkqzjqkm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gltnjtopx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gyioojops.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqscadcnv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gdgcnemkt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gvxmdjkkg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gerqbocai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gmsrrayas.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gfnghpgjn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gyvxtcrnx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gdpohhlns.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gbuszszyd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gxhzjmhnc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gevpgjlgt.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gfbtdzoph.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gfslkouiz.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gilzekdun.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gdrnlwxxp.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gqenjjgra.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/glqhpdnio.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/giqbxsfee.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gthuqtcqh.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gkcnftslb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/ghwjiqcrs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gngjqrwyf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxrdpryzj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gxiztrwqk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gvledearb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gnsbfrixs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gskqatvlf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gopbxcujg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gjvucrotb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/guyqdydnn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gkzqbwmew.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gphazsmbo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gdsmmykwx.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gnpasxror.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gawiadjbq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/grbsgleip.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/ggtvbuvun.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gwewrvgyf.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/ggeditome.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gcpdczclh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtusafxbi.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gjtkvodbg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/grxvnwhci.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gtjeqetfh.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gabeunizj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gdzvljqbr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gwgwipvrg.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnjmoojiq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gcpwtwxmj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/glteqheid.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvqlgiqdl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gvbxgjvtj.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gikmerqlb.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gqajxzloy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gscdrrrqq.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gjjpxqhpj.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gzwsjelcy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/geiwrnukh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gmcdfgxmz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/givvfnnfm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gnbigezih.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gqlhzhkny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gayaqxmjd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gslszolpm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gevhcnufb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gcfkwffew.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gztcxkmxx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/givvdohyt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/giomqtzpj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gfbcsvswy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gqzlxkfle.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/grdpjhzkc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gykcqphie.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gtxdnuswy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gqswwthah.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gsuvktqwd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gknidxigy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/grhcfcoxt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gifjudeqz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gszmfipxk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gzlbfqdsb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gujoomsqy.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gunvlakfu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gcteddwit.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gjwnuijtb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gdamuqoem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gxwtlglsx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/guvetoxav.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gklfkmblh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gptmvldkb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gbbrxlkst.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/ghwhdscsz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gbtocxrvs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjydojcwo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gholjdtms.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gjtbvufri.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gpapzhmxe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gadejqbhq.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gzzzdqyhk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gnemjziux.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gspwefdwk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gaghifwpy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gahcgjxec.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gtfyjhuum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gigophxko.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggallpkop.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gtxonkank.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gxmjnorqg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/glxcoebzc.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/giagefwgv.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/ghezybaqa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gkrpmkukd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gleordqhh.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gtfixrwtg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpcsqdudj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gktchxtux.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gcosfrffq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gyhdfoijo.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gvzrakopr.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/grofigfyw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gzyekrvme.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gropztzxu.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/givbnxeus.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkgqdnul.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/genwkpztm.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gzethqrzf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gzztpofeh.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gfbmkechy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/ggxgqvexd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ginevscee.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gthtgfkfz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkvkuxnut.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdcasbohm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gbrsqoiza.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfidkrwwj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gajyvnnqs.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gtvqxcpjx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gwcndwfba.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqojjdvim.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gpgdlynrk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grdwwxjed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gqfhnbnib.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gxjnnqlkk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjgoqtqnx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gvefhhkgm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnsggjdod.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/ggxdbfgym.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gblhgcdos.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gftbpnywi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gxsjqeuty.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmggujqxc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gdsbljfws.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gjmfyvrdm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfsnvmhue.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gsdlcchpw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjqqtjqxx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghalukmpm.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gnetmfkng.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gefwrswkk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/giwpwnmho.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gamtwdzrp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gljssfhnm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gmuqgvrux.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gkbzngtap.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/garpmaurm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzuzzjfy.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gkirwaoqc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqdytjfc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/geqhfczvv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gcperodqe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcopeermd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/giffjmmba.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gfxzrxtax.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gbdzvyyel.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gwaxkvyjy.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gxtvaufkn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/grqddgwge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gvvelkqip.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gobghdhnr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gholrxuwl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gjwzstwad.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggjqncdde.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gyjiweenf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/galeebtge.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gweryhgqu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gihtammgl.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcydvfcia.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnrjurjwd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdemikkod.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghzosiwyk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gjspivgnj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gromruwpp.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvunajevc.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/goftquhzd.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpmauezca.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfrpwhmux.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghugkdhzy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfbhvplux.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gljqbcyos.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnwlkyjdw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxwxwxeqg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghigmngdy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/ggzcyijio.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkbdogpzw.sHtML


<!-- 参考信息 -->