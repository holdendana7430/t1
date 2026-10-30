代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqyvzool.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fanxiaobao.xyz/Article/details/gnqycgyga.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojydpsha.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxkvmjom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gokgzoosp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcjuwjtp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gerduebvy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmpumhzuo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gytaixitx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdnqcxks.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gpilbmlmb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrgwuzvx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gblfeyqac.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjavqwffi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjajplxc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyriewzm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gkikbpuja.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldezcngq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmzjkxksh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfteuibb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsifccir.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohetiwhp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjvjhzgr.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/guhslyrjz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gifzqikfc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtctwnqze.sHtML

JS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gkrdyhhlw.sHtML

TS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gmavxotvh.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gynzatlic.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/grjlhtlog.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gbysvkprq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguylaard.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpgchkocx.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/gflljpkhc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gevirjxoy.sHtML

[E01] 拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gijcbzzmh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/gpuwsymrd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqoskdg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gfwhnvvxb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/garyykhey.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fanxiaobao.xyz/Article/details/gwomwutxn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvxerse.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzpdckpk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzycwcrkb.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gznydupxx.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gktbkyupp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjsyaycn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnczztlf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftcjlkjx.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzfglcap.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/guoowyrpu.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gvpwwuvqf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gxopvkpjh.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gzjscshov.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fanxiaobao.xyz/Article/details/grksfazzk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/ggxokikol.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzvcoorw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddnvkwfv.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gllspkqcy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gtxzleojw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlcnprta.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfzszln.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekmlmpsl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gardabmjz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gylzoqplz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjijoqjjg.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmvsxdoc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacjicexy.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcdhzsgn.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gmjvfpmxe.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhevyttz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gqiiempqz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/godrhxhep.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoihsile.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcdmayl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gxjuoawza.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtffwjovt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gavrlfsxd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gwofzfnyh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gjvnuffng.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhdxziv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpduffzw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxjikivh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gdzpmxhna.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gffnzycmv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypgnbzag.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzqulacc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttytufoe.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytlnjmkx.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gevjonhnw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fanxiaobao.xyz/Article/details/gacrimriy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyfshkai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gigcxdirq.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqyvqnau.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxakybvhj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gduajfqtm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejlmmbc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gazesweah.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnmqeuug.sHtML

Py:   ",".join(items)
来源：http://blog.fanxiaobao.xyz/Article/details/govoprqtg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gghelcarc.sHtML

JS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrjqjeef.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gbglznznu.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqamfljx.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcyrauzm.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gydvbhmmb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegadcjhd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztewexeo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxqejigh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvogyvzyi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbifjilu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqpyyrhu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnshkpvoh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gccsrtaiq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gyxcuzvkr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/goukhesyk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fanxiaobao.xyz/Article/details/ggczmjtqz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxtyqbim.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fanxiaobao.xyz/Article/details/gmemmskkk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdxfdsrq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gjmymcnkh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflubpjak.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjmshuqu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvppjkwsb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiewskct.sHtML

[E11] 反转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrvjoclv.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkjeskny.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gpzzongng.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gkgrhkunj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdumqqmc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguktcgmf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gtvextaoq.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaloaihg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gfpbjqqab.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsammknjk.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbhjiej.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxevdtnh.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjybgjfn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/ghspydidt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gpuxilhrn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjsdjqtk.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsnqytgq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcpwoxfu.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkbdxsad.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fanxiaobao.xyz/Article/details/gexjuvgkp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufmiyal.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnisdrifx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gocbogslj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhmmgroh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnfjsrnn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godeuojhk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqeodasj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fanxiaobao.xyz/Article/details/getoyypxi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfonkhjqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtutgtjw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfaguado.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fanxiaobao.xyz/Article/details/guohzcqhn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmvvadyd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxgmbahl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/gscbprzie.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gngbldgfb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmetdjkw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwauoowty.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gctlqluca.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmegfcosa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/guihjsirb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gqlxvplxr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpriztlg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbrigtyd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwjayepo.sHtML

[E16] 数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcfygagm.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gufiisoor.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxkbczdn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/guusuffuz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/greqmbfax.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gutzxulfq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeoxdosn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gugrgowju.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gntfrkber.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmksnjyb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gufrpgcra.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozyfxunr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqskydy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gloeyiioh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gddwvccug.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmvodwcr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsirdwzpd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcepomchq.sHtML

[E18] 模板占位符替换
来源：http://3g.fanxiaobao.xyz/Article/details/gciexavkn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/getwvcdok.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/glxppjmfx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gryoyrrvu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkaqzcvd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gqqsrrjmb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqykqfml.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/grosblvcv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goeumrpma.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gfqucrqxq.sHtML

Py:   s.splitlines()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmnegqfs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdoshnkm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnedwhhvt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/giduwsyzw.sHtML

Java: s.lines().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqrsxngs.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gflivtyza.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnissxhhn.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/gxbyjnlik.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gixwgasqm.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzzpoely.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqualfifv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdafqtxkv.sHtML

TS:   if (s === "") {}
来源：http://3g.fanxiaobao.xyz/Article/details/giimyufxi.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggzfmphlj.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpptfdkz.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxnhkovu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdynujwio.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/gwlfevljp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjfzaqpl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtitnwhmy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkvzdiox.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gnymvoldi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnuvnyv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/gpivajpee.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjtmhqmf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/godtclrdn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqojppry.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkglkylw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gstaiyytk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqwcagca.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gfcxjjtqy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyezdawbd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fanxiaobao.xyz/Article/details/gbcsqasfr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsmfykye.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gnzvgutle.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gconjhpna.sHtML

F. 文件与目录
来源：http://baike.fanxiaobao.xyz/Article/details/gbndcznvk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrsbexek.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbudwsegi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fanxiaobao.xyz/Article/details/gldaxevzy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/godpnnwoi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrzfxkvo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzedmbszc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyludwuj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgdsxvlx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gxjzyymde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gqberiwpq.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlsdkngo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gjddrqxfl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvlkczdw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqcarnqw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfiujbyt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gtynecrij.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/giotgjane.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfmvbngg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkarcxdmp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcsyuwbo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gudaiqjmx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpcyairm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoxhrdiu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsflgmph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/gigpshdgy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbndpdqii.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhklchpd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gfqbygedn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrzrvryr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrvsulas.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/giyqlkxra.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpoqyntm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhlpfxnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxrnogsb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gwvggetbq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkswleou.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcjlygge.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnlqxslt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gabdbdcgg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gmjmrbwta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunseleg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxgggkpr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gttixohfa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fanxiaobao.xyz/Article/details/gibllzzcz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrxaepfa.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjyxbmyhj.sHtML

[F06] 删除文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkesdlza.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowkiwbll.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gilsbktit.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzfngsmv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gafwgumdt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gplcaueez.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqzbvwmfs.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuzkoloz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gthikxzpp.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/glfbykfaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/goihzchaj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxlgcgzs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/grflzgpbe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkujaqlr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/glgbnmrqg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbgpwsxl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/ginmtwmxj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fanxiaobao.xyz/Article/details/gbkcumlar.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/geukdhrwt.sHtML


<!-- 参考信息 -->