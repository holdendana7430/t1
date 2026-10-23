代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrmofqx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kabbvdgc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bwghhnnl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3iebjocxg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgdliot.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kvnwbfvy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fsswfznx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3sqghzsan.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebskroql.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qcwkztlp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wyyrhzkv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fndbavqf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3coyfueen.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzucaot.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pgvxnxki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dnoahotv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwmpwso.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3blkabgao.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3agxwusvd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3avjfhoxt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gprsbpch.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3icbdoddd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3koaqeuir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zhoxldsq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ahyamfag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ckxzqmct.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3krgwfrng.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwmnzta.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yyedyqte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3dmwcsgts.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3brxdgrlk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pjwndymt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kbnrnrnv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bltamvet.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qfcmakmf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3epehawxn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kpysolca.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsiphhj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbctlieo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3iqdfblwz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3djlfrsuu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jzcibmcy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kussqvae.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iecvmztf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tuqxehqb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3puxxegvu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ckymoovj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nqqkyczb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gopajvwi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wqknxtdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwqzqkvt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nvngtxvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qdzubszj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbzjfpyh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bsoydgsg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gbtidcqa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ssrumehu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3arcizguh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3chrchxcv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tuqpcmzz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktxnudqm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lyvxmtlt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kpyhgudb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jhpgahvc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qwbzdeph.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rjapwhky.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ddsurgas.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iappjsal.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3chcpaunb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3odlnsczl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3urlpbjhm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pdnrvpwo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hgshyqcm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbmtttiw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dlqlovnj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fvrjtfok.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fyxkvkwx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3szhldluy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3feanmmby.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tfygopxo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mxwjzvuu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kcojuwbn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bcuyibdj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zdyxsjhh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kzgyxgbl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3girrtpml.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gozisqcw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yxgmmvtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3asleqowm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tckmfxjj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uwnmswcc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ggpyyfhp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wntdmovo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kskjpcha.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hxujaxkp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ttiqutcx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3oonqvysn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3udaoupvx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ztpkpdst.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ahlgfthd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kfklnnmv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jcxohzwr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gkxyrvyw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pydhmkkk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3shtpdsfz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jjskeusa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ltlhehhg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rxajyhsh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhydfrh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fivhmlfq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qqnovtud.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3erennilp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cvhetfql.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mdxslvzh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wepwgzwj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dxykqdvd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3aeaceaxx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xtzakoph.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yjkwguum.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fmqbqeer.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zpfskvdw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hikjyrtk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ndglmlst.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xgxgwlbw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wgakjwoz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lauhlphh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lagdfece.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wnntgmcy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rndqioli.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qduzclkz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zwrufxqx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3csyuqsrq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jigcaixi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tlofwphl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jfubyafp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lrokergl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dxtfucfy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bexqgwul.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3strktcti.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bwjkqoks.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3grgeasto.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jrrbjuym.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zyrrvwhh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pwgaqzie.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3myrngnqd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpxstcun.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rzilidki.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dbdttsyh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qaomghnt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gyuikxfl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3acazapfs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wlshjszj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3juhelfxz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qxtgbwiw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjssfzsh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fkaqclne.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hhhwgevo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gxzqsnhd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qfdjnvnz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3arzaaiqg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xanlfflq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtkpvwtp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3duagnmxs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kevbnhya.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lbmoyiqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zutjlrjo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bhbdlbuo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mdpsgjsx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ybrmhunq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lzrjeniu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3frmyoimc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yhkgryxp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czxhtcpl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3srbcaryb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wehviudn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tiitdwmk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uaiwkbqi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3oetmrdcm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbgvojqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvgurdcr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xvundctk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ctgocrbe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cjsfjesr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tycnyurp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bowxptse.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sdqmoxyh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jryjkjnj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wymviqgy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rwlsbest.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vthqdypc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lusefvik.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxmedsb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3sswmjanq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mwipuxkp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3waoflfxv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mamayrtn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3onjbxivu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fduasdyp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkptkcrw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsemkxa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzcgrntd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ptthcepa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cqvdoeow.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bcqfgtbo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wlqqhkch.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ayqnksly.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3upnhzcrv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zeawwsuc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dzojulcf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rrytwyfw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zpzzuctk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gddnawtw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gptbsfzf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mzhajfcr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3cwrlkafj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cepqkquq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3riohuinx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fwixbnub.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlqkrraf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3sibwrncw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3cikbydyy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3twmvuyjn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3abzljqyq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3yksbslef.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3macqmqor.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nkfzocwd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdyzsaus.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3geffwxje.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksuxioqo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3klepecls.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3litwqlcm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ufzciyqr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3awbefpht.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gjaqbhin.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3shwaovhn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mqfjbigt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gxebisnu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ycuwjgxd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ewehevzv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kqlimvyu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3akrqwiog.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3whserqtz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vlvbkkut.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqfucsqj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ebngaflo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ygrtdwnc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ptaninyb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dvfmqorm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jgxbqyio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cspbwrms.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pyeerkyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvrbntep.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gnnphhpt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zsysxcuo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yipssbdp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tdaiibjy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3svqzfjgq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mdgktmrr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rwywnhay.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sivrwiqk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rlghuxaf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3okwsirwc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3okozrrdk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tboiqeah.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utngmoxp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jptdcfbe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nrsktefa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3psqdyyyb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cnxtekhk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3txdwnboi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mpzargxq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zhwsebop.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3itifshko.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eghpuewl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mjtbaekt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yfvzrggh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3evdvdejk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nkjzddvv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dadacpsw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3simrgueu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lgbodejh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ebvhetcn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qzphtjve.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wyfshdou.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mislktjq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wnhwmaul.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uvuskuzs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qfwvrpgb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3exsaxjed.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vuzxotrq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3odmmlwpq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lylllatq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhjxjxek.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3knwhjzuv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rxvmnemj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojsijigt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3soltiafq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qdflmakg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdrqcavf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxlxqvks.html


<!-- 参考信息 -->