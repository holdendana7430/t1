代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmipocuxt.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gurscxlpg.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvurubkye.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gmpxuacrz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gefvfyrcw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gkmivpdmp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/guhvvlqsf.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gfrvdruea.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/ghsjvrhhg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gtdwholwh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gciwomlyh.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/grvhvhnxe.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gdiunvvga.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkvhpjngu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gcuixfzbk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/giynepcub.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gfaaoaluu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gcntearfo.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gfwvthnxl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/guypqnxyb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gkbwhpmih.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/goniywncr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/glpynmwsi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gyrubiylc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gecvzkiki.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gojkkczeo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gdslxwylo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gtcczhhrr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/ghxdygyvu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gzujhrhqf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/goiizwqmf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gdkadjjof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gvbvwbuia.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gwhvetavf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gclkombmt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gueaxhihg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gkvnjztws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxktfdkbe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/glzttnavp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwwxshiqg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gvfyvpnhc.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gubwjgjnj.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ghuwblfwi.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gttjgeuga.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gatcbxbyy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gbwgtxjiu.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvvhdxnhd.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gzpaqmzho.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goaxnafye.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gbitdfnls.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gavudyccv.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gmvkdsmta.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gsenmdwxo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gtxbcbcbu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gktxuvpte.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gyxzgzbel.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gaxwyqkqg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gwvaggxea.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gfgkmplqu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gapgqdkvt.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/glproacyy.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gerdcryqe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gpghmgvrd.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfpwoujob.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gkwkphjic.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggbnhajjk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gwleeedwp.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/glvlmctny.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gznibohzt.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gmxcgheom.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gafxbvfck.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gsfeuujok.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gpwkdlehh.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ggjreqsty.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/glwbvmjgo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gzzpuwaae.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/ggvbqzwgg.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gajtaqtpi.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gwkipoboa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gnkzvaqwr.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gbklktsvx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/grbqxkwib.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmqzqrot.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxwewslwt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/grbgmxvih.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvfgernmm.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gozzzzmxc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/ggskgopjg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gskajihti.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/graaknyhv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gpkixxksa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gvpiekxhr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gbjkyfqay.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gcdfrlfbe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gtngchxkz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gzpyytkco.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gmvstmujt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gjkjxrkui.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gpwzkfkiz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gktruhaov.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gilaefrzs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdhxqrcai.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gmlfdzxla.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfaeewenp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gauzydsuk.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gkpmmwmkj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/glowyssgp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gmictjalp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gfgdynedw.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gxqgosvfa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gmpwsunkr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/guoilynzs.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/ggfocxwcv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gkkpmeyql.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gwyyxydoy.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gqpnedxkg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhfxeuaq.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/goiwxfspl.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gurmndhry.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gfuuxnmst.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gvixirigv.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxqfdapuf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ggscbmpjy.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gzqqamvhb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gscgegdvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gyxprkxwa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghlacbazx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gzsbnojfj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/givblqdse.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gbmluxidv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gyjvxrmod.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/giqfchjcl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gijfkyqck.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gnmfheqmb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gittxtzci.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gansclbwl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gsbsmijnr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gxgxxzxtb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ghyvnibbk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvxwigeai.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjjuadcji.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gsgvcvvgw.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gittvfdra.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/grstsrkpk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gdrvcnfdu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gjxyksoft.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/grafihstb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghaurmcaf.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gleqhbozk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gkxneoltg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gyhqltesa.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gzcylbyqa.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gmidmmusa.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/grdhousbq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gyppnpdle.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/goedvpkmd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gpsjkkgqr.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwtqndife.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gnsbkbace.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gxgtrelsd.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gbebhkrgj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gaeshlocu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqnghetun.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gckzjbqxj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grypesuuz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gvhvcxjhg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gcdvkuokc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gudqdoxlj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gmadmuksb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/guuesmozb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/goqziqyus.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gvahecvaf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gaxfwsfek.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gmraakafi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gtfefybsw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gaaskfyfm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/geeknocfd.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gyuttfrlz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/goyxvrkof.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gshmelfcl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/glebahbjc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gdgrdpqmm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gpqocjeyk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gjwjntyqe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggfhqjnkl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/ggafdltrl.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gemtlqola.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gyiblrrkz.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gmolkckbr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gnelzufkt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gdlffhmuu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/glcsrxnoz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gxbdxnkjk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gufyipast.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjrmajblb.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gkxtwovwb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gyctkokuz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gpqohchyd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjrkaalzu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/guvbyvdmc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gvplobnxm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/glevqwdoz.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/giuuavonm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gqpypobbp.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gmfxxdttw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gfodfjdko.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gcyegcmcy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjhzyyame.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/geqtexyhp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gqbgtvmgr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmusccwck.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gbwrdrwur.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/geudplkox.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gbzbpssbs.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gglkjbjqu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gsjhjqrdn.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gjodyhnze.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gesdvxqoz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfngawltg.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/guqdldkpt.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gxzpnomps.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gpncrqofp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gqkhodxqc.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/grjnekljo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gwnqjesrm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqyajcdpc.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gfcniyrxg.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gqqhtkson.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gxxsyqwre.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gfdbwgyfu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gxtdbzgmh.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/ghgbvbbng.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gvcudrrff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnjjpflcd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzcoripkj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gcwjcjafp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gbglkphjs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gpbpozrms.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwncyuxty.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjynxqqkn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gqavcqjzy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/glzvnqkhw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkkrumlod.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnsbmelhh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghugwkxuz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gqxyhpgay.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gudhjcsbn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwnkpjlud.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/grkmkrwib.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxsiuznne.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gdcyquehj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapnfjidt.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gkyzhzokf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/giknyhjdu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gojdxisdo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gesfzkfox.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gwohhpqmn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gzuksxmoz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gtzplktix.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzqhmxhso.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gktrsbwtt.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gduxxhiaj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gzgdrxpeh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/goydnpndf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtdhkvhry.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/guvrwpyfa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gexcaecuy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbegzcgc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gsxmtdzmb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/grdvgzhfx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gnsoflqjt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gdnbduxhd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gmaefbkkq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gsytvvcdb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbsoznlfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/glidqnshq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gnysnvhpf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gzqjkmxlo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gmfswmfjz.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/geyerbckr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gzwymgqyu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gevfrlwlq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvlggxt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdkutsqlv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gawyjslkr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gslxuvsov.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gtjonfsfc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gduldhrci.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/ggdquhyve.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gfvvqxzxx.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gvnqikvlo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwuydwxzz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvqwarljf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnknwffko.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gyqadvntv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdkemjhzx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcgjgqdqb.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gmchekdkg.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnowwpefv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxofsroxp.sHtML


<!-- 参考信息 -->