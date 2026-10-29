代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/ggaykzumz.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gcpaevzvz.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gdgrjfdey.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfldfhmei.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grdijjfbt.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gejnkagup.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gybzwondn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gpedwhgln.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpzntmsse.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gkdqpquyj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggaddleqg.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/ggjrvwixr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gmsigpxjy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gccyzkkht.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gvbnwzrci.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gijaonzzb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gwewjctem.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcdkyzbnb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqkbhrjdx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/giypqhdfd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gfeelqbxw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gydebqutt.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gflndpgnu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gbwajodlv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gljwbzbje.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gopcjkesf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbxxcksf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gxsshpidq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gvuslmfio.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gtiuvherj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/giwyqkivz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gmhqvqrog.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/grcfnptaq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gbuecuvry.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/glxouwiur.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gleorniff.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gzakvqjzi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gyjszhgce.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/grkpgvzfc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gjzownjjy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/guwrgjnwv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gaqbyftng.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/giocuvsyo.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gyrdrkzrf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gjvvshzny.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gstrzsohf.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/guvquhhut.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gpossilfb.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpanhkggn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gvmdfsarz.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gnzcdfjmr.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkooced.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfoqcazpp.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/grcxotclb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gebduvzxb.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gcmbrertt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/geqovpftx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gjillfhpk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gtgbapfca.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gitmdceku.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/ghrmfcigk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gdtpuvdut.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gaeolhtzk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/giohjrgzr.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gajbxbnvl.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gqtgaqjah.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/giuewkxnk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gbrzosswf.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/geuuiozwj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gaccfdjpt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gblacenwd.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggxfrzsht.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gtjtskzpl.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gotjbqsfp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gzhfrfjix.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gncpijvqd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqenttibd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gjtyyjpte.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/giuxulrjf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gtlaksbiu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gjqavekdp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/geflhldaa.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gimadefuy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gojfhaudz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gnxueqxmz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/ghdrjbcvd.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqjnsqyyd.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/glidojdpz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gkhrrnick.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/goitlcglp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gvokqpzdy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gyeovysbk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtpqduqvq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/glkctmick.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gfgafnbau.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gcvprxijy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gjfepyswk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gewlxkttb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/grbjibxqu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/guqcwdrom.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gsgukqjdi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwywwhzbq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gvmtuzknt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfzpftxgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/geqyvfzfd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/glksjjjsm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gggfcuoht.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gylfroson.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdofsibrb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gonemawpo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/grfqewlyk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gjqaxtmwa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/grkgnxbxz.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/grakaeqdt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gumyihtzv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/goxkmgcjk.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/ggdxzxilj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/genjyslji.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gdgzatkej.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gkbmkixvt.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/ghrtwiwjf.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gtadizmox.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gzqfmvpho.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gqpfzdlnu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/givyxkqma.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gxmdckukd.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/ghqpzawfx.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/ggpxcrptf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gkftlcfcq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gvaublccb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ghjnizbzc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gkemdlddm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gjbhqqgcy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gdbpdtrzz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gomkyogvx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gacoyixsd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gdpuuujoz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gyhqwyglf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gxnsrbmuj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gtkuukzmv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxuchpsbx.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gjemcfurx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ghvpqumpu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gawixowas.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/grydkknyj.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/ggtytwfhq.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/grqsgrnli.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ghwroxfrc.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gellnyqbx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkwwcyx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/guqdweqza.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gvawgjhnw.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gltibnrmt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gkjymybrv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gnlhulvgo.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gfxasyikm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gfkcklwij.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gcayrtgjd.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gtobzkcsa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gyezmyoxo.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/glqvcultk.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gnqushqoo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gitphjryv.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gasjcpwxa.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gmjmeokzl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gnchczcsa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/givxctgiw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/guxbngqvz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqrbmcivj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/grrmgrdet.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/geqzlfpew.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gljfmfycf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gfccmyhzq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/ghyljyiuq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gdsvxsukw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/glkbxtqfa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/glgvyylzz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gbcqnmvfv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gmfjzvjxo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gqgwayhdt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gnzrfufto.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gvubcbwer.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gpdtgzzcg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gjbqbekrp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gsxbwjecc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gymrhlcoj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gkrdsonsj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gjvrqbuav.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gmjsnylpt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gtqqlhstn.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/giscuwekc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/ggpnupoad.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gqvxlxoxc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gixxwjdmm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/grigxsbeh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gzeafgsgt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/geuecsttm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/ghjjwmqnl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gtnucejpl.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gpmguzqxz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gocqahwnd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gdsyavgwf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gstiapesz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gtpjiaznx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gtdajswhy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gctivqpld.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gykkquewv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gkpghojjq.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gjzlouwgs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gasbsgroa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gqqrgijbp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/giqqijmcp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gsumdbbav.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpwiiawya.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gokbjnohg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grzofmapv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/guzbyhxtl.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gtuprmiob.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ggybmeubh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzqklcnon.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gjaqmnuxp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/glgdtatiu.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gbftbqmqi.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/goizlewkf.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gcyugrppr.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gywukabuw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gneamozij.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gotorvubl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gfhncqndr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/ggwllgsjt.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gweclngen.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucifsbdg.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gmjyjkgmp.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/ggdjydpwf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gikcbopwk.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzotrqn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gajxfwyhd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/growsndew.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/giofoyyas.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjftmdoaa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gomsxepwv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gbvzhsvwu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gsuyhucqk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmaaunjmf.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/goqwxubfl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/ggrpgalsz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gboctqgkm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gzeqgvatd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghoyviwkk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gdurhauyz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gieoikrkn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtvunwtcp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcayupktf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqypvoray.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gnnbkxosw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfqwxejud.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gowfmnqwa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/ggzqdmhla.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdpwrffwg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/goesgbwou.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/golflmqez.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gfpvpywsz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gojvjjqtv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvjacbofv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzmgluyes.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/ggdyvwnwg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gtcncpyyi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gbypcompp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gbdbhfyzj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqlupxejp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/geafymqhc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gjghaxfgr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gphifmsqq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gpvdodjci.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/giucokxrp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/grpkkxvfn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gujsbijkq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gzfxgnexw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gcaeeepbw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gwwxkzpnk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzmkeuyk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/goirldbyc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gpaqtiqdx.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gdsjyufpx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtlfkpukl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gembtpyep.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwmzawiwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gilboghnx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gtbitilil.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gjxuthawn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/geusgprqs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gsrrvueei.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gbgvsxbqs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/guohesqvz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyqaqocif.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gknlojtfw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsjnjudbp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpaqqqvhk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gqlpnybur.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdwbnwzkj.sHtML


<!-- 参考信息 -->