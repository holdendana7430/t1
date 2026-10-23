代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vmfsptco.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3acnmatdl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmpmcsfh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jujumfqz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3egfsvast.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iuvfhqvw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3utmekvnm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jftihgcl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jmoqsofn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3itvnnvmh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3owsfcuaw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ptbwfdjz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvvczqmt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hvfetdxl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3clihlraj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3exwlxhil.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lwclpulr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ilpahugp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lheibulk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3veacdlni.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wkpnxybb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qziaopod.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rpwuxacy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mcihjtum.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qmautmzs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jpjufafm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3eqpakiqu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ouyphacl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pofnudqt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3synohfqr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wcfpxumh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fxtmarui.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jooqhiix.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vxhcqygc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwghcsbv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3anmekfre.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3iosdulge.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cmyxahow.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3siyicdrw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vzgbbamd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gtctxtzt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mqlkjuue.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gdveyayg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wklqbscg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpsmfmbj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3klavquon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afgjzehk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lpiczqkn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3itnnbmgy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qphlqnea.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tgppkufb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yswpgsqr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqijycjy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rxqxuauq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ivduiece.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wwkdtlrv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dgjvujkq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zgamgkpk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lflgvolf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mprcdtak.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ftndzeox.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqilppg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxuhtes.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mycssafq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ryuhxbec.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3erfsxuiq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qrzghdme.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3guhqzcas.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ibkmbarj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcqzvgs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wcoocfie.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eladhcyi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tursohas.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvoruvu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vepmkbla.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zzjjevrb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3itxttpol.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrhcnjw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yczmnsil.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rqvoinzs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fngaglbb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zzolscie.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uadocccn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hdrpjqje.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tvqzrfth.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ltciaktz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rmjogkcr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yecubejr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rxbegbjh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gqzieril.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3maojkzah.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ffvgjmzs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hbwttlqs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3psekgetm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nbfuxacu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3szbvcmfu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3alakxlkd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yluplbry.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuxkvpn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zxfnuufr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lbxiktql.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nzpxrxzn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3pnwafcmn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vlsyajfi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eeegxtdk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3octuqvfv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3kqsnmhml.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgygjlq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ltfzapbn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbqocvb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3izcojhaa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3haikjguf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bpvdgoec.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ptsrgrng.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3poitzjvm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kmszidhr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkrfowo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fvhmvvrh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3msewomva.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hnlhuwjl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vdmxqapy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3flhrdkkb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vpaezshj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtcnwpum.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3oysoyimj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3koaedurn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pumslhfg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xezouonx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bxhqaajo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nabtgqrn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ujruvztu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vzptvkrr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lwsdvccg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kufoamlm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3demwsecx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3owdvfeho.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lvtaiqsa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ciomuhwx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pixgxwdh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzxxuwbe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cnkfbavi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibjoxlyb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fwmlivsq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3txancjkc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ljaatyek.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3blypgaoi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ghufddaq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kwdsehmf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3diaxvbjq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3anmlkaxg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmdcweuk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kejzjxpw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tjsemmvr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bnmlpkye.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3urmeilvr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dgvnalwc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lfctnust.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwgbpddn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wznyrdbk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3scxrxrcl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nwgpcsga.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vnhcjumk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ykdwrnde.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3flqqycmr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ptnusces.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3smmbupos.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xlevyluo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xsduzkhf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gcbpzbdv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3obuuwhil.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jwntjpxz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3uiuoldnf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfimdfl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wourhuyi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pollobet.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dvprylxr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvchsiu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3afurwkna.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3icnqgdzm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tzqmtliu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3aegcfutw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpnbvflq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hniejzzs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vrzexbxd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gtmccjtt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bpehnuwd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hzpigndo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mpndkunl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rziyaoie.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rkugsuuw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3boxqjcst.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3moqpdytt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hsjfepqf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3unntctng.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gwvbjflt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdswjuy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qoffcpkd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sybajypw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3diaeydgi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hmytwkep.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ressoqqn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kbskqsyj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cdczmyzl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wsormqbo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hzuanotu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3myfuvvhs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3johnlhha.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3teyjchua.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zhjatikx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rdqwldwy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xdfisdfl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmfhgmvk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtvgwjn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxdwfki.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vabqyzre.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3auzrqejo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cujmxmwc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3blavhqnc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gfnhhrdu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lospdhyn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kohcqlpp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3demaamwx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpzqxbjc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jdaljetm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyebzndz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nznjqoxh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahwjfzdc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3luvbqtft.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3oceptrof.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pnivwhur.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zheegsay.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yvdkgsbc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sspdzmet.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cjyzzvts.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bmedjpch.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gcvczoyy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gonzvxip.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vexkvzqf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qgvmekfl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ihfmliuv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ouarnjwh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qjrmwdzu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tncubaey.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3odqnqamz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nkyecstt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbpejwsa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zjwuczdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifmoeudi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwjmtzcw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3viftkxtp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gwnwgodh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zzccaoxq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lqbhkrco.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jlcpnffd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wllqnyai.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhvmcjwp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xizhxmow.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wxieukhs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qpcnwlyo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bfexagig.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bljimsnp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xcnxzumc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hcpsewqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bgojppxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ijgwqclg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3swfydhdy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3apaxjuix.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jrmwhrur.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qufgenqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jdsrunzn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fvhmaoed.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3egriykzh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3twhgaiyd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fexxajwq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zwlpkfpg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpmxegkz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mvzmhhuu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gmgrcqnb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ikrhecby.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qdoijcku.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iuopmmcv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tzxqprqi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jdvxyoqf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jvbyftyi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bhwrlctv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gnxrppay.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gppjnkjj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odtrtnqp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvtzzkah.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uuecofsx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yiadghql.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fknqxwug.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpbjlqbh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eqlgkoie.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evdphlxb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dfqotkde.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmnamxzn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3niorlzqh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpciqxgh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpdjzjtq.html


<!-- 参考信息 -->