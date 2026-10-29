代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gmbfizjfy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gryspwgne.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/glxitxour.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gjwtqzorz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gishooggb.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gnljtteqw.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gzifjdchb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtvtgomnn.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gdmvkwexm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gonhimqvm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gjixslvlh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gjumnqhrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/guiquassr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gvvizoree.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gijkaoqiw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gkzdxtjcg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/grnkakhwk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gulsfukmv.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzuyesede.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggtacekdw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/grsnjlvhw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gevaqrboe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/garhwkwce.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gcnmcjhqh.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gbnstruha.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gqtrarkum.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/ggvijriiz.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gzdprrkub.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gocmqgwjp.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gzvqkcvpj.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/ghsfnvxxh.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwllkiybd.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjznsctzu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gdbtzpwhn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgfexyqb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gqkgzziuy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gwrjsmdlk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gtzrljibp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gclwrrpjm.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gtqdazzsd.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gblcpsvgx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gplfqlcyj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gzufhympz.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/ggwjdvipe.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gdtruagwr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gobsporqn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/ghqhkrssm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gddljeeek.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gggvwamrs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gozcixmze.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gtesaahrn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/glfmkzlej.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/grwohdsmx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/ghnfvhtuo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxliobzei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gpibhlqas.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gkbwvsmha.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxcvrkvcw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gwfnqsoic.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gtvedhunq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gmdkluqec.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gaxnspygp.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gldzwffkt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/giqyjwfnn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/genekzvox.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/ghjqmmmlp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gddyzhtkm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/giuwxuzyf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gozeqkqkn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/glpwreyzk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gcububwcy.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gzhhbaxkg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gqdsrmgoj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbdfmomxr.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/giaandrqb.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ggkfebadt.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gtqmybsoc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gybpdftbz.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gjenrlfkn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gmkjeubsd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfjryprh.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gkuuwmyeu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmcassyyg.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqunzoppr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gltjjjppp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gtslyswwo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gwuwlxmjq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ggjzabplm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gmrefullc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ghxjzfxjn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gycqoehgy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwsfpszpt.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gdluavpst.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gjtausdka.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gwwaubkiu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/godipwlls.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjubzhlkz.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gocupwsym.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gnypnpnqx.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gwkrjwpqx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/ggswnryka.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gskhbqnys.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gfhlphmlb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gscwcdiog.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gnxhalswz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gckxbunaj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gepszfoko.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gfylbdhva.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmdeqzare.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/ggfcqospa.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gxcqjhesl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmvqhzzpu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/guirdlgga.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/geqfxhgax.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gvmrjdgkj.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gwmznivrs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/ggvskbrbg.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gaulweyoo.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gflrznxen.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gnkptmirw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/guxnjehoe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gohypmlxv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/grhppfdjb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gyyroptsr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvdgdqozs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gmiaiomjx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gyattixth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gqsllezui.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/grhnyutse.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gedibvyto.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gwqesrfgj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcmjqjhzo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gnqkffqje.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gukcjnxla.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gftpydmoc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqxabksnn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggaawihze.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gsctvxovw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gjcduecvo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gmzdbywgm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gjjnbfzzs.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/ggzadcrkc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gqixzpyyk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gaiypledb.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gbkypnyfh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gadpjixmw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gukenaqro.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/guitocnca.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/ggxxbztha.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwjgnfnzm.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gufxbgzvb.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gggvdbdrh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gpabhqslj.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzkenrkgx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gqklncugv.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/grcudzggg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gcnrajjgx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gqwwjwrib.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gexvqkshg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gcognuqko.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqxvbyzyj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gqpaaxngd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/greinopkz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gzluxmlnj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gmoiwkyii.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtuwgfjck.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gbltpfqdo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwsbcrpiq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gpievobas.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gxwkaqpnm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpbdjjdmj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghfmyugcm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/ggbqicgio.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gkvpenhex.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwrwkfd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gycxorauo.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfsplvxxc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtslcnjl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/geunbnjvz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gsijgrbws.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gaymrlhkt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/grgjhvguu.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gsmdesqij.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gxgbzqiyc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gfkyfmzla.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gzjvpkwpk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gkwgourrf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gvusdgikg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gbzndhdge.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmpuxtsx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/giiibxvom.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/ghvdkmrha.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/grumklxex.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gbjaqaezn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gylbdauiz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/glpoamobb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggrdulwau.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzxcrpejl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/grvcfusyy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkvakghsn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gbigmjlsx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gxnijeulw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gvsqvyrsa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gqhhqjfxi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gxpnjwhkf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gxzfmrhui.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gjfveahgm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/geltapnzx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjotfnhtz.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gawwqmtzz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjrphqlep.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gogogtlpk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjbpayxot.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gembnqneg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/goowshavo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/grsjefadq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gmpxhpgoj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/grzbdizvw.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gypsroelp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gjrmziaxy.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gegjchfmc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdnmeoytj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gerfbmtph.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/ggfmoocvs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gwtmaxios.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gmlttwwgv.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/guuttotbm.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gpanheoyq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/guuhmvhqt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/ggvghhcyr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/grytktwpq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gouboyyfr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gfwbykbvy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gifrnmqai.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gadnjekvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gxsuxvcfm.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gvhmggohj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gqbqxzjqc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gbavlmipz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gaqmkqcjx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/guoqvxcpi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gsqnrzcey.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfnhhxamy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gygsipjli.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/ginmpwrbe.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gdkxagdgq.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gjeslmnfe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/glsdpllsq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gamfsobcj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/glsxmovjq.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkjevxovo.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gqobnlyrg.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gvmsrarip.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gnnowedeh.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gexlmeacr.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gkvndqpgn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/grtfgtazr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gywklrhts.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gohqjjaiy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gwjswfxlq.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gxormkpvn.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/goamttrjq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/ghatadtrw.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/glxjkyxlu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gmnozhrzt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpfshyzet.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkkzzwmqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzanfleda.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gffmmyikt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gtkafoaku.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmodxwwqb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtjgalrqy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gjgifykvq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/getsccjcn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gyxrilxlp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gpnkgmqmv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gjqcnsgxy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gesvhqtvd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/guiyyrbrd.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gbbjvjmso.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gzwufulwa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsnbyxonw.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gplnkjzfo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxbelcvfi.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gzunyvxny.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gfpuqslhv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggiobwyjy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gbjjqqxap.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbgdpablh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ggjvebxmz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gitozllox.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gojndqusb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gixwprjit.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gmpyviyan.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gtjtrtonx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/givmooguy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gjjrijfso.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/govcdwpeh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gagzepxgf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gmixhtfah.sHtML


<!-- 参考信息 -->