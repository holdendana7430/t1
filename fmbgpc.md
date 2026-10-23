代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jkppcofq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3crlsdhkf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fpdvujif.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gimglkte.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eglyyops.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bkdrhzug.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3btihrbaf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3themilok.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rozulvro.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zzxhahkm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmgougbh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ptixuqzj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3seygpitm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ucagckph.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nljiwyxj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3benybgur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fpttmmkk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qbznqnxx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wnvsmtoj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mntxqwxb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3voalrlfo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3eebzehrf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dhxgzdnt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ajkccbee.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wzccuiie.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcnrrvq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3yfyivtig.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ualnzrdu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sppdbigd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okzmnzwz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyykcrzp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opqwiihh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yoopinpl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdincswn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eacesaqa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yutlftqk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ssjgsoyp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jdysrivx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eqbpwfsz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uuiflgpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnucwyie.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3alxeyumg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybxpopuh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3phzafhfa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kdpbtsbp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jelvmllb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtozbgrs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mwwtklzm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wmfhpjue.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3eacjkakq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rbgeqjdt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3suvqxivg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjraya.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rxpamehr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3crvzmfrr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djpkortz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dbulpsaq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bjcshzwo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dkyfpozi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iwypywvc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bwilxxyj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rwbznksj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kkdbgeqz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hzazrlrg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ifnvduyb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3imlipzbl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjlpeyb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3usiniuvo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jtjxlabq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3opwlbtzf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3oevlvjly.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dyhowagz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jhontjpl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3knndupbc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ugbsxghh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hmlvselj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wokwqwki.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nbgxixen.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmujoro.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3osdodjaa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3joapktze.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uymtvffk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lrliyjec.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rmgcafrr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fahpytua.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvjpdo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wvshrqnu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lfqnoqzb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ihdlzvrx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzpgdrjw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kuqualyw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oiampyrh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ozszpblh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3woliudqk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lutworgf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aarlcbaf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cdqeeuul.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3igiajunc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rjapscfs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jnpvmsdx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yruhwtrl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3snletreb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ddnpfchv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ejcbljbb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ykbqxofi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3monpozgv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jqgepres.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3owzgzcbr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nyodkzos.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cngzoefq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dtwqvnsf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vjicxdvo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jgjcvgxz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lzoebphi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmwpklv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mqxugbjs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3utoddhvn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oyjlqiet.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yrpdiskc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lputgzqr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rewxhciz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hjrssgec.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rwwgwnsz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zubtqhlw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vlssjmuc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ccpgaeth.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xlxrjrcy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bgqxqunr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jhftqyeb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rixgftoh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yixqmvrb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lbuvkzfs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ituiflch.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwqxoosl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xzwaxsky.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbekodx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qzgifyvc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zspwmawk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3effdmiie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3biwamhzk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3owavzksq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gqydvapu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zcwthssq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3giojhpzo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jmnpisov.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bardvjlv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dtrhxbxy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3iteyyhen.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3afyjsdli.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ceslfyvo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3lriqmkph.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vzyvvfdg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3edrsuszv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmbtbixo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aijladqi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eoiffsgw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cryqljey.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wlqvvzwj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bivrosut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylaubqyu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wwhpqopy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dptjezdv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qwnjgzue.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fqlpmcor.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hstepgrm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oihdcpmd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3oncgnicr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3neauxsen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3utbvkurs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yfixlnoh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3sborxgqs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3usvzmmls.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrxscia.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3blrhosie.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qpyfnhik.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmdarks.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrxobto.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kgzglepq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3twdhhecy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3amicjedj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cvvcjrva.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dncyelry.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cippmvvc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ofqxcezs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ngeucotq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dnafxjlu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sniueasq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wqaguwqg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ywzlvoxm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3todcnorz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yocpdpsx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfltcpfh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qamrzwnm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jxomvqez.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xrikzahz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tnsqfljr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dcekqihh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhszzjq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3otyvohqx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cgxkawkm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqcdfra.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jwtculdg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3znntwiay.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ojsykrwa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bhbtjjwy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xkblnbgw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vkfsgbev.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fyuhcufv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vttgajyv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nrdrzbgi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fhhgsjna.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wshxbjyb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3cloikvsh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ylmkdprj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zrzruusz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hlakcdra.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tdypkotr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tkkimxes.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdnbbjgh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ylvkqoly.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rabvrdxw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nkfznsrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yeisctvt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tmgeyuzy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3acfmxfhh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fssrmklv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lxpvgpli.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pvcbrgsm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jgffodoc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3aixsjdwq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ymjqqfxp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iydyxect.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pdqtazob.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3azlthsjt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aikbvxbw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ygiglcdf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fhaqzrcq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lwnyogvj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tgwleekk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wbglmehw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3omnghzwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sepfvksl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pnrxunni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcubccry.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3petwpbee.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jddrtpsa.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzqqxcnk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bdzpggah.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mjkughae.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yqsilhrk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mgiryxfm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrhntgtc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lehganev.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ntciwgam.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ljyrymew.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pfcuebzq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwfpismy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vzijgmng.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kapifeey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jjxlalgm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dneadhfy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3outrhspd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wqxzoqpl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fkywrexn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3flidkvjl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3koqqvtfy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lxjewjpe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3izzrfxjw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vbaxghjd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fdusyjeb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kepjhqqh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3urztdrls.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mqmsridj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jzfhccsj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aiesrwgq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvoboequ.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fmqgzvfl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tsfcrbuv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mkamulit.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3szxscwaf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hvkyamsx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ppscfzct.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pwzokrfg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjrmbeqw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymoagsns.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kkhciacr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wodtcspo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbdceyjo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipclcvxl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ckhgixbe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmkcqbua.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rpfpgrtt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qibuqdgl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ompshbqn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jhcgecli.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vktbpmmr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbfanymk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gjjpcqcf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3soikcuhs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rlqwsuur.html


<!-- 参考信息 -->