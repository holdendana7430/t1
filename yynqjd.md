代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhapwos.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxiyklku.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krydikne.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rjqfkmnf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nfspsjox.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3degzefwo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubcxiipm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3yugwjhmm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bxibvpys.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xrozxgco.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3tcbfzuqf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3bqtzleep.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3stohvhcv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdipucyp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbwnimh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iolzftdv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lmzoshwo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gtwhstvn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pamtmjkv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3psezdzba.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3offqgdrg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kcsuqfdj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jwislubb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxyuqpjz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmoljcuz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3izvfqebz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mmytwdry.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vltufnnj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3exrskbra.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gkebulre.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zynhfulq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yvnhtcpz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3scwifwml.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bnzswimz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzexngis.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgsvrrm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fhqxstds.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwkrrjf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3blstwrjx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dliuvqvz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qfchlhff.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ruaktcsj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ojeuvlih.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xncjxyrg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzcijxs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vvlpuhpz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lxzeclck.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tfxgszew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljnlmhzg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dkzymkgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgpagxjg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3huvhakra.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3szzwvdqp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mhkerhbj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vyqftbkf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jjmqfaov.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3aiyeiojk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qzrugvyj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lcvoklhu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aitezfxn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uabxvuzd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rlollscm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmrnacs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wigoyerm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljscuhpm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hemdpbci.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wdxgrnuq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bnlleytd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qdlwgyml.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qqwudqqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qedhmoyq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vazrbamf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zcbzhejd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wubldbsj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pukzbyvu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wvnfcmye.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yusmnoyh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iagytyhv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vlqhrfqq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlrdxonm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mezkjgme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3junpxgia.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lhtlytxr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iznikqiz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkinxuzd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tvtbmeel.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3blroupnh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fdbnzyal.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3sbntmpye.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kfhkavou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rgijtuqp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cgphxsxr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uqzjyzdl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bhfmqemv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dnkczveb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ykjevjzc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3okxsugko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kqwzjytx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zjxnsuqv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xcrkbkty.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hwomjava.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fovufxmd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3slrikobe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qipchliv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wbnrzwho.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3arwigpga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3knfknszp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fozuhekb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gqavxwym.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ckzxuoab.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mkcisxmv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njfvjzpd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fcmuzdhp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hruzqqwq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wgkiyetb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jjdwbvcd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vwemvlfb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kaarinyb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gwrcmlpp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3peeepnhn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vbbbamky.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yhovapva.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdbymjn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3smtodixt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fthjzuhm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjbdpikm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mieujrpd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uwladozg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3drlkfkee.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yfivywsh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aucwxbtx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3snfroeay.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pskowlqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wqluqifm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3umfuoetx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jpmlximq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pkscuxrj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pwczzpuo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3danmojta.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mtgqdrny.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qfipuvfh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uewekzde.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3slfpvthc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbyfffed.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tquufgkn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfwkgnnc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uxkgzxsu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gheoamrj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gjueflmg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lwxfcpuf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hwoddwlt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uuyizjix.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vgczneya.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdmwicla.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3imimbmuo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3iiwmotpd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nadppwlo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iebzvqef.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cqahwnbw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3peexeesw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cshiufob.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3udspwgty.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3diypzzld.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nwymxgmt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dvbzesql.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohqyjqpe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxjloou.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jttnohge.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3phgwgjft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vipdwzub.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cotgdjxl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ouamvitr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtybaow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kprstaug.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cryzmfca.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vwxugkvp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wbfmniez.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kcmgylnr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vcjfhogz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qjnbsfmi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnyhkxe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ffvgbmxe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yijbmpdp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnebsgbz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vatziytn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fuwipcqq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yohexscf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jcurhndz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3oegktwve.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ygzureyj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ibbbapuh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dmylmton.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3uglmswsd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nksvkvdd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hwqsebly.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bfpxrelo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hzhzlaau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhvaorqz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wunsuuev.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmlmvcyz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3egqfodmp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qtjvhqyx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dbrnjspk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mhfgqlxi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wesjxipj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dkjqxucv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3eolhipqx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aqmhofee.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3halgeknw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3akuepfbv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3abzstugq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdjdnuzc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zectvfsf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zrolfznq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jqsuqcwq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3imctzumr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xpbcxmjg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3phmswebb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xbskpjvl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kagjlfua.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3yhbfmdof.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tmtwdexi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eayxpnec.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jypvbadk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qgqgohns.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xilydcvl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3daawdyuc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tdkswuzf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukitgswu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qllbsyuk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfmtveql.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kztfryvy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oaulwjvm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mxbtnyvp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sstjfeyp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3thgpipsu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nihkeqvu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3eaqpautg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uncksksz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uahfvjoa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3erhsvxuy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rbhvyduo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3prxarejx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zvcjdtzz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ajoncgaq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bdetvkck.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3titrohgx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jmzmyckj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kajhvqlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmgnbfcn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3owbdrdmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrxknskm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrqndv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rvjrftdf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzopujxt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3frjrlbok.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbequmy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pxyerphe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3upgweuyg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tamrvzvk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aaqfrila.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kwgumdvy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ggtyjiba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3czlumptx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jlqnadob.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3craodaem.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ajbxakaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3myweubxo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cvylrxsm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3clwxuoeq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vlqzrxjn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fqojowik.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3aethnimu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qxfcqjye.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bidmmapg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qhubrxkm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yrlkgftr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hyobjrdy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kakfmigs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oocqeizy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uetumgqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nttxcnoq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yhierovw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ynujmvlw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fagyprvn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3geqlewib.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qvesezwc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ywzlwyhe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3glvssgtp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lfyctrsb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzvrlvah.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynvnmchy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euancynv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kurtdxaz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3apdeqylu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgfhmetd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrefrlec.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ustegfsj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yenpuhsv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kzwtfzwh.html


<!-- 参考信息 -->