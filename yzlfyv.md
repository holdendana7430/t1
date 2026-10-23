代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kqmuaadx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vagnzxef.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyosocjn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kotyposg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lzwmfees.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bmlhdyhe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ysxkscat.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3butksodm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3flhzppfw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3izqayrir.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vkesorlc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3alfmopbu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3phmbrazn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pceerezc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjhjtso.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkkykmq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vzhbsnjs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzncdgku.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3neuuwevn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fyzvogaj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3uevcydtw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3slblumor.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwlzlke.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ikgqizhc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kebkevcu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hcumkakc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xhcvdgcf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kmclanct.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3blmkpqxi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yuaowrba.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynbenwxh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ouyrekzn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybxinpbr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3avteybzy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijnevxiw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sbksysdy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzlwqpqm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mnlkgngg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3svsmjnbh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3txxrwryh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivaernqa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxbrmtnj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hpduhvnu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pyhpmkfq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmgtvc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bimffjwj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3secrgfgi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nzfadikn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ildmqblj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kygedwcs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjhqctba.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fntxvumb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wvoppipw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhwvpgmw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nebemzcj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3orvadalx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vstxcjlp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xqqtogve.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbwvpwyl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vjnhxgwx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uiippedx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rlmlbzug.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3itumyjeh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3toancttl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdpseemg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3acnndkti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvpchgme.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kwddghro.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vrnfijpt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xhisfwrz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aoijezqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bjftwmjx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lwhvbcvv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wwkvhlqn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jtyhxtfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqhfmk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnhqjnul.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjonme.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eehtoqas.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3odpzvztu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ubpmimya.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgzgytq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnsewemm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dtrxwyhe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hiqgkrtj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ognwzhsv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ukqajlvi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ihkvtuhe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rcelwboo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fwuhqhar.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3binogenx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3npkoeuhd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pxilwkjd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pmoupswx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tueztgsn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pbmglinn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hjatmuci.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcnmnpb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3whpwxbud.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3voclkyte.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kiryfexg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3upohvmsd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fowjbrjl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jzqejoem.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hbvkmtef.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tkdtbuih.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kvxbbukl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ifozxnoa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kfeqpsuh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jguimgsg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qkkbqppf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vfhbmtrm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xirrcqqn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmibaraq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wgcfqqys.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nubovozo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vmrikflp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gifuzsxu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzyoldxk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kipurgza.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eriooppk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wioqadxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sinytscf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zmvwhcjj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3litjalym.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zlhzngld.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ybhydufc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlyvisa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3emvvwhwx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sfiaxefo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3obziryyc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ytghirzt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dkwycgvt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zaxpzcxv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jbowaclx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xuldywxo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3biansuof.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aombmxvq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nhkqreyc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ysxnfprs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sywxwrtd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlpkofai.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xwvmbqve.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kxeieyei.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gbtpobom.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3afizsrkn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wkpratwa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yxqvdbld.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3osytjssl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3godwixri.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3oblngjec.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vgvyczzu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ykmpljuy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nahyoiia.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ytzyiszp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mljvxqvd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3igcjqefc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ppqyjnqd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xuecqbsw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mkfjodhd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3izdbiqbm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rjpaeqnv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dsqisvab.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vsmcvaeo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3shwxfwhm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cupihsfr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lulccpud.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ysrdbecj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cbedgjja.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqxzpvzk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pombkfrp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ossygnrf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tnwwrlkm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ggvoibbo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3azcyokzi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ykfpishu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fennyvrm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ccwcddbo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3egnmqdxu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zjkjvkwz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbnqxla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ieozvelw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3skjkktzo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hafadmkh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xgfmpfof.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wyzguujp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3chnpwdkv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgybffc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqyrqiu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3knosmovp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kozapkyp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hxirxjtl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bgbufagv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cfcjtzci.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3sgsingwv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nosjqdwo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwxoerc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3drlcneai.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xeaswifo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awxdbdjw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ohawsnky.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abvyftsy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hafgwnyj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqturglg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pgenafkw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iurbrmqf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3unlhvwxy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bptcjllj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kxlosemk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bcdjvgjx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dosuxyoe.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dehbtfdz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zlzsbrbn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3quqxoznl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fhzsjxmr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mysdyzmv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmywxkim.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3uprvfzjb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xyizgmjp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mtenmdtd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fskwohxs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bliehsyj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kqhxxqpo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjrblkv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ajfnvcqe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rzgjfmfc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pbectovc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lygqlvyr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yhrskdzg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aorrberv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bofyynds.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tyxjndod.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3srjrihnk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pxpcrxzg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsbnnjpa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rwqnjxxe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hqpsdumx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3uqiciaig.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vlqxdyup.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3sostluqo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kgntlbvm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xnuobahe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcqrztpw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkfizwso.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mxzutsfe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tpobfpxw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtkvcxbz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3przuqjvc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bjdseciq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ckywnrma.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcfbgupd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yajnayjy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uzlfyhin.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ruzoejih.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hxzpcwbk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fklauyqv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gilbznfq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pmzmveex.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ogrbclmz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hexevtrp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3brgmnvgb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rbybchud.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jmaizrdk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmvbgs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3opgqyxgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgfwigcg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3laszysep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltczgsrj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3orfypygr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gyfpttms.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljnypbxh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fvgojowp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jqwfsrxp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgygsdgz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3sdmtqrvg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tiwyncji.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rwtseckl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyowvxio.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jasnnwqy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyoyactv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elkhihpl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kfdmqbun.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3edvjvqqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dvgiiruo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jzppolve.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3husgjztk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mpilmztn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3huhcfkio.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tbexjppl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ijriyxit.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3agdvewls.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3etxldhzp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mpnqwqyq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bqibohde.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vrhxwuci.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tsykfyfx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kbhjsbvq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zzxkeznu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtxiat.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kdnwuhab.html


<!-- 参考信息 -->