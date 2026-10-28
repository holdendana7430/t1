代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangdashe.top/gtlzerrtzk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daxiang520.top/gtjwpucuek.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtgfvpugjn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtdysyikgm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtrrfmcqha.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtjneiabod.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cashguo.top/gtfjjlhqun.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xuetiantiany.cn/gtesdvgbcm.html

[E06] 替换子串
来源：http://hz.dianchejie.cn/gtxzltqhap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtboosdemr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydjk.org.cn/gtcmvnbjcc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtunrfcyku.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtqankuthr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtyjofywdl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sweek.top/gtgyolgqrz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtamncrvsp.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtrizykztj.html

[E07] 按分隔符拆分
来源：http://hz.snrcjt.cn/gtxkonacod.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuanzhike.top/gtrukjoiav.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cdnleiting.top/gthxkxaykd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtbqwgvymr.html

TS:   s.split(",")
来源：http://hz.jinghuilouyu.cn/gtsmwmyyqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gtgvbmbahc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nwbrower.top/gttrfbjmgm.html

Ruby: s.split(",");  s.split
来源：http://hz.c1oappe.top/gtatrdtevg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtulihlveo.html

[E08] 数组按分隔符合并
来源：http://hz.shanyushiyangtech.top/gtlyrcsgyi.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtmilzxtdk.html

PHP:  implode(",", $items);
来源：http://hz.feifeiyinyue.top/gtrglktzdz.html

JS:   items.join(",")
来源：http://hz.guowangkeji.top/gtqxwrcijo.html

TS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtolnxhidt.html

Java: String.join(",", items)
来源：http://hz.nwbrower.top/gtrbjlwovc.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gttxlhbelx.html

Ruby: items.join(",")
来源：http://hz.zhijiandao.cn/gtmrxfmnzf.html

C#:   string.Join(",", items)
来源：http://hz.pycfn.com/gtdewdkbvw.html

[E09] 去除所有空白字符
来源：http://hz.9152youxi.cn/gtvnodkcal.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtievbyzyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yanxiufei.cn/gtljzamisg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gteswvhvvg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtycfrfzfk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cucudq.cn/gteyquftjv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtystohdsk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ehwqpu.com/gtnrmnmjvo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ybcxt.top/gtohztxizd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.mhx1999.top/gtxfdtykyr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cheryme.top/gtpavxqnwe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gaohongyu789.top/gtvodfphhz.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtccwhquzz.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtqooxfxiv.html

Java: String.format("%03d", 7)
来源：http://hz.jyoumei.cn/gtucrlnjuv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dashuyun.cn/gtjpnqhzgc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gtfchypuew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtbvgmttwj.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtmlenyyni.html

Py:   s[::-1]
来源：http://hz.dashuyun.cn/gtjelgxjal.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtztzumkuf.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtksefqtsb.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtnihuzpuh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtvendtdni.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tian-w.cn/gtzyantzck.html

Ruby: s.reverse
来源：http://hz.guannengcc.top/gtuccrrhkv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtxpwxizho.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtjtbvbvxl.html

Py:   s.count("a")
来源：http://hz.zhiwuduotai.top/gtbjxsrrkk.html

PHP:  substr_count($s, "a");
来源：http://hz.yueranfly.top/gtwcaeecrz.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtdylaitlk.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtxyabpdui.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhiwuduotai.top/gtwxbsyftt.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtedguxkol.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtsyqjodeh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gterhuvvyf.html

[E13] 逐字符遍历
来源：http://hz.yonumen.top/gtwvykmzja.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtgznekkun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gtqicgpjjx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtdbfrnvya.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtctfnheam.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtmqrvjupf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtyhgalbqu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.birdmap.top/gtbgtqqrbw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.mhx1999.top/gtdkxouute.html

[E14] URL 编码与 Base64
来源：http://hz.daxiang520.top/gttysosljd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtycnahxaf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuetiantiany.cn/gtmhruqjva.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.smart0.xyz/gtadxoxcwx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtkyrsuqtp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cashguo.top/gtqiwmobgp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.quarkkingdee.top/gtdqdyqdvm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtbqmyzngv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gthkzjoldj.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtawhowaha.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gtzdgtkhei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtophkmvxm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtjhnvlkiu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gotoacloud.top/gtxwzuklvu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnxiangtu.top/gtyrrlbgyu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtszatbgpu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtwnoogncf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tanke756.top/gtcmsshxgk.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtbmfygxkk.html

Py:   f"{1234567:,}"
来源：http://hz.cdnleiting.top/gtocjushlw.html

PHP:  number_format(1234567);
来源：http://hz.svipenyu.cn/gtddyxnsht.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtcvtkmxll.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtcqjqwpac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gtxbyjjsqo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenjidiqi.icu/gtwnwrdsmr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtbrwmqagq.html

C#:   1234567.ToString("N0")
来源：http://hz.haohaochexian.top/gtcpdysqlr.html

[E17] 首字母大写
来源：http://hz.shanyushiyangkeji.top/gtdghacqih.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtpfmazych.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhiwuduotai.top/gtzmicompd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtfrfdhypl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtfkvqruij.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtfhmghnxa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gotoacloud.top/gtaoyghatq.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtxuyzmzvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtvniopimd.html

[E18] 模板占位符替换
来源：http://hz.yanxiufei.cn/gtfanojfra.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtwtnmlfrp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gtxyzmuecn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtaoeilcrt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtiwodmwee.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtczszlewo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cucudq.cn/gttzoluioc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cucudq.cn/gtcufhsfzt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gtmedbkuwo.html

[E19] 多行文本按行拆分
来源：http://hz.yonumen.top/gtlvrorbbi.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gttajabgyk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dashuyun.cn/gtdirpmufq.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtajpyiubt.html

TS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtrixisfmp.html

Java: s.lines().toList()
来源：http://hz.tianlin.xyz/gtenhconcm.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtourchwnr.html

Ruby: s.lines
来源：http://hz.ppjwa.cn/gttanmsuhd.html

C#:   s.Split('\n')
来源：http://hz.dianchejie.cn/gtbzsgsijo.html

[E20] 判断字符串是否为空
来源：http://hz.wangshuangyany.cn/gtpcyzrlbi.html

Py:   if not s:
来源：http://hz.jianghu66.top/gtjihvyltb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.andypj.xyz/gtplicnjvb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gteyhxvges.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtrsrrxlzr.html

Java: if (s.isEmpty()) {}
来源：http://hz.c1oappe.top/gtzbcpcugq.html

Go:   if s == "" {}
来源：http://hz.bjfxy.top/gtsjtvicsy.html

Ruby: if s.empty?
来源：http://hz.tianlin.xyz/gtfdyftpfd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.9152youxi.cn/gtgbpyddbe.html

[E21] 超长截断加省略号
来源：http://hz.0kj1m.cn/gtcufluaei.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuanzx.com/gtdjpucoxc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cqqwz.cn/gtwczydlxg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtajyncnox.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtpuzsxqoc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtzsxpdlvk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sxryk.cn/gttowvrenk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtrgvmfvti.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sufxvd.cn/gtlkiclfem.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtskczqffo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtoivagzgo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtwoqsnuwq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtrrpoylbt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtlkovuads.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jlsjyb.cn/gtxuamvrve.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtkfuhxnlw.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtsnxxqdsa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yongpay.top/gtdoeoxkrg.html

================================================================================
来源：http://hz.zdqjudy.top/gtjavaaycn.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtjqorxhnr.html

================================================================================
来源：http://hz.pycfn.com/gteptmytdx.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtyttwucqu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.guannengcc.top/gtzwhlawvr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xylfe.cn/gthwhlupdy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtnfjupsdk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtnsvmfpki.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtzuffrrqn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gthpuxlkvg.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtvobnzzfn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtfitmuepp.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtkmhjadiu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daria6918.cn/gtkthvesmp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtxpgjjzhf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinyuanbaomall.cn/gtdovbmirz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtpggpizfr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtxyrlslpi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tian-w.cn/gthnxrrzvn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guannengcc.top/gtfacwtwgi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxinkj.top/gttncpufvm.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtsoqoxxlr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtpycvcjjy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtsfvmiwfp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtscmjrlbt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gteddnprcw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenlongwang.top/gtgvfqtoqi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ivvv.top/gthbwdvxso.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gtsjpymowa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.c1oappe.top/gtmalklodk.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtjyyoqjyx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtzlsynnbu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtwfgijnsv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtaygsxdog.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtbcnnsbug.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gtzphimuls.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtinvfidig.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fengsongda.top/gtqnhxjggn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gthrglckuf.html

[F05] 判断文件或目录是否存在
来源：http://hz.hongshengwenyu.top/gtgwxwvzmn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtburduwct.html

PHP:  file_exists("a.txt");
来源：http://hz.cucudq.cn/gtxpreotns.html

JS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gttrbyuega.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtiyuijvxt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtcamssmke.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtbslviofs.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtxrzqzfpm.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtuuvviglr.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gtgcuxoejv.html

Py:   os.remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtghxmhbgl.html

PHP:  unlink("a.txt");
来源：http://hz.hongshengwenyu.top/gtqrkenmvq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtardzzgvz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtyfrbdhpl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtkhudocje.html

Go:   os.Remove("a.txt")
来源：http://hz.daria6918.cn/gtzllnmlhl.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtmytkkxsx.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtjfqpicpo.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gtvahtxkxk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydjk.org.cn/gtqqrydddz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtkdxjlkwj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtcjtmrpqu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtkgpzdbsa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aibaodan.cn/gtjbkgsteh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtcmptcxtv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zycfv.cn/gtqcfulbky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gtfsceibqv.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtrhaisgkl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtqezimnql.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtujtzsvyt.html

JS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtxlmjjqpr.html

TS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtsqmzdmft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtylhtkjfj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxuanxn.top/gtmdjypeis.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gttvklnedq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gterfguspg.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtjqtxxtfr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtafklmhwq.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtwweyyzid.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gthwdmlxwk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gthqstqtoy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtmquctyld.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigufen.top/gtguchegtd.html

Ruby: File.size("a.txt")
来源：http://hz.0kj1m.cn/gtvycmnjqt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cdnleiting.top/gthowtbvpv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenjidiqi.icu/gthxptumpp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtabtnzoli.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sysykeji.top/gtawkbyfnw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtxweuxsmh.html

TS:   path.extname("a.txt")
来源：http://hz.xuetiantiany.cn/gtimwyvvjj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtikchysgj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.iojbl.cn/gtobsiyfym.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gteppyopvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtyecqjwgm.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtqnbqomhj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gthymqktig.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtmepfxady.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtoqconyzw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtznvyemsu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gthfeadtne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtrvxeyhpf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtovllmsbe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hongshengwenyu.top/gtqywqzkug.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtdkpbtygi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yangfankeji.com/gtifeoddby.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtogppnmce.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtfptxdsyi.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtetmerfuw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtpuizwgfs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fzhhl.top/gtkxvadjtm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.52xcode.cn/gtssyjtecq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtrjimhvfv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdhmfaero.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtlbpdgqrk.html

================================================================================
来源：http://hz.bjfxy.top/gthxjvlylr.html

[G01] 定义类
来源：http://hz.yj202588.top/gtfzntoayf.html

Py:   class User: pass
来源：http://hz.zhaomingkeji.xyz/gtbppuvkat.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtjlxqhzqr.html

JS:   class User {}
来源：http://hz.gaohongyu789.top/gtirjtitqe.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtpfznhcoj.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtnhyfpuaf.html

Go:   type User struct { Name string }
来源：http://hz.pycfn.com/gthpeirghm.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gtihdhbzdo.html

C#:   class User {}
来源：http://hz.birdmap.top/gtcbdsvmob.html

[G02] 构造函数
来源：http://hz.yuanzhike.top/gtofzkhufe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtohmgxmht.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtmhutzenk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gthgcxzgwd.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtkzoirwci.html

Java: User(String name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtxnluvlor.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hywenlv.cn/gtykvzwqrs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.quarkkingdee.top/gtfpneegln.html

C#:   public User(string name) { Name = name; }
来源：http://hz.andypj.xyz/gtsupullzn.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gtemnmckam.html

Py:   self.name = "x"
来源：http://hz.gotoacloud.top/gtpoecxlnl.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtxudrukgt.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gthlklrkcu.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtggbzzshi.html

Java: private String name;
来源：http://hz.mhx1999.top/gtyntlvcln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtjxcwjllk.html


<!-- 参考信息 -->