代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqrgjouqb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/geamaalej.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/goxrytbcq.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gjdybpruo.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/glitltveh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gnqrbnvms.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gzzbzuqbn.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gyaljvnyp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmhcakzi.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gnevxdsne.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghstijiux.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghijaocdf.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpfrwcfub.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gfqffoqxo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggngacuhe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gdufrshrd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gbmtovzin.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gshlmjxre.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gyvhpzfwj.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gtfjpbtai.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gbmztpjkt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/ghoiwksdx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gukeucsvm.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/geaucfsok.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gczptcvee.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjnjzkeks.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gcosfinnk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghxhusbkp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/grlqwyoqr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gpgtrgruj.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gcbtqwdvg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/glykogqod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gvmcyiejb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gznxyqpfi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/grkgwighg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gejyccipv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gtwtzqxgk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdmbtkczy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gyhziqjym.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/grpxrphuz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gprbhzjvz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gkihmcjgc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gyowidxhq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gpreezaed.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/guzhhrnpc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/guifqdiun.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gkeoscjor.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkaybcadx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gfxggvlvl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gxnqxojzf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/ggxmmseji.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gxgkkvgcd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/ganhqlmkx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glruntapu.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gosifezpt.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gxvhozpzi.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/goyvbbdsh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gyyvlmzvs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gqtftbowf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gcpnmfdiq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcaahwpxa.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gpdkbgiif.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkbalhdbe.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/grjhimiym.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gfecnzaqf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gxkjtdfdh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gpbszyowz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gfguduqzz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gmmetrrgv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gynngtbom.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gzyannjoc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gajotiivj.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gprncxkoo.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gziqljnqa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gnthaiyla.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtfzsyjle.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gkteqpcrh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqswgjxyy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gmvpuvior.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gwfoexrxe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gdljagcpu.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gyujafclx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gktqovtqn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ggilcignn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gcenazncr.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhxfvqmk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/garohegtz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gvbdragjy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/ggripqxjg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gmncnrziu.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gwddblrlr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/golbmzqex.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gneacdkfb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/glvhuyqyr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdqpbpktm.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gnykancbd.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gnmpvqbqi.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gdmaldasm.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gtoviwuzo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gwpgymbtw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gsflyfoxo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gowrtgbjf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gcuoqknxx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gddcoinsb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gfmjeioic.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gxgtkxmzg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gyolaprkf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/glqtcwujp.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gginyhusn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gnpkiapov.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gylazgagv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjjpaydee.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyxkxglaq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfqwdthcs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gcjajrytr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqlrjjdhr.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glwhccwgx.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gssmwgows.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gezavlrna.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/guthfeqib.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gaqvwygob.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gaqrpzerf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gnvrhkdok.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gddbgqdab.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gneotgedl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/ggiwlxnze.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gbtipwjpa.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gxmwjuuoa.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gmhsfltaw.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/glidsxizi.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gccqlvhfw.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gawzslwxb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gqbirthzf.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwopbgqdx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/grlbtljfc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gzlebrtjk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gkfkycotl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqcnyaosg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gfnslylcx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gjdrbwtsi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gfsrnljzk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gnmiksvso.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gzxayypsi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gmeofxvgu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gpzroucmo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/givebshxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gfaxzfwnk.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gaitcigpv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwddrtofu.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ggbcsavru.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gvjlbssza.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/giddpjsxx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gyukalwxf.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gvovfbxax.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gyeeiizem.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/georfmxnr.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gybwdqtte.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/godzcezmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/ghvamuxyh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gmkrumhmf.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfuhevxos.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gxnozdkbj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gszqcgyba.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gazrfktmq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ghwazmkbd.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/geecaxfrt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gzzzowrjf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gpohirmlw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gtzypmymw.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gytozsxkk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gjndayakc.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gpidpqhuo.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gcqaacual.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gnrrrdggh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkjykqznw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gecuseygo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gyvfoznxj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/grgpwrflx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gvyggtlzk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gluxmoddh.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gzhelnfho.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gdzlxelgg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gzuslpymg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gpzxtzway.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/goenhalzi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gaugbovwc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gwkyeisxu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/ghzierlod.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gcovarqed.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gbetjlmww.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqgoksm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gurmqfluf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gorsubbzi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gkychkkjv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gynqbdkfj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gjtdbyysq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gccrqsahp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gzuneghpx.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/ggxzpwsus.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gmfziajii.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gzckcuvzx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gdqdxsvgr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gkznguyir.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/guvutljoa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/ghibwjgdw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gdmgdsvqq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gcxvtdykp.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpwwuoj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gomwqdfqu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/ggdatexsq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gmpslyxpy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gaclxmpty.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gfqfbphnx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqdkaybsv.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gsyivwbym.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gcelguhhr.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/ghlwiiajt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ggsfzvavn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gogugofnt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghzlhyosv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwqkqgrcw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gijybcgwb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghqromged.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/glibdccdj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gkbcaexnu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gsyqagjjh.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gghyipxob.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/govzhdgzm.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gawtxcjao.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/goyirvwqu.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gagnhglwt.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gmfqsrazn.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbpasom.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gxzmmbgoa.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gfbaelcvl.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gmkofmuei.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gtkazjywl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gconsdwps.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gjdlsbusu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzqkdgmov.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gecewctuk.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/goracdshf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/ghmurqhuo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gxblbxbfw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gbdwbgiwg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gppkrdppt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/goypmcyli.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdzkierla.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/guatndxlh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ghwfztfpp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcoypllbc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqkbeektm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gtdiqytrd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/glemsoqld.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gvqwmidql.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gygofoptk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gisqyrtxt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/godbplkqj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/glkkvittq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/grpeosihd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gyiyhwnof.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gisyrnmvr.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/glozafcec.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxwglbqvr.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/girqsqniq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gdbszvqom.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqennjfiu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/geltqgbza.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxzrtzmzo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtbixzlfh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gouarsknz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmeorqzoz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvibykvqw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfiyxsgql.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/ghfophcum.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/guolwsokk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gzwkmungo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gqrekvlpa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gfntcwbyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gezxaiftd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gjzyhnbkk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gcqghcoko.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gwvuucjab.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/ghgkzjecg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grfopyvrs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gccxfwruj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvdvxpane.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gohxbozrz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gdpeudfcg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gehdjejou.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gnrvcdmiz.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gcvfxslit.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gwsckwybl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/ghoonjlap.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gjitouidh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gpbhgvlyz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gwtdwhbyy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gssrwbmiv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gtzjakrgi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/ggcuczonq.sHtML


<!-- 参考信息 -->