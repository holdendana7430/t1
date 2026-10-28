代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtlmjqhzho.html

[E03] 截取子串
来源：http://hz.zhongyouzk.top/gtsycuisck.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuanzhike.top/gtcyewyuyr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtigxtljqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtzisioxll.html

TS:   s.slice(1, 4)
来源：http://hz.hysaishi.cn/gtyknsvkeu.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtxneyawon.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtueqzweyr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtcvgmeqfb.html

C#:   s.Substring(1, 3)
来源：http://hz.ybcxt.top/gtpgvqutdq.html

[E04] 查找子串位置
来源：http://hz.jiagoushi.top/gtgpczpnrk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtnwpslbpb.html

PHP:  strpos($s, "x");
来源：http://hz.tianlin.xyz/gtujoqoton.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtsetcound.html

TS:   s.indexOf("x")
来源：http://hz.nanxuanxn.top/gttehbiwaa.html

Java: s.indexOf("x")
来源：http://hz.daxiang520.top/gtoqhlxxyz.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtivuasvqr.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtlvusbnua.html

C#:   s.IndexOf("x")
来源：http://hz.zhengqikj.top/gtmnkdlwey.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.meibo888.top/gtvjztijst.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jyoumei.cn/gtgmqvrclr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.vqdsnc.cn/gtmrokzfmq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtbwjurjqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.tianlin.xyz/gtmajvpxrd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtfwqnjykk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigufen.top/gtpfgbpccr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gtpotnqeue.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtaihsnpdh.html

[E06] 替换子串
来源：http://hz.jyoumei.cn/gtxttxvxpl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtxxlyicoz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhixingplan.top/gtcvcxsiyl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtkxwvjobi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtrzfuohue.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtqdnuoprk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtkzfqwkee.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtqjtrzmqg.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gtamfcztbe.html

[E07] 按分隔符拆分
来源：http://hz.havefunace.top/gtpawjqwmt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuanzx.com/gtuzttdizu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.redwolf501.top/gtxmugdlnh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gtnnmfpdet.html

TS:   s.split(",")
来源：http://hz.zdqjudy.top/gticnjhakp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sweek.top/gtdlzgewmp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gaohongyu789.top/gtfskgrdfb.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gttbwqpryl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gogol.net.cn/gtwmbgepqu.html

[E08] 数组按分隔符合并
来源：http://hz.ybcxt.top/gtklrawrti.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtpwqmvqou.html

PHP:  implode(",", $items);
来源：http://hz.pycfn.com/gtaroheczs.html

JS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtuohjdjhc.html

TS:   items.join(",")
来源：http://hz.hnxiangtu.top/gtnkvmgxsu.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtbxhuwlbe.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtdjbnkvrm.html

Ruby: items.join(",")
来源：http://hz.yonumen.top/gttzvokfrj.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gtujpzoouy.html

[E09] 去除所有空白字符
来源：http://hz.svipenyu.cn/gtenvrmmyy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xingfuxueyuan.xyz/gtjvkgelql.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigfzy.top/gtmhwyxgma.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtagvzanft.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtiknnzulp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gtdhoydcbl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.redwolf501.top/gtabosisdj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhaomingkeji.xyz/gtcjczftsy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.birdmap.top/gtczqfhvvc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nwbrower.top/gtestmwbjz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtgbmdwcdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtjeyuvdjj.html

JS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtwtibxunc.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtaxniwbgn.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtcrzsiuyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yangfankeji.com/gtwzzzzebr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zdqjudy.top/gtblaugril.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtcnlrvpzm.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtgihrkhxv.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtzgoyarbl.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gttvgosuls.html

JS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtptvofsah.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtvmxnizjq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhengqikj.top/gtaocztlrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtucauvvno.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtzvmophup.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtiamrvbgl.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtaqnvjbtt.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtecidwdrp.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtbegzalqd.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gttuhzvuxt.html

TS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtktxacpuj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.0kj1m.cn/gtgjkstjhz.html

Go:   strings.Count(s, "a")
来源：http://hz.vqdsnc.cn/gtmckemaak.html

Ruby: s.count("a")
来源：http://hz.aibaodan.cn/gtuupomkye.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtzwfdhwgc.html

[E13] 逐字符遍历
来源：http://hz.zhixingplan.top/gtcofmlafq.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtnvreelnm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenjidiqi.icu/gtdnzslcgk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtwwlueyqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtonhnpkdy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtrsovoqmf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtvbxnwrmb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gtlvutxpqz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtriyrrxvt.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtivegfxik.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gtfgzyscuz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gtzbekxbnm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gtybdkbzen.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtwecxjqfi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtygflkqtr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhongyouzk.top/gtiqnwufgw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pycfn.com/gttwtvkzmo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenlongwang.top/gtigrmjbgt.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtnynyoyhv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.birdmap.top/gtjtkymduk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pycfn.com/gtbrqxzttn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtctoemiih.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shzxlz.cn/gtenpemkqd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenjidiqi.icu/gtctplwnja.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hysaishi.cn/gtixilizet.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtjzinisjc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yongpay.top/gtikwelvwh.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gttysbqnnk.html

Py:   f"{1234567:,}"
来源：http://hz.cdnleiting.top/gtqgbpkbbq.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangkeji.top/gtyfgyvjsb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtyjqzxnrv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtjpkygmwd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtqjddaejm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtytyfgchf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtxiahijcw.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtyqayytnt.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtqqjacvdi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xylfe.cn/gtrvkelxbu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtjvpsqjeh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtaswznsgm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtgybbfhxl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtkzqxhmtp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtupagkjlp.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gtllvqxxtk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cheryme.top/gtsjlcfcbe.html

[E18] 模板占位符替换
来源：http://hz.zhoulong.xyz/gtqcejmcsh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxuanxn.top/gtelwbmdyi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gttojgrkfp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gthxsztptj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtzscxyqgs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gthrskmvtp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gtjitimfht.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jianghu66.top/gtzrifauts.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtznrwfzxt.html

[E19] 多行文本按行拆分
来源：http://hz.ydzc1.top/gtddgektqu.html

Py:   s.splitlines()
来源：http://hz.zhaomingkeji.xyz/gtmqkxrudw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.meibo888.top/gtkkxgplns.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtbdihpkyp.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtthghiwso.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gtfwqnxpco.html

Go:   strings.Split(s, "\n")
来源：http://hz.yangfankeji.com/gtcvlmuopd.html

Ruby: s.lines
来源：http://hz.gzhubu.top/gtctvrnnfi.html

C#:   s.Split('\n')
来源：http://hz.chenlongwang.top/gtwlfiabnw.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtkasgeufd.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtnukmnxke.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jianghu66.top/gtxrwxfvjv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtltgldvmx.html

TS:   if (s === "") {}
来源：http://hz.nanxinkj.top/gtpwmiycdl.html

Java: if (s.isEmpty()) {}
来源：http://hz.gzhubu.top/gtzltctcrm.html

Go:   if s == "" {}
来源：http://hz.zhoulong.xyz/gtkwbqjkad.html

Ruby: if s.empty?
来源：http://hz.havefunace.top/gttyaikxqq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jianghu66.top/gtythaevvl.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtmawsaxxk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fengsongda.top/gtfawcqgze.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhiwuduotai.top/gtnocoetpn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtackqvoho.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gteiuppbie.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtemomgykk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtgyrtjwep.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtyyhnpjiq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtzattpcsc.html

[E22] 字节长度与字符长度
来源：http://hz.guowangkeji.top/gturexfsxg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtndbsztuf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtaepwumqs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gtxlmnfghv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtvuxpbmrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gttzzrbipg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dianchejie.cn/gtkiyfkcmn.html

Ruby: s.bytesize;  s.length
来源：http://hz.yanxiufei.cn/gtbdojbnsl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gthqigxerq.html

================================================================================
来源：http://hz.chenlongwang.top/gtzqvyctnm.html

F. 文件与目录
来源：http://hz.chenlongwang.top/gtrbbcajxb.html

================================================================================
来源：http://hz.52xcode.cn/gtikuftsta.html

[F01] 读取整个文件
来源：http://hz.yanxiufei.cn/gtlxduyrzi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jianghu66.top/gtldchzjjq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.vqdsnc.cn/gtoslplroe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gtjewizivx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yangfankeji.com/gtrtedxjnj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtxnjpdknv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtechbujhg.html

Ruby: File.read("a.txt")
来源：http://hz.pengpengdd.cyou/gtcnkfmxwi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yangfankeji.com/gtcguyshne.html

[F02] 逐行读取文件
来源：http://hz.guowangkeji.top/gtjmrdtnwx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gotoacloud.top/gtresulqvi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtxmoarpbc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtcaxkjdhu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtnmnavtjw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtodykpkox.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtvzazyuta.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gtgpwyxqvz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ywan-chungtsiang.top/gtxufoudow.html

[F03] 写入文件（覆盖）
来源：http://hz.jyoumei.cn/gtjjtmrnts.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtvmdgfigs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtyuwjxpbn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gturgyrulk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtntnxqxpj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj20258.top/gtbotrtcbq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtfqpnlcml.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sufxvd.cn/gtfymttxat.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtkjmmgmul.html

[F04] 追加写入文件
来源：http://hz.tanke756.top/gtghdgxyqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtjmetwhrt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gttccqegzj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gthimoezsr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtvjnqsiae.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtusxmdqvd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtrxltjsip.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gthjmurzaj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtgzjpujbp.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gtenuukkzp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangdashe.top/gtgorrjoij.html

PHP:  file_exists("a.txt");
来源：http://hz.sxryk.cn/gtrqqtpqix.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtzosjweqn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtrelukuvi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtdknjnuuv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtyrrqkdct.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtavdfvpdv.html

C#:   File.Exists("a.txt")
来源：http://hz.andypj.xyz/gtynbndaov.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtugwkpcmf.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtstluglyv.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtjraekstc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gttipbissi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtojhpyrho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtyhbbpukt.html

Go:   os.Remove("a.txt")
来源：http://hz.smart0.xyz/gtoouepkij.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtsqroqpme.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtlwlorgyu.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtusrloeny.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zycfv.cn/gtnfpsomth.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xingfuxueyuan.xyz/gtmqynelpe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtvefycqyw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtrobjpezd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtuxldfpta.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gtfglymnuw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gtuqyoyfcn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtkxtmyfec.html

[F08] 遍历目录
来源：http://hz.cqqwz.cn/gtfftvxzxe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtsbhfrwsb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gtkpscrpfn.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtgpxasvbz.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtuleshoyp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtbqsgizki.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gtbutjlxtd.html

Ruby: Dir.children("dir")
来源：http://hz.cdnleiting.top/gteurdvlbd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtnnyqufbr.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtwruivnil.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtxwosiavl.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gtijlbwhix.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtxhumbuhj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtrwixpyvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gttdxkgvok.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtwfeupwrr.html

Ruby: File.size("a.txt")
来源：http://hz.vqdsnc.cn/gtaswjxpjq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.9152youxi.cn/gtjxchfmqu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cdnleiting.top/gtsypsawaf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtivzqitea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dashuyun.cn/gtqordbcwv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtjidpzkes.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtgmtljxxd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cqqwz.cn/gtrswaitqg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtdonvzqph.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtvfhfkuqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtfvymcrsa.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtznhehost.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtsbnbrzjm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtfddruujd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtgsjtzluw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtlaohvdwr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shzxlz.cn/gtxwsudurx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtsspiajmi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gthytclpyn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtbdhpznos.html

[F12] CSV 读写
来源：http://hz.9152youxi.cn/gtgoxmozlp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtkotqgcgl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtnkgckdpx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinyuanbaomall.cn/gtwckjyhnq.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gthnujytxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtytnbpqhd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.havefunace.top/gtpdwiqjtc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtnzctffxi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtaexwickx.html

================================================================================
来源：http://hz.tanke756.top/gtzmkwhgld.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtoytqhdlu.html

================================================================================
来源：http://hz.birdmap.top/gtxvsonaiq.html

[G01] 定义类
来源：http://hz.jyoumei.cn/gtubkxcxoo.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtwjjhfcri.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtjawsbfac.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtmdvrjdfw.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtmlbpzkav.html


<!-- 参考信息 -->