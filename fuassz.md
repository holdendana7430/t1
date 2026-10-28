代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtpffblpky.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.9152youxi.cn/gtqeavwcmu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtvkntwbmb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.aibaodan.cn/gtpqkibxmt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtrgzlcjao.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtygrfmwaz.html

[D25] Set 集合去重与交并差
来源：http://hz.zhixingplan.top/gtxdahfoia.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtfqwhrxyz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sysykeji.top/gtwvqjvtsj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daria6918.cn/gtejzizowa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zdqjudy.top/gtqehujksu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtizuibspa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtrpdxynyc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtpohpgnvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aizwys.cn/gtnupqmfvh.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtzqesvbfs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jianghu66.top/gtssfujqgx.html

PHP:  implode(", ", $arr);
来源：http://hz.birdmap.top/gtbsxhitwq.html

JS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtxrivakso.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtjdzzpjvf.html

Java: String.join(", ", list)
来源：http://hz.haohaochexian.top/gtfrdfffaq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zycfv.cn/gtaqjviguo.html

Ruby: arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtpkuoumuf.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtodxijzae.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttlksejnh.html

E. 字符串处理
来源：http://hz.dianchejie.cn/gtiydyxodq.html

================================================================================
来源：http://hz.bjfxy.top/gtnsfkgmdv.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtjrohqmqz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.havefunace.top/gtnnqvljjv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtgbhsgsdo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gtljltbjoc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtogtayzyk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtavhtlffo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtyupddcay.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenjidiqi.icu/gtgkikvjoe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gtxosntugi.html

[E02] 重复字符串
来源：http://hz.guannengcc.top/gtxktynewu.html

Py:   "ab" * 3
来源：http://hz.tanke756.top/gtxrmfusry.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtslenmsfa.html

JS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtupmdolpx.html

TS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtlasomvka.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtdziyuakq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gtgrfvmkyj.html

Ruby: "ab" * 3
来源：http://hz.jinqigufen.top/gtcrrntymh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pengpengdd.cyou/gtiscqppgd.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtwtetbgiz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daxiang520.top/gtzpcslezu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuanzhike.top/gtuwryfhui.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtveckzrsv.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtryvcdinq.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtmobpdhfv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jlsjyb.cn/gtdgfpzbyz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtwasscmfk.html

C#:   s.Substring(1, 3)
来源：http://hz.guannengcc.top/gtlpbvumjl.html

[E04] 查找子串位置
来源：http://hz.kuanghao11.cn/gtceriejfa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gttmdzqqmp.html

PHP:  strpos($s, "x");
来源：http://hz.sufxvd.cn/gthdhfhqbp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ehwqpu.com/gtlvumzsls.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtifhxkfuc.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtfrjfrcpn.html

Go:   strings.Index(s, "x")
来源：http://hz.snrcjt.cn/gtpwgezqsk.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtpjjijbdl.html

C#:   s.IndexOf("x")
来源：http://hz.zhaomingkeji.xyz/gttlrkulnd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtlubnlrcd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtmlnakjuj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hongshengwenyu.top/gtqwlcsdyk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtslzucgxz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtvdjxizaw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtmjfixgft.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtxajdvduk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtassbhbfl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sysykeji.top/gtjhxehxtb.html

[E06] 替换子串
来源：http://hz.cdnleiting.top/gtkkmgiapf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtaisuscxs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.feifeiyinyue.top/gtpwnbmkdx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtszcqdnjb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtksaxgrdf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtxkfdytjw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.316326.xyz/gtdntphnbj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhongyouzk.top/gtxmbifyey.html

C#:   s.Replace("a", "b")
来源：http://hz.gogol.net.cn/gtgskxxddj.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtclgmkncz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtmwskpanm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj202588.top/gtmqgmknyz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ybcxt.top/gtuddwqtxp.html

TS:   s.split(",")
来源：http://hz.ydzc1.top/gtjzxgjfrl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtirnvwuwu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yueranfly.top/gtndrdrjer.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtzcdyngcx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtbspqzwad.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtuumpmdpe.html

Py:   ",".join(items)
来源：http://hz.c1oappe.top/gthiiljabj.html

PHP:  implode(",", $items);
来源：http://hz.yuanzhike.top/gtfekloxvu.html

JS:   items.join(",")
来源：http://hz.nanxinkj.top/gtgmnwyojz.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtcdqwkzay.html

Java: String.join(",", items)
来源：http://hz.yonumen.top/gtcvehsbrd.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtpyevrkju.html

Ruby: items.join(",")
来源：http://hz.xuetiantiany.cn/gteuwpjenr.html

C#:   string.Join(",", items)
来源：http://hz.zhiwuduotai.top/gtqqdrxjgv.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtbnlzwbgi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangdashe.top/gtrhuowrcl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.smart0.xyz/gtzupvbbge.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtbqlgquyz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtjcfpilym.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtuvwgcfgh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtlkqfgpyx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gtskcgeubg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guowangkeji.top/gthssokvbg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gtchdvdgak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hfpthk.cn/gtnbeomjrx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinyuanbaomall.cn/gtcjkdurjd.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtdorzyrnw.html

TS:   "7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtwlnevwvo.html

Java: String.format("%03d", 7)
来源：http://hz.andypj.xyz/gttytqlxtp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtjfdguuum.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gttzombmhx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hammf.cn/gtrroxnhce.html

[E11] 反转字符串
来源：http://hz.nanxuanxn.top/gtmzqrrgbs.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtpjpgogez.html

PHP:  strrev($s);
来源：http://hz.jyoumei.cn/gtjljllsvw.html

JS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtenivrpyq.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtvuoufgjn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydjk.org.cn/gtfvplealo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.feifeiyinyue.top/gtjnoqjxqx.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gttaowuxvq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtulensnwy.html

[E12] 统计某字符出现次数
来源：http://hz.cqqwz.cn/gtcjacqihb.html

Py:   s.count("a")
来源：http://hz.feifeiyinyue.top/gtmxjaielb.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtbkjdhiei.html

JS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtpkgsqrzy.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtdtaaugym.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtshaarosz.html

Go:   strings.Count(s, "a")
来源：http://hz.ywan-chungtsiang.top/gturkwikwa.html

Ruby: s.count("a")
来源：http://hz.shzxlz.cn/gtnmhwyfrn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guannengcc.top/gtltqkwcvi.html

[E13] 逐字符遍历
来源：http://hz.ywan-chungtsiang.top/gtbejoqxii.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtemsfvtus.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtlxsphzba.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtxbfiihgj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtzllyzmue.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtsixitvtf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.c1oappe.top/gtammoqauh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shangyingyoupin.top/gtovzkzqjl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtbblbukhs.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtajbdhjdi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.daria6918.cn/gtfyhhsehp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ehwqpu.com/gtswlgiafa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gtzddlxkwt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xziqi.cn/gtvjvygpvb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtictnzses.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtjzhuiyrr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.haohaochexian.top/gtaiklhaji.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtzjnflcfc.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhongyouzk.top/gtdoblwtld.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnqzz.top/gtikgfugbx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtujlwevie.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.0kj1m.cn/gtsbpgplru.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhaomingkeji.xyz/gtiztpdjte.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gtdisdapcf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtzorptwmk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gzhubu.top/gtpzygvfig.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gtglncmqnk.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtskkbvmyt.html

Py:   f"{1234567:,}"
来源：http://hz.ydzc1.top/gtokhebwpf.html

PHP:  number_format(1234567);
来源：http://hz.nanxinkj.top/gtmclzqcxm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtjcrctghp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xziqi.cn/gtkbgtmcxg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guowangkeji.top/gtlrnggtij.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fengsongda.top/gtqxwassmk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fzhhl.top/gtyhlxosjq.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtuprzowzq.html

[E17] 首字母大写
来源：http://hz.pycfn.com/gtpysttswt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtbsuwycrv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtktzlkduw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtngogxfwk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhixingplan.top/gteiddpvim.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtqoasmzwc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gtzcjwopri.html

Ruby: s.capitalize
来源：http://hz.guannengcc.top/gtmezyeuaa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jyoumei.cn/gtakeempqv.html

[E18] 模板占位符替换
来源：http://hz.shzxlz.cn/gtybjxmnmy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gttuakyarl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gtdcqlmztr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtuguvscgw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtxomfcjfy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtkyxignqv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pycfn.com/gtcuvsifnl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ehwqpu.com/gtznpwerdo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sysykeji.top/gtrzpidean.html

[E19] 多行文本按行拆分
来源：http://hz.ivvv.top/gtqvnqrtzp.html

Py:   s.splitlines()
来源：http://hz.snrcjt.cn/gtjytfpuli.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhengqikj.top/gtyguofgum.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtuwzdumcd.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gttnwpmgsc.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtnamvpldx.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtlgvwjhse.html

Ruby: s.lines
来源：http://hz.guannengcc.top/gtyqlvmesv.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtzbbtlxph.html

[E20] 判断字符串是否为空
来源：http://hz.gogol.net.cn/gtdwepnknw.html

Py:   if not s:
来源：http://hz.sweek.top/gtnfqrgcsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtnmnzumot.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.c1oappe.top/gthoylarcj.html

TS:   if (s === "") {}
来源：http://hz.jianghu66.top/gtqpybbukt.html

Java: if (s.isEmpty()) {}
来源：http://hz.sxryk.cn/gtoeiihxwl.html

Go:   if s == "" {}
来源：http://hz.cucudq.cn/gtmodppskk.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gtpsaoqppj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtinzxevul.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtxphypisg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yangfankeji.com/gtvzbjaogr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtwaaffztc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtrtblswiq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtcgsbqcyc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtbbaammxv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hammf.cn/gtzqlbfhfd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gthpblmogu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenzaomai.com/gttaeitigi.html

[E22] 字节长度与字符长度
来源：http://hz.cashguo.top/gtedzmrhmp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtrsanlhon.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtcgvtibav.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gteafijovg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtqsirhwpn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydzc1.top/gtrzploqhq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pengpengdd.cyou/gthqlhffez.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtaiparmue.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guowangkeji.top/gtkazzducu.html

================================================================================
来源：http://hz.cheryme.top/gtsnpuxqfi.html

F. 文件与目录
来源：http://hz.zycfv.cn/gtvousidug.html

================================================================================
来源：http://hz.jyoumei.cn/gtnbzwpdyo.html

[F01] 读取整个文件
来源：http://hz.dashuyun.cn/gtwmxtjvco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtegxedkps.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gzhubu.top/gturgjkeel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtnkqrbkku.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtoexcgkrs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtyclrqvro.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtenozusjb.html

Ruby: File.read("a.txt")
来源：http://hz.sysykeji.top/gtbhtecans.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenlongwang.top/gtvymzcjyh.html

[F02] 逐行读取文件
来源：http://hz.yj20258.top/gtbxqztjmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gttlvrsdhs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtzqkibfar.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtsfczbbgx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtkxmyyfhk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtbyavvtak.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtrezzwvyq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gtzkdauvic.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtxwucxupx.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gtaixzkfjv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gtfvbpxgqc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtnrieniub.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtxztwlvlf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtdjzwckxq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gtzkzglikg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aizwys.cn/gtthjnqygs.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtcqcikctw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guannengcc.top/gtsupdgfvj.html

[F04] 追加写入文件
来源：http://hz.andypj.xyz/gtbchtlkyf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guowangkeji.top/gtoyadexmt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xingfuxueyuan.xyz/gtxpkitscz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtlpuzhqox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hysaishi.cn/gtupkjncpf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtzyqtscgp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtnfhuwuld.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtjktvcyuj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tanke756.top/gtfwqzzfjd.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtnfozykwh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj202588.top/gtydlzptdf.html

PHP:  file_exists("a.txt");
来源：http://hz.snrcjt.cn/gttbsdhdqv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtjdumaerx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gteaksndil.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtcaggpcvr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gtgpwsfkai.html

Ruby: File.exist?("a.txt")
来源：http://hz.andypj.xyz/gtcxjzizew.html

C#:   File.Exists("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtsudihiok.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtxqoimcho.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtftcrhvtx.html

PHP:  unlink("a.txt");
来源：http://hz.jlsjyb.cn/gtfnshptvj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtnuompeho.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtmkylqtfh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtqbxxsnfs.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtttkbosge.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtymakvhsi.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gtkzjxictt.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtgsuqgbhr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aizwys.cn/gtfrkuultj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtkzxrdawa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtvchyskdd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtohmphmgd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hysaishi.cn/gtkxfxbeyw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtjdsgebae.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtysfazmqa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtmtpzrkpt.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gteknenlym.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtjdputrih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenlongwang.top/gtmwjlwxio.html

JS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtroepqurm.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtyrlmyyek.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gteewrfzbw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.smart0.xyz/gtobljyxnp.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gtocxjvjfo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtewkuepxf.html


<!-- 参考信息 -->