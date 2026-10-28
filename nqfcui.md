代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtysjyslud.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gtxqyeqage.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tanke756.top/gtwbhwxlnz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtgzqhyhuh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtnzaymqpb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hywenlv.cn/gtlcfdirox.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zdqjudy.top/gtsuhufsvn.html

[D26] 数组转字符串
来源：http://hz.xuetiantiany.cn/gtpkzzuysq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtewfuagln.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gthewlhyga.html

JS:   arr.join(", ")
来源：http://hz.havefunace.top/gtmzsqjmid.html

TS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtnmwefdqa.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gthvvclmjz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.c1oappe.top/gtsfgniclr.html

Ruby: arr.join(", ")
来源：http://hz.gzhubu.top/gtygwmpnui.html

C#:   string.Join(", ", list)
来源：http://hz.hywenlv.cn/gtqycjvfnb.html

================================================================================
来源：http://hz.sxryk.cn/gtqbbaclca.html

E. 字符串处理
来源：http://hz.iojbl.cn/gtrbrtqsub.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfauziehz.html

[E01] 拼接字符串
来源：http://hz.pycfn.com/gtietploog.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gtnuzbagnr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sxryk.cn/gtomdftajq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtfmzexpbq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtpkuttibl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yvedp.cn/gtwfampbni.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtqbixpgia.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yanxiufei.cn/gtpqtyxfgd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.iojbl.cn/gtjsuhybyg.html

[E02] 重复字符串
来源：http://hz.mhx1999.top/gtyrhseibv.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtyexrgxec.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ywan-chungtsiang.top/gtejpiskcw.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtbhdnhsol.html

TS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtyzxolbpq.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gtprkgbpqa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.dianchejie.cn/gtblxuxfcs.html

Ruby: "ab" * 3
来源：http://hz.jyoumei.cn/gttufmstxf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sysykeji.top/gtrdzbldja.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gttkztrgkh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtmtjrotyl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hywenlv.cn/gthsorkagf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gtruxkdogi.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gtzypqgfbs.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtquzfjncy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinghuilouyu.cn/gthxexwifu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtnmcrwulp.html

C#:   s.Substring(1, 3)
来源：http://hz.0kj1m.cn/gtndesjbzx.html

[E04] 查找子串位置
来源：http://hz.hywenlv.cn/gtzdromuft.html

Py:   s.find("x");  s.index("x")
来源：http://hz.52xcode.cn/gtyhnrarhn.html

PHP:  strpos($s, "x");
来源：http://hz.jiagoushi.top/gtvpgajiyd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gthndcuitx.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtmmrqakvp.html

Java: s.indexOf("x")
来源：http://hz.yj20258.top/gtgnepogop.html

Go:   strings.Index(s, "x")
来源：http://hz.hnxiangtu.top/gtsnkkllqa.html

Ruby: s.index("x")
来源：http://hz.yvedp.cn/gttajydebh.html

C#:   s.IndexOf("x")
来源：http://hz.hammf.cn/gtxhdgvikq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtwygabgsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hywenlv.cn/gtsdtbwple.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gtepnjgwku.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtlfewsudt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yanxiufei.cn/gtdvfrzycu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtqqwqtvvr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydjk.org.cn/gtmtfzlqjy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daxiang520.top/gtcorzbapa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhixingplan.top/gtzkosodvn.html

[E06] 替换子串
来源：http://hz.cashguo.top/gtxzkwxxtv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgfzy.top/gtvmhzeolc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigfzy.top/gtndfbbhmr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtqjxoyiut.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtxxlppaxn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtjeofzzws.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuanzx.com/gtrprggpyq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shanyushiyangtech.top/gtedkfauir.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangtech.top/gtoyyuasnr.html

[E07] 按分隔符拆分
来源：http://hz.sweek.top/gtvcmtiyea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtwlkgtbbv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aibaodan.cn/gtjnybbgcx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj20258.top/gtyclmdxdz.html

TS:   s.split(",")
来源：http://hz.quarkkingdee.top/gtpxqmfjpu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gogol.net.cn/gtkttqklul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtedogkcfz.html

Ruby: s.split(",");  s.split
来源：http://hz.yuanzhike.top/gtnscppwmj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.bjfxy.top/gtlpoyaizv.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtimefvhoz.html

Py:   ",".join(items)
来源：http://hz.quarkkingdee.top/gtnuzhjagp.html

PHP:  implode(",", $items);
来源：http://hz.yj202588.top/gttdzuvjxe.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtdxuiscqs.html

TS:   items.join(",")
来源：http://hz.gaohongyu789.top/gtawhfcrxd.html

Java: String.join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtuviwfzub.html

Go:   strings.Join(items, ",")
来源：http://hz.hywenlv.cn/gttkbfzkee.html

Ruby: items.join(",")
来源：http://hz.hammf.cn/gtzcullmnu.html

C#:   string.Join(",", items)
来源：http://hz.jqgufenzy.top/gtspswchka.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtjpkkwkop.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gtshyogrjl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtommtmygk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtmnuuizwn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtqmgigwbj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtgnupswvu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sysykeji.top/gtgajjnlye.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtkmhemglb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangdashe.top/gtwsoxfyjq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cashguo.top/gtaozuvrsy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtisbarbbc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xylfe.cn/gtjgkoosby.html

JS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtblyefuim.html

TS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtbypqogik.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gtjckjfkoi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtcpwfkzvi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydjk.org.cn/gttwkhzugk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.mhx1999.top/gtyrhqvtvn.html

[E11] 反转字符串
来源：http://hz.sweek.top/gtxtzbfhjf.html

Py:   s[::-1]
来源：http://hz.yvedp.cn/gtqlmcievd.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtgosqrmta.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtzwkpuggy.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtglqyiwwi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gtwadtkhgj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtflkaejyt.html

Ruby: s.reverse
来源：http://hz.jinyuanbaomall.cn/gtbcauwlkt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtnzudqbor.html

[E12] 统计某字符出现次数
来源：http://hz.smart0.xyz/gticxtfobv.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtzsauefin.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangtech.top/gtfvrrgboy.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtzrsoglni.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtjkzghcem.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.birdmap.top/gtmfypzjrw.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gthsqqqfdl.html

Ruby: s.count("a")
来源：http://hz.wangshuangyany.cn/gtcssrmzou.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aibaodan.cn/gtcomllujl.html

[E13] 逐字符遍历
来源：http://hz.redwolf501.top/gtmhgyibpt.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtciezykzm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuanzx.com/gtntkfosvo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtpntfqhxj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtefstqimi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtgrdmdcec.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtvdivhpcn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuanzhike.top/gtcurpdcwu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangshuangyany.cn/gtijeqzklt.html

[E14] URL 编码与 Base64
来源：http://hz.zhijiandao.cn/gtvzlpdnps.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtgqfuiagk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtoqhhvfws.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtaueynbgz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gtmauvtkuy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtdfkkkhak.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xingfuxueyuan.xyz/gtburzfycp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gthsqhqqah.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtqyovwdwq.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtvdltvsrz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.iojbl.cn/gtctzarzzd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtjejhczyj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tanke756.top/gtnfwnpzwe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.316326.xyz/gtbvtxiwac.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gtqgmsigcy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtdlhvpxga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dianchejie.cn/gtsytigglm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtvwqvsxsx.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtxbkdoxqk.html

Py:   f"{1234567:,}"
来源：http://hz.mhx1999.top/gttqlkmlzq.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtqeamybld.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtdslnsdyo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gaohongyu789.top/gtqcxgkaim.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhijiandao.cn/gtzlpwprzh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.c1oappe.top/gtipntyalb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xinyue.icu/gtisklesok.html

C#:   1234567.ToString("N0")
来源：http://hz.gotoacloud.top/gtdatghdls.html

[E17] 首字母大写
来源：http://hz.sufxvd.cn/gtdzthhtqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zycfv.cn/gtfmzcvkkq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtztgxlejp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtfedyjxcc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtmpihicks.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.redwolf501.top/gtpmvvorgx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gtjzcxqeuo.html

Ruby: s.capitalize
来源：http://hz.xingfuxueyuan.xyz/gtgjfkoeeg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtapzfhbzr.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtfdiwytzv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtfkpdorgv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ehwqpu.com/gteqjdcabi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtnrjuureo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtbopgcwbg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtnkuhvhwl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gthfhgpsvz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ppjwa.cn/gtoqiozhos.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenlongwang.top/gtsroxsntw.html

[E19] 多行文本按行拆分
来源：http://hz.tianlin.xyz/gtpxxtccpw.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtfuwlrksu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtxtmkmpnc.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gthbqahmab.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtouirmuby.html

Java: s.lines().toList()
来源：http://hz.yvedp.cn/gtlmjtrnii.html

Go:   strings.Split(s, "\n")
来源：http://hz.shangyingyoupin.top/gtlcclphvs.html

Ruby: s.lines
来源：http://hz.ivvv.top/gtswazapio.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gtbwchrtro.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtoonuqltu.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtbpungiup.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258.top/gtunqipoaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ivvv.top/gtzxtevfxk.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtrlaorlac.html

Java: if (s.isEmpty()) {}
来源：http://hz.iojbl.cn/gtecxlytjr.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtypbzkmyn.html

Ruby: if s.empty?
来源：http://hz.zhijiandao.cn/gtqqbgxqpo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigufen.top/gtqrkahjet.html

[E21] 超长截断加省略号
来源：http://hz.wangshuangyany.cn/gtycmcujrj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hywenlv.cn/gtefrbxrfw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtcmamqdzq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtnifayisb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtygeovjzp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gttxpkyfki.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtbdtjvohs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sufxvd.cn/gtdbeofdas.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgfzy.top/gtdfstekpw.html

[E22] 字节长度与字符长度
来源：http://hz.meibo888.top/gtiwmgdtht.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.redwolf501.top/gtczvcmhxa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtyslilung.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtbjudwvfm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtwlxgweza.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtpbiyrlfh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.9152youxi.cn/gtdmawfrkk.html

Ruby: s.bytesize;  s.length
来源：http://hz.bjfxy.top/gtokgbkyid.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtvuyxscfn.html

================================================================================
来源：http://hz.fzhhl.top/gtdyimkmcf.html

F. 文件与目录
来源：http://hz.aibaodan.cn/gtfyfssloi.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtszecrrqw.html

[F01] 读取整个文件
来源：http://hz.smart0.xyz/gttongjuwf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gtyfpuxqya.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtotqvfbfp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dianchejie.cn/gtnniynuyj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.0kj1m.cn/gtxsopihyh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtqghephgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtetoikyyy.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258888.top/gtlxalloxz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gticjjryid.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtbgqdavtx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.kuanghao11.cn/gtbyrhsbom.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtzvndtdpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gthnuzqzzk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtqwescmid.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtmnizcnby.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtrebfrfjx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shangyingyoupin.top/gtzkpazxwk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtyrdyoieb.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gttcaekfxf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtnqajsrjg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.andypj.xyz/gtdwvulvof.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gthjezzlxd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtwtxrvxva.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gtkwxmrjxj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gtggjukazr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtzrzwjbsd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtwydgxmyz.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangkeji.top/gtiwhnpoia.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtojalgprw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gtzcaxussx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gttkzbqxpk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtdrlcvpls.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yangfankeji.com/gtcbtmvskf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cdnleiting.top/gtwxubuwmp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.vqdsnc.cn/gtiwvkblfr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gttbvqfsol.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtadrmtrmi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinyuanbaomall.cn/gtkwmcnlsz.html

PHP:  file_exists("a.txt");
来源：http://hz.wangshuangyany.cn/gtgceoptpp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtmdrkevjc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtdasghrqd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtysrgksoy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenlongwang.top/gtlsfwidbh.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtviwaodvq.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtgirkpsey.html

[F06] 删除文件
来源：http://hz.yuxming.cn/gtkxpeiylo.html

Py:   os.remove("a.txt")
来源：http://hz.chenlongwang.top/gtoenzqfdj.html

PHP:  unlink("a.txt");
来源：http://hz.shangyingyoupin.top/gtbbvmyqhv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtldepitbr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtismyhcgu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtwugwhgvw.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gtooizxkgv.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtlngfkwci.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtjncrcwey.html

[F07] 创建目录（含多级）
来源：http://hz.c1oappe.top/gtlbunniui.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtzdfcumcc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gtedabbuqu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtdeppmydb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtruuuzryw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtiizjxtdw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtjdcqqkxp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yangfankeji.com/gtczcaicys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtdnazsydv.html

[F08] 遍历目录
来源：http://hz.yj202588.top/gtymfnnuce.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtvvsjxsyf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtrhiskyaz.html

JS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtwncqrhrf.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtarjdavoh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtrhdvbqul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxuanxn.top/gtzjebynnd.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gthaifokuw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xinyue.icu/gtqlncqevl.html

[F09] 获取文件大小
来源：http://hz.jinghuilouyu.cn/gtbbmnmukk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtyihyvmsq.html

PHP:  filesize("a.txt");
来源：http://hz.nanxuanxn.top/gtuypybobd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtkrfezvfz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtpzeqrvhe.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtanrgwvnp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhongyouzk.top/gtbprtkpgb.html

Ruby: File.size("a.txt")
来源：http://hz.bjfxy.top/gtcztltlol.html


<!-- 参考信息 -->