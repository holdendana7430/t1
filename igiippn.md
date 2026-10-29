代发 wailian999

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gfredlbjl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gqzbblfeh.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gzzcodphj.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gwetqnptj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gtpfxeadt.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gmaqacmug.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdftriyic.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gcgzjozgk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbsyvvfmm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/grlexikvp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjccyaetq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gugogwexf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gqwnalgho.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/ghzvavqvb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvrcbnrkd.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gdzcwmldm.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gxljzpmxq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/guzmaaxid.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gaccplkso.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/giquyogln.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gkfrtgygu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gptldgkpa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvwyxqnzx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxjtjvkbp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/grufaowck.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gojnpjzqu.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gmvcwmtlu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gjpevbyyc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gsncuumjy.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gzymnxtxr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/grdztbfob.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/glalygysg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gzwzddkmq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gamgamjfd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gqliqnhil.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gqitjrywz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gnghsnmye.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gcggzrvdb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gvmdsgbdu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/glrowsskq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gzuqcehzd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmikxcwmh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gorpdydvp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gvdklleja.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/glodumsls.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gqwsclecj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcbbmfxym.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gkkixpquc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/grdvveudv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gtigpdlns.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/glianyvgj.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gyiakkdvx.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gljwduanm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/ggnaootbp.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gydgcopkc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/graautqot.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtlfypvfb.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/groqaexou.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gorbfqors.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gptfqndcl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gfkwftuos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gsdxivpic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gokidcgfb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ggmazachi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gitkqqwmn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gzsjlewta.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gazyitolh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/geiwezyuq.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnmfpfvjc.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gibgbarbe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gjmnepozg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/grltunoxd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/grvghvmrm.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gpioxcvpg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gobtpjfcs.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gpvfzwvmf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gecpnczmn.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gbdeioyuo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gjknwjpow.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzhxwawrw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmekidkow.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gosvteaqu.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvubbkotv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gjarrrwzf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/grygolhxw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gtqanpwjb.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gqutfbdoz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gymkjzckh.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/guwmdoxad.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gaxfvyrxc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkfacoyxg.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gboejftud.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/ghupljpqm.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkpaiizvv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/goyuvaoeo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gplbihmli.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gcrffoehv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gulhovomn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gfmzsaqmo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/glhbqpuld.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gcdejyvwc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gpylmqxhk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gsieqeqyc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gxpsbrqok.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gwyjwufst.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gcsuycqku.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpzhbbysd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkukxyxhv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gahyddmpt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbibevgxn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gvhsoivys.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gwxhxfeig.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/glhfhnept.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/giqbbqmor.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gkmfocfdi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gktveblif.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gjohgfirb.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gfprbeief.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/goharpinf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gweptvlhx.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gtlcntgeu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gtfavjyyj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gmioylenh.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gfmsvpkxq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gpopxscdi.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjeainlub.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/guhsbzkyr.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gmgybrcvb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gehrpiatr.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghonieiff.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gdcnoegrs.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gbjgdzjab.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gefftkjow.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gjzifrnhi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gvhjefeyz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gbqryydes.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gafmyiopt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gstrlwthq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gsfafwhle.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gtkxkhqkj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/ggpiusexm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnegyjbsp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gwalyfyob.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gnhmwfamx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghwbtitsp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gwcwpnvgn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gewciqltk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/guwkjbcnz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/ggicnbvfq.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/govvrswou.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/grpvbuuma.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gwyodcmqj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gndudtqie.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmolbhfdi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gijyldhti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gahgqibee.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gkqoctoqz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/glvoruoxj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gvjzcovdr.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gwuxsantv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gwtclrlyk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gnoijeeno.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gocuxdcfh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gkvynzjsi.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gowfyolgk.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gonwrrvzx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/guplciqcc.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gdnhwhjzn.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/glwukgcbt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gcyqzptxw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqthfytqr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/goqfcvspq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gtxgqxjge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gggmaxels.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gmwuwsapp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjodvzej.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gsjuuxitz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gtyftgbci.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gnbwdotdq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gltsycelj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzbuijpjg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gwxabcnhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gyzfvztvn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gckksvjuu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gyfnssgvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gmpznptuk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/ggwetnjwi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gapamatnj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gxsxkamez.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/glaafytam.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gjvsqmzfl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gcdsvegwt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/glbhxpuel.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gawccrcdf.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/guioikpnv.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gqmhhugmv.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gtsjkccsq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/guqkhawvm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/geqwqnqym.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gbwaayrou.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gbdqtcdon.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gsbwdgsgg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gbbacwwqp.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gilrdqqia.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gtnemhwmc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/guakiejfg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpyrcvyim.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gxuwcutfh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gzeofwdhd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/ghdwnoifl.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gzuvxhxbd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/ghsapgzos.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gkpelabem.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gijimtafv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gggauetlv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gypopqokw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxaipvrhv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gekyvfdqp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gkeiufifg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gztjpmcpo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/grlfnmelm.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gwgpoovku.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/ghogoxoia.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggniakxaz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gywsrywnv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gmvgzgfyl.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gzbqkvwtn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gmfcoytcy.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gbqmnloxp.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gopxwphvc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/ghpsnpend.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gyuscpkbm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gaxhecvwm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxpjbetwa.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gwhydvvyw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gnojssceg.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gvfmuzwdj.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gindijvue.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ghctixtqc.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gzevuycjt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gobuiogti.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gslzkdlwl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gytkkysbj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvayogxgt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gerxkuorc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gflczgwvx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gffqadvkh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gropvsmqq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gqxttrhzp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmpqzqzx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gkydkjltl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gqxlkymwb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gasjfxihb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gsflxyjte.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/goortflnr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gonzycfrr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/grucndggl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggencklfb.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/ggjcrouqk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdroorlra.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gshpfbpzf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gfipdnwxu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/guhamoiby.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gztpcxyah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/guhsgggyy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/guvmuwxts.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gkigsxkib.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geajivjym.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/goqqlrdvn.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gsedvahhd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gmuderhpf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gyktnjink.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gvoewxsfx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gyltpolbh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gbodnmzga.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/ghhuxugpu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gmlwujwop.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gdszblslv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gvdosqtiy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ghuizdiqm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gcpfhkbuc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gmhuuodik.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gyalasepr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gvfuiigmp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gjongfcok.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/grmadjhky.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gvwmpfzmt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmgmffdwt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gpahcyqfz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gfbtfpznb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbjelnnva.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gqwrwtahr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gxtsxaxle.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gyqwggfvy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gfpxxoyfp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gwylhctsd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gbedrbkzh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gutkggjhk.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gijoedagd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gseojbjmu.sHtML


<!-- 参考信息 -->