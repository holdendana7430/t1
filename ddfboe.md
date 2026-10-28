代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.hfpthk.cn/gtmpbedsnt.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtrjtvyytu.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtdcqpqdem.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gthvzragdu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258888.top/gtrgelyxka.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtuzybhprl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtzzkbtumf.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtbydtqgez.html

Java: new ArrayList<>(list);
来源：http://hz.ivvv.top/gtklncwavc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtvgidqvua.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtskkgovdh.html

C#:   new List<int>(list);
来源：http://hz.gotoacloud.top/gtoyxvttwe.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtglmzpjzk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtnxknmadv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtjayjgswf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtnucyrfef.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gtbgynrxqt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtmgjsttou.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtenkmljhr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtjlwdlebn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yanxiufei.cn/gtilykdvoz.html

[D24] 字典 / Map 基本操作
来源：http://hz.gotoacloud.top/gtrttwoxpc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtdllodzud.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtnouxiqux.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ywan-chungtsiang.top/gtkbpyiaro.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtbecmubob.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sysykeji.top/gtuevbidfq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtpodjgqgy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtplhuckkx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ybcxt.top/gtkrcdnxzy.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtnogfbboi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtdasvgiaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.feifeiyinyue.top/gtemspzeul.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gotoacloud.top/gtnvtpsenu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xinyue.icu/gtmskevaet.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cdnleiting.top/gtypreyufv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.haohaochexian.top/gtvlxrlpib.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.redwolf501.top/gtwimeebgv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.52xcode.cn/gtbnoeoqvl.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtivgffnct.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ywan-chungtsiang.top/gtfvekidot.html

PHP:  implode(", ", $arr);
来源：http://hz.316326.xyz/gtfkkjbdvg.html

JS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtfvdzmddp.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gterqwokjn.html

Java: String.join(", ", list)
来源：http://hz.ydjk.org.cn/gtjodgrubk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj202588.top/gtqvyutmhk.html

Ruby: arr.join(", ")
来源：http://hz.ybcxt.top/gtnapsrqwa.html

C#:   string.Join(", ", list)
来源：http://hz.mhx1999.top/gtndmzpqxh.html

================================================================================
来源：http://hz.gotoacloud.top/gtznfzqixz.html

E. 字符串处理
来源：http://hz.chenjidiqi.icu/gtbeetmpqh.html

================================================================================
来源：http://hz.daria6918.cn/gtteuoohwq.html

[E01] 拼接字符串
来源：http://hz.zdqjudy.top/gtdwxrvypk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtylbhgfvo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fzhhl.top/gtbdhvsysz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtfixqwbmb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtzhdckkym.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtuulqhzgp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gtxnmblhgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pengpengdd.cyou/gtwkrwkvil.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gttkoppznb.html

[E02] 重复字符串
来源：http://hz.yangfankeji.com/gtrpzludnm.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtxysdzvxk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.bjfxy.top/gtkljxfohq.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtpkfbsmar.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtgceppyxh.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtagzaqbbp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangkeji.top/gtbmiqwuve.html

Ruby: "ab" * 3
来源：http://hz.yongpay.top/gtofsnccqq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gthbkuixro.html

[E03] 截取子串
来源：http://hz.316326.xyz/gtaenfbvds.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gthwpnnpbx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtiukoreli.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtdzoheren.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtyndwsusv.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtzdtsdwsb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daxiang520.top/gtbszgnatv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xylfe.cn/gttjalypzb.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gtvfolbipa.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtsbqviccj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aibaodan.cn/gtwbpusutb.html

PHP:  strpos($s, "x");
来源：http://hz.sxryk.cn/gtxkhaclmd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtrvkzhomw.html

TS:   s.indexOf("x")
来源：http://hz.zhixingplan.top/gtwagwzwho.html

Java: s.indexOf("x")
来源：http://hz.tanke756.top/gtafnqfeuc.html

Go:   strings.Index(s, "x")
来源：http://hz.jianghu66.top/gtdppwqfnw.html

Ruby: s.index("x")
来源：http://hz.yongpay.top/gtqswxanbn.html

C#:   s.IndexOf("x")
来源：http://hz.shuidangran.top/gtfdyywxjm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.havefunace.top/gtbwzgwtjp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigfzy.top/gthjaepxjw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtunkzrtns.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtrhzzkvvj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinyuanbaomall.cn/gtdsyvxgjx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtnnnyscrg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.daxiang520.top/gtselvmbvi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zdqjudy.top/gtejxjjzdi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtyewecutf.html

[E06] 替换子串
来源：http://hz.yangfankeji.com/gtyoqjhdnm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gtmmaismge.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydjk.org.cn/gtytvlyxac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtuztwbeqz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtilnisnzp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtucrvxtbp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhixingplan.top/gtqeojobka.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sufxvd.cn/gtrlarrdbb.html

C#:   s.Replace("a", "b")
来源：http://hz.ivvv.top/gttwxpzqxv.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtiaahfhmm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daxiang520.top/gtuiitafdk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigufen.top/gtvcxpclqg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pycfn.com/gtfttdellj.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtwzyieayf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gaohongyu789.top/gtkhpuxjno.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shanyushiyangkeji.top/gthqjvfxba.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtqcetihzn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gthygdekfn.html

[E08] 数组按分隔符合并
来源：http://hz.hongshengwenyu.top/gtsvmwwkkk.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtflwyphez.html

PHP:  implode(",", $items);
来源：http://hz.yj20258.top/gtrbncfsvr.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtgpgszyhk.html

TS:   items.join(",")
来源：http://hz.xuanzx.com/gtfwrewgvq.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtkehcdhbf.html

Go:   strings.Join(items, ",")
来源：http://hz.gzhubu.top/gtvjtrdywb.html

Ruby: items.join(",")
来源：http://hz.cqqwz.cn/gtybqbblpn.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtezjtpeot.html

[E09] 去除所有空白字符
来源：http://hz.svipenyu.cn/gtrbxmptbp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.mhx1999.top/gtqkdfpseh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.iojbl.cn/gtpnbxpoig.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtjgaasgxz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtslwtudtg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.dashuyun.cn/gtdwrkabvz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtmczdfshw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtwgvofaal.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ehwqpu.com/gtqbvbgjau.html

[E10] 左侧补零 / 定长填充
来源：http://hz.c1oappe.top/gtfoujvugm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtfrgachix.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinyuanbaomall.cn/gtzoktvmar.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtszddsmwt.html

TS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtzmhecnhl.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtnruegddo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxinkj.top/gtduynitle.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtcllfiycc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtnimzanse.html

[E11] 反转字符串
来源：http://hz.zhaomingkeji.xyz/gtnbybztuc.html

Py:   s[::-1]
来源：http://hz.dianchejie.cn/gtehfjsaoq.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gtvzpvkbmq.html

JS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtnnmvvzjo.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtyigqycjl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtmccdrrcj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.smart0.xyz/gthfkywbid.html

Ruby: s.reverse
来源：http://hz.jqgfzy.top/gttxhebvpw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtsungpqst.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtsemliipf.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtnabrgpmh.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gtyaxbhhvz.html

JS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gthqwixrvc.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtcfobdnal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtjpvyeamj.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtphcxqgcy.html

Ruby: s.count("a")
来源：http://hz.jinghuilouyu.cn/gtjjxvirgg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gthjadihip.html

[E13] 逐字符遍历
来源：http://hz.ybcxt.top/gtptgqdsas.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtwjlkwqsw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yanxiufei.cn/gtemwdpfbm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtghkuudwx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtozgvliju.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gtkdnkqkey.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtyypfhsqo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtpyjemzpr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhiwuduotai.top/gtbqhwldla.html

[E14] URL 编码与 Base64
来源：http://hz.svipenyu.cn/gtagtlgble.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cdnleiting.top/gttruhtwbc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtukmfahri.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gttjvuioyh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtmdrvzbee.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxuanxn.top/gtvgpuzsjn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tanke756.top/gtqmwabhld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtkrsivzwf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shuidangran.top/gtfnvdnysh.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtglogsgiu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtcejprjhn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhongyouzk.top/gttgptajii.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cucudq.cn/gthcmezqlo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hfpthk.cn/gtomotruqz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jiagoushi.top/gtqlwoyots.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yvedp.cn/gtxmxagdsa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.feifeiyinyue.top/gtayvqlbpm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tanke756.top/gtquuoxxfz.html

[E16] 数字千分位
来源：http://hz.ydzc1.top/gtyedjedvn.html

Py:   f"{1234567:,}"
来源：http://hz.ywan-chungtsiang.top/gttvyjpgjh.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtngythdkw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtfpewlrvr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gtiiiixymw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.andypj.xyz/gtphyghave.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtsodwpnyi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gthuegvfjk.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtluwngigl.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtotinegvk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtntdgkznk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtpljpdmzc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtpqdfnnic.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtazrjgbnk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtigyhxjny.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtarhjkvkv.html

Ruby: s.capitalize
来源：http://hz.hfpthk.cn/gtmuieoznf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.wangshuangyany.cn/gthlwejuvp.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gtldktcagw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtksmiwgdj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtzhlwkczt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gthnmafpek.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtaxhzwuif.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tianlin.xyz/gtfuojozxd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.haohaochexian.top/gthslevrpe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.0kj1m.cn/gtlsvwldaf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtekzdynvs.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtqelspqtj.html

Py:   s.splitlines()
来源：http://hz.fengsongda.top/gtqaaqpohi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jyoumei.cn/gtowdmchbk.html

JS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gtvekzkavn.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gteyocqtqg.html

Java: s.lines().toList()
来源：http://hz.haohaochexian.top/gtvdwgthfp.html

Go:   strings.Split(s, "\n")
来源：http://hz.xingfuxueyuan.xyz/gtqgrpepeg.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtjddomybb.html

C#:   s.Split('\n')
来源：http://hz.shzxlz.cn/gtcfbnoibh.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258888.top/gtdeaghkhf.html

Py:   if not s:
来源：http://hz.cheryme.top/gtvfalkjud.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtgmavximt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cdnleiting.top/gtwqmvatjo.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtglmkmnjy.html

Java: if (s.isEmpty()) {}
来源：http://hz.yongpay.top/gtmhhffccm.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtyvdljvje.html

Ruby: if s.empty?
来源：http://hz.hnxiangtu.top/gtvqohfjeh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigfzy.top/gtngbuwddi.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtbzuwnlwt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fzhhl.top/gterucnikl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtrkszpvkn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gteveestio.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gthhgixaff.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtsknvihrn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuxming.cn/gtdvuwffey.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtrhzarczj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hammf.cn/gtkkhgtamm.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtvjyvecuz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gthjxnkizf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtlusxcalp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtdgfqysnu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtuvumholv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yanxiufei.cn/gtvdoncogk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gtlozvsilu.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigfzy.top/gtjyybwvbx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtrkykjjks.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpnudojsm.html

F. 文件与目录
来源：http://hz.mhx1999.top/gtixkxiqae.html

================================================================================
来源：http://hz.hammf.cn/gtdldnjxoo.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gteqqreuye.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shzxlz.cn/gtbongzoax.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtoifvaopv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtrkykgftu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtoarxmenz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtzllyhksm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gteztjyivx.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtczgwgwad.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtkmaltvwc.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gtetwimmjc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.havefunace.top/gtgluyirvf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hysaishi.cn/gtuegtjqaj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtricvygcv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtaqkyzquf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtlmydcbde.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtyfwmcgsj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ivvv.top/gtiezrrsjl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.birdmap.top/gtqobcnfpl.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtikvxlrhb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daxiang520.top/gtaimaidgt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtxtgckhop.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtaawphkau.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gthavfxnfv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtlqzirtyu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gthpeceoxc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gthoijidna.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gtthkrcxoz.html

[F04] 追加写入文件
来源：http://hz.zhixingplan.top/gthiksruxr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenzaomai.com/gtiersexss.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtkzexgbey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtezpbjyay.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtkhksfpep.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.redwolf501.top/gtxkwynrfi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtvccgjuez.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtdmbfqibi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtquaqnmte.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtcwpcblrn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuanzx.com/gtvaipomzs.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtllgzxhud.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtfkecexan.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtmqxokfkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtssxuhpad.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gogol.net.cn/gtelypsfxt.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtugqfueaa.html

C#:   File.Exists("a.txt")
来源：http://hz.chenlongwang.top/gtjhtdcqxi.html

[F06] 删除文件
来源：http://hz.jlsjyb.cn/gtvdrhmjsq.html

Py:   os.remove("a.txt")
来源：http://hz.shzxlz.cn/gtlbbvurve.html

PHP:  unlink("a.txt");
来源：http://hz.tian-w.cn/gtbzmepvwu.html


<!-- 参考信息 -->