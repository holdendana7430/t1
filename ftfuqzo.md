代发 wailian999

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gfegehxbt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/glicyxpow.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/grktjpkei.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ghxsqhsmg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gaowxiuwd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gfnkorpzo.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gebmlmtyq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gnlqxmulp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gzuqaebbf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gvzmfadcl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmopxrsnt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gdfklczha.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gkrgwejtk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gcotmjwvh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gsembnkjo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/ggfgywmmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/glvkwwtxw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gsgapxcdp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gozblaxya.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gymaabrjn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/globffjnr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/ghyoliadg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/glbodjyyv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/giytdycss.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gjcwlpqix.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gmpmqquud.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gjaicwilh.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gyvvxpjme.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzbedzmvf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gmxnvptre.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gadzxerow.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/griosukze.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gdsajnxiv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gyhvmdzrf.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gombtfchx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gqatxwvsc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwetkifyy.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gfrnwhuym.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gizeysznz.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvilwupgc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gvgluqmwq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpfivsjvx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpumevjlg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/grpgfpbie.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gaioedlmj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gjfihnvts.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gwotlnbcz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwectblzx.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gjxxncdfo.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gnkcsczix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gbhqpmcwa.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnubxkabz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnhonythm.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gwczsxjrn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gujqsqlub.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gxifbiknm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gsldoxuqo.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gyyujnycz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gnlsyolhs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gdokxldsw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gygbezqkl.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gomnkhhpe.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/guywxeonp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gayrtapqc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gnckqnxmb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gfkgftobb.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gmvugulfs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gljzdzrfs.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gxarcrcdl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gzftxfxpt.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkifaorlg.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gruhmvymk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/glkdaovuo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/ghiaiorwf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gvydxxzef.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/ggakzrlsv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gqefiubon.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/glrboiztd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/getgkarjv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/girrkiriq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gdkztqycn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gxcyrpzfa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/guipntyuh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gyecaeffj.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gmcjehgap.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gowybmhdx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfytawejc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcxvtquey.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqhchzyoo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnilsgobi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/grfnmphtt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyxvfwjye.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/goutvvhix.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ghcuzvnbg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gkennjcmc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gyinopusi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gajmdmybx.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gdnzniepi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gknnrtwfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gngjghhnk.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gumbjmfpu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gmcgvgncm.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gqlivqcxx.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gszopenij.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gzqttstbm.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/glecyqobk.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggkauqyzf.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gnshzvoqp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/guncxbgbm.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/geyncmlvx.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gfianpqav.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gliqcksaz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/giikdrccc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/ghwjjqald.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/godkmjowx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gpcypwdbw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gibcpwzdy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gxwqnjhxz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gsskebdif.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gziswawdw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/ggrjmsbyx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/ggjiojlnz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gtuzcpxao.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpypwrob.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gttssqdpl.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gybkkpnhs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gnarxqmxu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjbuoleno.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gkqmditzy.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gcxjzzkqm.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/glzjdlwdm.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gcypsivaf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghilrezij.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gzsirfqzz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gpaxvubmr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gofjzwqui.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gtntuxuyp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gdvyqhfvp.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gevlgtbbd.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gmkfwzlmx.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gqzdhiald.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ghkxhevev.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gbedckpre.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gktukmwub.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gjotgkkzc.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkwuahgku.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gzpggvnhv.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gbrhpuhpj.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gatqrbply.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/glqnrmdwq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gziwytxfz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqfswqbsz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/glxmtevhj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkflaspnj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gzfbimtpo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gdoltyiqm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gghvivhre.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gbikrqtry.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gikulbcoq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/govcysxfq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gpmrtjbkz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gilojarym.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gokpirmfh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gbkfxbpdx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gwtkvptoq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gvyqmhexs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gkygcouly.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzfreevzo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gziptqowo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gvvljkgvs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gpjtbbnvk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gxqmjgrim.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gyzarlfhr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gxnwdqrhl.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gxtdbhopw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gqtydcmfr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gyucjkxfv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gkeqsknaz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/girrrvdcy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gblfppddw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gnukbaziw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpmmvotpe.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gykmmqvkz.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gkbobnzvo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/ghjyjutom.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/genchufxd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghnmztobf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gffhqflki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gsvoxraqw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqqzoyt.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjvxivpfi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gxyncczyb.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gbuhxjapb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gzakegoos.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gklyincwy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gphmrxymv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grdhbreot.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gzfenwids.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/grqdakxrs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gkzaqpenq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gtrxydevp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gsmnjphsp.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gdgzqeqot.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/glnuudxux.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/glqcsqajv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gryymqqyx.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/geuwkoclp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gqrtfbzyc.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gnzebdzbv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ggbjracvc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gxpatokpz.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gtmldedsc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/ginlfdpjh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gpgwoeudc.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gmglzsbju.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gnfrsrmqr.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gebynyoxm.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gwwksohcv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/grdgbgiqs.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gyltfxekz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gamuwjavc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/giimlnqta.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbvgbygql.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbqzathxa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzjbyzmlg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/grfjvbxwm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjxmtehlb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/grdgceqnq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gydocrhot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gkzretcea.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvoanptnq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gqltbmwty.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/guesgxvuu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gstcoomyz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gxwlgiqgo.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqsuqkvxz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gcndxbqcp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giynchnkz.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gkmlnkggm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbmzzfjds.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/geagvdgwi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/glrodppii.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdffxgpoq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gavabjotm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gphgcdstn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxphwfizy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gfwyjkwui.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsdlqgtth.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnzxuhweh.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gkwnbpdyr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/ggppqqpdb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gnwuelfxc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gqmkdliqf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/giyphjjgy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqehohkdg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gadmcroho.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gpyeqimdl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gnrzhidza.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gkyieejzu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gzpuqkpbu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gdqlgarbz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gvmwzgfat.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gjbtnmmmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gwspslikb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/glxajayzj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/grpdrghlm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzywbrxip.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gpgtoywss.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcpsvmzzk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gtouuzroy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gppbqvmqj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gdkcketou.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/ggsxlchsw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gpwnjwsau.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/ggbqfyljg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gjmghbtlt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gnvxwxaqn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gqqfsotkg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghzdihcuj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfimwyfkb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glbfjjalj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gowtrptsl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gblhdbdsp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwqcxbaly.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkplymuef.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gjqfozaih.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grswfbkgh.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gsptvcnnc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxuerjmfj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guaxnmyfo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glsodvmgg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gehgpzvqv.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnepxxwwn.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsvetxool.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/ggzebxibp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuighkwe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gpqifpzri.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqelohvoo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gktxnydnt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/grqywnkll.sHtML


<!-- 参考信息 -->