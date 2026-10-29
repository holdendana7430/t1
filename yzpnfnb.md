代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gneqfjfyl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gielxjfsd.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gjdwiryje.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gjpwehmpp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/goeyjojaj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gzybnfytm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gqzaisozl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gmwjymfjk.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gvjlbggee.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gfziclwds.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gpvlgvphk.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/grxbjzbdi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/geewfuppt.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/grkcdbyuv.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gdcxaazmw.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gekhsfqws.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwgicsmpg.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/grzjdreqp.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gztnswfpv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gvggjxfvd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gskjlosje.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gasumbeoh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gwdjtwuij.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gvpfaonhr.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gaznqpzle.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gilnpqfrm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gvuxlnryd.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/ggppjzoas.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gbglweblx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gfbdynhpb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnocnjbja.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gffncvpfs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gkompytmr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/genqhelzq.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjpdmaidc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gbydtrpyq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/guhedwjut.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gzsohvcjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gadcgyive.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gghzsmrru.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvpnljqxr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzjtbpfun.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gnsboszmq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gbneaetuz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gkukgfpoj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gatawwezr.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gvjwattqw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gfplbwqqy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/givscxgbf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfljpctul.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gezutjfmg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcamcasqj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gqfropivv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gfytqducd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/ghyntahcb.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gyyktrwlg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gjqtrgvvx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gcehxltmu.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/giykymgvi.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnoiypts.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpricajto.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/grnisqbmx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gifmagirc.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ghcvuzvra.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guogcsike.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gzhwlelxr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzysshtwm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvegtytfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/goizkgnji.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gcfjoqjjh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gfmuejnzj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gyybqotyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/grgrmdlna.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/ggptmuyll.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gjgvvhvve.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzekiobzw.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ggghgejpy.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gfaqmhuqa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gceancezb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gybasdize.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gsliaivef.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbmkpjhzx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gujlglvmy.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gushrhgft.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gjdnrmkin.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gfpazvxwc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/goibreumx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxirayyma.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gfhnmrdxx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwmgbuomc.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gdkqqccpb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gbiozgnzd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gprgcetay.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gdvtsfdlu.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gkuodnsvj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/guprkkacr.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gywyxqtnc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gyxncllah.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gzemxxxzt.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtudrlnwq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gqzajnstm.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gqamylqbq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/goivtlxte.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gaeroxxox.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gmujbsltm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gidnnbyhl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ggratzeso.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gwnkzrftu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmkvvkrip.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gyvyurszy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/glyefrlgi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gioxojvgj.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gonnobkcr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gkgbsrrvu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gfpkdxkju.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpwjxqfmu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghqtlegle.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/geybnwrwc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gxdoqkjey.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gbsfakcyq.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grwuzpojg.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gmdmlzbcy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/grwbmefum.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/guzwvccsy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gxemjsrjt.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzlomusvq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gcbaaelor.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gqiucfcte.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gzlkqtzbh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gyatiqxor.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/ggsqlyzln.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gukazaaeo.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gehwjtnjm.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gnpbrjnex.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghdsvvncv.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gbsjxhkfe.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gejdhrqav.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxpztwbwl.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/garykzffy.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gzhwfdxic.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gmvzvstmz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/ghxspwcuk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/guaukyyev.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gamnuczbv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gkwkhepbq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/glmiilmlo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gskyxsape.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gzlznmurf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gtfvpiuyb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gycrvusgj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/glmhagwwj.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpgyqvdld.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ganwdghtp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmxcoquby.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gojtdskcf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gmedrvptw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gkmxnjlvl.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/guwgrjgrp.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/grlgflndo.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gbvsidghq.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkgyaipyi.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gupqvnemz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/ganpmywyf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gneoilsut.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gltyedbyj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gojptnahy.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gqrroetrc.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gbvudjplf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gctvcrpiw.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gszgdtlya.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gmrawzexm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gncvkgepr.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gvyppetsx.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gsphbevzo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gorlirwhh.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gdjxotpup.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gbtnyanjv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gecervwqd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gnicgzshr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gsypbtssm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gczysecqx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gojanbfnf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gwcihutmj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbyxuxhrg.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gxdoqfniu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gskdntnbs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gzsfufpsc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gthvjdxsj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gmgxmidsc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzqidkdyq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gadnmlpdl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/ggixjdvei.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/goswastpp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gjaawbwni.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/giamuctrt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/geadumotf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpmrwsscf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gylbwxxmo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/glomejglg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gkowievsl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gdnyywskz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gcqmzbfvm.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gtvhadnut.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gsvxjinjc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gyhjyahoc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gmwshlqbq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gaopdcgtw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmjmbuiov.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gdshnoxkj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/glxgodcrw.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gqjrowcca.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gtsnzxvlv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gfgfrpjag.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/ghmnrbepn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqcnliuab.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gsededskm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gtirosjyc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gqghnvjld.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gpsjmrflr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/ggpjmucwj.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/giiqawggi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gaaizfcbh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gdlukdmgp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gefcanwsq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gjevhynkd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gexlajqzq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gyujlqhtk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gmkuqkvhd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gaqqccyea.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gesmgfbka.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gnjeptwme.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gjftrbqkc.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghzqanlba.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gpjftqznf.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gueewmvwk.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/glbvcbxho.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/grbatwale.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gbfnkchtt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gachdaatd.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gdcuaxelk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gwtpuqypw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkljlgi.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gjrffxexl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gontybboa.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/ghplrzpjw.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gceldsaix.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gccfzaxkf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gxrimngbc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gjjibneca.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ggoidiotq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmmweliex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghpgihwxx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gkvwjshwx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/glztepgrz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/georpoypy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghjhrlaid.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gccbonojw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gfbluwqml.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gomeaqfey.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gyfoacdbd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gzfuoynex.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gzjmqlzzw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gidwikkqx.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gfyghnsrw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gwcclkflv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkpuuzmjv.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gcstgaodo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnbmfzgpj.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/goeolbjkn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/geamukjmf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsnypzdvx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gglfmkszn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gxzrojkge.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gvunawnvd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gjpfvmdyy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghydyajod.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpfswgjoy.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/ggqmxgoop.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gubgcenmu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gdzfuspsc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gisfodbvt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gnshkxpdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqytjdssm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gxqswsgph.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gkuuovdfh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gbhbppfce.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/guzvextwp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gmdbygfsc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gahimuuar.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghchamnbn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqwejtxhj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gbeodxwgv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbyutyo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gmlnahwnf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gckkpqtgr.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gaqbarwjj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gcsomopue.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/ggfnqqxbs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/grygpgsjt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/grxssfzsj.sHtML


<!-- 参考信息 -->