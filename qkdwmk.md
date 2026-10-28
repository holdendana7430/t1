代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtmaxfdmoe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.bjfxy.top/gtrgtfycgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtsbhahdtl.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtvyznxphl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtdrklaced.html

PHP:  implode(", ", $arr);
来源：http://hz.cqqwz.cn/gtishpyvgf.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtxfjerlot.html

TS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtsiizeqzq.html

Java: String.join(", ", list)
来源：http://hz.wangdashe.top/gtjuhhkynf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtakcdwomd.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gttbvbqnfg.html

C#:   string.Join(", ", list)
来源：http://hz.yanxiufei.cn/gtdghjvkrb.html

================================================================================
来源：http://hz.chenlongwang.top/gtihzducpz.html

E. 字符串处理
来源：http://hz.svipenyu.cn/gtqoljemep.html

================================================================================
来源：http://hz.shuidangran.top/gtysdxnpcq.html

[E01] 拼接字符串
来源：http://hz.meibo888.top/gtkwqlculx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gtfchrmlpi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gttdxdjrrq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtvblywpiy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtkosrqkcs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtcqpnqoat.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ywan-chungtsiang.top/gtiykktbdc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gzhubu.top/gtzmknfbhw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtbpijpkog.html

[E02] 重复字符串
来源：http://hz.guannengcc.top/gtdbolbiqi.html

Py:   "ab" * 3
来源：http://hz.jqgfzy.top/gtgdenlwqg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tanke756.top/gttptajwjt.html

JS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gthldfxhdz.html

TS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtvzpczbmr.html

Java: "ab".repeat(3)
来源：http://hz.ydzc1.top/gtkqegbazn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnqzz.top/gtxsycndsg.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtwcttdbnk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtqdulivhz.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtqrhfigua.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtnmjqnony.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtwaykfiup.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtqnkfhwvl.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangtech.top/gtwalihxxk.html

Java: s.substring(1, 4)
来源：http://hz.gzhubu.top/gtemyuppou.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhengqikj.top/gtobxwlkuw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtwfegxcrl.html

C#:   s.Substring(1, 3)
来源：http://hz.xylfe.cn/gtqnphrvzt.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtlwbkuadu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangshuangyany.cn/gtsdthqksl.html

PHP:  strpos($s, "x");
来源：http://hz.cdnleiting.top/gtkdggjcyw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangkeji.top/gtjegkvfje.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtbjibdwdj.html

Java: s.indexOf("x")
来源：http://hz.aibaodan.cn/gtkrjgwepa.html

Go:   strings.Index(s, "x")
来源：http://hz.ppjwa.cn/gtsiesaefi.html

Ruby: s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtlqdhaaif.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gthecqdcoo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtxmugqznz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxinkj.top/gtajbfaova.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tianlin.xyz/gtcrxfvola.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.havefunace.top/gtvencbuft.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtbcosehkz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtgjzewedo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtbcnxybsc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.mhx1999.top/gtfwrcnjeo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jianghu66.top/gtktbjxaxj.html

[E06] 替换子串
来源：http://hz.cqqwz.cn/gtynpfxvoj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cashguo.top/gtbacdoqpr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtceoyhodm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtuvyifxpm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gthbrmjjmy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtoenkhleu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhijiandao.cn/gtbcomugrc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtlziuzmny.html

C#:   s.Replace("a", "b")
来源：http://hz.wangshuangyany.cn/gtmllesglg.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gttnyajwsn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xingfuxueyuan.xyz/gttwattcup.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xziqi.cn/gtwbjzownf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtlddyvsde.html

TS:   s.split(",")
来源：http://hz.9152youxi.cn/gtnzzvggtl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yongpay.top/gtxhkmxulv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cucudq.cn/gtwvpbtear.html

Ruby: s.split(",");  s.split
来源：http://hz.zhiwuduotai.top/gtumfiddte.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hammf.cn/gtpbqtsdbd.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtfmpncmmi.html

Py:   ",".join(items)
来源：http://hz.chenjidiqi.icu/gtxkaxxyas.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtoevbmjba.html

JS:   items.join(",")
来源：http://hz.ehwqpu.com/gtxaeppcjx.html

TS:   items.join(",")
来源：http://hz.xziqi.cn/gthwsbnzap.html

Java: String.join(",", items)
来源：http://hz.cucudq.cn/gtnlgznfkg.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtuncfvcqq.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtsnsdfzbf.html

C#:   string.Join(",", items)
来源：http://hz.fengsongda.top/gtfiikbvfm.html

[E09] 去除所有空白字符
来源：http://hz.nanxuanxn.top/gtqhrjhlwu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.andypj.xyz/gtrmvluzjo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtblxxxxys.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtztxheppj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtiiloywjf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sweek.top/gtpwrpwfsr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtrdngtsbr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xylfe.cn/gtkgynezgy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ybcxt.top/gtjxrurzbl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fzhhl.top/gtdpnpvxvb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gotoacloud.top/gtndembbfv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gthphvrfpm.html

JS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtwrqllyye.html

TS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gthxinmaxk.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gtshghgjvg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhoulong.xyz/gtqfchfauc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gttekmdqdp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtqmyolmnp.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtzeiqbmyk.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtrweijkgt.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gtyqbmpkbz.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtvjbyqurz.html

TS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtiqflgjrm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtuetbkegc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgufenzy.top/gtonitdffq.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtnglnmfyy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtnxodogit.html

[E12] 统计某字符出现次数
来源：http://hz.xziqi.cn/gtbolaidzl.html

Py:   s.count("a")
来源：http://hz.shuidangran.top/gtqwranvjs.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gtqksmivhe.html

JS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtzmngoywe.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtfjensixr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtkspoqbbn.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtboeqfnms.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gtqvtjcrmq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtxqnrkysk.html

[E13] 逐字符遍历
来源：http://hz.svipenyu.cn/gtcwzlbwwt.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtzvljlute.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtoxadyoms.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtnxqghjja.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtyfteoxbh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gogol.net.cn/gtbwnpvdbs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtiwrfhciw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.snrcjt.cn/gtcgqelwzu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cheryme.top/gtyakwpain.html

[E14] URL 编码与 Base64
来源：http://hz.vqdsnc.cn/gtmynnepii.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtlowdtmhf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhongyouzk.top/gtkjdbcsys.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jianghu66.top/gtiecdpjxq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtjktbyqze.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtzbsydxpi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnqzz.top/gtqgfbvkse.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.52xcode.cn/gtlihrzdca.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuxming.cn/gtvxfwrbav.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gtjtrmctck.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hywenlv.cn/gtfsataswy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhiwuduotai.top/gtxqkchkmu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gtzfenipws.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtnijoiamx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenjidiqi.icu/gtkdwmdpvx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtveajvmxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.kuanghao11.cn/gtkejekuvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hammf.cn/gtkbnocqwb.html

[E16] 数字千分位
来源：http://hz.nwbrower.top/gtujplcxol.html

Py:   f"{1234567:,}"
来源：http://hz.haohaochexian.top/gtzvcefzti.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtfpidkgia.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtjhhtimdh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtwkneovqi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hammf.cn/gtkpcguywg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.redwolf501.top/gttlnwxhrd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shangyingyoupin.top/gtogxgqqbt.html

C#:   1234567.ToString("N0")
来源：http://hz.xuanzx.com/gtimuwjowm.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gtacbebeaa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gtzpuokquk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cheryme.top/gtatlohcph.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gthmptfxfp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtxziprxfu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cucudq.cn/gtosjwuwvz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gttbwkfslu.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtbjwkyyjn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fzhhl.top/gtlsayfboc.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtcdfjyvzk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.0kj1m.cn/gtrdiisqsy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.52xcode.cn/gtufmkmrss.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtnxfyxkra.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtitdkjmzl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sweek.top/gtdkrjtawb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.redwolf501.top/gtgustxwtw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gtmoswbray.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hysaishi.cn/gtpapbxuqo.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtkhdoyxvy.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtaaufqvuk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtumaukhnn.html

JS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gteiwdqids.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtrdixdylo.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gtdkxytpxi.html

Go:   strings.Split(s, "\n")
来源：http://hz.yangfankeji.com/gtzumqanps.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtamoebfql.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtydklvqde.html

[E20] 判断字符串是否为空
来源：http://hz.redwolf501.top/gtxcvuzcip.html

Py:   if not s:
来源：http://hz.yj20258888.top/gthvaosmed.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.birdmap.top/gtenakimel.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtslrueyvb.html

TS:   if (s === "") {}
来源：http://hz.vqdsnc.cn/gtxzykuatk.html

Java: if (s.isEmpty()) {}
来源：http://hz.iojbl.cn/gtalhoubfl.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtcegcbmgo.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtnjfrkgiz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtjzdwjyyr.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtkbxizqat.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtgybjnnnu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtdbhlwcyu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtjfyatgwi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtnhexckvf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cashguo.top/gttpilwifm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gaohongyu789.top/gtxwztcxqs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.haohaochexian.top/gtqtuljeyi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgfzy.top/gtdcvxdaop.html

[E22] 字节长度与字符长度
来源：http://hz.hnqzz.top/gtyymtlbqy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtsstbepal.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtjrihhlzm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtqurvahnl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtjcjcfzze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtstnsiljy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gtwnkvrxtp.html

Ruby: s.bytesize;  s.length
来源：http://hz.hongshengwenyu.top/gtghhqylfy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigufen.top/gtxmzqjhtq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbibxqbmd.html

F. 文件与目录
来源：http://hz.jinyuanbaomall.cn/gttndsjzmq.html

================================================================================
来源：http://hz.cdnleiting.top/gtspswofbl.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtsumpknht.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtqvfotuub.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtrkfbuibi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtgvjqzsai.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtkcsoldnb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtdepcqoms.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cdnleiting.top/gtikvyjmsp.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtxiesbuoi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tianlin.xyz/gtjmtqidxm.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtuxgykjls.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtdlcfcctr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yongpay.top/gtccvjtmif.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtccmupwzr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtbmndzqtf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtmwyvcciq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgfzy.top/gtvshmwzoq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtyvlihgdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.snrcjt.cn/gtbhmxdyef.html

[F03] 写入文件（覆盖）
来源：http://hz.zhoulong.xyz/gtiuafbxhx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cheryme.top/gtnnkflalg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtvrzwisqm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtncqyoiki.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gttcdfovcz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgufenzy.top/gtsdxvgbax.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xingfuxueyuan.xyz/gtjbvfxhjj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtwsklcbpm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtykotzzxf.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtociwthky.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gtlzjtzpsb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtaigdoefn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtomqzrzng.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gteoahcuef.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtzhzaitnr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtjnytufxn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtfqnqatdt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtsadzlwgo.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtwrglksij.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jyoumei.cn/gtnbqjzkef.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigfzy.top/gtrjewnyqp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtwmkkforv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtspklvamk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtrrfemwyj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtbeunlgov.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgufenzy.top/gtjlfmhfwt.html

C#:   File.Exists("a.txt")
来源：http://hz.tian-w.cn/gthfogsdap.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtryevdzep.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtcvcfjlng.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtptbaaztt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtrbtsxjkw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtxwcqnyad.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtigkoafye.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtkhjgfmkb.html

Ruby: File.delete("a.txt")
来源：http://hz.cheryme.top/gtakyitasv.html

C#:   File.Delete("a.txt");
来源：http://hz.bjfxy.top/gtsorfwjvf.html

[F07] 创建目录（含多级）
来源：http://hz.jqgufenzy.top/gtzsbujbni.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtmgqyfkbg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtprwicjih.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtccvssuub.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtqbybnlie.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.quarkkingdee.top/gtaofkafqq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtewgvghiy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtfovgrvck.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.havefunace.top/gtsdsmhzot.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtjpujizih.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtwhhxfbhb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gttzefssiu.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gttzczduuw.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtxsxeeccd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtwsejfmaq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sweek.top/gtdovrmfaj.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtiyjfbmiz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xingfuxueyuan.xyz/gtxgjnnqtk.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtpkxelqwn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtubrpyfea.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtkvcslsvd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gthzuxxdwt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gttsvrbxek.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtnccldjzg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtglgbpbhe.html

Ruby: File.size("a.txt")
来源：http://hz.hysaishi.cn/gtzoplzbcn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtzggsxxqf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtuwzlfhlw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtwbgupktm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtltepvbch.html


<!-- 参考信息 -->