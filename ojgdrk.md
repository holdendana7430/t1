代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gthbpezmnw.html

[E03] 截取子串
来源：http://hz.0kj1m.cn/gtbuvsxlfz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtdwhaaevu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxinkj.top/gttovzjjtz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtbohbrqny.html

TS:   s.slice(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtbnvmiycq.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtikkofsef.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gtfpnidwsl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtfrnzddvu.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gtededpaov.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtzdxglzmu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tianlin.xyz/gtpyfrcntr.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtioebtmip.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tian-w.cn/gtqxgbovta.html

TS:   s.indexOf("x")
来源：http://hz.mhx1999.top/gtgshlywek.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtvwkwrcdk.html

Go:   strings.Index(s, "x")
来源：http://hz.yangfankeji.com/gtibmiunon.html

Ruby: s.index("x")
来源：http://hz.dashuyun.cn/gtvtrkxuwi.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gtxucvguwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daria6918.cn/gtfmvdjpuw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.feifeiyinyue.top/gtkeujuydi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yuxming.cn/gtludjktsm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gtavnolboo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fengsongda.top/gtgcagkjgj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuanzx.com/gtkmzdytwl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtditcyoaq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hywenlv.cn/gtfiwywulf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gtkvamesnh.html

[E06] 替换子串
来源：http://hz.xylfe.cn/gtgfclwkrq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtpjebpybf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.smart0.xyz/gttrxoycuo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gttxpyyvzt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtmlkaosjq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtwxepkgdy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dashuyun.cn/gtjsjqyloo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jianghu66.top/gtrgrpnyer.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gtpnjublof.html

[E07] 按分隔符拆分
来源：http://hz.chenzaomai.com/gtkutdsqal.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nwbrower.top/gtufvespyf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shuidangran.top/gtzvpipova.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hongshengwenyu.top/gtamjsovth.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtwvxocied.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tanke756.top/gtzdimzzvv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtlmojpnyw.html

Ruby: s.split(",");  s.split
来源：http://hz.zhengqikj.top/gtqvrmewql.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gtquwxdpcp.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtjmwbyeqy.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gtctpbvgcl.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtipywmvuy.html

JS:   items.join(",")
来源：http://hz.iojbl.cn/gtuhinbpot.html

TS:   items.join(",")
来源：http://hz.yj202588.top/gtmytcubul.html

Java: String.join(",", items)
来源：http://hz.aibaodan.cn/gtzspdjzew.html

Go:   strings.Join(items, ",")
来源：http://hz.vqdsnc.cn/gtmkcaboxk.html

Ruby: items.join(",")
来源：http://hz.birdmap.top/gtxgyultdc.html

C#:   string.Join(",", items)
来源：http://hz.aizwys.cn/gtsvonidxb.html

[E09] 去除所有空白字符
来源：http://hz.zhoulong.xyz/gtljvajivz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tianlin.xyz/gttvmaftjp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yongpay.top/gtuvfpkaeo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtqliqeuld.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtgcccfvjp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.haohaochexian.top/gtslimbwtz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtpmoyxkah.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gthcouqrgx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtvncczdew.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangtech.top/gtpmflhtcb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtkajolzdg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtnfyqllfk.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtqrrxnbfv.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtxeitdiif.html

Java: String.format("%03d", 7)
来源：http://hz.redwolf501.top/gtwibgvojx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shangyingyoupin.top/gthlqpghjq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fzhhl.top/gtxpqtptef.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dianchejie.cn/gtqmbkdyvm.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtdvgvhqoa.html

Py:   s[::-1]
来源：http://hz.wangdashe.top/gtcxzijnng.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtswumtoug.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtsyqgsure.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtlfpmmure.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuanzx.com/gtptiwrsfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtdnsojmav.html

Ruby: s.reverse
来源：http://hz.fengsongda.top/gtkfwvvmbb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtjnhcfmuu.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtyfbyqbxe.html

Py:   s.count("a")
来源：http://hz.0kj1m.cn/gtlfqueugh.html

PHP:  substr_count($s, "a");
来源：http://hz.cheryme.top/gtgxssbpfr.html

JS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gtpwzlvdrl.html

TS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gttmmcseyg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtkkcxcsth.html

Go:   strings.Count(s, "a")
来源：http://hz.hnqzz.top/gthbxfgvfq.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtseaadgij.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ppjwa.cn/gthjbejqgn.html

[E13] 逐字符遍历
来源：http://hz.yj20258.top/gtoosuxlyr.html

Py:   for ch in s: print(ch)
来源：http://hz.jlsjyb.cn/gtambxtpub.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zdqjudy.top/gtglegqvii.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtgnknmntw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtvbiabfgw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtjdcuaukd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtmpsvnhme.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jianghu66.top/gttukvjuht.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.haohaochexian.top/gtrjbjcbvw.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gtdiiqrwqj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gogol.net.cn/gtpdijowyy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtzguhsvco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.316326.xyz/gtjkwvvwiy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuetiantiany.cn/gtpiomtihz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gtskaiyldc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gttwzhbsax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fzhhl.top/gtuwyimxal.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtqgcnxnky.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gtyzmwrudg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gterxeiure.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yueranfly.top/gtmcwrkaqo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenzaomai.com/gtqshkxbad.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gzhubu.top/gtshqdyktx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xinyue.icu/gtaekxbvqe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtycqanqeg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangtech.top/gtfdtzqjup.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sufxvd.cn/gtccpvksjq.html

[E16] 数字千分位
来源：http://hz.yvedp.cn/gtlygmejhk.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtqkyuklot.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtajhexpud.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtonuwlirp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtntglhmxy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuxming.cn/gtaynepcmp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtxixveaik.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daria6918.cn/gtjwhzivhw.html

C#:   1234567.ToString("N0")
来源：http://hz.chenzaomai.com/gtnsbvuiei.html

[E17] 首字母大写
来源：http://hz.xinyue.icu/gtcqchquae.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gtddnyeynj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtuziplypn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gttaldheih.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtmtqlwzys.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gtykvdzrxs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtxkomsjrb.html

Ruby: s.capitalize
来源：http://hz.yangfankeji.com/gtupwhhiro.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtldxqpkqu.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gthcypwrxv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.andypj.xyz/gtffaysnwx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtmxbiybso.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtmautwbjd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtqxsavbss.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtkthqyryv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.andypj.xyz/gtrkhgyveu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhixingplan.top/gtvjnheqzk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj202588.top/gttjykprcx.html

[E19] 多行文本按行拆分
来源：http://hz.jqgfzy.top/gtawnarssc.html

Py:   s.splitlines()
来源：http://hz.xziqi.cn/gtmepydozr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtejkawsmq.html

JS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtwluedkxe.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtyqavhonb.html

Java: s.lines().toList()
来源：http://hz.jqgufenzy.top/gtqplpsnrv.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtpznxnwsp.html

Ruby: s.lines
来源：http://hz.ivvv.top/gttspjoelv.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gtoopaerln.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtcasipwls.html

Py:   if not s:
来源：http://hz.shuidangran.top/gtnpsxliwg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.kuanghao11.cn/gtzbvlvqrq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhongyouzk.top/gtmwxomfcs.html

TS:   if (s === "") {}
来源：http://hz.birdmap.top/gtkocufpne.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtdmupmgag.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtdpdavsfw.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtqrjztake.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gturzkgnwi.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gttpddudfr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtzcfidlcl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtzgibtloe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gthzthgfvi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtfnrqlsfc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtcjdpqimo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtmqgkzhlq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daria6918.cn/gtcqzkrdfv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yonumen.top/gtdmmyvoiw.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtfrwzkdrp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hammf.cn/gtovtlavaf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtrotozlze.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtcslgedxe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtfhchuwlb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtoeotgrqw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtbnvqtmzm.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtmybkntkb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zdqjudy.top/gtqcubdepu.html

================================================================================
来源：http://hz.mhx1999.top/gtesaryjxf.html

F. 文件与目录
来源：http://hz.yj20258888.top/gtxbxxmhhp.html

================================================================================
来源：http://hz.wangdashe.top/gtyvucfdhn.html

[F01] 读取整个文件
来源：http://hz.9152youxi.cn/gtrwujzfqj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtadhfdzdf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtyhiotoox.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gtmdvhdswm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtadmnzuda.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtkmueowoc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.c1oappe.top/gtmwebbeac.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtctcssmmo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guannengcc.top/gtyiedgwpg.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtupylgtxu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gzhubu.top/gtdsbnbuan.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigufen.top/gtjtebrnck.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtumoqpnjm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtzwteunwo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtruiawtap.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gtdpphzbjv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtzxaycavf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gtpuafywqz.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtdtsumhdm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pengpengdd.cyou/gtqmosfufx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtioofvcjb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtcsjiqtym.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtyvbrbqrc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gteicryqnr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hysaishi.cn/gtrgtygqkm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhixingplan.top/gtcdmfyxmi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtochrbhhd.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtsbhpgwwt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gotoacloud.top/gtxfxauifw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gtqvgfmjxs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtnhmxpjzr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtkwysfvia.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gtrppbxyoy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtafgdgnlo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtndkewuhb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtmveaakkz.html

[F05] 判断文件或目录是否存在
来源：http://hz.sxryk.cn/gtkgayscxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtukqqjleh.html

PHP:  file_exists("a.txt");
来源：http://hz.yangfankeji.com/gtwxkxzsvc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtvlojzusa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtacpdacor.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtpqkhjgmu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shangyingyoupin.top/gtbwpzbmsy.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnqzz.top/gtkvwnsmou.html

C#:   File.Exists("a.txt")
来源：http://hz.svipenyu.cn/gtkvnopvdz.html

[F06] 删除文件
来源：http://hz.yongpay.top/gttwxlwpgp.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtvlwbuwsc.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gtrrleohmi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtvptbrvvi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtfcmjevvm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtxiythfni.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtrodpmomy.html

Ruby: File.delete("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtmmjtmjce.html

C#:   File.Delete("a.txt");
来源：http://hz.9152youxi.cn/gtzkjwfioq.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtssgqulgv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtibijosxh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtjyrmezrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtqlisssda.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtfzxcoonv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.svipenyu.cn/gtgwprecdj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtrkeqyvph.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtxpnkqnyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ppjwa.cn/gtxnhtvgoe.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtpndanuyi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtptqlgodo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtqwmzeyza.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtpoqkjeuh.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtjbkcbqkn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtygkxbpup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.andypj.xyz/gtwcphcavr.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gtlpbfqxtu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtpmgbnjxd.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtmkloxxcb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtapfzeykn.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtdaomhcyc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtkynvhuoi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtiqpvigab.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtittrnsea.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gtpsrjxalt.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gthgllvkrl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gtrutwzybk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtsoqckskr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtbsssacpd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnqzz.top/gtmnguejvh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gthfwtbbjj.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtklyroiwc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gthouehdvc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtvbusaegh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtgrhkwaot.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.svipenyu.cn/gtsmvpmvbh.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtgtbkxzxx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtsschmabl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtaeftmvwg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtvmdgkwvd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtxsfjoosv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ywan-chungtsiang.top/gtzvgymkht.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yongpay.top/gtcstqkdga.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtjoyvqkpw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuetiantiany.cn/gtgurzxvzk.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gttyjpoifz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtkpaqcugm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtfbbogkof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtephfyztw.html

TS:   // 同上
来源：http://hz.zycfv.cn/gtatvykwvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtcdlogumn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gtjwbvkmpx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtgfurkmbo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtarngmcdo.html

================================================================================
来源：http://hz.fengsongda.top/gtawdmkijc.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtxixgkrfj.html

================================================================================
来源：http://hz.cdnleiting.top/gtxscyruuo.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtyqmpbymd.html

Py:   class User: pass
来源：http://hz.zhoulong.xyz/gthxaslhjt.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtripjillm.html

JS:   class User {}
来源：http://hz.meibo888.top/gtrbrcwwfl.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangtech.top/gtmymxxfze.html


<!-- 参考信息 -->