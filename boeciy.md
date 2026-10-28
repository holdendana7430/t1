代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gticurexml.html

[D20] 统计每个元素出现次数
来源：http://hz.fzhhl.top/gtudyndand.html

Py:   Counter(arr)
来源：http://hz.xingfuxueyuan.xyz/gtopatznwq.html

PHP:  array_count_values($arr);
来源：http://hz.gogol.net.cn/gtcdcvjvxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtbpmrvwky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtctzxazco.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.0kj1m.cn/gtamnpcgpl.html

Go:   // 手写 map[T]int
来源：http://hz.sxryk.cn/gtvmbdqtzx.html

Ruby: arr.tally
来源：http://hz.shanyushiyangkeji.top/gtolyvmilm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sufxvd.cn/gtaqwwtnaz.html

[D21] 判断是否包含某元素
来源：http://hz.kuanghao11.cn/gtsbhffxyj.html

Py:   x in arr
来源：http://hz.ehwqpu.com/gtoicvfjng.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtqgrlyxhf.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtimasmjln.html

TS:   arr.includes(x)
来源：http://hz.wangshuangyany.cn/gtzgqvmomt.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gtxsohwgso.html

Go:   slices.Contains(arr, x)
来源：http://hz.aizwys.cn/gtjkxptjdg.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtcgpexhhi.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtwvnjkgod.html

[D22] 复制数组（避免共享引用）
来源：http://hz.andypj.xyz/gtncdzggyj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtdrreztov.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gttojwiulx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtwryzqhpa.html

TS:   [...arr];
来源：http://hz.316326.xyz/gtswdzrycn.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtaogyntqk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhixingplan.top/gttquzfdkj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cdnleiting.top/gticsiztyh.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtehwukifc.html

[D23] reduce 累积计算
来源：http://hz.meibo888.top/gtyavixcmg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nwbrower.top/gtuehuvhnr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hammf.cn/gtujycbizd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtuewinpmt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtnflwcltj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtoamkdwgi.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtfzmpxqhs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gzhubu.top/gtgtdrqbbk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hongshengwenyu.top/gticvbwnei.html

[D24] 字典 / Map 基本操作
来源：http://hz.gogol.net.cn/gtqyzyvyva.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtmqlrdanw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pengpengdd.cyou/gtxgkbgncj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtgmnoxeni.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxinkj.top/gtuzexwvnf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.smart0.xyz/gtpfyrfitw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtmmpygdcu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtgbolsatq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.meibo888.top/gtwpimeugq.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtcpvlepfx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtglwllrrg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gttpanooog.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtgugjlocs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jiagoushi.top/gtawonetwj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gtzzklzmor.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtxfeekpew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gtfhtcwbkl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtsiwbezkf.html

[D26] 数组转字符串
来源：http://hz.sxryk.cn/gtgsqndaha.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gthfafahbw.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gthfmfpesh.html

JS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gtuarbwxmi.html

TS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtclfvkfbl.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gthdmzulyo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtoaayjnux.html

Ruby: arr.join(", ")
来源：http://hz.mhx1999.top/gtuenoztzt.html

C#:   string.Join(", ", list)
来源：http://hz.sweek.top/gtxxznijhu.html

================================================================================
来源：http://hz.snrcjt.cn/gtihtzshgp.html

E. 字符串处理
来源：http://hz.shanyushiyangkeji.top/gttlddfuev.html

================================================================================
来源：http://hz.yuanzhike.top/gtoikvzttd.html

[E01] 拼接字符串
来源：http://hz.jinghuilouyu.cn/gtsjjdxwht.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtrojaysaq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ehwqpu.com/gttboywcwq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtuondrbrf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtndkqjpnv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtcqfweegg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aizwys.cn/gtqkfnnkgb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtjnthgzcl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sxryk.cn/gtlvuievqk.html

[E02] 重复字符串
来源：http://hz.jqgfzy.top/gtmcwwzisl.html

Py:   "ab" * 3
来源：http://hz.cdnleiting.top/gtpssrkuyp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jianghu66.top/gtqyqwpmxn.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtdvoxrisr.html

TS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtpjiauozg.html

Java: "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtxfdlhrgl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtssbtqqim.html

Ruby: "ab" * 3
来源：http://hz.tian-w.cn/gtqaereflm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtbmnyoprx.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtofokeoly.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtasqrlwrw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtgmmuocen.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.andypj.xyz/gtmjyrdmfq.html

TS:   s.slice(1, 4)
来源：http://hz.jqgfzy.top/gtpypgwnmn.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtjewuubzw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtacouuchl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jlsjyb.cn/gtltxxccgm.html

C#:   s.Substring(1, 3)
来源：http://hz.daxiang520.top/gtvtavwwqy.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gtdlzouifj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtrvqdktdr.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtudygjpij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.vqdsnc.cn/gtxmabxfey.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtqkdlessf.html

Java: s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtvuwpakwc.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtuklnfivy.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtobcgqyyo.html

C#:   s.IndexOf("x")
来源：http://hz.cdnleiting.top/gtttwsahfh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtkbmhfobx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuxming.cn/gtejldziic.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangtech.top/gtzxulfkrc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtqucqkdze.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gzhubu.top/gtouwmyhjx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtvlnuwbch.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtfvufwmvo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zycfv.cn/gtbfwcisnh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gtvnlsmild.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gthymihuwz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtkvlohent.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtiwyqxled.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtmhsjhpox.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gteaqtrvaz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtfauxdbkp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtcldnbvuf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtdybplyxs.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtbrztjyil.html

[E07] 按分隔符拆分
来源：http://hz.yangfankeji.com/gtscaxpcss.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtoqhgqnsx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangdashe.top/gtigudcdws.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhaomingkeji.xyz/gtxtjvjqvm.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtphyzjomc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtgcffomei.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xingfuxueyuan.xyz/gtjxosfobd.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtcphneqnx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pycfn.com/gtfinkipgi.html

[E08] 数组按分隔符合并
来源：http://hz.cashguo.top/gtmbxrkbkh.html

Py:   ",".join(items)
来源：http://hz.cheryme.top/gtyohbbbyh.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtjpfssvzo.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtaolxikwz.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtoieanaze.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtjpshaduv.html

Go:   strings.Join(items, ",")
来源：http://hz.redwolf501.top/gtwlaujowi.html

Ruby: items.join(",")
来源：http://hz.zhijiandao.cn/gtaarcowjw.html

C#:   string.Join(",", items)
来源：http://hz.hywenlv.cn/gtnuzxsxwh.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtdbrsswyp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgufenzy.top/gtfkuyudum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtkcbxgbbq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtfvddaqxq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtmviqpgkv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gtnqkmiktd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cashguo.top/gtbzphlrqe.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cqqwz.cn/gtijwfeatq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yueranfly.top/gtibbbetof.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtmeopbhua.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cheryme.top/gtzxzdsejk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtnevxmctt.html

JS:   "7".padStart(3, "0")
来源：http://hz.jlsjyb.cn/gtunumvulv.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtknzriiah.html

Java: String.format("%03d", 7)
来源：http://hz.snrcjt.cn/gtvwogpnzr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtdwjzyogv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtakjetfzb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.haohaochexian.top/gtadxadzco.html

[E11] 反转字符串
来源：http://hz.redwolf501.top/gtqtaesrmz.html

Py:   s[::-1]
来源：http://hz.cashguo.top/gtvlptetzb.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtsvkudmzl.html

JS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtxwpgqmmy.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtfyywkmcq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtkdgjvpti.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sxryk.cn/gtfwcpwqft.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtkteofrad.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtyuhtevbj.html

[E12] 统计某字符出现次数
来源：http://hz.316326.xyz/gteufcihpa.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtuqtawzjc.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gtqlqbsoqj.html

JS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtcnxxujta.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtfoqkqtnh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.haohaochexian.top/gtrdnfmqbm.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtcntdptoc.html

Ruby: s.count("a")
来源：http://hz.jinghuilouyu.cn/gtivfixbhy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yueranfly.top/gtlzeryxog.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gteceybokf.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtyjmhfbnn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hywenlv.cn/gtjmntjbvy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtqnnhrcdl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtvpeqwuqg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cdnleiting.top/gtbdjbmibh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenzaomai.com/gtrytjhqrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gtpnryuixp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtjfnajixi.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangtech.top/gtysjtboro.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gttriphivy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtpcrbheoh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtwlxsqjyw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aibaodan.cn/gtwomuhwmi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guannengcc.top/gtlobxfxth.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgfzy.top/gtblyuducn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.mhx1999.top/gtqarmdrjy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtwfwjrpzu.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtchamtmtu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gtsbdourmv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtxweosybi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gtfoaggett.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtxmcvbgdf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zdqjudy.top/gtiputporb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tian-w.cn/gtulyngccg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258.top/gtnrktbhcm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gtyuzkbplg.html

[E16] 数字千分位
来源：http://hz.ydjk.org.cn/gtvnlwzjmm.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gttetteugt.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtbfzerdsm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xingfuxueyuan.xyz/gtiifcmgzg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtkjbwsukg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cdnleiting.top/gtjtxtpbxm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtitbcqumw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtdacyoltk.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gttipunlky.html

[E17] 首字母大写
来源：http://hz.hywenlv.cn/gtkibodriq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangkeji.top/gtnrkpoqts.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.haohaochexian.top/gtvscnkrdv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gtevhpyucy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtwypwhtmc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gaohongyu789.top/gtaxmljnqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhijiandao.cn/gtmrhelbga.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtndjakyko.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtolgofrak.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtjuwgzjrr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtufvouzdt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtyjydksyl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gthdvrozli.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtfvpxvoqt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtdeukfnes.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gthomjrdzs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gtvyuvbmum.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gtvtmxnlvk.html

[E19] 多行文本按行拆分
来源：http://hz.jinqigfzy.top/gtnmqxzzfu.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtblxsbdbr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xinyue.icu/gtsntgvwyc.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtqjbjrjvs.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gttzdnkjvu.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtuixeoanr.html

Go:   strings.Split(s, "\n")
来源：http://hz.sufxvd.cn/gtpdhjijyv.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtcsoijbrj.html

C#:   s.Split('\n')
来源：http://hz.ivvv.top/gtmfpbygbz.html

[E20] 判断字符串是否为空
来源：http://hz.yonumen.top/gtknxsxmve.html

Py:   if not s:
来源：http://hz.yvedp.cn/gteetptuje.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtkcprdlgr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pengpengdd.cyou/gtocmtkppg.html

TS:   if (s === "") {}
来源：http://hz.xuanzx.com/gticxsxvdj.html

Java: if (s.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtcpyabsqf.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtkchefdrw.html

Ruby: if s.empty?
来源：http://hz.zycfv.cn/gtbdpamchq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtgsdaktwx.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtbzggniie.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangdashe.top/gtbdxytntd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zdqjudy.top/gtjdoahndd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtwdsqxxzr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtaypgyych.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtyodxfoun.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.c1oappe.top/gtkzgvpgxn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gthikmegls.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtzbimmtni.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtsswgbkap.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtmqghykkx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtwqwabsyh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtfeyoojom.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtywkktcjq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yuanzhike.top/gtfrrnqrqp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtfqotbwea.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangshuangyany.cn/gtejxoeczo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtzlvtncbb.html

================================================================================
来源：http://hz.yonumen.top/gtrzmyopsx.html

F. 文件与目录
来源：http://hz.pengpengdd.cyou/gtzcktvlyo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtdiyezasv.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtmvkermsk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtqlxaouhb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cucudq.cn/gtppecfjvf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gtscmtklvl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtzhierwcn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtuqqyetpi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtjmrxnzmc.html

Ruby: File.read("a.txt")
来源：http://hz.quarkkingdee.top/gtchunwpid.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gtqhgltlyw.html

[F02] 逐行读取文件
来源：http://hz.andypj.xyz/gtgqplcbtd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zdqjudy.top/gtezjkgxla.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtidljbpuo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtuhcygoxc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtezdnsnnf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtclsjslnq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtdzzgaoxc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xziqi.cn/gtaluuidxw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ppjwa.cn/gtyvkwbloi.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtjtmtkopa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gthgxaxeds.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gzhubu.top/gthcorxmga.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtucptwpta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtcsngtqub.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gtmjdclkcu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gtmqbyfapq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ivvv.top/gtwbewawdj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtuwfhlanz.html

[F04] 追加写入文件
来源：http://hz.wangshuangyany.cn/gtisbxpgtd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtaeeteyxi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuanzx.com/gtxousthal.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtwwvdkbbm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtzwxxxxja.html


<!-- 参考信息 -->