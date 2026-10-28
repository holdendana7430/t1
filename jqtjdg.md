代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigfzy.top/gttlckfymr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtibamzxvd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jlsjyb.cn/gtyfqqcbyp.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtbdftnwmq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gtzjyjqlkm.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtbvhzlstp.html

JS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gthwmeyvyw.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtinuishxw.html

Java: String.join(", ", list)
来源：http://hz.zhongyouzk.top/gtapjcmdnl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yonumen.top/gtxyzfohqn.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtuszibgig.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtpicdueee.html

================================================================================
来源：http://hz.yueranfly.top/gtosfthmbi.html

E. 字符串处理
来源：http://hz.jinghuilouyu.cn/gtsdutwdxj.html

================================================================================
来源：http://hz.0kj1m.cn/gtdptrghcv.html

[E01] 拼接字符串
来源：http://hz.hongshengwenyu.top/gtpathailp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgfzy.top/gtjuudrlyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtvtxcqybl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtcnyyhrnl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtavsbujpo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hongshengwenyu.top/gthsmceoit.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtjuhksvmp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gthysxpdmt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zycfv.cn/gtuvisugua.html

[E02] 重复字符串
来源：http://hz.daria6918.cn/gtepnbjudr.html

Py:   "ab" * 3
来源：http://hz.nanxuanxn.top/gtixnajlvd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtsqikixmn.html

JS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gttrenurkg.html

TS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtprzspqef.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtxbltcpcr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.havefunace.top/gtkuexbdyu.html

Ruby: "ab" * 3
来源：http://hz.yanxiufei.cn/gtmfmbooxf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtfepuxggt.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtkpznhffz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sysykeji.top/gtqmruealh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtbqiufecp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daria6918.cn/gthsavhmfj.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258.top/gtoreqrplj.html

Java: s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtdbrzxsvl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zdqjudy.top/gtueerlycg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sysykeji.top/gtvspuwbpy.html

C#:   s.Substring(1, 3)
来源：http://hz.zhiwuduotai.top/gthgkvziyq.html

[E04] 查找子串位置
来源：http://hz.0kj1m.cn/gtxojltuwj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtrambqrso.html

PHP:  strpos($s, "x");
来源：http://hz.ydzc1.top/gtawdefwgl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jyoumei.cn/gtyofiamtk.html

TS:   s.indexOf("x")
来源：http://hz.9152youxi.cn/gthvliizom.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gthzkdacnk.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtrcclajfl.html

Ruby: s.index("x")
来源：http://hz.pengpengdd.cyou/gtgpvnpbrs.html

C#:   s.IndexOf("x")
来源：http://hz.shzxlz.cn/gtplskwcek.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhiwuduotai.top/gtwiplfkvf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.redwolf501.top/gtdkfbbwep.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yuanzhike.top/gtvbpnvsbu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtcjpbqbge.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yangfankeji.com/gtzpxxtpmx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtfutgzuit.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sufxvd.cn/gttokkjjnj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenjidiqi.icu/gtmihaoebp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtmtvocdpm.html

[E06] 替换子串
来源：http://hz.yvedp.cn/gtziukhftu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tianlin.xyz/gtgchjtrqf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.vqdsnc.cn/gtgyjroitv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtivksbyiz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtmubwcnqh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtmugeuack.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gaohongyu789.top/gtrmecudyk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinghuilouyu.cn/gtvejhbvis.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtnippcsrt.html

[E07] 按分隔符拆分
来源：http://hz.birdmap.top/gttdizmsbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.mhx1999.top/gtqwrokuwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gthxzupely.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtwyybibbo.html

TS:   s.split(",")
来源：http://hz.sysykeji.top/gtaiyxsqvh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.52xcode.cn/gtphtqzxtd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gtdzbyfncc.html

Ruby: s.split(",");  s.split
来源：http://hz.fzhhl.top/gtnnnpcurc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangkeji.top/gtmicgcctn.html

[E08] 数组按分隔符合并
来源：http://hz.quarkkingdee.top/gtsmeofvfv.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gthbllihwg.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtpupcxego.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gteegvnsoy.html

TS:   items.join(",")
来源：http://hz.ppjwa.cn/gtevnkdsql.html

Java: String.join(",", items)
来源：http://hz.cucudq.cn/gtrhqupkxx.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtsexwwdna.html

Ruby: items.join(",")
来源：http://hz.hammf.cn/gtvqleadbu.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gthvtgafwq.html

[E09] 去除所有空白字符
来源：http://hz.chenlongwang.top/gtgvrbrzxa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gtzqnctppz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhiwuduotai.top/gtszacwqvu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtlhaoxqhy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtprznnhcp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gtahfiacsk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.feifeiyinyue.top/gtzbluqcqc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtxlhrgcfd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.0kj1m.cn/gtyomcqixt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.52xcode.cn/gtxcmkcbfy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gtmarvamov.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.kuanghao11.cn/gtoepduywc.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtuvovvwul.html

TS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtczysfwqn.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtfexydfju.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtvkaawkpd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtoiprfxxg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtainksjhx.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtwewwanso.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtbkrvuivs.html

PHP:  strrev($s);
来源：http://hz.haohaochexian.top/gtsdmyofqz.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtrycyzqjr.html

TS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtafeejvmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tanke756.top/gttvcdfzzd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gtkpauitqf.html

Ruby: s.reverse
来源：http://hz.cucudq.cn/gthkdwpula.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtkcdcwoso.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtbzyefvyc.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtwtwszmbs.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtogmlbskj.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtifgprnfw.html

TS:   s.split("a").length - 1
来源：http://hz.cheryme.top/gtommthwko.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.snrcjt.cn/gtgnnbyqeo.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtzkuwtzfz.html

Ruby: s.count("a")
来源：http://hz.zhijiandao.cn/gtebmzlxux.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtgioqlxcy.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtayoddomr.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtloqgmmom.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangkeji.top/gtwbltmupj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtpsseriqk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtvuhxmnkf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtoedpuala.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.316326.xyz/gthbpmyvos.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258888.top/gttoygcvbl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtfuichwhu.html

[E14] URL 编码与 Base64
来源：http://hz.yuanzhike.top/gtummzzsdx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtxrfylyrl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangkeji.top/gtjmeybmtt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hongshengwenyu.top/gtxlromgvh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtlcslpckl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.smart0.xyz/gthziqcxdd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.haohaochexian.top/gtugwcalzv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtyciiihdn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtrjuynswl.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtxlvbggvp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnqzz.top/gtfpynxsal.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtmeflnbzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtfpirsiya.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shangyingyoupin.top/gtivvworrx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtniwelarg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhaomingkeji.xyz/gtgeuaafah.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtfiovkucl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtynwvoghr.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtgvxosqfq.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtedzxzmnz.html

PHP:  number_format(1234567);
来源：http://hz.daria6918.cn/gtcouxnrne.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtsuhaldzx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gttookugrh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnxiangtu.top/gtztjgsevz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtlhucfpso.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.vqdsnc.cn/gtgddnrryj.html

C#:   1234567.ToString("N0")
来源：http://hz.316326.xyz/gttnjtzpwm.html

[E17] 首字母大写
来源：http://hz.jianghu66.top/gtbclssdgx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtwdnjpvtu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtevvpgjll.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtonsvelby.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtqbsmuqse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yvedp.cn/gtragmqmqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtivjsttza.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtgwciadgb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ywan-chungtsiang.top/gtmammtbhs.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtylitreih.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtcwbcvjvc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtvdxfvclj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtrwrpudmi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gtrrmxkabm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtpposamkp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtzyxorpek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.0kj1m.cn/gtsbboodsq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cqqwz.cn/gtymsrttfb.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangkeji.top/gtcmfbqlgz.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gthksgwwjn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtkzrygtnh.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxuanxn.top/gtivjshagm.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtspxgnftl.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtpajnsdpu.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gtnfdvgmjr.html

Ruby: s.lines
来源：http://hz.hammf.cn/gtaqgaxueo.html

C#:   s.Split('\n')
来源：http://hz.sweek.top/gtbyhugrxi.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtpwfibzhp.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtrbeuhsnj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtiplxlixt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gtecdclsta.html

TS:   if (s === "") {}
来源：http://hz.hfpthk.cn/gtdyvxskrx.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtlzlgyqvm.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtldsiqzjg.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtbyhrodor.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bjfxy.top/gtvcuwihnu.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtfslxmwwk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sxryk.cn/gtrimzbqjh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gttzeseuzi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtvdklokfv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtkomgpvlv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtesyvopqf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guannengcc.top/gtjerxupib.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhoulong.xyz/gtchrasqhs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.redwolf501.top/gtjpznykeo.html

[E22] 字节长度与字符长度
来源：http://hz.kuanghao11.cn/gtvxpwwcrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhongyouzk.top/gtyezswiju.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtkvnnkihu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtjbpzbzrq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtxqjcxdza.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtjwdwtloa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.snrcjt.cn/gtgsdxpoxb.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtusdbfhjp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tian-w.cn/gtxudpkvxa.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmgwpwwrb.html

F. 文件与目录
来源：http://hz.fengsongda.top/gtbdhfxrfa.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkenllmvf.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtjcrpbakj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ivvv.top/gtjiiavnwx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtoxjzmict.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtscyzbxuu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gteleyibsy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gthxbxvdpo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gtfpxwcaee.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtighqhpxv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigfzy.top/gtakxjxrfc.html

[F02] 逐行读取文件
来源：http://hz.52xcode.cn/gtvgftmylu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gthreujgxs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtkabnrvct.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gthpulhzyi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtsuwtxbfv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtsqrdiuei.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtvpukbgjc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.quarkkingdee.top/gtboqpnair.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.52xcode.cn/gtvypwfazy.html

[F03] 写入文件（覆盖）
来源：http://hz.wangdashe.top/gtahmfnswv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hywenlv.cn/gtgpntpwqn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtqcfqappj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gtmtqmhgrq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtxthrrbei.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigfzy.top/gtwfnpjszn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtqmlcuxpe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtxmyiekqi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gteozceidx.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtxhgxgeob.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cheryme.top/gtbklbtcfy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtwoedckyn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtuhjoogrv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtvmzwguqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhaomingkeji.xyz/gtmecnbsqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gtdkvowqzl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hywenlv.cn/gtmjgxjfyd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.daria6918.cn/gtjpvidaxk.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhaomingkeji.xyz/gtswbmqjdd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtsryhsynh.html

PHP:  file_exists("a.txt");
来源：http://hz.mhx1999.top/gtvfkqzvlk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtblqnbbmf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtvfboxzas.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtzudzjsrh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtqcntdufa.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtbkwwqzex.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtywxeywsd.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtxymparam.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtotgyeevu.html

PHP:  unlink("a.txt");
来源：http://hz.hnxiangtu.top/gtfbkvneza.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtejivchwm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtxvlgytob.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtrwmnqfip.html

Go:   os.Remove("a.txt")
来源：http://hz.hnxiangtu.top/gtxgcsdocd.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtagyvpkli.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtjuvoffou.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtwkmbyqnh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtoqqtjtsr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gtgxsfubmx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtblnivfvt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtsndvrnxa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shuidangran.top/gtcwmnqbvx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtrakzkjam.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtmgvatmbr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gzhubu.top/gthaieuvvt.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gteofplmwd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtggqvosvj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sxryk.cn/gtocpbkdbo.html

JS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtwzcfihab.html

TS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtpwnzxybr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtdxxockyt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtvxzktraj.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtzdyuhtvi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guowangkeji.top/gtsjepplys.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtcdufyckn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gthhfbtpwl.html

PHP:  filesize("a.txt");
来源：http://hz.meibo888.top/gtgeqetnpa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtdunkxfeq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtblteltly.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtzlujyofi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jyoumei.cn/gtyhuasmgm.html

Ruby: File.size("a.txt")
来源：http://hz.pengpengdd.cyou/gtigqdolbi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtppvtivna.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jlsjyb.cn/gtwviwbdiy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtouaequyi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cashguo.top/gttcdfiqvp.html


<!-- 参考信息 -->