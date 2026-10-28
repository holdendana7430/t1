代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtvvlqkrlt.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtnoafqwmy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gtyihpzloz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtujsatris.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pengpengdd.cyou/gtgcwydbmz.html

TS:   s.split(",")
来源：http://hz.redwolf501.top/gtxovwjqmt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinyuanbaomall.cn/gtfxbaspyk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gaohongyu789.top/gttmodigjl.html

Ruby: s.split(",");  s.split
来源：http://hz.gotoacloud.top/gtzhdqawmq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gtivumksnq.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtxzxhmwdi.html

Py:   ",".join(items)
来源：http://hz.smart0.xyz/gtjrvudrzn.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtqdgsrbmp.html

JS:   items.join(",")
来源：http://hz.yuanzhike.top/gtxzzkmkau.html

TS:   items.join(",")
来源：http://hz.sysykeji.top/gtjmisrqfd.html

Java: String.join(",", items)
来源：http://hz.sysykeji.top/gtonuprrwv.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gtznxbpuef.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gtaoefsech.html

C#:   string.Join(",", items)
来源：http://hz.gotoacloud.top/gtkvaihjtd.html

[E09] 去除所有空白字符
来源：http://hz.gaohongyu789.top/gtykrxpjlv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ppjwa.cn/gtgobburdw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nwbrower.top/gtorbzofwi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtstdifmoz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sxryk.cn/gtyuhrzbyp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuanzx.com/gthaelemoe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yongpay.top/gtmqnisavf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pengpengdd.cyou/gtzyobklqe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.haohaochexian.top/gtyxfuwmif.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtswoawuhy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtwxfwjnpq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtdlkpsgsj.html

JS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtnmrivrra.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtgjovfddh.html

Java: String.format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtvqkuniyk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ehwqpu.com/gtbjpdqmag.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sysykeji.top/gtqvsjdfcy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.kuanghao11.cn/gtwtglibwv.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gtpdaufgcr.html

Py:   s[::-1]
来源：http://hz.hammf.cn/gtljynzjfq.html

PHP:  strrev($s);
来源：http://hz.jinyuanbaomall.cn/gthdskjsuw.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtkyohmgqw.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtksmzefhw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cqqwz.cn/gtidjhrnaz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtvthuqdwb.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtasamzhhm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gthhyigwpr.html

[E12] 统计某字符出现次数
来源：http://hz.ppjwa.cn/gtnwybdpjw.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gteebteehy.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtqnnqjzpr.html

JS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtgtxnebid.html

TS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtkkeqgcqy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.guannengcc.top/gtibtrinyr.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtlmrjmxis.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtehxgoacm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtyijrnsxh.html

[E13] 逐字符遍历
来源：http://hz.hfpthk.cn/gtwgldmylz.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtyogqwwsi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.9152youxi.cn/gtsbzwumlv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtggvcnauv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gttvznssxd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtylsglkfa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gtmjxnnrbp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtimuxqzdm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtxbxvptrp.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gtdwujobzw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtquukhmcp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.kuanghao11.cn/gtjzjqbvcc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj202588.top/gtbtootchl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jlsjyb.cn/gtnyadtcir.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhixingplan.top/gtfttwrgdc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gthmwjjkbk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinghuilouyu.cn/gtjjezpyak.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtbmhcgtzg.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtbjezuluq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuxming.cn/gtwconxzht.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtzbtbknrg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtjyjtzysf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtilarzqoh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.havefunace.top/gtvxoztemh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtjtznoztr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuanzx.com/gtcuzcrhyz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gttadhnmvn.html

[E16] 数字千分位
来源：http://hz.tanke756.top/gtfledqptl.html

Py:   f"{1234567:,}"
来源：http://hz.xuanzx.com/gtxntxdxwm.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtqswbgbid.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtfxohkhah.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtkgyerros.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtnsmpubsa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.meibo888.top/gtbxtuuiyi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sufxvd.cn/gtavbhbifw.html

C#:   1234567.ToString("N0")
来源：http://hz.sxryk.cn/gtqxjxywqz.html

[E17] 首字母大写
来源：http://hz.ybcxt.top/gteweqhezu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtokxziqcf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gtqgrplbve.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtaafcfabr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gtjzdygnmz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtksuxrdwn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtcpiaqsjj.html

Ruby: s.capitalize
来源：http://hz.wangshuangyany.cn/gtqvrqmydp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtuevhebqf.html

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtewoalvle.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtwvrzbctf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtocrpzagi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtlaqfkkti.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtbwqonutc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtxilldejx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtosjbhliy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtyiezndbn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtedlmhvye.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtxfhkcqpr.html

Py:   s.splitlines()
来源：http://hz.wangdashe.top/gtnlsfhczx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtxbsqtlwu.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtizsrkuql.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtnxxhmqtb.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gtbqsdbfms.html

Go:   strings.Split(s, "\n")
来源：http://hz.mhx1999.top/gtcibondmp.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtduylajjp.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtkhdxupbk.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtckafzxum.html

Py:   if not s:
来源：http://hz.cucudq.cn/gtirljvkat.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cheryme.top/gtaaijawyw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtxoqfdexh.html

TS:   if (s === "") {}
来源：http://hz.chenlongwang.top/gtswizzcoo.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtnuudbzgx.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtcjnlfuto.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtjglxhlzj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtaqbbktrf.html

[E21] 超长截断加省略号
来源：http://hz.jlsjyb.cn/gtbqcacltr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtcrucimeg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtbbmcusjd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtwalzrpvz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtbdoqhzav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtthxbxwut.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gthwtmdmsp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtrdhqlclu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtohmkwmhr.html

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtaawalqap.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtmhnnjfdg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.haohaochexian.top/gtdtbntlwy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtvnnuqkxp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtudqruaxz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dashuyun.cn/gtmrygjsov.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenlongwang.top/gtbmontord.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangtech.top/gttabpkeuz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangtech.top/gtuebuqmpm.html

================================================================================
来源：http://hz.vqdsnc.cn/gteyzauoha.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gtbgqzmnga.html

================================================================================
来源：http://hz.ybcxt.top/gtdyzthcdy.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtizkutehp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenjidiqi.icu/gthuhcslis.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtalwpgyti.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtmrlhrqua.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.haohaochexian.top/gtytkldors.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtvgivrngv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258888.top/gtftamtihs.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtvlbywqrw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenlongwang.top/gtraaqatjy.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtuvwfmgnw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangdashe.top/gtyjqbmjdp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtuqfuejxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtaelxdqyr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtpuvnoubz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtbvtbtreb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gtpgflzntp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenlongwang.top/gtmmhmlrtn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cheryme.top/gtugnyblnp.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtgffmgdnq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhengqikj.top/gtxdegjdxs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtghspbouq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtgjxkbxcd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtxlvjvtdi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gthphykatf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtpkgpeuty.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gogol.net.cn/gtpbbpvofu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cheryme.top/gtmteqcros.html

[F04] 追加写入文件
来源：http://hz.zycfv.cn/gtncihajip.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtfmwkhcmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinghuilouyu.cn/gtvhvgwrpj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtauikhyyc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtfecthdtr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtwzypnrhp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtvdxwgsad.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtxgolujdp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.svipenyu.cn/gtjxszngth.html

[F05] 判断文件或目录是否存在
来源：http://hz.jianghu66.top/gtllqqvltk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ppjwa.cn/gtjqxlheif.html

PHP:  file_exists("a.txt");
来源：http://hz.mhx1999.top/gtogocinvm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtuvpfvcio.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtftkcmfkb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtymczkdoy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinyuanbaomall.cn/gtwxmwdovi.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydzc1.top/gthgniyemu.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gtexyoemop.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gthratmmre.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtwgvjnyua.html

PHP:  unlink("a.txt");
来源：http://hz.hfpthk.cn/gtintzrwqy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.andypj.xyz/gtwzsvabug.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtqccrnybh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtqobxnvqy.html

Go:   os.Remove("a.txt")
来源：http://hz.dashuyun.cn/gttccoowxe.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtaakylvoe.html

C#:   File.Delete("a.txt");
来源：http://hz.cheryme.top/gtmhdxidpx.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtinwzyark.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ivvv.top/gtwjlyfkur.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hammf.cn/gtqgeykfws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtnzmwzsgd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtqeskxlyo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.meibo888.top/gttetesagi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gttxhaqipz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtyohobksd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fzhhl.top/gthspppsyd.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtiqoaiygc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jianghu66.top/gtkpemssqq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtcsxuiwnb.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtymiwntex.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gthngzsgxj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtpmqsmisi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtohyvkonr.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtsycxyxqd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nwbrower.top/gtpnoiyqyh.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtbmomeuox.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtayazlqnj.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gtrgofgtwd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtjbufvpja.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtkhhpffux.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yongpay.top/gthnumctuy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tanke756.top/gtrephruyn.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtvinxbgbj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtcgeeqjcx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jlsjyb.cn/gtqdumabxz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtnziaykbd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yueranfly.top/gtzqcglgrt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtjqfyfyyv.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtnypqmsxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ivvv.top/gtvysvikqo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtrtnrbvqn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtxhbwgjfo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtortgcqwr.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gtuyxcdiex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtdvlvebcw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtregzsjuk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtotmmepgf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtwrlrwiwv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtfadzkqlm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtpcwmbdch.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtlfdewhex.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtqomdsftc.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gthdimejwo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtnidlfmds.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.kuanghao11.cn/gtraibilpt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtgwohlpkw.html

TS:   // 同上
来源：http://hz.316326.xyz/gtwwxmsfhh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.316326.xyz/gtahjfvbgm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gttklromkj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj202588.top/gtaqnrhsxw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtbycgnvha.html

================================================================================
来源：http://hz.pycfn.com/gtvxawnoyc.html

G. 面向对象
来源：http://hz.xinyue.icu/gtkmloczza.html

================================================================================
来源：http://hz.gzhubu.top/gtfkeezxmw.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtrohljmyv.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtgtkinvzp.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtpeonubrm.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtzwebtxbn.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangkeji.top/gtfihturtv.html

Java: class User {}
来源：http://hz.hysaishi.cn/gtyfijtkwt.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gttvpmobkz.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtzbwxzapy.html

C#:   class User {}
来源：http://hz.jinghuilouyu.cn/gtpfnfwxps.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtsbmwzcle.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtnpiohdrc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hywenlv.cn/gtzuvtodke.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtpiibvvye.html

TS:   constructor(public name: string) {}
来源：http://hz.xuanzx.com/gtrllfdroq.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtfpjuxsdx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gtwloixmee.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtltjyyuvl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtjnawlzdr.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtyqnsusbh.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtsfjruyyk.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtvuurzqzp.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gtfpeygtvy.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtzvsrqrif.html

Java: private String name;
来源：http://hz.havefunace.top/gtraopfjsj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtklkpuycx.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtpmmhwxlt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtuaxkylfa.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtsomfwbyu.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtcmxvizqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtspwbyyfg.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtecmazwoo.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtniwowdqj.html

Java: String greet() { return name; }
来源：http://hz.kuanghao11.cn/gtajbhomce.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtozatwezm.html

Ruby: def greet; @name; end
来源：http://hz.52xcode.cn/gtmhjururm.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtzylkpwkb.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtyprbmxpj.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtcmvpbkcq.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtzyqwyvdl.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtvuuldxwh.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtqkfsmqxc.html


<!-- 参考信息 -->