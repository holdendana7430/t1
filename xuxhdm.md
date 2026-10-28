代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtzbuxcscn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhoulong.xyz/gthwxnukbj.html

[E08] 数组按分隔符合并
来源：http://hz.meibo888.top/gtqppxcykx.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gtztuqmxzj.html

PHP:  implode(",", $items);
来源：http://hz.gzhubu.top/gtzdgmefhi.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtvfknvxnb.html

TS:   items.join(",")
来源：http://hz.zhixingplan.top/gtrqfpfkjg.html

Java: String.join(",", items)
来源：http://hz.gogol.net.cn/gtdagtdpvq.html

Go:   strings.Join(items, ",")
来源：http://hz.cucudq.cn/gtdqswsyje.html

Ruby: items.join(",")
来源：http://hz.nanxuanxn.top/gtfbaijlzc.html

C#:   string.Join(",", items)
来源：http://hz.yanxiufei.cn/gtfvbndsro.html

[E09] 去除所有空白字符
来源：http://hz.tanke756.top/gtndrmsarv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangtech.top/gttrhzised.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.redwolf501.top/gtdepfptcm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtcplhazxy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtyakzcblk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtmottmnsj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgufenzy.top/gtuvotzblz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yangfankeji.com/gtwdiuwmze.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydjk.org.cn/gtshxihyso.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtoaofhamb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gtmbutaegf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xziqi.cn/gtihxaqbzy.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtfxdnwhqw.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gtldrojbnd.html

Java: String.format("%03d", 7)
来源：http://hz.fzhhl.top/gtllhwccwq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gtvyigujsx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.vqdsnc.cn/gtmhcrwkls.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shuidangran.top/gttchnatse.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gthqxiestt.html

Py:   s[::-1]
来源：http://hz.zdqjudy.top/gtztewymhi.html

PHP:  strrev($s);
来源：http://hz.jinghuilouyu.cn/gtxcrxwcct.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtljjuhpdi.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtodnqnyov.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gttwobtisx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtncgnicrf.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtfeisscvp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtemeesbgg.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtbnesyqdm.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtjbgsonkg.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtgctcbfxc.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gttvhqurag.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtyqjajuse.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pycfn.com/gtjgenyhia.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gtbyunjydn.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtiaozzwuy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangtech.top/gtrowhcwsk.html

[E13] 逐字符遍历
来源：http://hz.ehwqpu.com/gtscvzbddh.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gtfvrqigyc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xingfuxueyuan.xyz/gtpiudbrzs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtldscwbfp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gthwjejmti.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.birdmap.top/gtpidfficj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cqqwz.cn/gtxhdoxpin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.c1oappe.top/gtlraipywt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtmiaqujvq.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtuelwyyju.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigufen.top/gtgwtqttgg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtiqubejtw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xinyue.icu/gtzxgqiidl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.kuanghao11.cn/gtzgbtlpwo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtnkszqpew.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtjsrujmuq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtevadsyvo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gogol.net.cn/gtoixirkcl.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtjwgpzwiv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtzzwzzinq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.0kj1m.cn/gtvxvewvrj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtuknycbdc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cheryme.top/gtiyvqarun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtzlmxpzjl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtmmdzwavn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fengsongda.top/gthypfxpjq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gthhsfscbs.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtndfeatfd.html

Py:   f"{1234567:,}"
来源：http://hz.jyoumei.cn/gtluvzrwdp.html

PHP:  number_format(1234567);
来源：http://hz.52xcode.cn/gtukwbaewk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtpsqynehg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtptqyudja.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jyoumei.cn/gtcscoxapt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtgseotglk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gtptexozkv.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gtwaillaie.html

[E17] 首字母大写
来源：http://hz.jianghu66.top/gtibmpohpr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtlxgxdimp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ybcxt.top/gtqkssuuof.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtnszlvfsd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtfsosxpaa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.smart0.xyz/gtpxzniwru.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtfekqeula.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtqmeflzuq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.quarkkingdee.top/gtutlszuqe.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gtqndndzpe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtgrjhknhu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gtgcuvawiz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtzrlbhkxm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtopwikwme.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gttvhmvaoe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yueranfly.top/gtuvvbsxww.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daria6918.cn/gtqfkgqxtq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtndozdval.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtasngmsxh.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gtwwwsvtrm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tanke756.top/gtnbihfugh.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtjzhxdvyo.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtpynywney.html

Java: s.lines().toList()
来源：http://hz.jianghu66.top/gtdrvdgsfi.html

Go:   strings.Split(s, "\n")
来源：http://hz.sweek.top/gtykpmtlpx.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtohqwrpup.html

C#:   s.Split('\n')
来源：http://hz.jinqigufen.top/gtbqqbbtwk.html

[E20] 判断字符串是否为空
来源：http://hz.sxryk.cn/gtinecibyz.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtiebtemuh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sysykeji.top/gtquscptaj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gtydfgqznu.html

TS:   if (s === "") {}
来源：http://hz.aizwys.cn/gtqipbgprj.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtlojncasm.html

Go:   if s == "" {}
来源：http://hz.chenzaomai.com/gtevrnchxh.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtcbzwfruv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtafylqgzf.html

[E21] 超长截断加省略号
来源：http://hz.hnxiangtu.top/gtirzvhbsn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtpvhjfois.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.birdmap.top/gtmmigsddk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtgweyczvv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtwtnhqymu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtvzchgkww.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gtirognjpl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtnozyohvj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtvifoqaei.html

[E22] 字节长度与字符长度
来源：http://hz.ehwqpu.com/gtwfwvkzgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtjgfkjzdg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtbdhuzudq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtycjjaoeq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtbanhqpjh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yuxming.cn/gtonxmcqkr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.havefunace.top/gtozrmcggq.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtxglgfsyo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtvhsayqql.html

================================================================================
来源：http://hz.xuanzx.com/gtdexbvvbn.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtlfaqcvlh.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvknhmwkt.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtbnicqpim.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtfdusyzjq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daria6918.cn/gtgqhlqegb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jyoumei.cn/gtqkbquvxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gtttonmpwq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtvfizejfl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtdnjeqrxg.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtplxoxozx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtdlxrbylk.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangkeji.top/gtqlbnjppd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gtlqsatrdq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtjeaxvjwl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtddutnpxw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtdnwheted.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtpmjvzvvo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinghuilouyu.cn/gtcfvkfqfq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenzaomai.com/gtqfnpkrqh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenzaomai.com/gtzilattfo.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtxeyengyr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtudvqgqzk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.birdmap.top/gtwtnesvfp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtcvcskjbz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtqzneonma.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtzrfckgtu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtrxxxfogx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yueranfly.top/gtgeopjrmi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtiwndukpf.html

[F04] 追加写入文件
来源：http://hz.hnqzz.top/gtscjpjrin.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jyoumei.cn/gtbzhlraom.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenlongwang.top/gtakthpact.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtycwmkwso.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtdybtjola.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtdbwjnplz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtgxnrqkez.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtafaiovmg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtwmoczfjz.html

[F05] 判断文件或目录是否存在
来源：http://hz.xylfe.cn/gtuubeyyym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtfgxrzvfl.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtdqqafooe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtatzjhvhx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtrkxzuwkq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtqcdduckz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtkdvlbcon.html

Ruby: File.exist?("a.txt")
来源：http://hz.hysaishi.cn/gtrkwiwvnx.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtnrfeuipg.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtumznhffh.html

Py:   os.remove("a.txt")
来源：http://hz.smart0.xyz/gtzmderupr.html

PHP:  unlink("a.txt");
来源：http://hz.cdnleiting.top/gtbvdssohj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtbzhvmqsh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtcncbzxoc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtvxhurxdp.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtnlsdiuxn.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtuljoccyt.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gthwzqcwha.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gttvihprat.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtxqqpeiwo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daria6918.cn/gtoyrvekdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtbhnvfiyt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtfhkwcbgs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtulxaomng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sxryk.cn/gteabfipqk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigufen.top/gtwleuwslr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gttproeuxa.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtghnteagh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtimjdfmqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtlndupfkb.html

JS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtkeepdznu.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtqbqttffa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtmjetyvgr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jlsjyb.cn/gtdpprbore.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtkfrjrtiz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtqnaelcro.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtdmcaxggr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sysykeji.top/gtxryekxrj.html

PHP:  filesize("a.txt");
来源：http://hz.pengpengdd.cyou/gttqbqegdl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtpvinphio.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtgmukukhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtchfvdaat.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtwfgyblne.html

Ruby: File.size("a.txt")
来源：http://hz.ivvv.top/gtxeoryozi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258.top/gtkpxoereu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtjwjrjuoi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtfvnuhjuh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtqyspwdhb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtbxrnaaep.html

TS:   path.extname("a.txt")
来源：http://hz.gzhubu.top/gtumxwdfpe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtsgxelplb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtxcddvjds.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtcbyxjske.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yvedp.cn/gtvbecoghk.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtfrmukiuo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gthvfsjpds.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtujuqopkm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtozjyuael.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gthrkapyuv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.bjfxy.top/gtbrbpqpdp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jiagoushi.top/gtfrvhxyxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtbepauazq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tanke756.top/gtexyfairi.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gtiscohdbm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fzhhl.top/gtglgjbxvf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtzrcfocaf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtliklughh.html

TS:   // 同上
来源：http://hz.hongshengwenyu.top/gtikzzuejv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gtaehxongh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hfpthk.cn/gtugovaltj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtmntzgvnx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jianghu66.top/gtdjgwlznf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtswdkdqnr.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtlmylxnoh.html

================================================================================
来源：http://hz.haohaochexian.top/gtpkcanqpq.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtrbhwurwk.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtjxacrnch.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtfsmsthdz.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtgmblbzbg.html

TS:   class User { name: string = ""; }
来源：http://hz.cashguo.top/gtfidquett.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtbxsewzcd.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtzatzxkam.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtgimdvkuy.html

C#:   class User {}
来源：http://hz.yuxming.cn/gtnumupdeq.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtccaeyoqp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.kuanghao11.cn/gtxmpypdfn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.bjfxy.top/gtjmfjuioo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtsbmojotu.html

TS:   constructor(public name: string) {}
来源：http://hz.zhixingplan.top/gtanrakpsb.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gtfgxcumec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtwpuiwqqx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtdmjdyocx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtnvcfjhzs.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtpmpbczhm.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gttrccuebb.html

PHP:  public string $name = "x";
来源：http://hz.xziqi.cn/gtxvpqydzi.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtisuyavws.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtyappdrel.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtibnvhdin.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jianghu66.top/gtokwtcpeo.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtdvihmffo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtmkshbjxw.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtrayddwou.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtrfdkdgpo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtjxroosio.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtceaoxtje.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gttumeahcl.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtjnzukpoq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtrupztaua.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtnzxhuzss.html

C#:   public string Greet() => Name;
来源：http://hz.birdmap.top/gttpfbfols.html

[G05] 继承
来源：http://hz.cashguo.top/gtmhqxzipz.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtmvoherhh.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtoeyodjpj.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtxcehszum.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtnwslutou.html

Java: class Admin extends User {}
来源：http://hz.guannengcc.top/gtsojysjlj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtdivltsdu.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtmlxsffrm.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gttolaypim.html

[G06] 重写方法
来源：http://hz.bjfxy.top/gtbhljwnjs.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtfpbqoqva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtbqonmtbs.html

JS:   greet() { return "admin"; }
来源：http://hz.cheryme.top/gtozxebnmf.html


<!-- 参考信息 -->