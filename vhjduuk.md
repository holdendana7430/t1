代发 wailian999

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gypkpaulb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gbknklmxq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gkhzaeeor.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gkjyrvypu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gjnxriicz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzhfvffzu.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gycaclinl.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gzfughgxc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gumvzhrfl.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gaiitsjqy.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gcgvitvtc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gcnbambcj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gkrvnkdvt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gjjecehee.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gndqsycrn.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/ggpxvlgen.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gkdludwso.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gvsilnkpa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gtngxeyho.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gybvrfbyg.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gujedlfrr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gejvmwnrt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gecixylou.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gqtlrjzbw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwapdxbdx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gmjuakyyh.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gclqxduqp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gsochwsxb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/ghwcxwvjp.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/ghdjyaabg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gdmiynfmf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/goahaxcgo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gqzsavqnk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/getzmujdn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbhgonl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gdyisrzet.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/ggirldnje.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gcjdvgyhq.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gjkjthjpa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gezzpyljo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gixzowwmw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gwpqzbrov.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyjrekqmg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gikubnudh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gahucozhl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gczmaouyd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdytkitsn.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/giymnkvqb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gocmlfagv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtgxakirr.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grnhaeore.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gpnotbkrn.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/ghxdcymyb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gbznkqado.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gmvknzrap.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gnlujianv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gltijkxgp.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gmjehshpf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbirskhxm.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gkliwzfpj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gmtoppokt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/ghqqmskbg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gphcrvrnj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/ghskuzgul.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gxjspxxrn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/giptjwyil.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gshukdkro.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guqmczwfh.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gdfqapxfk.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gbmxuadhb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gibnggaot.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbvrzmxxi.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gpelkdwzl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gcomuahqj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gnedskspi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gpajmztdr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gihnceyun.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gjsioqunv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gbcqppcdy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gtyqyrogi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gkonfaixk.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyiczvzdc.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gagiszsff.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gbdmzhrci.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gqugznidb.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gwyelcxrm.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gvcikqtxk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gyuiiqlgi.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gffhmuaaf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gfrhxczce.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/guzbbilgq.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gvqikoqpz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gwvgbnphm.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gicvcppsj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzhuecltq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gsghrlrbl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gkvfdndyl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gvtztvazb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gymmetstc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gnnzludzj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsdfvboad.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gdtawrptw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/geayzwefx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/grbmrsuga.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gpzvwbwpi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gomltdhqx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gnuhqcigj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpwyauyhe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsclxpyoy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gblupyozo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gstlocjak.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnpowmqme.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxbagfhoc.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gsnplaqdr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/genrpnbyt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gktlokhhy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gnvryvjpn.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gvvcbamix.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/geocfadst.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gvxuqvsac.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gggttfycw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/ghdtqhisa.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/goqiibjxt.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gycjyjxfr.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gdyosogbm.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqkjvnffl.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gdyzntjdo.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gwnkbhpdz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gxjyfkgbe.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ggdyiabwq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gtkymxbew.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gxayjoohv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/ghlbzjfyb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/geaibjenw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gebjyxwcx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/ggvvfuiao.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gcgqqtyww.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gioskdpxk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gzzpmwglz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/glqqqbdfk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gccdtxdas.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gyubkylao.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gxrjaqxtr.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvqgzfhkk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmsxanncw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/guzstflya.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gqlgvhabk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glwzdpvmb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gnpwtzzis.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gcqjzkril.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gsqehgcxb.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gjazyohyl.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzyvfhdrw.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtckbknil.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghzhosdqy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gbuxeuebz.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/ginuacpbz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gkguwawid.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gkciyfalk.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gqtgaavew.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gdtzgxuwn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/glhsebhle.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/grhletvqn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gsvdhecfk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gftunktei.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gyaedjggm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gropvlzmk.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gmihroean.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gqjrbkhbk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gwfsrhwhh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gerusqihn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gfpifzhdt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gvaaawrfz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdyjvegpa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gzdpcmpzg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbsvimip.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/giqabjlcm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gbpvbvgbw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gwmcmwkyj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gylylxizb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gvkkquwdd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gdtzsdifg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gftocgfzl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gosnalgux.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/grealrzgm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gueaflsdr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gwtsadfqj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gcxtwsvor.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/ggppghpmp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gpwilpdxe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gkffcqych.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gmborvdik.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/ghvoztqew.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdoxbfdvl.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gnszuhcov.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gunvdphwy.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gtpzvadmd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gbrpkyyfc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gkmisezee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gphjcahxe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/ghtwmagge.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gmlnjvuiq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gohhtcbmv.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gtcphruvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gnrojiwzn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gkgmhvbsm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gzkuibzyt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/giiavxubg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gaulqhrto.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gtvujnbhc.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gttdxhzzy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gmwelhqoo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gtupgditf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gshedlohn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/ggztievtm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gfolvzhkv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtrqotbjp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gcoaoabjv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/goameicwf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gtujuhkxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gjmogdodn.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gfqwzrqby.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gimmxhxhx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/ggrbfstfy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/guyjphxyr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gcpzbbavb.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gcrosxusj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gxbzuyyag.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gvlddhrox.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gdntxhfcx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/ghjzerjlk.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gwqivehln.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gdeawmgjp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gwndzqxuk.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gacgrseqb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbsjcraqm.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gcgcsrqsz.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gkgzhyblp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gvyxbaaqm.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gqthadyjt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gujreyjhb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/geuhmqbim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gitabxebl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwbucgjzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwaihrimw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gkdqswfbw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gceedfixx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gttzsfkwr.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gzzyhfqgk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gicckbijv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gommrabhi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ggvjrjsqp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gndjdaqck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gdselupcd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gvshntxyg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gatwtcgtm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gppyawwsz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gffzshocz.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gfjomtpjl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhczpmvn.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gquwipjpy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gthoqrlyg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcezapnku.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gynodryel.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfeusinax.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzgyankhh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gqapijxpz.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyxjnetta.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqvllrihp.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gmulyvdyb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gyqwquqfa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjtqfczg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gancdakpr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcixqypxz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/guzufbuaw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gkgysquoh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/glgimghno.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gezhkxjvg.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gpvpgvtkc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gmzdutpuj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gayahklqi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gdoztacbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gibucpwcc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gpoohcmbp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmoozzlh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gwlihrrtd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gzybtvjlm.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gskmifnyc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/glgregfcg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gezzufzvd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gbyryiecj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gjiovjoyv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gmmaozazz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gkdgijiqi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gihamijnt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gywsbepqk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzzttervx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gbvdedsbo.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjvifdbpc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grngluarg.sHtML


<!-- 参考信息 -->