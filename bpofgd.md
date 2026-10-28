代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtlrmawrwz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aizwys.cn/gtopidykwr.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtltcviwvp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gtzixeuhfo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtyffquxao.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtexjvgjqx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.birdmap.top/gtjlbpgmmy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtnidnprus.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tanke756.top/gtoyjfkmlz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gtpeuafxso.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gteavwwzlz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtpblobkqa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuanzhike.top/gtkbltiwsx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yonumen.top/gtfjaquzbc.html

[D25] Set 集合去重与交并差
来源：http://hz.ehwqpu.com/gttlahypxn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gotoacloud.top/gtzlxzeplj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cucudq.cn/gtbqjvzicy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yanxiufei.cn/gtdvjbyhhy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xinyue.icu/gtpkrvgwou.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dashuyun.cn/gtomnzpnxk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtfbkrysek.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj202588.top/gtszsckmbb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuanzx.com/gtpnjzqaav.html

[D26] 数组转字符串
来源：http://hz.zhixingplan.top/gtywpyczql.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gttedghxfe.html

PHP:  implode(", ", $arr);
来源：http://hz.pengpengdd.cyou/gtabsknzrj.html

JS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtqheznbfr.html

TS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtvbialhjr.html

Java: String.join(", ", list)
来源：http://hz.pengpengdd.cyou/gtiuohzwru.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtvqcckook.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gtegggsexn.html

C#:   string.Join(", ", list)
来源：http://hz.bjfxy.top/gtcjvnlziq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvumnlqpc.html

E. 字符串处理
来源：http://hz.vqdsnc.cn/gtwuslujdr.html

================================================================================
来源：http://hz.chenlongwang.top/gtjafhgwrk.html

[E01] 拼接字符串
来源：http://hz.jinqigfzy.top/gtcelebagi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtbijnpzrr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtoajtdptu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtchuhqzdk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtmmvpyltg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.svipenyu.cn/gtvfdifnfg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tianlin.xyz/gtsfzkmcao.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gttxzwnfrm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hywenlv.cn/gtuzzhkycc.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtbcuwugpl.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtoihcrikd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtuzhszazp.html

JS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtoachxjlg.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtrxcsjqln.html

Java: "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtnerkulok.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xylfe.cn/gtmbrphknq.html

Ruby: "ab" * 3
来源：http://hz.tanke756.top/gtpnmnpsfs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtbakyipgn.html

[E03] 截取子串
来源：http://hz.yj20258888.top/gtrylewmbt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.feifeiyinyue.top/gtugqkiuyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.bjfxy.top/gtbdjeldly.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tian-w.cn/gtwegagrsh.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gtzqoeaxub.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtrywibktw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hammf.cn/gtahuzcmoa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ivvv.top/gtmhqhjxgm.html

C#:   s.Substring(1, 3)
来源：http://hz.bjfxy.top/gtlznuyexr.html

[E04] 查找子串位置
来源：http://hz.ydjk.org.cn/gtnauysxac.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xuetiantiany.cn/gtnixifsya.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtoznhvzzf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guowangkeji.top/gtpwljvkzk.html

TS:   s.indexOf("x")
来源：http://hz.9152youxi.cn/gtwnmhhcuh.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gtrlrfqekp.html

Go:   strings.Index(s, "x")
来源：http://hz.redwolf501.top/gtlekorrlw.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gtxbxivfsw.html

C#:   s.IndexOf("x")
来源：http://hz.ehwqpu.com/gtnbiibwqd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtivgsxxgz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnqzz.top/gtnayxppws.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.birdmap.top/gtftvtvtbb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtkkhzhgcx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hysaishi.cn/gtqvxwhbvh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtazwmeuyt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jyoumei.cn/gtaagsttkf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtywghnizh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yangfankeji.com/gthjienciz.html

[E06] 替换子串
来源：http://hz.yanxiufei.cn/gtidnjntnb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ivvv.top/gtwrjcvszq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtliagffim.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtguhlclqb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtkezozjsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtwmxtavgq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtcvjfxglj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtwbimckmt.html

C#:   s.Replace("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtdggmsmvd.html

[E07] 按分隔符拆分
来源：http://hz.cdnleiting.top/gtslxvijmz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj202588.top/gtcclhnian.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtwgyhliie.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gzhubu.top/gtrcqbygtf.html

TS:   s.split(",")
来源：http://hz.hongshengwenyu.top/gtqlxmqdxv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gthvlvxabe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cashguo.top/gtligyjjri.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtdvesyzar.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhengqikj.top/gtohbnddha.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtdukliqze.html

Py:   ",".join(items)
来源：http://hz.daxiang520.top/gtlttxyncv.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtwnkyocxa.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtygxhkkfk.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gthmhsmega.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gtklpeqhuu.html

Go:   strings.Join(items, ",")
来源：http://hz.hammf.cn/gtnvhrextz.html

Ruby: items.join(",")
来源：http://hz.hammf.cn/gtrlwanigm.html

C#:   string.Join(",", items)
来源：http://hz.daxiang520.top/gtvfeaexxi.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtaircypkx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtwozrrqlq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cdnleiting.top/gtwplsumuh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtxuhhqdrj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtwobhpvnr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtabnmeyck.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tanke756.top/gthxyacjwq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.9152youxi.cn/gtlodmohxl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dianchejie.cn/gtngruhakn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtiedddign.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daria6918.cn/gtxlpbfskr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shangyingyoupin.top/gtutdhbctl.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtvxpgnvuz.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gthmpfgqzw.html

Java: String.format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtlkavuzgb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tian-w.cn/gtzuaemlei.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtxjbgzsvj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtsaitqksy.html

[E11] 反转字符串
来源：http://hz.daxiang520.top/gtvyruzltw.html

Py:   s[::-1]
来源：http://hz.yj20258.top/gtckvdzeum.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtzgyjklvn.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtvaldqcyw.html

TS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtzqlbedmc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtdtakgqmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtwargeanl.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtjinhyngc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtboocurbe.html

[E12] 统计某字符出现次数
来源：http://hz.zhixingplan.top/gtnwttgcjj.html

Py:   s.count("a")
来源：http://hz.xuetiantiany.cn/gtmvyqpbgi.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gttesafddk.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtzgocwywn.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtowbnapub.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yueranfly.top/gtxslnalfc.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gtmlqroiku.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtxcvdkccx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258888.top/gtztkpkbdq.html

[E13] 逐字符遍历
来源：http://hz.birdmap.top/gtgezoyahv.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtqryoyhri.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydzc1.top/gtmcgfbnbf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtsmyxsixj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtkrdnnujp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sufxvd.cn/gtdmdxxhde.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtmptaruaw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtsmkxvwne.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daxiang520.top/gtnhzrkmap.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gtkdagfeoq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tianlin.xyz/gtfenhcwwj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gthfehfyvt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhiwuduotai.top/gtukndeqhh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtbnrvrujq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gttkslmdpt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtxoflvdlv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtbqwbfboh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtaupzshbl.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxinkj.top/gtbgzpbpad.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnqzz.top/gttwexynau.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigfzy.top/gthecjbskp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cashguo.top/gthdcbikdp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gotoacloud.top/gtsjpmzzxo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtvskoypbr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gthnuzkfcg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtidkdteqq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.c1oappe.top/gtbkwyfuch.html

[E16] 数字千分位
来源：http://hz.yueranfly.top/gtrxdfcwkr.html

Py:   f"{1234567:,}"
来源：http://hz.bjfxy.top/gtvdwkcizr.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtworpwlib.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtzztjohed.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtrdkfsgjb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtflabwotv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtfxjfuuhc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtvrozyebf.html

C#:   1234567.ToString("N0")
来源：http://hz.xuanzx.com/gtdrxpsajv.html

[E17] 首字母大写
来源：http://hz.yueranfly.top/gtjgbrqtsp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuanzhike.top/gtxbspbyfq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtomqmeapc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gttdbsizky.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtelxirzga.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigfzy.top/gtdfohlxsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pycfn.com/gtqrneqkfd.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtkknxntgd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.iojbl.cn/gtpsculxub.html

[E18] 模板占位符替换
来源：http://hz.jyoumei.cn/gtblvcadwq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pengpengdd.cyou/gthinxnxxa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zdqjudy.top/gtpmzcgolg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtnswyukvj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gthippgdil.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtyhiqjdez.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.vqdsnc.cn/gtxzdexjda.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtwjisfyqv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sysykeji.top/gtlowsyiyy.html

[E19] 多行文本按行拆分
来源：http://hz.smart0.xyz/gtrzxejoib.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtrbeylnxf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtjjfgofek.html

JS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtgfczfggw.html

TS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtwteyqvfg.html

Java: s.lines().toList()
来源：http://hz.hysaishi.cn/gthdcbferf.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gttkknciqv.html

Ruby: s.lines
来源：http://hz.wangdashe.top/gtmmfkoqva.html

C#:   s.Split('\n')
来源：http://hz.hysaishi.cn/gtvjhkfzbj.html

[E20] 判断字符串是否为空
来源：http://hz.yj202588.top/gthdibnirz.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtsbunrlbp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtmnluhpef.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gtrgpcczis.html

TS:   if (s === "") {}
来源：http://hz.cashguo.top/gtulsaytfl.html

Java: if (s.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtfupmdytl.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtmljczapl.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gtwldyckhf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtbsdhvdey.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtktqkukul.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtzkfrzwem.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtziaprhny.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtbelftfni.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtndquwnjf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtbbjueohf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtwlnowflz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtzjjogagi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtbowdaicl.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gtwntciyhj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtwxyhnuis.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtsomvfqvm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtsuqhwjzy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtkgmmyldp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.redwolf501.top/gtnnizotqg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtcbcmuwsw.html

Ruby: s.bytesize;  s.length
来源：http://hz.cashguo.top/gtkglvalmn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtljvideao.html

================================================================================
来源：http://hz.mhx1999.top/gtbxmnxjuc.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtcvhfgjxr.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzohwkgml.html

[F01] 读取整个文件
来源：http://hz.ywan-chungtsiang.top/gtgtqdrihc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtnhppvttv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtgdujxwcj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.snrcjt.cn/gtgprsyfdw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.52xcode.cn/gtriqlzaex.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtwqftvmwh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gttywfcnpu.html

Ruby: File.read("a.txt")
来源：http://hz.chenlongwang.top/gtiqbtiiwp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydzc1.top/gtnmdtvdqb.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtqkhgrjhu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zdqjudy.top/gtigqvkcba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhaomingkeji.xyz/gtnxqmlldx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtotdatiee.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtwfpebced.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtsvlzykyj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtrwufngov.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.0kj1m.cn/gtdqzpxxcz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gthidtblfd.html

[F03] 写入文件（覆盖）
来源：http://hz.hywenlv.cn/gtftkixbqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gteyvwspgy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuxming.cn/gtvrwjujed.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtzejqzpaw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtxowopbiq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtusfqapxy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gthlqdsbsk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gthelwfmka.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gtjcnkuqzn.html

[F04] 追加写入文件
来源：http://hz.xinyue.icu/gtddvmlczt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtlxvonptw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtvxyaufea.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtregiibcl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtuvjveqai.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gtaouxhkus.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtgakayljn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtvdmmqcqx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gtumuselii.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuanzhike.top/gtrwuvxkan.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtohvyzlwg.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtvtmfjsyq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtorrayhzx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtgynxvbvh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gteaosvbvx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtmkohdjil.html

Ruby: File.exist?("a.txt")
来源：http://hz.yueranfly.top/gtpfuytllg.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtdmmnkxfx.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtkyxhakfk.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtdcwnakoo.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtsxpcfbgg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtyiivhsta.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtdygpipaa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtjksrqweq.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtxvdmghhk.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtuiozszfo.html

C#:   File.Delete("a.txt");
来源：http://hz.havefunace.top/gttfnfmrwj.html

[F07] 创建目录（含多级）
来源：http://hz.chenlongwang.top/gtefhwycdf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtptraxjla.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fzhhl.top/gtpgzfnryr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtabyhslht.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtanumgspx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtbunmktra.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gthvmujawt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtexmsuawy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtybhmkpia.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtehpdruqq.html


<!-- 参考信息 -->