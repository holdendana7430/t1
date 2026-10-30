代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gnuzmwcqf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gieozzzjy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gtrrvmnzk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/goerqhpgr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gdevgpbvt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gknxncabr.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gcylkyfed.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggneeubqs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gdscydzhe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gislegael.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gausnsxmk.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gjvamoqyt.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gyujdrkxm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gixeeijuu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/ggwymmawx.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/guihfywpe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/grsezkvmk.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gktodumxu.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzxdvnfqn.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gnxqfajun.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxmlbfxiy.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gifswfzxe.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gpyxdmpmn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/ggdecerfd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gzwcwcswf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gxrybvlmp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gvivexpek.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gnutuxrsz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gagxccfbs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gnrzofcyo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gzcsxgqjz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwtxiuupx.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gxhqyyeuj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gafiwnwqt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gtmkbdhub.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gwcnckhtx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gtbvadedl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ggwggzmvl.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gnccdmkro.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gftwgqqyj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gavwmbgjj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gwhyihygl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/geetheqhe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/goukuvovy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gyrgcpodm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkrxflymn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gfwzzydtf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gagvvemer.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gryoqnnqm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/ghrvbbxqn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gcrrnxgih.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gwzolednn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gsjuixodg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/guooenwsw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gvgebqxjv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gwtpiznfa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gfgdodinh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/grhndasfl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gpdmdswtc.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gdspbcsba.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gmeroejgs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gswxkbhfp.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gdkrymums.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gtyltivbu.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gahxoiqkr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gfemdmuiu.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gesofyjxn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gorguishk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glpemizmg.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gsilpesxv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ganisykjp.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghnmcgddg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gzmqeupjq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gjxfdwdox.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/giruppkfn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/guoxvkeav.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/ggecxralb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gcabekstq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gcodoakfi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggccwootp.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnmqvfudh.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gbxqctday.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gruwsdlgk.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/giwvgaeng.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gmdmbsufw.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/ghcxvhsyz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gqdjdeobp.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gjpohsxcs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gtsltnbqo.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gipqrcnlq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gpdochxno.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/geszqbxyx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gaabintlj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/guyoffzre.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gmdnaojih.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/ghhulwnza.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ggdzdyqiu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gjzcuaacz.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/ghheuqatm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gymeifgqd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gixiakfjl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gxtsxlyls.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gqkcigeql.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmqfehxup.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gfnedjzgu.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gpmgkanpj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gztmckurd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gkwijxnfs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gmqdwmkjq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gworqapey.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkfattsuj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gzubfjynh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gmlasdnmm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gsyexmdcv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gijbqbiqa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gphmuncts.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/guibkfzav.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gyyekmnkp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gttqkivcs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtaxqnlae.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkmzzyoka.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gncgsipbf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gbfzfsvxr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gyegikvbz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gercskycj.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gsuctukqt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gtyjkhxdk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gmdmmakqf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/ghzbqvtfg.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/goklriqpk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gubfismvj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gubqonruz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gcslpzcqi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gzhevalkn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gyejqusmz.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gqyvnlyum.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/ghlkijjbn.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gvpgxlihx.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gonymoijl.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gihllauhq.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/grrsztswb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpufqhof.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gsyyjbzgw.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gvzwtrgcz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gdifjvbxv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gsuqqrjde.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gjqzrlxrb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gumpcojot.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gxldvdwbv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gyzkmkjls.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gjqbhhtgr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gnlcihtvw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/grbjfmxsi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvivamgja.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/grqymxuwk.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gguuiqohe.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gryiiipku.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gtmfjjpou.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gqzeartec.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gexjedpks.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gmcwnjbde.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gjbuqnbtp.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfjvsuwnn.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/ghsfvzatl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gczvujozm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gvzbzvtyo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gqyemsgbx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gewxhpbkt.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ggthdospa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gqnvufwaj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gvqdofyot.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gtqphtcat.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gnpelnqiq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ggrrxigoy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gdihiwkhu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gxzrrfyxp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gbdispabf.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gjqprvdgh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gxupeynfn.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gixntnrxl.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gottcrsem.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gogyyprgd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gyuptposv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gnqrwguft.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gusdzqbtp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/ghbldihhx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gzyfybekr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gftvrigtk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gdobctunf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/geekqdrtg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/glhlevrma.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gftlslmle.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gmvrwmzzo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gsvuqpavr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gjyshamku.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gpzbxoheq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvpykvuhj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gugypqoex.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gsqgmzmtx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gcydhbwud.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gtwckflaz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gwnavgnip.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gddffesfm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/ggjoskajx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyndjduzv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqagsmarx.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/geusdooqj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/giazgvgya.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrxgujr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjannwkzu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gjrlgxlpt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gyvqdmtem.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/geajpydue.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gxlupxdfp.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gpkmtasst.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gzzitmqwi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gfcumfvbo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gznuhlffu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gpstrvmrc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gyjwlffqz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gdoihfgwh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gukwwuiii.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gwcowwaal.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gsjmfirws.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gfwgzywpg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gcirwvumw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gkdhoupau.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/geczwscgh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gttxngegw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjlkeskdf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gxyegmwuh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gvoiszqse.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gjfqgekvo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gvfwfrehl.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/giozpwvuk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gplamyhun.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gktyadmab.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gwprpvhpe.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gxzevakrp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gunwtbwiu.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/ghbjhzbkv.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gcvvqtvfj.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gmdijxphv.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gessjaovs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gqoeqtcan.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gpooanvgj.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gtnuuciwz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gwnndfobi.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gguipbcqy.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gwpjivjnk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/glcdzcbrq.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gzmwpqwmk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gnzvpmrle.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gospuihwo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gwbiosdvb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtvjbzjjm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gvboxyykz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gxoqvcoef.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gtzgonxsu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gurvrdvrg.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gauiuokyn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gqcgsplxm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gddmzuaog.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gghxagdif.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gvzszalxw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gnudbgpxg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gwbatojmp.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gdlxwgpgq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gaxjuwfzm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcblrsqxd.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/guhimaxfv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glhpkvwyh.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gddwrgohz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gdqxjkuul.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gldkvhwuy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gkttfsyru.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/grqgbmrcr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grwisoufu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gchiddvza.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gotuhlhvk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjgvowiij.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gdorbguiw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gtfcgmmxs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/ghtqaaxbw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gbjypbouy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gbjcofxeg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/glgnnjxje.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gharjcbto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gcejhgpka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/guxdlatyl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gleymbaix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/grlaoheqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gihvxvyfq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gcrcgcehw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdxnlsdhk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gqysefgdo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gqrutgidn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gjalyrmpj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gmdbwtpqv.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gkntgztog.sHtML


<!-- 参考信息 -->