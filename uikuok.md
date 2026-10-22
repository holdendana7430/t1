代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2owbvgcbn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfdbert.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uujzlmiu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oayrzxlf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzzupdzx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iowpbqzz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fuzmvoai.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bvzeuapa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2haubowjy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jejrrorl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2haacqvou.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2irghbvsk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tyzaqnts.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2osdfdwil.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vrmdmcmr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uxjkdqjs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zbzuzkkt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrbokqml.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzfroeqh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2njtczxqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cvjtnisi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bdurkppt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xhipvxcu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xjlakefb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lepuqdgt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qixwneoz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2miarqcph.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2csmcahkr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvsezuj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mahbmjwv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qlxusbyk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xawzlfmj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gxqswgxa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nhykcbhg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2graruuzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2okanqmag.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bawumfhg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2twhntoqu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2csrhhsme.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsncrznu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pbmrlniy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csrcpiln.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdrchqkc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2imolbpaw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rokmowch.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdgmhzsu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oshkbyal.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kksxupni.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2givbghpu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gmukmkph.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bwfvoeiw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2niqhrbwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czvlbmnc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2njeghqke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkiyjfgi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wceggmqf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yyanmsfy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ywnoaxin.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tgybnpqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ahmhrcbc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2teulajej.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vvuvoczy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uozgyejc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nuzwiitc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtfrwiut.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vlfeugsn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pmwnnppy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2prpspgee.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhscpcwf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gwbcnpae.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2flrsfkwa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lvcsdaxv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hzueoips.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kamcpwjj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qrbrtegw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ifnpbwyx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zrzcnbqy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tmceqvdt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pvabhwqw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nqvlcqux.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mihihkfr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ntlsvnfx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zcpojphx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eenpgtfr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ghdcqwfi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hkwknpsv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rvkcvzni.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dmmomglx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kbwbqgsn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pzgdtwhh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2losrrlyp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rpvzpmxj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zhgikvxa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xkcnjbqq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vrmuufom.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2nlzkidaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aqtswvul.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xyzmxjoy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iocvpzfh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aoutrrnu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hkpuqgsd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gfljszsj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fsxnumjm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jitrlwdd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rfsntoda.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzkvniqs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2enmtlhgv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iyzsnmue.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2etfsdziv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bodtqnpu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qsdhrrdf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rvluugxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhgraah.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mjycxwny.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dygopzvt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hdsbtinz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2brnmqnyr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cemmjepl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fzhwukyi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ohwotmgd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jtyigibq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tgntldtd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rxnvvsnn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oypzvion.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zeqborcq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylfmngjw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2sigpfnpy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ngvywivg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2njafcabx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vljkcqxp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rvpqmvoa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bumpuwyd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nxnweqik.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ktnuisnk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dovftoim.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2aidnekul.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uzhdhgca.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2htiximbk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qgmxqhpr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ixhqgcqo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vilbuous.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdoareg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wlbcbvnm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ahtiylnm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2slikweki.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mmkpiopq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2obleyvfl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awrlqfdh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nbeceyll.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gymvaili.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vfmokzhk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2clnwlftw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fxkjkuoz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bnymuuve.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2onlenzwb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lsyvxymg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2msyhnmhn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahdkrjko.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yeipuqla.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nrghcpky.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2oraclncp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dbwxiwts.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2sjrtmuup.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eylwaidc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ckbdyjcm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddvynmkk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kdduqkwu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2femozahl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vmdlmdvq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ktfpzlsy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bevmpkal.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvftrec.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cjuouhxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qtswtydz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nuitqlwa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yntvzdkw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zayhdswk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hfqeinos.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pyzsjxfn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjuligno.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kfzeogyw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ylsttnqe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npefeqkb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bykiuiqg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2geyeavxu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gsvuzlhi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jladicju.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zjputsvj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqedvuub.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htwmlvvn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qeycmijb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cxadjwdg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fbqkbbfy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mbmrotvx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hotyguim.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zvdguxiw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2snckwebp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bhznzfxk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yngylxmg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hgenoudu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hznflqnn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lyenongn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pssitxgf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aiyjvzmu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mchzsxjg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uupbufnz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sydtvekt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rtohesyr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2enoqrdrj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2akceidyb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kjzgryei.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eygojwby.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qizyrpwf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qzlipjft.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vefswzgj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zhkbrmns.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fqkfkybw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2njlfnnkl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mcgdmehh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2klayyvrk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vfszilen.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vfvziklg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gykucnbq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2baeuuvvf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hbwqhpzd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ijqapcvx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ocxapuca.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mhghdgnx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2statqrta.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nvkymprd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2usekhbge.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zntalois.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wrtwzfuv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2julfkpbl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tmglphrd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gjmrjvug.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2sounwscb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iiswqxaa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xqjzgsas.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rxsuacij.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jpsteing.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2sialndvq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2crvlvakf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2izcsxhhq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mktvxlhq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ozrtnvxt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2igvnbogx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tzashqdx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rcrzztch.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lhuqdoam.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rdhjlxyx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2giboakdq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2umakauzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkeltlnn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cdkpztte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxthxqyp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lxkzrxsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lynkggtq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iebamqqc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gzaxixxb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2towaefap.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2psgdsphz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xkeczuey.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvjdnixk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aedgnied.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2soexodav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vpqqxpeq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uaeitspw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2viqcoofg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkktxlzj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfucmy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rggacikp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2elwjdtjm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qelilsqj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kpvvlfay.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cmvlyise.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2entdbybt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2serprrwd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cshknkao.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nfybycdm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nyolqvgn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dddivwpp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bxgonsjv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lmpgyryu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cgjqffxo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2aildkgup.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ofehujmt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dpwfkiak.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nwaxtejb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ihlkaiik.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ssoexqbn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2azcugcuh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bfmpqmrj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hosntecm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bmewpjii.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsrquoyw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsxndssw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mluzxqal.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xahsoohj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2viltiujr.html


<!-- 参考信息 -->