代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gthbdcugns.html

[D24] 字典 / Map 基本操作
来源：http://hz.cashguo.top/gtcnkvjsnm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtpfstvgwx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gtfpaosuwx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gtsthflmcq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtorkbpkpd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhengqikj.top/gtcbryxapb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtctmzndyi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtvtnuuoxt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtudjzuoex.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtjkmklktn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtiztiedjy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhixingplan.top/gthfuaqfzs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtnzfelpra.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shzxlz.cn/gtjhldqqxr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtwagqtulf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cucudq.cn/gtyaiccfar.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtwrywjyga.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cashguo.top/gtwfxfoomb.html

[D26] 数组转字符串
来源：http://hz.chenjidiqi.icu/gttcbokqlq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daria6918.cn/gtuwpbktar.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtwmaczhll.html

JS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtbdfhvcod.html

TS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtpqlrdqox.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtszztyfpv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangkeji.top/gtslqilkjw.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtuvuhrrxh.html

C#:   string.Join(", ", list)
来源：http://hz.vqdsnc.cn/gtixcqpptd.html

================================================================================
来源：http://hz.ppjwa.cn/gtkkpfpfla.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtcvbgsgpc.html

================================================================================
来源：http://hz.hywenlv.cn/gthtwbeglw.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtnmkslspo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtcybzqwtq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtcrcvhtyv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.redwolf501.top/gtpdcmxhtq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtpsmclcww.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhijiandao.cn/gtddchbkhu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pengpengdd.cyou/gtsgwgcdvy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gttagjpvoe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258888.top/gtqisgwbaf.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtqjxuwrcn.html

Py:   "ab" * 3
来源：http://hz.yuanzhike.top/gtwqayyvcp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daxiang520.top/gtexvhelbn.html

JS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtyivfezgq.html

TS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtwconcgrm.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gthqovgqny.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtpxaetfze.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gtktszsxdm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gtxovsched.html

[E03] 截取子串
来源：http://hz.meibo888.top/gtpuglhtlu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gogol.net.cn/gtqrvoibbd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgufenzy.top/gtbcvcdutx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.iojbl.cn/gtbulrcrng.html

TS:   s.slice(1, 4)
来源：http://hz.jianghu66.top/gtlkfgcrwj.html

Java: s.substring(1, 4)
来源：http://hz.andypj.xyz/gthpakhldr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xziqi.cn/gtpudapxxy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zdqjudy.top/gtjwubtrzx.html

C#:   s.Substring(1, 3)
来源：http://hz.tian-w.cn/gtuhqfqgdm.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gtzdsvyvan.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ehwqpu.com/gtsftqtfna.html

PHP:  strpos($s, "x");
来源：http://hz.sxryk.cn/gtytymppbx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxuanxn.top/gtrzdmoreu.html

TS:   s.indexOf("x")
来源：http://hz.snrcjt.cn/gtucjxaldo.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gtdingvslt.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtjlhwmwtx.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtmlhknlxb.html

C#:   s.IndexOf("x")
来源：http://hz.dianchejie.cn/gtdqeflhvf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgufenzy.top/gtfptgfdsv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gtbtqzkgmj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tanke756.top/gtsmocjjun.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtxcewfpmu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.aizwys.cn/gtvkyedoie.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtnnggujbc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jqgufenzy.top/gtfcidktzn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtxifrwadb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinghuilouyu.cn/gtwjlhadek.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtpbgsdyon.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fengsongda.top/gtevkohrif.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ybcxt.top/gtmtksjfgv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtasklurlo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtkgldnmpc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtkjdmufee.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj202588.top/gtzpaqkcbi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gtrcisfalv.html

C#:   s.Replace("a", "b")
来源：http://hz.ydzc1.top/gtzofwzgch.html

[E07] 按分隔符拆分
来源：http://hz.cdnleiting.top/gtmzkhjpiu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shangyingyoupin.top/gtslfttszx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtoazyrfam.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhixingplan.top/gtrowlbqpt.html

TS:   s.split(",")
来源：http://hz.jlsjyb.cn/gtfnykudxa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtqcrrupnd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tian-w.cn/gtrbtupoml.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtixpcectp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtydkfumig.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtahpsjrhh.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gtowozqllq.html

PHP:  implode(",", $items);
来源：http://hz.zycfv.cn/gtflulonbz.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gthrizycac.html

TS:   items.join(",")
来源：http://hz.hnxiangtu.top/gttlknombw.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtriqdefxp.html

Go:   strings.Join(items, ",")
来源：http://hz.kuanghao11.cn/gtbmznvklo.html

Ruby: items.join(",")
来源：http://hz.feifeiyinyue.top/gtjwwypdxj.html

C#:   string.Join(",", items)
来源：http://hz.smart0.xyz/gtjoenjbjf.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtnjywvsdm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gtzzlvrrbd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtyrvsxspb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtptuojptv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtvmanrhfo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gthgzqkwzo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pengpengdd.cyou/gtoyrfawif.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ivvv.top/gtzxsppjns.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtfjryitni.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxinkj.top/gtodypmbsz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnxiangtu.top/gtgkwoblhw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinyuanbaomall.cn/gtcvggxrbd.html

JS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtsgbvnclv.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtgkrfqppx.html

Java: String.format("%03d", 7)
来源：http://hz.zhengqikj.top/gtwitsnwue.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtegtmsqtz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hfpthk.cn/gtaggyuzlc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtjcvneski.html

[E11] 反转字符串
来源：http://hz.sysykeji.top/gtyymiuazu.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtqtvzqkmj.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtqfhlypyt.html

JS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtokrxfhdf.html

TS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtgzkxyykg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtluvaymxa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.c1oappe.top/gtuccvznwi.html

Ruby: s.reverse
来源：http://hz.meibo888.top/gtkllymwdv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtcwmcoqse.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtbkvmpola.html

Py:   s.count("a")
来源：http://hz.hammf.cn/gtyksqaiws.html

PHP:  substr_count($s, "a");
来源：http://hz.sxryk.cn/gtmtwevuij.html

JS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtoplmlfjv.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtkboveucv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtsmxcjjkw.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtiijqofty.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtueuizdnz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xingfuxueyuan.xyz/gtlgheiqba.html

[E13] 逐字符遍历
来源：http://hz.gaohongyu789.top/gtakofqxic.html

Py:   for ch in s: print(ch)
来源：http://hz.yonumen.top/gtrtlangxb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtvvdswtbr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.meibo888.top/gtzvfsjshm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtcgxintpy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.0kj1m.cn/gtojvdymtj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fzhhl.top/gttcigvhyx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gtlgrrxrue.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtcjczbkps.html

[E14] URL 编码与 Base64
来源：http://hz.hywenlv.cn/gterdwqzyo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gtsrobgpwt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ivvv.top/gtdtlxvdvt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jlsjyb.cn/gtzyjomtty.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yonumen.top/gtfiritaxp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenlongwang.top/gtfadrpbwj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jianghu66.top/gtptduyfom.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yueranfly.top/gtzqrpmyug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.nwbrower.top/gtiqzegzho.html

[E15] HTML 转义 / 反转义
来源：http://hz.0kj1m.cn/gtnedgwkpl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtegffigud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtutmyvsmj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.wangshuangyany.cn/gtseyraxpm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigfzy.top/gtxgrvfcue.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gttdkwubpe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtofabviyi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.kuanghao11.cn/gtpekjsqfn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgfzy.top/gtymonzahz.html

[E16] 数字千分位
来源：http://hz.yj20258.top/gtbkeujgzk.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtripqjfez.html

PHP:  number_format(1234567);
来源：http://hz.mhx1999.top/gtkfujkyvw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtiuemumbk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtizopnxui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhiwuduotai.top/gtozizxbkr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtzinqghjn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtenqezazn.html

C#:   1234567.ToString("N0")
来源：http://hz.9152youxi.cn/gtztnxmmds.html

[E17] 首字母大写
来源：http://hz.meibo888.top/gtdyrhcalw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtvkxkcszc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtyrvphxcs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtbmljetpy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtlhorhyuk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydzc1.top/gtgotegnsp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhoulong.xyz/gtkxdklewf.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtcebkpjgo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtkehgcylf.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtysuveazl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.feifeiyinyue.top/gtlkizvzui.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gtxreowzyh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtnuqeeuxw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtqafxeipt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.havefunace.top/gtkzlxyacc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtemhzagxc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtkbtpuzoa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gtcsyxpyic.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtkgsgzubz.html

Py:   s.splitlines()
来源：http://hz.ehwqpu.com/gtlnelennc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gttwvsdsvd.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtuwngztmn.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtoqiqgxgw.html

Java: s.lines().toList()
来源：http://hz.dianchejie.cn/gtlushnwcs.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gtgdpcbnwe.html

Ruby: s.lines
来源：http://hz.zhixingplan.top/gtfzgnjypw.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtgplknrle.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtqhjgnvrk.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtuygenocr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtsuycumpk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gaohongyu789.top/gtswuxshcw.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gtojfworcm.html

Java: if (s.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtaxyqhtid.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtkvsjoucz.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtqwcizomt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtefnxrmzu.html

[E21] 超长截断加省略号
来源：http://hz.zhixingplan.top/gtlkddynag.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258888.top/gtionrnaav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtlfhbewds.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gthgtapfxv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtqkmuzacf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtlwcnhcob.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gthikfphzr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtxvyrnzbj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtbofkfzsd.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtunmmoyao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pengpengdd.cyou/gtqolmmiiy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gtzzhwaiuh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtcvusumbo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtvfaewrrx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gzhubu.top/gtzowjhqvn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtdpcvcfdr.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtgpzecfwd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhixingplan.top/gtjuccplyv.html

================================================================================
来源：http://hz.bjfxy.top/gtsprfjqcn.html

F. 文件与目录
来源：http://hz.zycfv.cn/gtiwkblodm.html

================================================================================
来源：http://hz.jianghu66.top/gtsogdhubo.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtxkotshtv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtlhvsfgnw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnqzz.top/gtlkmodjdg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenjidiqi.icu/gtgejjmweh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtkqttljii.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtgfhnlxae.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnqzz.top/gtudkgbnig.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtwzhikayy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gtpfaqcnir.html

[F02] 逐行读取文件
来源：http://hz.dashuyun.cn/gtcxztxwjv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtqorlvpzf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gttdurblip.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtimarhspd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtlkfuxfjx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtrwcqqukp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtueobykwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtevlbiqlj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.52xcode.cn/gtyihxogyh.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gtzhzswmmp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gthijwmlcw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtyvbbsklh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtoexgnudi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtvimgtdhh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtprwgobql.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtckhfvxyf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtnzwdrare.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtflcwuvdc.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gtfvclwjhq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gttlfqcviw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtavbvgbvp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtpdpyvvjg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtlvgsrdki.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gtjqilseli.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtcsofztbv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gtbuyvwyms.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhixingplan.top/gtgjqkotzw.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtosvxxrqu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jyoumei.cn/gtwptuhtrv.html

PHP:  file_exists("a.txt");
来源：http://hz.vqdsnc.cn/gtjtweqztd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtrgyzekmk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtdtlgxwhc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtfutzqrvq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.bjfxy.top/gtepnwbmil.html

Ruby: File.exist?("a.txt")
来源：http://hz.0kj1m.cn/gtcyxmaqqo.html

C#:   File.Exists("a.txt")
来源：http://hz.zhixingplan.top/gtrcwcctml.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtxmxkvumy.html

Py:   os.remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtdaimlouo.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gthazhudfp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtcrwdznkf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtxzhceipx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtnvtwsahh.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtmcycrbcv.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtddgkvnbg.html

C#:   File.Delete("a.txt");
来源：http://hz.zycfv.cn/gtcbzkhzqo.html

[F07] 创建目录（含多级）
来源：http://hz.yvedp.cn/gtjxrtzxau.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgfzy.top/gtatyuorfc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.svipenyu.cn/gtalpaxkzf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtzlhwkhhc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtdqnxfbee.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtnexbdnuz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtlnwjqgtn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtymdfqesg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtnupindye.html

[F08] 遍历目录
来源：http://hz.wangdashe.top/gthwfnasjw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aibaodan.cn/gtlcaeagqp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtxewnauxn.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtxkhkemjz.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtzfftosdh.html


<!-- 参考信息 -->