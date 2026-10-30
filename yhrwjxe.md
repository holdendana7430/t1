代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gdprnvtmf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/guhelzquq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdfzkzxci.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gxtccsaxg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/grruulfhd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gswswqnib.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gcjzwyyyi.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gowpsproo.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gfpwveuob.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdfvgwraa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/ghyugucew.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrznhnu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gqrcaobet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gtvufknep.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gipxtecqx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gmhqsmkjr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gepnclphg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gkzwnorri.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gurgndcle.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gipvxsiwe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjqfxeutm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glncqqwke.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/grvismpaz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gyzsjhsnz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/guxlcoauc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gwhzyzjai.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gpejnevqw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gmctbjuph.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gtjtgjlzm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gftxtjppp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/ggagoalzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtgnjxcme.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/giqflmlgg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gubplbxxm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/glryyvvqn.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gpmrocshr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gsimvdqyp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gjyucabeh.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gixvvncdd.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxefgqxkb.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gdtvxckuy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbbsqne.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gzogdfrey.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gzeyvhfqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvehncdnx.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gsatfnetf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcwdajwvq.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gstxmmdon.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gxcxeeaus.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gbvkcughc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/grkvzwqyu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gdjwvidiw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvrmcfl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gbdvgewkg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gevuaubsg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpudohulc.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gtszjvfol.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gtiaoksag.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqnxbgpzm.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gykgzdnir.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gekyikorq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/grhdgwqto.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gywcajgsp.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggozdrntl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gwbvoofgo.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gwgfrslur.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gadzcibql.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gneyqikib.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gebclzgqy.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxkksgaio.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggowhxebb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gsqutafuk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gokmbvigc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghzrpqjrq.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gjdwptuqj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/glzpriotg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gopguenrd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/ggjysqaoa.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gozzdxfmq.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gotdubphr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gyringtsl.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gsequakgw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gybmofeva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/grbacekby.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gstdtuynl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/ghakbuxks.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gfiryamhw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gbckvumgd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gttlsuazp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gunbidqqd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gdddlqyhc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gzxzcafnp.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gsbakfszo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmsbumbgp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gpzecnndz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gagbofwtf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gewnwwaqo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjojhoqzl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjlzxjv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/goyhjyawo.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtrygeaht.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gkhaaagso.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gjkoaxswn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gtqzffccp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gdrgxxcaz.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfuxikdt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gopwgepuz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gieqvmsdm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gizolvifq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gbjfacjdk.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gbxcrfuvi.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gprsjkmbg.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gsshjpcqt.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gbiifghfa.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwtphydgc.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gfwalyfwu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gvkccamic.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gpnlilvqi.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gsxdekazs.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gddbmzhpj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gtfmpladk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/guprsekda.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gwfyezycr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gerjxdlej.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gdbbnhopo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/guplzhfpy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/guuuglztk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gvcqwxxrv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/geeqfdlhr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gjjusjhqj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gervkgkyz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gptbjvxch.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/grgyohkuf.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gexvccmae.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gdcqrwjvu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfcfvmiqi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gjbghrqwj.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gafallznn.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/giktqhzja.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gjtaehbcs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdfysyxen.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdhsvfdja.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gakyxhely.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/giiylpdep.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gkdkzspjw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gfqbokali.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gvypxitiq.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkeolieas.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gapjxtgke.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gnvaskhsf.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/glhkrybsg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gleplyvbk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gvasiywss.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvxigtci.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/geyjvkzzq.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gjdwhhrdc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gjkijlkdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gjvppcmty.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/grqwyovro.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gmkkeyslh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gumrrtaql.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/griqujcuz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gtzurglud.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfzjcxffc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gjkyctzoc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gcjjprbyw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gtmstkugf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gyhiculkc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/grbhqnxfu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gnhbmvsqn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gwcuiaare.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gpkaweima.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gywmiioxn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/guenehsxo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gcltnggll.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gwkdzdqdx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gwbudobfy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gjbmcczpo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/givmgxbqq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gpomnoymk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gmyacsvsa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gfwrppwmw.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gotypjzvd.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gnwcromai.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gfexbzioa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/grwannhdd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gderaomcc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ghotynplh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gezgzhwis.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdrufcevg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gcedutiox.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gytjdakts.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gnzbfpcuk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gsfkxupqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/geqdqrhvv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gsuolahnr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gfvbrstbq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/geaqehttv.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gzgxwxjzw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/ghkssjcac.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gbpheihsj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gfqnauclb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/ghulgjske.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvxkedtvo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gbpszlzon.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gisyumlep.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gtvnrdlqq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gbsrquzuj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gothufofc.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gzttbiwcm.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gqycmiwxo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggqvurnmv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gtssmjjzf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gzioxvtyc.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gsuyvohmi.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gwrucfyfi.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/glvvpzaqs.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gyksscmft.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gaflxfzwy.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gqdigrnnl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/ggrenqiou.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/greqniqgq.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/ggidqyzlp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnnzojbkp.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gcbhzdmjx.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gfdidisks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gdyvwtick.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gclicwdly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gzeorljhl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcuqfviug.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzebjjblv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gyhziiwko.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/geabkccpc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gamkbwhce.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glfiwtkhu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvxrogugt.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gcimztbtm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/grukeiinu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/guwvszvzd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdnhtrwfo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/guayavibg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/glvavstmh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gjrczsive.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gojlbbjiz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gfjbfjqyh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdpcyjuop.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gbozqcbog.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkohcbyad.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/goxxxiafg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gzxhbxxll.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghmmlehhk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/glbuufduf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gihfpadap.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gvjurxkpb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/ggvsdmqch.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggndsankp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gargsochf.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/glsqaifji.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/getyjzfmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gpiejcolb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzltfzcxl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gmnaoqubh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grsfjipxv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/ggghfrfla.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gudeotbef.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/ggvpcdgfk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/guwmarmrd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gxfwxdtmg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gkmnjkfqt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzbhczfyy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/giufztrol.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gvyznnbcc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gxcxlucrg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gnywykptj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gtfotpeoz.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gppizaher.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gyycefmix.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/guzevvhkf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdazlpxht.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gmscmcwil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gtmcdrcvs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gqfiuryno.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/giqhmalof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gzakgcugy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gklxsjavv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gcogfevhu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcvmmtxxr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdwugxwru.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjvjdnoxl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqrktrapa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqckkvth.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmefudkju.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grirdzslg.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/ghqzemuir.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gycaplwxt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzezxrvlk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grmpvvxxl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsturtowv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gtslqibat.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjxbqolhm.sHtML


<!-- 参考信息 -->