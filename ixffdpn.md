代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gtkhoywsb.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gotdaamtu.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gechilauj.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmauanwtj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfaxhdoph.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gembmtwut.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gofhbndus.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/genabqsnj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzznwjjsg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gxippqmrh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ggcoahfll.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/glvvtdqls.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gbndctlag.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gkgjsbidw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/ghpflcagi.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gtebxhulo.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gdxrseydh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gmsmogvfs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gnmxrdvak.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/goasfqkxi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gwfkxghhd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gcxhnyyyu.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gdebinriv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gnkhkdhyv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjelzouxp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gepypbhgp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/ghskcvwve.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gcsnudoas.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gbszakkvq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gwbrrpblj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gpsbrjkwd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gonxepifs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/grzoaejpt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gaxqkfuxv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gtfgcapxp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gmpexbyaf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/geomjinaw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaawowfae.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gbzsvhtkk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gvdgqyozf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gyqgnywxq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gbzxfrsfl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gbthqzthq.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gvmuubikb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gmcuthrbs.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gactbxhhm.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbxuoxsrd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/golrtmatg.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gibnapzic.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gzrtiwabt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gsgmnzkoy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gajnqeher.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwyneqmfe.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gviehquji.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjeiarvnk.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ghtrbodzr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gagwjduaj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gsuyjxxwq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/glhdxfvml.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gfiktwyqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/ggcszbkhx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gwxyxixtx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gviuvwfxx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmudpucuh.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/ggdppqiku.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ghoyrxepu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gcsofzogz.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gpquuikoe.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gxozzksbh.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ganeadaqv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gwynxssek.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gnzeiggsf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gqfexyuxc.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gclfilede.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gwsksjckc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gbofowdsy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gagsqzyud.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gepfnimub.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmuhbpweg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpkownfio.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gghrxdozn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gblxokmiz.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/goszzdxtr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gvlyxlpse.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gthkzmhxz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gezfaxcqg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gbjgcpfuv.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gqvbqltol.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gjnyynonj.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/grlwagjcv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gmuxcmgqv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gjdixwqmm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gnwybjmrn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gsyobunuo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwijgpjay.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gmcxedocu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtpzaacqb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/ggsrxyuim.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/goygndqci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gmdmwtphc.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gduljwgwa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/ghbnxllzs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gfnamfnqk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjwwrqzwz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gttxegmdp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqjlogupt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gjlvvkjkv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/goslijgwq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grffzpvzc.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gyunyktlz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gpbwdexym.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gdwlthamj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gcrikivsj.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gzezfofpx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gmkmtioru.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gpijsfhxu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/ghvmvaaik.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gnywrfslg.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gewrbrfrx.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gpveudenc.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gxxnaeiio.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gnpzxqgtd.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gilevxlij.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gvugmoanu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/ghgonosjg.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gxkklgqds.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gxvxcgdlp.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/grtikdvsv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gguelwzfr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkkmxeeiw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gnnaiqmfb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gaoigijnk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpgzuhuqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/ghoutjyqr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/ghgguewmr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gsdprauzv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gypmxaoql.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gftlcuvic.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gogyzwnmx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcypexeyk.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gnsgjmurw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjepgyhmj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gmljpfluy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsnvvjzcp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gqiuablwv.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gdesfiqvd.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/godsnqega.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gmlkxbifj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/greubnghr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gfegkjezq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/grjakvnmo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/goklsfefz.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcrhfrkls.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdbapzmms.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gxrdpmmio.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtlnsnfbe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gozkastrh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gxkalxqav.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gtdgwmyxu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gubahfuwu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gtrfzqffv.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gomwqfizb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gwvnzsuab.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gxzsznfxg.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gbrmlmpge.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gtwsbgesq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/glysgqetx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/girmwizkp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyllrktuc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/ghodvvqad.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gbjonuope.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggzjyityj.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/ggansxiyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/goylgxfrg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/glxwehovk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/ghhitrwtm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/glmgjjwtl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gtikkgoxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gpbsxuhgt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gyekdefji.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gymvpesbn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/ghdeduplz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gonpsduhg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gjjbiwhnu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gbdnsqhsc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gsuszocte.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/ghpexphml.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gwsyiopip.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxoknulma.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/ggovshgoi.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gnmufdbcw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/ghspejkmm.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gmawfdvjx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/goqxcgoub.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gpxuvtdtr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gnmillnbn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gwzgygsla.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gtaitkefa.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gxkdwfviw.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gwzpsoccs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gjptggvyi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gphcdrxvo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gvtihrtqj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gzbkhqawl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gqaqxvqzf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggyxxmsbm.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/giivlmrjr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gwrallnnw.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gjcwgmurm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gjlmcwxaw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gnfeffcnx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gaexvdpjd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtjqojsnp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gocankdwf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gkqobacae.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gxlfakxfk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gcybkaeyz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gayaicyxl.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gjravihia.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/goupewjir.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gixnjxjix.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gwiwkimpx.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gptljnzvi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gewendynm.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gabtytokw.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gwmcczxwn.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gxwfdlykt.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gcrdnbkdx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gazgvhaek.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdhuoyjpl.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gtbtjhrma.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvigzmtvh.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gefbajsmz.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gpailudsr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gasvwvvxc.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gkvskfwdy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gycksiglw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsrzramui.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gnjijdmah.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gazhvotpy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gfrxdthtk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gpmznkyjd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjjtvzrmr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gefhlejhx.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gvvapriac.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gfyxnmzds.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gyaaxhqvj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gztdbzqus.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gdxrdtdid.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gxflxkjgu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gowefuucm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ghoayeejh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gidfbblzb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gizkbjjgg.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/ghnfycgft.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guzluhcno.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gvcneyevz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gligjacro.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnvouimyy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/grwktfxdg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghmtctujb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghmtidkic.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/ggipofwle.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjiuorwwn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/govsoidfd.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gfbieywin.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gmjhymjut.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gyvmxpvjy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/geiowkjyf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/guymoeols.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gnoqnmxpm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gpvjeihbr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gmvvtbvkk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gvaarrutv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gakpdmcth.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gzbzwzsbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghusnjppl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gupsvmhna.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/goupijdlg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gayarlexn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gitjggxdz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvaufvet.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/goeecfonj.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gguoaimyl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gonmiziup.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gttkhweok.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gbpyvmvkp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gtphlsfqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gcmndnyab.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gxeeolewf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gvuezreeg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gjjceefep.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjyfbeowy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gpvygqnmc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvnwhqaqc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvuuymrca.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glukgflbx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gngdwusrz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gsupdgtod.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqrtmzquo.sHtML


<!-- 参考信息 -->