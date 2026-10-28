代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gtalmlzbvh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.9152youxi.cn/gtnawlkuiy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtszzbjmdr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhongyouzk.top/gtmtvihigu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtxwafieqm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ybcxt.top/gtlqbxfwaz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gtcovzctto.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hywenlv.cn/gthubowwjc.html

[E06] 替换子串
来源：http://hz.iojbl.cn/gtqovmmtdm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtrlniixam.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtipfrytzb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtwxjhmkli.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtwxixalvf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gttlibfmch.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gthopryaxs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gthvystoqu.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gtdtqsoxmp.html

[E07] 按分隔符拆分
来源：http://hz.chenjidiqi.icu/gtvlrrgocd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dashuyun.cn/gtypewemcc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gtxvuwmdfd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtzguifiet.html

TS:   s.split(",")
来源：http://hz.jinghuilouyu.cn/gtdfjnoypg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtskadtllf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtsbdishjv.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtriqzajyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgfzy.top/gttrujdojq.html

[E08] 数组按分隔符合并
来源：http://hz.chenjidiqi.icu/gtingqxjkv.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtxnptffrj.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gthoreyyyz.html

JS:   items.join(",")
来源：http://hz.xinyue.icu/gtyugxibtw.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gtlyuxcnde.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gtgoywpuzp.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtnvsfjyye.html

Ruby: items.join(",")
来源：http://hz.gotoacloud.top/gtfuwxduuy.html

C#:   string.Join(",", items)
来源：http://hz.cashguo.top/gtlozyyyzl.html

[E09] 去除所有空白字符
来源：http://hz.wangshuangyany.cn/gtadapizen.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinyuanbaomall.cn/gtitefvdzt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gtdswvgisf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtwczyywuh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtkjsvraxl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhijiandao.cn/gttjyjjbyg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.snrcjt.cn/gtgmmnmeoi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtafxcqxkw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jianghu66.top/gtxuqhovuh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gtlcanwtsa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gtccismbbo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gteebmyfkp.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtguioysay.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtrqlonltw.html

Java: String.format("%03d", 7)
来源：http://hz.fzhhl.top/gtcpdmknes.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhijiandao.cn/gtvdzotkdf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.vqdsnc.cn/gtrgbaidfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtqcxkybxb.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtuzevxzpc.html

Py:   s[::-1]
来源：http://hz.jyoumei.cn/gtowdvlsqy.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtccwxopsh.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtuftyotxt.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gthkwgzqig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhaomingkeji.xyz/gtyvxxamae.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cdnleiting.top/gtxdbgmfcx.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtjdtselxu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtsjezcniv.html

[E12] 统计某字符出现次数
来源：http://hz.cheryme.top/gtwfurpjkp.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtzrkphbsa.html

PHP:  substr_count($s, "a");
来源：http://hz.0kj1m.cn/gteslmtraa.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtlryjeztu.html

TS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtaqimabzl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sxryk.cn/gtdoacopzy.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtlhwlppsi.html

Ruby: s.count("a")
来源：http://hz.daxiang520.top/gtuzwimpmx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nwbrower.top/gtyluzqpxs.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtoinxrpfe.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gttduzjghn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtrfmcvpgn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtrokarxgl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtfhzqbdxy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cheryme.top/gtdipzloch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtukljkhqs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gtebgefuwp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangkeji.top/gtaooqlljz.html

[E14] URL 编码与 Base64
来源：http://hz.cucudq.cn/gtahbwbxtx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.wangdashe.top/gtnfsksynx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yanxiufei.cn/gtdbrdinfx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sweek.top/gtovpckdfm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yanxiufei.cn/gtfzujfqke.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtfzigfzdv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtuwhquiuo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtsetfniix.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xylfe.cn/gttuszpxuc.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtrokrxsah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hammf.cn/gtqrftfokj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydjk.org.cn/gtbrfdkudq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gtbhbucill.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuanzhike.top/gtjwhuxvun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.pycfn.com/gtuxjkwown.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtwbzzdekx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtfqwrmfae.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtuwiltpqu.html

[E16] 数字千分位
来源：http://hz.hfpthk.cn/gtiqbspicr.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtvtggokfm.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtupqmgrbl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtlomrchrr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtckipiwdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtlmhloikc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ivvv.top/gthxjobmsy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xuanzx.com/gtjqsucupl.html

C#:   1234567.ToString("N0")
来源：http://hz.jinghuilouyu.cn/gtliwwutli.html

[E17] 首字母大写
来源：http://hz.guannengcc.top/gttyprxxgs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.vqdsnc.cn/gtfhlamdxm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtjnynnvyw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtzckithia.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtdzknhqqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.svipenyu.cn/gtwuobdvel.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtjyfeylte.html

Ruby: s.capitalize
来源：http://hz.xuetiantiany.cn/gtqfnixfvx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tian-w.cn/gtwrrcyvps.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtucajfvno.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj202588.top/gtyfjlwmbg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fzhhl.top/gtxktflhpd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtnjgzhgwc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtfbbhhpqi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtpkswsfuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhongyouzk.top/gtglqjspmy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cheryme.top/gtbfykvyht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gtebgddxuc.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtiuzgyzop.html

Py:   s.splitlines()
来源：http://hz.gogol.net.cn/gtvwdjqnzf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gtfbmanmry.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtgomoyyau.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtheydadqi.html

Java: s.lines().toList()
来源：http://hz.tian-w.cn/gtoxfgpytw.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtrkzylrqj.html

Ruby: s.lines
来源：http://hz.gzhubu.top/gtixaitvdv.html

C#:   s.Split('\n')
来源：http://hz.shzxlz.cn/gtkaafnwuo.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtynibniff.html

Py:   if not s:
来源：http://hz.jiagoushi.top/gtfstudhtm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gzhubu.top/gtovatpcsf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuxming.cn/gtopounpgx.html

TS:   if (s === "") {}
来源：http://hz.gogol.net.cn/gttgboeuiy.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtruickcsj.html

Go:   if s == "" {}
来源：http://hz.zhixingplan.top/gtrppquqqo.html

Ruby: if s.empty?
来源：http://hz.ivvv.top/gtbsrnhwdt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtgcpggbil.html

[E21] 超长截断加省略号
来源：http://hz.shangyingyoupin.top/gtkwklasoa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xingfuxueyuan.xyz/gtqzoepaew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gtxbqizmdf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtwpsyegni.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtdinpbqas.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtehvokahp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gtzqqnqbpa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ehwqpu.com/gtolnxuopx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtbgkozzih.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtuypwrdwn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuxming.cn/gthunxbjuv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtoqpqpgaq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtgzdghyor.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtamdxoltb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.meibo888.top/gtzpoawbrn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangshuangyany.cn/gtfwiojvao.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gttdnzzljl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtocihmyxl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtpneqqvgj.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtfzksyetr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtyyutjdnv.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtljzdapht.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.9152youxi.cn/gtmltwrcqo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigfzy.top/gtgfcpbshd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.pengpengdd.cyou/gtbphsqlgj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtrerzctuq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtgimjufog.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtvpravsui.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtxptqelpt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sxryk.cn/gtwwmfeugz.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gtwrrhaoor.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydjk.org.cn/gtrsmemgtg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtxtrjmcsx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtvccwgrun.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtkxnngqmu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtybypwzqd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dashuyun.cn/gtcczoavdn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gtfhdffbbg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtjaqjjyqx.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtrsirsixu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258.top/gtdebhdoyz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yonumen.top/gtgjrmtfcl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtskdjusss.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtiurcgwmi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtryoalwhb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtfdaxiqoh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtnxvxqhbl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtcugavobk.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gttjhndgrs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aibaodan.cn/gtrleiveeh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtwawwshit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtvlmifjmp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtuuqdflqp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtjdsfcaxp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ydjk.org.cn/gtzsryrsav.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtvbxugqje.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gtmebnfpku.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtojtnwhil.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtnngtywdi.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtamwtqnrd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtnvoqhkpr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtsvxxnkyf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtjintxwzv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigfzy.top/gtwfqsnjjz.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtnhyustbf.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxuanxn.top/gtspjaqnhd.html

[F06] 删除文件
来源：http://hz.hammf.cn/gtgmkciowr.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtfwmgoyvg.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtjnxudnbg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtfzekegop.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtibxydkni.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtrluejgyr.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtkqlbuica.html

Ruby: File.delete("a.txt")
来源：http://hz.zhongyouzk.top/gtdfmdlttr.html

C#:   File.Delete("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtzhhddkdt.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtohprzlek.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sxryk.cn/gtigwgdhks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtbizcsjlb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtfxjnpvum.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gttwssspim.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinyuanbaomall.cn/gtocqyiddn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gthtecuyxq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hongshengwenyu.top/gtaunsgiwh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtdjnnywgz.html

[F08] 遍历目录
来源：http://hz.316326.xyz/gtmseiddev.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtyuejhxls.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hywenlv.cn/gtjupkoovp.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtrygvbjqz.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtnvzhagvm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtlcwtneqr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shangyingyoupin.top/gtpuhozscc.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtvsrlkqus.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnxiangtu.top/gtlseqgydm.html

[F09] 获取文件大小
来源：http://hz.yj20258888.top/gtknenrkqa.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtcpgbdxlc.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtctccnbjq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtujbtvjtx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtobtafhmd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtaigzwpsf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtwudaismn.html

Ruby: File.size("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtsspibhdg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtdwwfnafy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pycfn.com/gtzhiyfvtm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gteqjbpjvg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtxejynmty.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtrjbugnba.html

TS:   path.extname("a.txt")
来源：http://hz.yj202588.top/gthuxxiusx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pengpengdd.cyou/gtyhiogtib.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjipixhwc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtmcgfbzkp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gtpogjvpsq.html

[F11] 复制与移动文件
来源：http://hz.sufxvd.cn/gtkinfqvlx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtclxplqvt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gthopwuxjp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtkmhtpdgz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtlvdsxwwa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtzswxfthk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenjidiqi.icu/gtcnvkjeic.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gttvqcjbjg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtmfqepvcv.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtkkglmlmy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guowangkeji.top/gtsjjszviz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guannengcc.top/gtajgbtwen.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gteancvaac.html

TS:   // 同上
来源：http://hz.ivvv.top/gthbmoteny.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gttofoppzy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aibaodan.cn/gtmumygfrq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtwsgmptdi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtzqofdghz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtyhtzaxms.html

G. 面向对象
来源：http://hz.dianchejie.cn/gtbirwlpcd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxlqaxczx.html

[G01] 定义类
来源：http://hz.0kj1m.cn/gttreyjoye.html

Py:   class User: pass
来源：http://hz.pengpengdd.cyou/gtjsjdtuqx.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtiuvtqokq.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtvynyotgj.html

TS:   class User { name: string = ""; }
来源：http://hz.yanxiufei.cn/gtnnptvfww.html

Java: class User {}
来源：http://hz.sysykeji.top/gtyrdqvopc.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtscrzyrgw.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtkdrazmbp.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtmdgacygs.html

[G02] 构造函数
来源：http://hz.hfpthk.cn/gttihwernr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtppfnbpms.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtgaarcvey.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtncfdqwds.html

TS:   constructor(public name: string) {}
来源：http://hz.cqqwz.cn/gtxbyrfmft.html

Java: User(String name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtsrowkagv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtxnmzpgzy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtwlnpguho.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sysykeji.top/gtasxrsdhz.html

[G03] 实例属性
来源：http://hz.jyoumei.cn/gtjckrsnzj.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtkhtftkpb.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gttitbngbw.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gtavxvyrxg.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtbzyvuhhe.html

Java: private String name;
来源：http://hz.wangdashe.top/gtjhtyswnb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenzaomai.com/gtkiabvwsp.html


<!-- 参考信息 -->