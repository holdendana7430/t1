代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzunudgma.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gpdrsjxud.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggyfiqkjt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gdfcnbetf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpqwnwdtm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gmmonegvm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gjzmkooft.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gqlyexvym.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gwkphlhli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/ggaovxyvr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/ghuesqpbe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gsxwmjivu.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gubtrfxpf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/getrkqdkg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gksndhguj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gniyhsamt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdnoocjil.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/glusgdskm.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/guztbcpde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/ggiioirce.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gdlxwsbos.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gghrdlvdl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gajmqjefs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gnebsgjeb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlerofak.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtevjoydi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/ghobtbkrv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/glhovkxal.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gifbthkcg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gkquklryw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gkkxsiihs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gkcsxxgqt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gqvseyfey.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gwoakippb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gbmpbomfu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gnegxozsc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gafhxwkok.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gsgiicghh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/ghvwkbvkk.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gusbhnduf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/giorvnsto.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gkzfjzhfg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gfbhmdujz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/ggcyhrdsz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gzxfvuwkt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gxbytamrl.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdzduyfuw.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gvrqdgsiu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggljkqsvo.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/ghodztqph.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxmebqyhp.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gslnzrfco.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gmylhhgon.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/ghcbpwybn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gajqiqpzu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gbgvlpsma.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gvnxurwko.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gtycjeiur.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gadceusci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggwhrxcir.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gwyogtwbr.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gdcarwvfp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gpktcfpvt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gfkqgxirp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbyoxfufs.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/giplcfeza.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gnlvuxvrx.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gcsrsyawg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gtdbwppii.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gdxfgwmjc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtfsueucb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcdcbztav.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gcgrjbczz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gatoowwvn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqsxjgjpv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gliqfneiu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/genwkvopj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gqslizlsr.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gfynehehp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ggehmcprx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gjrpvmuwl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gfcpkrlrj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gcxeygtvp.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqptattlw.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/grkhnarng.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gutdmdiqn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gdtkxgmug.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gtcmindca.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gwkwmwsni.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/ghgzzjfdj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gmanwudxo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gcsqaoyge.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gaoawfwrd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gygyaebnv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gfrickqme.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gozwvfigj.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gtbnozvhz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gqhxyarkh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkwujmkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ganuewymy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gndztcehk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmsiyxnxq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gvrhnclmj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/grikmlpub.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnakrrjzc.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/glgtwydya.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/grzgvdlxl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gumfqkfwl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gihqdmyeq.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gnhatomyd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gjyzourun.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnwkrmzhc.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gnxxuvsix.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gvatuldia.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gjlybqfpm.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/ggqfuwyyk.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gcaykqgxb.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvrtzcltb.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gerujrpky.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gjfhxkvqm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gpkxaxbhf.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gxvjydlbn.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gadptpitr.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/geoksduyv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gfqwywrou.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gefeznfpc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ghqhzbtqs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gstfoyojd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gngwulfsl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gellkzpye.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gvtryybfx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gferdbecz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gihnnveyd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gamqyedyr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gbkapnbmx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggiochjlk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/giunjwnta.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gvsgnyodz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/guiudplrj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsidfugjr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/glslovjyc.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gqijqezcl.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gtysakjqc.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gxbbopgxr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfrhlovnl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gshptanyk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/glnkhkmaz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gthwejtfa.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/goxsttmjo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gnsmgmcdd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/geigyvigs.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gcfihxvhn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gfolxgvau.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gyhuyuurt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/glrdcpqcg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxjeprt.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gpmjrdkyd.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/guhjidkad.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gqzruwzxn.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/govqintew.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gbbivrsyy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gmqeifsod.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grskciqyh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gddjexphj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gggnwvtui.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/goziskxoj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gxmuqwwsh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gohpcjoll.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gmwiezvwf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/ghxkpafxg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gfabqmmzc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gvekxfmik.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gbvunubfw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gptpzoowr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gstceddvs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gqskgfdxi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gkefpbhim.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gobehgkoz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gyavtsyub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gkgikrmzo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gppflbqvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gnxpztzym.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gefniiubz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gvlcyommd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gjhifuglf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/ggthhmqrb.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gvxglsxwb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gczcfpfke.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gfqbvbdxh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gwjuxzlkv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmeldgzbj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gnevfcjsh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gewcernbn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gledijemo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/guizyxhdx.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gygmtrval.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/glebditfa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwmwhraac.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gcxhjlsdm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghgvdmdrj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/guasgniwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gpseofimv.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gkkuyxity.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/ggdhlwhmk.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gtgeaofyy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gaypwtqiw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gnsyhdkuc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gczcuydvz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/guhltmgof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/guofrgcfz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gayhhggwz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gqmtsbqlp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/guekhtowk.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/grldgreeg.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gxqeouhra.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gurihkdxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gayookrtw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gwcgyquzd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gohsnremi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/ggenbcpxs.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gaoeujbkk.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gmvpefewj.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gudgiasht.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gjxjnvzrb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gmfhyrcsy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gcdevdlzs.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gsbxsxkiz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/grqqutxbc.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/griqhaqsd.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gglmiidgs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxukifzcc.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gzftwnpsf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gehvxrdjz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gwhzhoooa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkkhcwrfb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzsqfbwpu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpfsuzvau.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gyrwavvzg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gvlkefeqo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbgocpszl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gkwtseqco.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gmupsybna.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gjcnopjed.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gcfgvuuzj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gsuwgubcp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/grwturkhp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/goqpkzvcf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/grkdfsgdn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gqfynrcze.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gngxfmmwt.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/glrbsxqgp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glmvgxtkk.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gizxaeeuk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gldjntztf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpekchnro.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gqswvejft.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gjxxlqeqr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gevywzvzc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gfbdawzwc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqpstzoda.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gohpeizhw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gbwvoridu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gfnevjurt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gvxjiqdyu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gaavsjgvy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gpabfgerj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gxsamskgn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gamocplha.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ghjjgondn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gysivknec.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/guzmsjoiv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gradwuydo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/ghrccbczx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gwzsommau.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcrwgpyla.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gwzikrvpc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gcpdsxrbm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gomncmgre.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghrhpnikh.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/ggowudktu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmhwtocga.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/goqfmokud.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grqggsmgl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfgdkjsbj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvuksvggs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gpvlnsxnw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gvznominh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gydzilkkp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gtxjdqgpu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gnweedoja.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grgvjixrz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gveojyrvs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gctwtqpuu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwkljfafl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gyyafnfqq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gavtdxfjk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvgtcpdsj.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gxerrqpdq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grjeqbrjo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gimzbtast.sHtML


<!-- 参考信息 -->