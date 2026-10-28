代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pengpengdd.cyou/gtfjawfuxk.html

TS:   s.split(",")
来源：http://hz.hammf.cn/gtervgtpdk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtgtreogcy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xingfuxueyuan.xyz/gtdalnvpns.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtdurnzsin.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zdqjudy.top/gtofbdswiy.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtncvjjgnv.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gtynstnmix.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtcuxefcfq.html

JS:   items.join(",")
来源：http://hz.fengsongda.top/gtrvlvgjuq.html

TS:   items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtwkvzrtde.html

Java: String.join(",", items)
来源：http://hz.shanyushiyangtech.top/gtgoqzqrgc.html

Go:   strings.Join(items, ",")
来源：http://hz.ivvv.top/gtfumtuwio.html

Ruby: items.join(",")
来源：http://hz.redwolf501.top/gtxgtqszya.html

C#:   string.Join(",", items)
来源：http://hz.ywan-chungtsiang.top/gtiivsjqbv.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtmrqseldm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yangfankeji.com/gtdkoyzyef.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daxiang520.top/gtcbvipygv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gtopmfefsj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtbgnmnsrk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtcqntzjbw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.birdmap.top/gtasbeeqhv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinghuilouyu.cn/gtpnbhmlul.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sysykeji.top/gtdjyrnsqh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtgbsxahtw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinghuilouyu.cn/gtyuijmxnw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtzoldmwpn.html

JS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtlisvbujs.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtbhhcywyc.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtbgveguxu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtsuydluzw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dashuyun.cn/gtvbwjfemc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtxhldbruq.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtlfenouza.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gtxfzlnvpa.html

PHP:  strrev($s);
来源：http://hz.xuetiantiany.cn/gtxatbtpsl.html

JS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtdkfjaebv.html

TS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gthgybmqwd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj202588.top/gtdgesudhf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.kuanghao11.cn/gtszmcvhzc.html

Ruby: s.reverse
来源：http://hz.pycfn.com/gtegskqlqs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtlqkoqqre.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gteorewfyk.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtymagmjnf.html

PHP:  substr_count($s, "a");
来源：http://hz.aibaodan.cn/gtilmsldls.html

JS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtipnbhfrg.html

TS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtthhfnroe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fzhhl.top/gtwyqkelbk.html

Go:   strings.Count(s, "a")
来源：http://hz.guowangkeji.top/gtyqxowuox.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gtvuwsjfuj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtiqeckcnp.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gthnpffznn.html

Py:   for ch in s: print(ch)
来源：http://hz.yuxming.cn/gtmbasnkxq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtnqvlnmgv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtesxkdnfm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtorggsesj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtregmhwkn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtjhfmneyy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtihdxbuwt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinghuilouyu.cn/gtanncyhyv.html

[E14] URL 编码与 Base64
来源：http://hz.52xcode.cn/gtsfotsexx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sxryk.cn/gtlauwkyad.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhiwuduotai.top/gtifpcghdn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gtbdbcgguo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.wangdashe.top/gthsgvfiio.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ivvv.top/gtfiucbjqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtgnqxudiq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.mhx1999.top/gtmczfkaow.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigfzy.top/gtvgwjcghr.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhongyouzk.top/gtsnmkepjz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tianlin.xyz/gtjzmgnoer.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtifvocesj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtfuwjltea.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gtxwbxadzo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtmfcdcpbo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dashuyun.cn/gtssmzhwew.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yueranfly.top/gtoneoeolk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtpivursax.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtmvfxrjsq.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gtggtmzygw.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtweowwaoo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtjqurknnt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtmsygzqdp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dashuyun.cn/gtzxfyzvkz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtzhsihkws.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dashuyun.cn/gtwdlxnnvc.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtiqiadiab.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtxxrhryyc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtxmfbvlim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigufen.top/gtvesejnsv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtpjdkojtw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtwwwzezsy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.havefunace.top/gtfhhjgtry.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtgcekeaas.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtzfeqgvvo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.haohaochexian.top/gtsatyxcsc.html

[E18] 模板占位符替换
来源：http://hz.yonumen.top/gtupxidklg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cucudq.cn/gtclbecuia.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gzhubu.top/gtetwhivps.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtcbnspwqw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtyancfonp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shangyingyoupin.top/gtnktybloo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.smart0.xyz/gtafykgaxs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtpbamuiuo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnqzz.top/gtlfcetoha.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtmizukznh.html

Py:   s.splitlines()
来源：http://hz.daria6918.cn/gtxhsiuzli.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtbuaanacs.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtujiqvpus.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtjzexvgsh.html

Java: s.lines().toList()
来源：http://hz.zhijiandao.cn/gtxtpqvxwo.html

Go:   strings.Split(s, "\n")
来源：http://hz.shzxlz.cn/gtbopjgaxn.html

Ruby: s.lines
来源：http://hz.mhx1999.top/gtyzucdmyt.html

C#:   s.Split('\n')
来源：http://hz.chenlongwang.top/gtiqjgejmi.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtvylnrcme.html

Py:   if not s:
来源：http://hz.yj202588.top/gtwmmjigdy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xziqi.cn/gteokrkkea.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtkikkoetd.html

TS:   if (s === "") {}
来源：http://hz.nanxuanxn.top/gtyggkqjne.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtskixcpwj.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtdnjwptti.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtusgjrqmo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhongyouzk.top/gtoglorwss.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtagpnxrmw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258.top/gttiezvayu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhiwuduotai.top/gtwqzfjqti.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gthqsxnvwm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gttqdwytns.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtksggpkxp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gtrhdllbnj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtngrjpmht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtrihsdiuh.html

[E22] 字节长度与字符长度
来源：http://hz.zhaomingkeji.xyz/gtccludlsk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtdwqdtjzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gthlujefzf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtbthnmrzu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtxqlizwkh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtnduyluwg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hongshengwenyu.top/gtzeapmkju.html

Ruby: s.bytesize;  s.length
来源：http://hz.yongpay.top/gtkuowfonz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtgxuwfbie.html

================================================================================
来源：http://hz.snrcjt.cn/gthlxkanjj.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtfrqtprtl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdoykjauu.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtucfvpzqn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xziqi.cn/gtwbvjhtlt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gteysdaqes.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtphhuwynh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtgfqtcrgo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtfqwvmrpz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtxjzqqppm.html

Ruby: File.read("a.txt")
来源：http://hz.gotoacloud.top/gtofquujap.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtgsqicrxx.html

[F02] 逐行读取文件
来源：http://hz.kuanghao11.cn/gtavubvucb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtfsicmdkb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gtqyigvufu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtzznkfjqa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtjpfvaoyy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtcvrservn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gtxnueivho.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shuidangran.top/gtzounkdwq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtesbcohbx.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtunhrrpbg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtdbthhqaf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guannengcc.top/gtdiqjplzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtcsxskqgw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtdezdwrhc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yonumen.top/gtwjwmrdvj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtrlgmchep.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinghuilouyu.cn/gtuzwtiicz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtypkecpwb.html

[F04] 追加写入文件
来源：http://hz.fengsongda.top/gtvkclrhgs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtyabqrvai.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtejpkvhhw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtaoxtopka.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtctzosdjd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.0kj1m.cn/gtzqmgodhl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtazcuzbob.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtkhtasvnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtzcctqxwy.html

[F05] 判断文件或目录是否存在
来源：http://hz.zycfv.cn/gtmayghbjy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zdqjudy.top/gtjnhmunyc.html

PHP:  file_exists("a.txt");
来源：http://hz.zhixingplan.top/gtsrfmajun.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtefytorbt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtlczuiteh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtccpyrkgl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gttsdsgsge.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258888.top/gteyawnqtg.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtjafkvwbm.html

[F06] 删除文件
来源：http://hz.zhaomingkeji.xyz/gtkyuwulxv.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtfrxdkyzg.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtdcexvvgh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtocpcslai.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtvmdpyrqi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtwcvpvgol.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtjdyocelr.html

Ruby: File.delete("a.txt")
来源：http://hz.hnxiangtu.top/gtyfsnlggz.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtjjbqotlf.html

[F07] 创建目录（含多级）
来源：http://hz.yvedp.cn/gtqqdsgfyw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gtzzsxmpwy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnxiangtu.top/gtbemqnuun.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtuekvvmra.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtphvwktaz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtdigcasbz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dianchejie.cn/gtrstefgnj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtsuuwtrqa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gthlbzqvmd.html

[F08] 遍历目录
来源：http://hz.gogol.net.cn/gtylevtdpg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gtlkzgevtt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gtissnnpia.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtalppcqwb.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtmcrrzyrs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtugyebtqp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jlsjyb.cn/gtmdxxnrbh.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtbcqjncvr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtemcsomac.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtsricoerm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gtyicfwims.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gtyqtsiqfn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtcwgyhqat.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtffranfxp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtnmfmgjhe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtpgvieydl.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gtactatqko.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangshuangyany.cn/gtogfqgdkm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangkeji.top/gtkokdvhnj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtvzaokhoh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj202588.top/gtjblvjqxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtpekkerlq.html

TS:   path.extname("a.txt")
来源：http://hz.fengsongda.top/gtrmpkgmng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtbqibfhry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shuidangran.top/gtejxqmljs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtkkosxvwo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.316326.xyz/gtgjekhrpa.html

[F11] 复制与移动文件
来源：http://hz.feifeiyinyue.top/gtxdponkte.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtowfhhlpm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtxyahrivn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtnxcuwkzh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtfzfacwow.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtvotpdawu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ppjwa.cn/gtkibudfzs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtbhmtcqld.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtfzwiywgk.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtyrocxrdt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtoqexbyhc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.mhx1999.top/gtfxhddeet.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.mhx1999.top/gthtjzmskl.html

TS:   // 同上
来源：http://hz.shzxlz.cn/gtmoboefqx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.316326.xyz/gtmltscogs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gthcinhftc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtkubzpdkl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtqndxijak.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gteyxivlrd.html

G. 面向对象
来源：http://hz.pycfn.com/gtkhkuzicq.html

================================================================================
来源：http://hz.guowangkeji.top/gtiswogshl.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtiflrnohs.html

Py:   class User: pass
来源：http://hz.316326.xyz/gttsnyuuxh.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtuukpnbnf.html

JS:   class User {}
来源：http://hz.zhongyouzk.top/gtttlusxul.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtpnnpuysy.html

Java: class User {}
来源：http://hz.0kj1m.cn/gtozdfafsg.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gttuzlvoqv.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtkpattemi.html

C#:   class User {}
来源：http://hz.guannengcc.top/gtrezrguva.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtqtbikmhg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtczkivlto.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtbzjhakck.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtvtyumxlc.html

TS:   constructor(public name: string) {}
来源：http://hz.aibaodan.cn/gtqexfqlnw.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtnxnyrswd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtemrpimed.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtqnxvatpl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258888.top/gtedojycrt.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtkvojirxr.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtxieqtven.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtqncavdxg.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtkokjbert.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gtvljdgdys.html

Java: private String name;
来源：http://hz.sxryk.cn/gtarqitbzx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtjuqjblib.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtgegphjvz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtpiyfuxon.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtpozwhdkx.html

Py:   def greet(self): return self.name
来源：http://hz.ydzc1.top/gtzswvjdxs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtkndswhpf.html

JS:   greet() { return this.name; }
来源：http://hz.redwolf501.top/gtcnofinha.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtqkgrgqda.html

Java: String greet() { return name; }
来源：http://hz.yvedp.cn/gtrzbxpltf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dianchejie.cn/gteudwqcqf.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gttiffityj.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtzujfszua.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtvtmqovpx.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtluiipegw.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtaxevlefl.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtygsmxptq.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtkddsgrsc.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtnpyonglz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gtidihbtnp.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtdjtgykqg.html

C#:   class Admin : User {}
来源：http://hz.xingfuxueyuan.xyz/gtuobidssv.html


<!-- 参考信息 -->