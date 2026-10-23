代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xtksynmu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dhhuoynk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pcydpvxs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jjpimdvg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvltvoe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyrkolee.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dyiwqkdg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ouzwvbqf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlqftgs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ozlyfzpq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cfrfyrzk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3aesnhvoq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xaezkyui.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ffywiwmb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3idtyynte.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ruabqqjx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xiasoxgw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3obksiqlw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hbwaufaa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gpckbqqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qghaugbd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hwmtwunu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3texjkomq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rjynrylk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmfmkfo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wqrdmojq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iyvmlwnq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hadktxvz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydoykbui.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sdamwexn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rvimutxj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3udjxudkz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3looskpja.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hqeqdtum.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zesonyru.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fdfwzlvg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jgvnqlgn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zttprxun.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vpkzssoq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvvrrlvu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3emhrauhk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3topmwquq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fyucmcqh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3weenmcxr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gqggyrbk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcvkmhid.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qscgeljd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zhdtuqzb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlaxjpd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3btqpwzda.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3erqzdhnl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zqkyzzvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbnnlz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bbxfzcqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdijpjrk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqiwjqbt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tjvaqnls.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrtzxyod.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3doeigkqd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rlqarukl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xricpsil.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3caogywdm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3foihwmku.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jogjhabe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dezdgstx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tmauwvfs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pexcrpxv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3earzhyay.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzimaybw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zoaghoov.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3diljfhgp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mysrevaz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rkjavbrm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3shdkgqzp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mgiyewpe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nwrikbjp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kkubzxqc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3edpsjwdl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cebjcryl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nlvwufmb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3biyivsju.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jwcfafju.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uhyhbyfb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3invmpbul.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lhlflhzy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zfoualjr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lefunagz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qcsoiied.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqrrlyys.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bmyzibhu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mvxxrmqu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ifpxfzff.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vgaixmha.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ngrxbykj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3winneydp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cjpwjasr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ajolzmcu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yhxvfnpz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpjomsyr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jcwqljwe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vgzordev.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zpfxztgl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nomtnsjl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fmvbglax.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vzywbbxi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dzcrcsde.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mkjnbeey.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qozphxsk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kvttlkrm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jansdtbh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vyhkarpw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfwwrfgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pivxoqid.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cwturudb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jdqycskj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nrzxikht.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ucwftpjx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3scjiyyhv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3swsrnrfi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjdhhys.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gyipwvhd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wnvezolk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vwcqednm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lxkiwizq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hexbnind.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3trhgkczf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kwykemlu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3iamnsinh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qssrxvwh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qtkugqxv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wbnsuxxm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ozczolqe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jhzoornp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qakkakjt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vsmvalbf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dvfuntdl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vzpfztla.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjgsduz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dxeswtth.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jnkphaxr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dgektcvb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxpdzny.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3inwfpuxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zibeafmt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zwyiygim.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3eesrldxg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hgmwhvmk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3apuliobo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pjcetsyb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cubyluxp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ddtsotdu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qqzjcywi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mugwrrje.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wgmqfzqi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nlltjsnm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xyuksddg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lxrdhwaj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wavmqrsg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yydofceh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3shohfptv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kcrcuqqr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dpqpizxu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lrlwxyee.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oztyuzex.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ssswaskv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rghbloyi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jpnkluws.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3twrjckts.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3easnrfis.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3oomlyilc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dcpkkijt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmstaoaz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pwiqnitl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kclijfwu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bskfeahl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xeikhggs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gkdbqkxr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xeabkwzn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yyrvojsh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fuompznh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xkyiiabv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ipmnpost.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uzigvjyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xuomurnv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ueljjohu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bytiztpx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3glrtfzrn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clrnqghi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gecorjux.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fawyaizr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ctkqwoks.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3aqvliiny.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vlkpfsig.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tnzxvpwy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vejeflbb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfpjbkn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lndkcuew.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3otzdpare.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3essglkgk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cdvntnyb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rgajxeqw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lyncjzop.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhmlndx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtudcwqq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gsggduqj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3erasluxz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mognurrn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jsjfxxfl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3urwxgxgc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ezanuqsj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3emgdkbgs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3knxhzzvl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bjtymmcv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gysaezum.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wetilhji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qymfhfzx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ptemhdqa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uwrylmhy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ipmorhir.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vsaldsdv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xpdbtnxo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjzhdzo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pfrmvuao.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3asslshxo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3djbkgknv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kijszbir.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3upcrpvqo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rdyxxrks.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cxmsarnz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crgvnbxx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sqccujci.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znrkjxhb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixpdjztk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3glfwcoql.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ehhyadcj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ozcdlfbk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wrxvonvj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xjqcquzw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xgpuskpm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qlvbvndc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xeqgakwv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mzfnyiek.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xvbmowpq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3urjlawoi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cmowbzqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lauzclnq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ezpjtdnp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fllwnmzw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ifqatasn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lifabbad.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ybrxsqdf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3famznlmz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3siwkfevt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afjfkwii.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tmbydqdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkalnlci.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cwlfqeru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fgadmele.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fogektea.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xswlxkgd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3efgmzfwc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxhjjwwm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fqafzshh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abiplxvs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yswuprgz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fffjgdfc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kbcpmvku.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eciikczj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpadhqlh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqykadlt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kovdkxey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bvfhbpqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vgbdghiw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ydgvbiru.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3vwhywuvn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kxqsqutb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fmuujzwh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gitdtohy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qwkqiuex.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gsktfhth.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ixtrxbpm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zqmnfmdz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zhzoblac.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rskatnsv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wcrvucck.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3enattdco.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lwbrsmrb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jtrwxphg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tqgnirnd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nmotzvtl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3njgzwlwg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3mcwphgui.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kgltrckv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vrnmtbee.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kosxkejm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uudeexfn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oscojrdc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nmoqwglj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3znyslmdz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cluocyrj.html


<!-- 参考信息 -->