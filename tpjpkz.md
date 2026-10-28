代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gthyczfnzc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtrwyldubx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangtech.top/gtexiamufi.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtxhrxmpzi.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtntqfjvap.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtgnvwbubc.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gttjnfjqsp.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gtqfwtxxvm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtlrpjvzia.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtzrejmhhm.html

TS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtbgsrixvw.html

Java: list.contains(x)
来源：http://hz.wangshuangyany.cn/gtueonmgft.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gtxmlejguj.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtjuyzqovg.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtazivadee.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnqzz.top/gtanbwwbek.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shuidangran.top/gtoozsokhk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtjgzpcmsw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtkdkkhcll.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtumhlzrxh.html

Java: new ArrayList<>(list);
来源：http://hz.ydjk.org.cn/gtfmkhxcor.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtassoiyvc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtgqhasrbw.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gtzjupxftj.html

[D23] reduce 累积计算
来源：http://hz.chenjidiqi.icu/gtvyzacogs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtiiycaoqb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtxqksrxtf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtpispwpwc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gttphdokne.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.feifeiyinyue.top/gtivneumbb.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtliynzwht.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yuanzhike.top/gtxiekdvba.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gaohongyu789.top/gtrdhjlkyi.html

[D24] 字典 / Map 基本操作
来源：http://hz.xingfuxueyuan.xyz/gtmmgqescz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenzaomai.com/gtccgqyuzf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.316326.xyz/gtqjedrrvx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtlnhbnzsc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtzdpzfnvs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gtqglzxdko.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hammf.cn/gtuphpfqug.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gtxnzybyuf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hongshengwenyu.top/gtlyfwvpsh.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtebnisejh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pycfn.com/gtjvtocmhv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.redwolf501.top/gtcmeosqwm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtbnuubeqs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhengqikj.top/gtlmgzckrv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangkeji.top/gthmxsnkvu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtjprplknv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.0kj1m.cn/gtfydwjktq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinghuilouyu.cn/gtgpyolbgd.html

[D26] 数组转字符串
来源：http://hz.jianghu66.top/gttgmxjmjv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tian-w.cn/gtqsrgtlqu.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtxajqbunp.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtqeouuitn.html

TS:   arr.join(", ")
来源：http://hz.hammf.cn/gtbnmjtqoe.html

Java: String.join(", ", list)
来源：http://hz.vqdsnc.cn/gtflllbqnx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtranbvmdj.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gthoywxoem.html

C#:   string.Join(", ", list)
来源：http://hz.yueranfly.top/gtscwantkt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkcxtmyqw.html

E. 字符串处理
来源：http://hz.ywan-chungtsiang.top/gthhnkoqzo.html

================================================================================
来源：http://hz.dashuyun.cn/gtptrimlql.html

[E01] 拼接字符串
来源：http://hz.ivvv.top/gtiikdpbip.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxinkj.top/gtgjhyfmhf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ywan-chungtsiang.top/gthgkvmslg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtlgcytcls.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtealdoznu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtqhhssurf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gtsmettpbg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.kuanghao11.cn/gtogovfbwr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigfzy.top/gtvcmxtfui.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtziikeght.html

Py:   "ab" * 3
来源：http://hz.jinqigufen.top/gtlhwkouaj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.feifeiyinyue.top/gtbliltqkv.html

JS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtiiorwiar.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtiqdcfqbc.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtlwfxyuxv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtwjitfzwv.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gttolgmbxq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gthrmygafd.html

[E03] 截取子串
来源：http://hz.jinghuilouyu.cn/gtvpqmwqev.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yangfankeji.com/gtkobpsmzb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gtsapzuaqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtotxnjnfl.html

TS:   s.slice(1, 4)
来源：http://hz.yangfankeji.com/gtgoouimlp.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtjzkunbed.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtxyzhlhwp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtsavsegah.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gthzzugvpl.html

[E04] 查找子串位置
来源：http://hz.yvedp.cn/gtjuuxwntf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhiwuduotai.top/gtlcjzcnwx.html

PHP:  strpos($s, "x");
来源：http://hz.shzxlz.cn/gtodwnznwz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtagmyymsa.html

TS:   s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtpzsvpzhj.html

Java: s.indexOf("x")
来源：http://hz.zhongyouzk.top/gteeapespq.html

Go:   strings.Index(s, "x")
来源：http://hz.pycfn.com/gthfdlopib.html

Ruby: s.index("x")
来源：http://hz.xylfe.cn/gtplgtczvk.html

C#:   s.IndexOf("x")
来源：http://hz.zycfv.cn/gtyhrdhdzb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fengsongda.top/gtshghkjbf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.svipenyu.cn/gtrlfycmog.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gtpzocbeco.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtueipfece.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jianghu66.top/gtsefpxloq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtaislhvrg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jlsjyb.cn/gtboxulgyw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tianlin.xyz/gtwjsixmqg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.vqdsnc.cn/gtpxsgzvbz.html

[E06] 替换子串
来源：http://hz.hysaishi.cn/gtfklpfble.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtxcldtwoo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hnqzz.top/gtlekkvnez.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtkiqrajxc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtoyxsrkyh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtlnmwizrc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gtliqojvew.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.quarkkingdee.top/gtrfhdhqlr.html

C#:   s.Replace("a", "b")
来源：http://hz.zhixingplan.top/gtnxdkcxkq.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtyqlyvatg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangdashe.top/gtnobgobju.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenjidiqi.icu/gtkpulmzhb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtqrttirxn.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtancgiejl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.mhx1999.top/gtjigcunvl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.316326.xyz/gtftinvkxr.html

Ruby: s.split(",");  s.split
来源：http://hz.xuetiantiany.cn/gtasrhopdp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pycfn.com/gteakbyvku.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtumnzidxj.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtoqdtoirh.html

PHP:  implode(",", $items);
来源：http://hz.snrcjt.cn/gtcxvqntld.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtwchntrrv.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtpxrtylqp.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtgbpsxqab.html

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gtgrrykrie.html

Ruby: items.join(",")
来源：http://hz.jlsjyb.cn/gtndznxeif.html

C#:   string.Join(",", items)
来源：http://hz.shangyingyoupin.top/gthmzyofoe.html

[E09] 去除所有空白字符
来源：http://hz.chenjidiqi.icu/gtibelbdhs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydzc1.top/gttkpzcnxn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sufxvd.cn/gtijcjdwjq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtczvxcsin.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtqchvzsfy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtbfulfruk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gtmuuttqkc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gtxjnlidcu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zdqjudy.top/gtfecturig.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtqlvwzvfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtybnhwjki.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangdashe.top/gtycqghzys.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtfgxcmknb.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtjobwruss.html

Java: String.format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtuyldxlmm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.316326.xyz/gtjpoiutxh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dianchejie.cn/gtptqgbqwm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtrlawtrix.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtfkujcpwl.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtdyccgfjc.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gtjzwanwgi.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtwwkxjqap.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtohoznbjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ppjwa.cn/gtbewwjheb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtghfysufl.html

Ruby: s.reverse
来源：http://hz.fengsongda.top/gtmqztrbyg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtptfghvee.html

[E12] 统计某字符出现次数
来源：http://hz.316326.xyz/gtdzrzyyyq.html

Py:   s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtokvrqyvs.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gtembftllp.html

JS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtobamzrby.html

TS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gthtkzyjms.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtbtoypkqk.html

Go:   strings.Count(s, "a")
来源：http://hz.52xcode.cn/gtmfmhmjec.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtaiuupvwj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtynlbudzr.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtjccufkcw.html

Py:   for ch in s: print(ch)
来源：http://hz.nwbrower.top/gtrypduldo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhongyouzk.top/gtzupxvgrd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtkuqzhfds.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtfwaprxrd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtfukvxrlo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtldlgdjhn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenlongwang.top/gtrfkncycm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtnwseszlg.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtrmdkxtjb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxinkj.top/gtjdjeduyi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtnvkukmpe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydzc1.top/gtkypmulvp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gttbzfymfd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtnmekgcpl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtfxpldmpz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuanzhike.top/gtgrvfnmee.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtagjbmmwe.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtimtysmgu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gttvzyumjh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtrcnsdpke.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtyrkrfwnh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtfglepvnp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtzowechys.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtevrvlkwg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtxmdiiesa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenjidiqi.icu/gtorcyuzql.html

[E16] 数字千分位
来源：http://hz.jinghuilouyu.cn/gtqylvsied.html

Py:   f"{1234567:,}"
来源：http://hz.dashuyun.cn/gtrnfmxidb.html

PHP:  number_format(1234567);
来源：http://hz.sxryk.cn/gtesaacltb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.316326.xyz/gtitymqhbb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtqymaszbf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xingfuxueyuan.xyz/gtiaxppkji.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtjymiwfpo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtilfpahqp.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtcrbdfqiv.html

[E17] 首字母大写
来源：http://hz.shuidangran.top/gtkhtubttg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jiagoushi.top/gtbmucczqv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gtaourfods.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtpkzrxrcf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtpmzgnqgu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.birdmap.top/gtkdavcvgl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtmrlnimcx.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtkbovgpvx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.iojbl.cn/gtfugqllay.html

[E18] 模板占位符替换
来源：http://hz.nanxuanxn.top/gtaxmjsrwk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daxiang520.top/gtzatniweh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtacxskbza.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtbceatkcl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtabcgoltu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hfpthk.cn/gtdmwgijbi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuanzx.com/gtieweucve.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtbiijxnud.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtqtkdmmuy.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtsmwtpqkh.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtmpufdnne.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtbwfrlggk.html

JS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtultehykp.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gteqxatbwi.html

Java: s.lines().toList()
来源：http://hz.xylfe.cn/gtfdwmhmti.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtzmbbqfgt.html

Ruby: s.lines
来源：http://hz.ehwqpu.com/gtebplywdx.html

C#:   s.Split('\n')
来源：http://hz.tian-w.cn/gtxthqgsfs.html

[E20] 判断字符串是否为空
来源：http://hz.hammf.cn/gtctuhplgp.html

Py:   if not s:
来源：http://hz.xuetiantiany.cn/gtevoascdr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.iojbl.cn/gtnqjozwhf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtdaowjkrh.html

TS:   if (s === "") {}
来源：http://hz.yongpay.top/gtwfgsjkgd.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtyjrefqib.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtuukbvjqs.html

Ruby: if s.empty?
来源：http://hz.xingfuxueyuan.xyz/gtazzbzkzx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hnxiangtu.top/gtuwpcoplr.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gtvawjozzo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhoulong.xyz/gtuhsztdrh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.feifeiyinyue.top/gtqzlwwabz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtyckbpehh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtsmhptpjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtcpjgddwh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hysaishi.cn/gttsjrjeww.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gttfxyorun.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cqqwz.cn/gtgtaxuvcc.html

[E22] 字节长度与字符长度
来源：http://hz.zdqjudy.top/gtwhfizjsq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zdqjudy.top/gtwkghdexx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtuvcpmkxu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtlpgkfixp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtuxheuunv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.mhx1999.top/gtreyjfbkb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gtezgauvnj.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtaoocdvir.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtxdllhbtu.html

================================================================================
来源：http://hz.yuanzhike.top/gtgwxomaqb.html

F. 文件与目录
来源：http://hz.chenjidiqi.icu/gttwliymln.html

================================================================================
来源：http://hz.xziqi.cn/gtuiiqgdcg.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtkplovndj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtodksfpet.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtzjuryahe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zdqjudy.top/gtbvtcbskb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtnhopmgzo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtjmvpkbef.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtbetgkbig.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258888.top/gthoujwdqu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenzaomai.com/gttsbkrewb.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtjkekpkis.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtjsfidqbv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.316326.xyz/gtfmklulzl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gteokyclyr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtnupppxus.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtsubuqbep.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtidybbbul.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtfyggarkh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gthqftlckl.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtawsxoynn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.quarkkingdee.top/gtthhjvnlb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gttouopwcb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gthfcvbipo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtesuoyyoh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtxmnlczui.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.smart0.xyz/gtzcmollke.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.kuanghao11.cn/gtahouwmfq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtpapvowvu.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtewhhsfzj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtnbuculas.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gttjbhjpxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtpuwqmppi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtmjvvawqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gttkwiqese.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gtejokrjnu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtvjgasikk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtphfwqmcm.html


<!-- 参考信息 -->