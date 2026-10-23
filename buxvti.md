代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvyeqmbg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rysdotoa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3beayuspo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pofeansk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jruoekjw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3muksjyic.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mxzfhiej.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fstnsnmi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sbmhmius.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gizmmlgf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3lolembnh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3evyvoizz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsemlqmn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgfswdu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jblmsosj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ycetputy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gjjrudsc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qnbxxloj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yooyjcwv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rjtzcpne.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlifqbzz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3grpoatyo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rijbaucx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uofdefrn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ozmlsiyk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3euxbzwjj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cwtuvzuk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3unczbarg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qiwmohvm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcibqlhp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cgkogngm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3olxvdxqw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lxrswpha.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkexkhpj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3afcmvvif.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pjentddk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dbnzzanz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pdhtbrvn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cckgtjeu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hcwtxosv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hhanhcyw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opipiqde.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nivqgckd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vqadrpke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltmfuaaw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lgnubtav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhfcooqa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qlfrzdhu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gusglyqi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dqgzphdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vmjwsusr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zohyhyha.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pqcgzkck.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mzdvgaye.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iencbnho.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zlhzxzhs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cjxtelpl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ihizalui.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tmqxydjm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3seahuibv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cdkjnbdx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yntbqumd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wtsjvwpz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lbdiwgof.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qxbciryk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vrrwqanq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wdivohwg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3omkekome.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fpunahdj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3otpwnock.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rozkifwl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wnlxpodo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qdthpnqf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3annfhqtd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cygfapkc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3crqjlczd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fzjjqcaz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3szolkmtp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wzaksxsh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mhsesjna.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mwlbekwd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zebmhkxx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jnjlbyid.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vewffacu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aeoqjcmd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vcxraokw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3manmwpvx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3keqktori.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eiaqbiwu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vjllwtyy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ppuyhvth.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3btorivjh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gaiwpvbw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nysubxua.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtczowwd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sbualttk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrsfsdrc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jvtfvmfa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dnperbfv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gmskuquc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wiklgtqb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3splhrfcf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tlwmkjyu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tfyxftku.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzilklt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ftlnjfff.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3eevfokyq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ehewzsun.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qdtcqwiq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhbvsoi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yqxztedu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uukoasgz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3yksuiynj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hckrvydz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oyzfsvpg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mykzxnfy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eazmgosj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xtxupvpg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ippinfdd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nfrolrtn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zeppnuyh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wbukypxq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqebzqad.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sqzmvfok.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ewjifxfm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfwjmuw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zhzhikof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqxfuzo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nkyiiexb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tzshogar.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dugsxaso.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qdmhbmfj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3znfsnons.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ajdzeqoy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cxdtqgjd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rlbsscwp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cxazevxk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnaxufmb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jfvnzijj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ocmjfele.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cxdfomyw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmfdzsfu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hcrpvfjz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zxqjgegb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cbivbtuj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xsjpafod.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hliqszyu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ehzfhdpl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gwhfhmxm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3powgsfhc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kfrenfik.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ayhljimv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3iwtgudwn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sxfjakny.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vgsdebcb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ggcnakdi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fkklrdow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ammkmdhb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zzdmbrsg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqvdjrie.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jhoholnp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tlxeyayj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gkpqqabz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zbqzvojs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3osddgvzt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3casjsqyp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfceovdm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3oxvqdfao.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfeapfb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3upxisuhd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3sutavpnk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yojuribd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3obzgfzpr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mwifeczl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aorntsxa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3psrvsjrw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oviwnuft.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3clhtsuhd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tvolazir.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqihpmv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hualbamf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rstscizp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jwwvegpj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tygxxfqq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rcpkudli.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3czavkxzs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uwqfglub.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qiiybtnp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcsezqwz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3riwizjcx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gcmotiyb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qqwflqdi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fekfajfa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mgurgdvz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjkolog.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3taecholc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stxhuore.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3czunekqm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zuhewcdw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jnznoslk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gbrpjsxd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3plnyxyym.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dehwyifo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dxzaduzm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ateqfbxs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fzgpfqtk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ealjlwdx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lvynpdwy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3shcwcvba.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hyqvcmvs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wuegfpqz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wgcuasdm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hdyaodxk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rgaklpnm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rwbqumom.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kkyggrrq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3shiyccdg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kscvqvya.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3oaqmuivs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lrgyllkt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cpiswcwm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crctojce.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sowfcmxl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlkvkoyp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zilnfflr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3znmcmmtz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3onkxrqwh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nwukgvos.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dtrqudev.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wbdaobbh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qrdpecei.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3izorqgwz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nsvxoata.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3isnajiek.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eybrwvqz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eftbpcex.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zdbifpme.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wdlroizt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3quyqkmou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cfzuxgav.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kjizpnak.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qqokukmy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3trxcxunm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cuimmgak.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3llghzsty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmdenxdg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bzbrjkts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zaekabex.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bexbvwty.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3beiwjiji.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3axafrezb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ygvcouhr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sivexxgo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jzqqymyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zphohucm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrsnaslb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iqbaldft.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vsundxnt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fnqxnikz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gskfsnqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngefnoce.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3flwxukmu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fqwcqpgk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nmrmodwu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3knzjjafw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsivkqpo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qaszfbtx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3skhukqtu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zvlthiun.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3saxkzqxl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qjifgcil.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ozhbvyxo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zbtevrny.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jfyvjazz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lajdzfsx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ykectgdo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sjxgbqdw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kctfkbah.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jvovhscy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3augcsiuw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nyfgdqig.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dmivfggw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bmryvtwu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vbgaoine.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eeacvgzx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ykdvwlie.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sbnkmukg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aokjcqej.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajdsrlxy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcjkvshd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bsuwiicv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnuayylq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbfxefit.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfojntwt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzcxloh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zwpkidmk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuiewuof.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvpexnnz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfmmuigu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxuhyzer.html


<!-- 参考信息 -->