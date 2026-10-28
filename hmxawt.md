代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gtyxknkxhe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gtslelfjvn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gtkhabcsxo.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtdcxhmavf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtynhdydow.html

PHP:  implode(", ", $arr);
来源：http://hz.daxiang520.top/gtttjiihik.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtavopblwn.html

TS:   arr.join(", ")
来源：http://hz.sxryk.cn/gtdvajxpmd.html

Java: String.join(", ", list)
来源：http://hz.feifeiyinyue.top/gtxblwikwv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigfzy.top/gtqnxihnep.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtipncwgzt.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtafosotab.html

================================================================================
来源：http://hz.dashuyun.cn/gtupoagpda.html

E. 字符串处理
来源：http://hz.cheryme.top/gtxsnwidha.html

================================================================================
来源：http://hz.yongpay.top/gtawypwkld.html

[E01] 拼接字符串
来源：http://hz.pycfn.com/gtouecyfyw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtkkqzwfsb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtvmsggjcs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtqjgslehb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtigfawvms.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fengsongda.top/gtcjbtewpk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtkyechucw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhaomingkeji.xyz/gtrrotfrga.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigufen.top/gtmukxhpna.html

[E02] 重复字符串
来源：http://hz.52xcode.cn/gtfqmtulnn.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gteguclfmr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.mhx1999.top/gtiolyxaaz.html

JS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtmyakquvm.html

TS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtxzqvxohb.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtqmmlizyk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuetiantiany.cn/gtsgbwjemj.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtdrcachcc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ybcxt.top/gtafxltirx.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtdquvjbja.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgufenzy.top/gtevbjhgoy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gthwdxzcib.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtrslfigyo.html

TS:   s.slice(1, 4)
来源：http://hz.jyoumei.cn/gtdamdgqbe.html

Java: s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gttzcbjltl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.dashuyun.cn/gtxvsgwrmv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jlsjyb.cn/gtyjhdkpmx.html

C#:   s.Substring(1, 3)
来源：http://hz.gotoacloud.top/gthtdjheuy.html

[E04] 查找子串位置
来源：http://hz.havefunace.top/gtlphowlbn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtsufyqtgk.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtspengsbe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtkhpoztke.html

TS:   s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtqquructk.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gtjchnsava.html

Go:   strings.Index(s, "x")
来源：http://hz.jiagoushi.top/gtfpunbrsx.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtkusrikcp.html

C#:   s.IndexOf("x")
来源：http://hz.havefunace.top/gtpuxdztil.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtkyoosevl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shangyingyoupin.top/gtjhislnwm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtazwmsoby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxuanxn.top/gtyapxttty.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtxscggkod.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sxryk.cn/gtzukqbsll.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jlsjyb.cn/gtwhqqzsqa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dianchejie.cn/gtohllnsqh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gtcldqkgbx.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtutmlqdfi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtcslqwpjm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenjidiqi.icu/gtsddooskx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtkatbiaxp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtqdruuxrm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtljlutakq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtycpbtzzs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yongpay.top/gtjgjpzmyk.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtdfdmolxa.html

[E07] 按分隔符拆分
来源：http://hz.52xcode.cn/gtqmxkqznf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daria6918.cn/gtakuajgtd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jiagoushi.top/gtiwweolgh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shangyingyoupin.top/gtgkorpjyh.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtdrtvzwvj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtavkeglmi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fzhhl.top/gtzvgefvwj.html

Ruby: s.split(",");  s.split
来源：http://hz.ppjwa.cn/gtbrrzwizo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.feifeiyinyue.top/gtzbyczvkj.html

[E08] 数组按分隔符合并
来源：http://hz.cdnleiting.top/gtisqqecwg.html

Py:   ",".join(items)
来源：http://hz.zycfv.cn/gtbcsgrkuo.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtgsohbncq.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtounvmdiz.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtamhyssaz.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtujfjykag.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gttulovgpb.html

Ruby: items.join(",")
来源：http://hz.birdmap.top/gtfikqwrzp.html

C#:   string.Join(",", items)
来源：http://hz.daria6918.cn/gtntswguxf.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtkwiapeyj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtowpazmuz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj202588.top/gttxkidaus.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtwoxdttgc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gthlqfsyut.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuanzx.com/gtkvtkbizq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenlongwang.top/gtqezzomsj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtfxurjaes.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtaobsastz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtrshnygwy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yvedp.cn/gtsmngiwgk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.havefunace.top/gtandmjmgm.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtfvmxslun.html

TS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtiulqmbxp.html

Java: String.format("%03d", 7)
来源：http://hz.meibo888.top/gtdooowhrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gtvirxhiba.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhengqikj.top/gtpokyluxr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gthandhnhh.html

[E11] 反转字符串
来源：http://hz.guannengcc.top/gthgpduoeg.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gtwyuccxem.html

PHP:  strrev($s);
来源：http://hz.zdqjudy.top/gtqvekkztd.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gttggoptbx.html

TS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtarvvdgxo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.redwolf501.top/gtneysckru.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cqqwz.cn/gtgmsambql.html

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gtspcgdvgp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtkexyspee.html

[E12] 统计某字符出现次数
来源：http://hz.feifeiyinyue.top/gtmjpuzdnp.html

Py:   s.count("a")
来源：http://hz.yueranfly.top/gtzatuncpx.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258888.top/gtijnjsnay.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtsjvbjvot.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtsjjszbsr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtekihjequ.html

Go:   strings.Count(s, "a")
来源：http://hz.yongpay.top/gttooxtmdy.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtbltaqqax.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hfpthk.cn/gtwunqmzkk.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtskxufawa.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtvsgjjaxo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.kuanghao11.cn/gtbvvwvzof.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtjlaearux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtvlmdgnra.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gtdtrouuxt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.snrcjt.cn/gtyvkguqax.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtdzzopkic.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.snrcjt.cn/gtgkxdwjja.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtznhxqkyi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtpkkripjt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.9152youxi.cn/gtcjpdynyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gtesicbaqu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtiedivxve.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtgsfnudlk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtjqcrulfn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtdtqeoalp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.andypj.xyz/gtrnoxmvln.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtiofncokz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtlfxzeajc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhixingplan.top/gtzgeebzgu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtasqfpnrl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhijiandao.cn/gtlvsetdal.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtfgufqztl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hongshengwenyu.top/gtndldwihz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtqfwwqlur.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.c1oappe.top/gtpvhwbslz.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtwnpsayjb.html

Py:   f"{1234567:,}"
来源：http://hz.gogol.net.cn/gtsozvlspm.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gtpiphhwof.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtxjwohryw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtjdxbaapp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtomvdaegc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtvbsidjzf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hammf.cn/gtiwtrajna.html

C#:   1234567.ToString("N0")
来源：http://hz.jinyuanbaomall.cn/gtmmhhihen.html

[E17] 首字母大写
来源：http://hz.jinghuilouyu.cn/gtnsrivhjc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangkeji.top/gtcocifzbr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtbpbsjwdr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtfqvlvwla.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtjhgmrnry.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hfpthk.cn/gtfdcbyhiy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gaohongyu789.top/gtyjiclken.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtybuidvlx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtpzdbwhch.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gtgukqzbjd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daria6918.cn/gtmacnsimb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dianchejie.cn/gtcexxgdqr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtbavhyhjj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtjjqlougu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jianghu66.top/gtamkntded.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cucudq.cn/gtztvfvuyk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tanke756.top/gtfxrscrql.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgufenzy.top/gtviwflaal.html

[E19] 多行文本按行拆分
来源：http://hz.feifeiyinyue.top/gtpoqdvtid.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtclakhctf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtxipikiuy.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtkujhxpue.html

TS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtmznnshlf.html

Java: s.lines().toList()
来源：http://hz.snrcjt.cn/gthmodsgzt.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangdashe.top/gtovxrqdds.html

Ruby: s.lines
来源：http://hz.gaohongyu789.top/gtypucnayy.html

C#:   s.Split('\n')
来源：http://hz.sufxvd.cn/gtxkazsjrz.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtmkrztoin.html

Py:   if not s:
来源：http://hz.nanxinkj.top/gtmnzxgcsn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yangfankeji.com/gtjsuwyfnx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yongpay.top/gtsaatusuu.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtdahgejes.html

Java: if (s.isEmpty()) {}
来源：http://hz.yvedp.cn/gtcyhszexn.html

Go:   if s == "" {}
来源：http://hz.zhixingplan.top/gtunrxqrgk.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gticbreixq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.snrcjt.cn/gttvetuahr.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangkeji.top/gtcdlviupb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtzqmegicg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtfnukgavl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gteeocpxrk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtfrknhpuz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtkxoomjxz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gtjktbtckr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtmrcvdbcs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtfhtkffoi.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtibjyyrui.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.bjfxy.top/gtqmzvanvu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtpcovjnoz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtquqjxgro.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtegjckmww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gzhubu.top/gtjmzzbjcm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gttomlistz.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuanzhike.top/gtojzwxcah.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtdzwonvzq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrepjcglv.html

F. 文件与目录
来源：http://hz.daria6918.cn/gttoadoace.html

================================================================================
来源：http://hz.yuanzhike.top/gtkfgtoghd.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangtech.top/gtwvgklimz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtzbloalpm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtrgyztlfe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nwbrower.top/gthimudmqq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.haohaochexian.top/gtzvmtfnjl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtvzgoskpj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtslxsnfty.html

Ruby: File.read("a.txt")
来源：http://hz.zhengqikj.top/gtvkrqmcdf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hysaishi.cn/gtlbpzgvyp.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gttjvjxajc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtrjphcgmo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtfjtujktb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtvdaijeis.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtytglpzqn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtbifevvdg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gtlkltrehd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtjifhwwgi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtnejmrhke.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtbscfmwsd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtxlapqnvt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.c1oappe.top/gtfdsfijcg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtdkalagdd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gteycajqfc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtafgrjyhc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtpaxnbirg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cucudq.cn/gtnnuzptgf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtjzdotbew.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtaosovqkn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtxmgrcakv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtiwtldjec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtcguktaib.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtxzdvbaju.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xylfe.cn/gtjwdkwkgi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtpjytwnzf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgufenzy.top/gtupsnbsls.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtfgjoevno.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtxlqwzrcf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dashuyun.cn/gtfmdenbuf.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtrpmjoyiw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gttenzttei.html

TS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gthiittgnj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtyhanawnv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tanke756.top/gthkdycbeb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yvedp.cn/gtpsqwsbav.html

C#:   File.Exists("a.txt")
来源：http://hz.sysykeji.top/gtscpvylnb.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtdrszgcpd.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtgtfzjvag.html

PHP:  unlink("a.txt");
来源：http://hz.shangyingyoupin.top/gtlzamaaop.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gtejxxzcuu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gthyljrgfs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtvhlczbjs.html

Go:   os.Remove("a.txt")
来源：http://hz.smart0.xyz/gteklcndop.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gtroksuzmw.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtbojvbeim.html

[F07] 创建目录（含多级）
来源：http://hz.andypj.xyz/gtdmdquilj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cdnleiting.top/gtjolyhqhw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtbkpyuoro.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtyarrygei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gteeselygo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nwbrower.top/gtvmpntzfx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gotoacloud.top/gtgsaaxxvd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgufenzy.top/gteemjkngh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gturftnnjp.html

[F08] 遍历目录
来源：http://hz.xuetiantiany.cn/gtkccwsqds.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtcbymowua.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gtrfvkuocv.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gteymggypw.html

TS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtzblcmehz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gttwhdtjch.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtownlhbgs.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gtdrfzfzfa.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtqmpzcxpj.html

[F09] 获取文件大小
来源：http://hz.hammf.cn/gtbngxhleg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtpsrgusbm.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtlilfcpne.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtlcscfted.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtcwjamxqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtqybdvalq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gtgaipespc.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtmwzzdims.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gtpsbicwtp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtgomufept.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtwhaaulzi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigfzy.top/gtjvnwsitf.html


<!-- 参考信息 -->