代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtznxyyhba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtxsqdbsof.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuetiantiany.cn/gtrudjnoyb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xziqi.cn/gtogkkdvdh.html

[E06] 替换子串
来源：http://hz.ivvv.top/gtphxoxsna.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtjqystfdk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtlrutnnch.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtxvfkubxr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtezoxjhpu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtfmnwoyko.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sufxvd.cn/gtmfcpocdl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtecgafcyy.html

C#:   s.Replace("a", "b")
来源：http://hz.tianlin.xyz/gtukzrodmy.html

[E07] 按分隔符拆分
来源：http://hz.daxiang520.top/gtmohndrhp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.mhx1999.top/gtjebzeths.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fzhhl.top/gtbycjferm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cucudq.cn/gtvsmktzcv.html

TS:   s.split(",")
来源：http://hz.zhijiandao.cn/gtvzrakhun.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yongpay.top/gtvcfyjusn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.guannengcc.top/gtvfabonqw.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtljcftfgg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sweek.top/gtvedxrhgm.html

[E08] 数组按分隔符合并
来源：http://hz.jianghu66.top/gtfplouufc.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtimlhrwpi.html

PHP:  implode(",", $items);
来源：http://hz.jqgfzy.top/gtvbofhxvr.html

JS:   items.join(",")
来源：http://hz.cucudq.cn/gtiimngxmy.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtsmlwebqo.html

Java: String.join(",", items)
来源：http://hz.wangshuangyany.cn/gtswnsmyzc.html

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gtxbfquqvc.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtlqrpjybx.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gtscdkbddm.html

[E09] 去除所有空白字符
来源：http://hz.gogol.net.cn/gtzkbwrytp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtyabgfxjc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yongpay.top/gtiufnmonf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtquavabnb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtqdnfqgcp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtttbhwvpx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hywenlv.cn/gtuggqepgz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cqqwz.cn/gtcoywumdn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangtech.top/gtjzrswalq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenlongwang.top/gtwwwudtmp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtivrhyofg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtdfwweuzd.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtqltmkxqy.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtdskrbami.html

Java: String.format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtivjvfwtl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtnrvpnzzj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ppjwa.cn/gteizyrmzl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.havefunace.top/gtvonyotke.html

[E11] 反转字符串
来源：http://hz.havefunace.top/gtffzbhlpm.html

Py:   s[::-1]
来源：http://hz.haohaochexian.top/gtwekyimqx.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtqnegmwle.html

JS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtjlwlbadp.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtvetqhwoi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtatrplpxb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtqpweeqca.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtxtmgdqyb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gthhxgfxqg.html

[E12] 统计某字符出现次数
来源：http://hz.yongpay.top/gtinqkxxzm.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtmfrfmzee.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtsiipznyn.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtcmsrbmpr.html

TS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtojvjzupb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtjfwmpott.html

Go:   strings.Count(s, "a")
来源：http://hz.yuanzhike.top/gtrxyatbqr.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtsoivuwls.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtfzjiecjr.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtcmuykdyr.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtyhdjfodb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cashguo.top/gtshwlvijk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtbnzilmlc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtwnpkjvod.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtnrkpwwzw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangtech.top/gtfgklrjnk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aibaodan.cn/gtziymvyrt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shuidangran.top/gtaponwknl.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtxtwukfkc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gthyfkqote.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtjkeodsmq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.feifeiyinyue.top/gtnrltyciz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtnzyeipbz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtvudzasul.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtgrqtglza.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.birdmap.top/gtvpuwdigz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgfzy.top/gtokgpvjyq.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtxsrycwiq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daxiang520.top/gtptqdqfhc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtxptbsyqo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtumeiwwpd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sysykeji.top/gtuwluewcx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gttunomule.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtvqpicnpj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xinyue.icu/gtutxcjtjl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtpdfwszlo.html

[E16] 数字千分位
来源：http://hz.daria6918.cn/gteyhbtlqk.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtzkrsretg.html

PHP:  number_format(1234567);
来源：http://hz.hnqzz.top/gtohrfxdrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtrjnatody.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtiiijsqjg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtvgjpncxb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtdxrawslo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cashguo.top/gthnauqxdb.html

C#:   1234567.ToString("N0")
来源：http://hz.shangyingyoupin.top/gtxwjrruvm.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtbwdwtcet.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtlnlgmeqp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtdzuebktv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtjbpkdytg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtwivwqmba.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuxming.cn/gtxukuhsje.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtyrrpaybf.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtwvooltkp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zycfv.cn/gtutwibpry.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gtnczfhpot.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hongshengwenyu.top/gtdteqflkm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtozhywrib.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtbpulctfi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtdxboorez.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hfpthk.cn/gtxzndfsut.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gtyilewltl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gtdogbonww.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gtmvewmmkz.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtwocpdilv.html

Py:   s.splitlines()
来源：http://hz.yj20258888.top/gtoegbrifv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guannengcc.top/gttoevxycx.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtwceymwuf.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtuxnqnkcr.html

Java: s.lines().toList()
来源：http://hz.hysaishi.cn/gtcaicoihf.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gtlmvovxch.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtyfoyvejv.html

C#:   s.Split('\n')
来源：http://hz.dashuyun.cn/gtutprmokh.html

[E20] 判断字符串是否为空
来源：http://hz.zdqjudy.top/gtnfoicsxc.html

Py:   if not s:
来源：http://hz.yanxiufei.cn/gtsqaduldh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinghuilouyu.cn/gttceuwfed.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtzgktbtwj.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtjnegorsw.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gtkaeglndf.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gttybbcdmb.html

Ruby: if s.empty?
来源：http://hz.xingfuxueyuan.xyz/gtkiupmayc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hysaishi.cn/gtrcabycqu.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtfzgullwo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fengsongda.top/gtkckyjghw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtztnurzkb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtaqetzxal.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtbphtondm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtpbjvlqbj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtlgfacusz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gtrzozubef.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sufxvd.cn/gtfmubnwzv.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtullotkmm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtdqunxugy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtxjmphpdy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtwkkgoklv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtovuombiy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shzxlz.cn/gtgmxxckcp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xylfe.cn/gtsqcmioys.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gteosamzpc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtgbnzoyhh.html

================================================================================
来源：http://hz.meibo888.top/gtmgvqqurl.html

F. 文件与目录
来源：http://hz.guowangkeji.top/gtllkiajeo.html

================================================================================
来源：http://hz.ppjwa.cn/gtljsinajp.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtphkxxlum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sysykeji.top/gtzwtxtguq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtaippmcsd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtudelyjgt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtvhsdmjrl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gthjsjeiux.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.svipenyu.cn/gtzmowzxpe.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtrlnqsijz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtbzpxbaob.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtipszdrfz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtsvdnvuki.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtpakxjxqe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtgwchllkg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtlnqxmoih.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtghyfkzza.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ywan-chungtsiang.top/gtlyvqnjkj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtwacleuzc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gteuydrphl.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gthxfqzwee.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtsshgtvhi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtcuhnkjrt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtlwsjudpl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtxvgrbycq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhaomingkeji.xyz/gtssnwkkis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtupkidhus.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tian-w.cn/gtjyfogcnb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.redwolf501.top/gtpipiimuj.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gttqekcxge.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.316326.xyz/gtidobvqsq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gtzpkbssyc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gthlrrffvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtnzwxmixd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ywan-chungtsiang.top/gtctprstbh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtwmvtjzvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.smart0.xyz/gtrnnyzmhg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.meibo888.top/gtjxruftse.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtpnlvgeas.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtanpqyyud.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtrfqooiyw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtazepiamx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtgljgpmhd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtohokvpwv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gtoqnbhgup.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtgstgvwmm.html

C#:   File.Exists("a.txt")
来源：http://hz.xinyue.icu/gtgaicadtq.html

[F06] 删除文件
来源：http://hz.meibo888.top/gtschgyjvr.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtctxffqra.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258888.top/gtmqxxyoik.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtsfivcbch.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gthezuqcdu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtiydujklq.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtvldqyexy.html

Ruby: File.delete("a.txt")
来源：http://hz.hnxiangtu.top/gtaxzfjoku.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtipmsjwor.html

[F07] 创建目录（含多级）
来源：http://hz.shuidangran.top/gttczismxv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ybcxt.top/gtnsyngyii.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zycfv.cn/gtfttfhinq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtfaweubqy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtezwuzbpd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtbbzcydep.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtfoaegaav.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtjduznypc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtwazgqpul.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtmodtbqwb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hysaishi.cn/gtokcqialv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtmihybxzd.html

JS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtkhvfjtdm.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gthuhqosas.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtncdwfoel.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtufiuvztf.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtwnyxhbyp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtdiwmbfwi.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtrijscsvz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtwlsozxvd.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gterqpxgcg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtsudfwhsw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtadupgdsr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtxblafgqe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gtnjbpzxrn.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtckqbyqdx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jianghu66.top/gtuujbzvvr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtxhubnkop.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtbdixwghb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtsvorglrb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpqlsxqfj.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtxwogrjde.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtalbnjojr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtqpqvtklq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtghmcthov.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gttqmynaxh.html

[F11] 复制与移动文件
来源：http://hz.pycfn.com/gtglnuwset.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtnbzkmwkg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gthinjhlgq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtdadtsewq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtsxmatlhb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cqqwz.cn/gtwxshyobp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtlticmolp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gteapmcyxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nwbrower.top/gtizjxgicy.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtsacaerrr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hywenlv.cn/gtvrbqgivo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258888.top/gttmwgcygu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtlhlbnfan.html

TS:   // 同上
来源：http://hz.svipenyu.cn/gtkpyvvzzs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtpihbztma.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.vqdsnc.cn/gtfexgxrlf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtjyhvrpyp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtzwpwjwcw.html

================================================================================
来源：http://hz.dianchejie.cn/gtqjlvvfxq.html

G. 面向对象
来源：http://hz.nanxinkj.top/gtbvkroslx.html

================================================================================
来源：http://hz.bjfxy.top/gtwpnnyxuj.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtrgxvvect.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtixdvnoyy.html

PHP:  class User {}
来源：http://hz.wangdashe.top/gtdkwdjjhq.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtzufzjtdb.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtubczpzye.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtbqmyphcf.html

Go:   type User struct { Name string }
来源：http://hz.sufxvd.cn/gtcsszhpvy.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtptyhikjj.html

C#:   class User {}
来源：http://hz.316326.xyz/gtggcgnznt.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gtfidvffqp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtktnzuqvr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gthptoruzn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtejstnjng.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gtaivkngop.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gtnbqfcowm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtueqvqxnu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.quarkkingdee.top/gtariuawul.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtqtuxhxir.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtgzuiozma.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtwjpvyapv.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gtujgenktv.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtfrukcjdb.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtvtqsrugo.html

Java: private String name;
来源：http://hz.snrcjt.cn/gtlmkojyxg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sufxvd.cn/gtujghnzfa.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtahqcdhkj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gtbksdpbpw.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtfeeuekdg.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtxriabdhn.html


<!-- 参考信息 -->