代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gttogiccsp.html

JS:   items.join(",")
来源：http://hz.andypj.xyz/gtqkmmewgx.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtjijburin.html

Java: String.join(",", items)
来源：http://hz.shuidangran.top/gtodnoehhb.html

Go:   strings.Join(items, ",")
来源：http://hz.haohaochexian.top/gtcoeeiujc.html

Ruby: items.join(",")
来源：http://hz.cqqwz.cn/gtzzmfexiy.html

C#:   string.Join(",", items)
来源：http://hz.9152youxi.cn/gtfvfemhfc.html

[E09] 去除所有空白字符
来源：http://hz.zhijiandao.cn/gtixsmfezw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtedczwfxr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xingfuxueyuan.xyz/gtybbzlpvb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.mhx1999.top/gtsxvbdjpf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtbtnmdbpu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gttcrzcnkm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gtouqllkva.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtgwlhnyqv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gticaohbzg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtfxqfjyvv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xinyue.icu/gteoomfbsg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ywan-chungtsiang.top/gtwinogbru.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gtsnrrfjyk.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtxlvkvamf.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtwuwhigrh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtyfqytmva.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtrtreqzfm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtsezsajxe.html

[E11] 反转字符串
来源：http://hz.gaohongyu789.top/gttgvsxzyh.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtrppeatxt.html

PHP:  strrev($s);
来源：http://hz.jinqigfzy.top/gtoiiqowgr.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtbgjqrglu.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtxiiyascb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtevnebuhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gtnbqeufjh.html

Ruby: s.reverse
来源：http://hz.pycfn.com/gtdhzgumit.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtglqkxefo.html

[E12] 统计某字符出现次数
来源：http://hz.quarkkingdee.top/gtesqjotsa.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtejxhrwos.html

PHP:  substr_count($s, "a");
来源：http://hz.haohaochexian.top/gtclnbvvoa.html

JS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtpbsqpkzz.html

TS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtndufdnqr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtwgbtcjhk.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtglqzmnbh.html

Ruby: s.count("a")
来源：http://hz.yongpay.top/gtswqtznzp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtltyiuzrx.html

[E13] 逐字符遍历
来源：http://hz.dianchejie.cn/gtotpsalln.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtlqvswceh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258888.top/gtoqwfhzwr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtofjpnwle.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtblfdszbu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtrlphjqch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtrlhhzbtr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gzhubu.top/gtvmbruwtv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhaomingkeji.xyz/gtljtgirbv.html

[E14] URL 编码与 Base64
来源：http://hz.shuidangran.top/gtdegnwkwq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtwqngocqw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtiiwyvevv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinghuilouyu.cn/gtjjortctu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtoogcnals.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtbmqyzkvw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtcvqbslhp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gthryuwnfd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtmlpptfin.html

[E15] HTML 转义 / 反转义
来源：http://hz.ybcxt.top/gtlxclzuye.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtzdxihqbo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtdhwyhfua.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.kuanghao11.cn/gtopktuihe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtmmnsixcq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigfzy.top/gtcvbkrvjp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinyuanbaomall.cn/gtsuhvnnpt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtrepyhnvn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gthassuveg.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtuuaskmtf.html

Py:   f"{1234567:,}"
来源：http://hz.havefunace.top/gtwnpucckf.html

PHP:  number_format(1234567);
来源：http://hz.zhoulong.xyz/gtpdiktexc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtxjrnqdnk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtpsmrcgny.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtsmgujeyb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guannengcc.top/gtntctngwk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigufen.top/gtpzaxkvqb.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtftyobgkq.html

[E17] 首字母大写
来源：http://hz.pycfn.com/gtvjbcjuio.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtewsbsxvi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hfpthk.cn/gthxtahhes.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gterdemita.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtyxoydgwn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dianchejie.cn/gtixxqdnyh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gtdohvqkfz.html

Ruby: s.capitalize
来源：http://hz.guannengcc.top/gtbbrurvjx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtwuktbaqp.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtdmbdbibx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenzaomai.com/gtlnpqdvwc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xingfuxueyuan.xyz/gtvaqrdfky.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gttsonklyc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtvijibbrs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtaavedfix.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtbunndufb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yanxiufei.cn/gtottusmom.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjfxy.top/gtadkxkbic.html

[E19] 多行文本按行拆分
来源：http://hz.yuxming.cn/gtussjipcb.html

Py:   s.splitlines()
来源：http://hz.jianghu66.top/gtmafpzbfg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtvxdnvckj.html

JS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtjoqfsptb.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtguffevoj.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtipoelysk.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gtggkfcdoz.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtotirhrpb.html

C#:   s.Split('\n')
来源：http://hz.cheryme.top/gtyuswidlx.html

[E20] 判断字符串是否为空
来源：http://hz.redwolf501.top/gtnehhdcyf.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gtrzwhwgnl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.iojbl.cn/gtunbmlkdh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dianchejie.cn/gtxzqddqid.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtojhtxfom.html

Java: if (s.isEmpty()) {}
来源：http://hz.yueranfly.top/gtwrkltmok.html

Go:   if s == "" {}
来源：http://hz.ydjk.org.cn/gtoztozyjt.html

Ruby: if s.empty?
来源：http://hz.zdqjudy.top/gtfmkeohze.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gthqkyazei.html

[E21] 超长截断加省略号
来源：http://hz.hnqzz.top/gtqntfzlmc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtsqrukexw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtuyazoqga.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtgfinxeid.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtvtbjjvhm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtkmlxyuef.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jianghu66.top/gtfoxejhoz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtjaddvutu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtqqoqxvor.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtgpmsszlo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nwbrower.top/gtnenlpbif.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtqshdtuxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtdjrfcban.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtwbnkxivf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gtphcwowex.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtezhcnkyi.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtwocjrwpt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guowangkeji.top/gtotlcjued.html

================================================================================
来源：http://hz.52xcode.cn/gtcjojubof.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtoxbfizcd.html

================================================================================
来源：http://hz.shuidangran.top/gtqnhkrqvg.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtokrdkjbc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.guowangkeji.top/gttqgcnmnh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.vqdsnc.cn/gteowailgx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtaiscrqcm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtsdmvmzlk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtnxpsnxmv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtqovkvbyx.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtufpfovca.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtdqpuevip.html

[F02] 逐行读取文件
来源：http://hz.jinghuilouyu.cn/gtdoxfaxzv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtznqochfi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtxgqhaqzm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtiwhweiqx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtmtyppayi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtkklqazmp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangtech.top/gtwbjywett.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtugjqkxwl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.birdmap.top/gtfombfqhi.html

[F03] 写入文件（覆盖）
来源：http://hz.xinyue.icu/gtlzssxdrz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtyunlxyab.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtwfhremor.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gthoctlsxz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtuxayevfg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtyuwiexeo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtgnqyckrc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gthqjrdylj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtvehpppcq.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gteyrovshz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gtpfupanha.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gtilrvpems.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtqkqsszhy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtqkiyggtj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgufenzy.top/gtuepkmbkg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangkeji.top/gtfsuateln.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gthvrocmss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtuqsradhp.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtiwihmdkn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtwkxjoccx.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtqhgwgwfs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtmfjvttib.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtcdifktyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gttgprelnw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtsuifyctd.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtaexkeirw.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtvxzchxmr.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtsuarqgcq.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtxjjvnfso.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtzroosbdf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtusjoqbtp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtydgcwwtk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtdgzqxlvr.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtsgyrhmwt.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtvmcjnlwl.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtnrvlkucm.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtitzrbtkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtaaalylbd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtlnmhpgqy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gteiwdbxmg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtbrkqasrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jyoumei.cn/gtqfpiblax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtshuadbde.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xziqi.cn/gtiuhuuhqn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.quarkkingdee.top/gtkesaorsv.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gtpngdjjes.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtntahiqyh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sxryk.cn/gtrpzwgkks.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtpzailrry.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtdzdcnwzj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtoocbxagj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtwfalbvcr.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtgzifwfez.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtabtpvzjp.html

[F09] 获取文件大小
来源：http://hz.tanke756.top/gtuewoabuw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtubizigbx.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtdwnhfcpf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtvykntykx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtrgecopnm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gthdcadpvy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtdckknski.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtcfvracxr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtbhkfawmt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gteetdgzdf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtnahbtwmo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gaohongyu789.top/gtsxoworjd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtkyuuxfer.html

TS:   path.extname("a.txt")
来源：http://hz.yuanzhike.top/gtpdvefqoo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gotoacloud.top/gtjshgdroc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtfmaiwcsd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtizitlxum.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gotoacloud.top/gtdqxxpoiq.html

[F11] 复制与移动文件
来源：http://hz.jqgufenzy.top/gtdkrlxxkp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gttpatqmmp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.andypj.xyz/gtnodpzypx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gttaljfqtk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtwwsfkxdv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuanzhike.top/gtrvwpwnhs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yueranfly.top/gtpqljdzki.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtfasvfobx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtxwivwnbe.html

[F12] CSV 读写
来源：http://hz.cashguo.top/gtcxwgexwd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cqqwz.cn/gtipoukoct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtjpqemkcm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtjztejgif.html

TS:   // 同上
来源：http://hz.havefunace.top/gtvrthjulm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gthjeptycx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jiagoushi.top/gtuyfaylqa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cashguo.top/gtilhypyoy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtcihxbeie.html

================================================================================
来源：http://hz.zhiwuduotai.top/gteofmkeie.html

G. 面向对象
来源：http://hz.wangdashe.top/gtungvxxmz.html

================================================================================
来源：http://hz.sxryk.cn/gtxqovynwf.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtwwrbdgym.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtwrfnzgrm.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtdmbpbaot.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtaavnjbsc.html

TS:   class User { name: string = ""; }
来源：http://hz.ybcxt.top/gtmtnoohsy.html

Java: class User {}
来源：http://hz.wangdashe.top/gtwxjmlrmi.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gtuvpfpref.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtqckudlpn.html

C#:   class User {}
来源：http://hz.ppjwa.cn/gtjdkvgxzf.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gttvlarozb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnxiangtu.top/gtsgodptmn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhijiandao.cn/gtgxoeltbl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtxrjweebx.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtfdmghgou.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtrlqyuydp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtldfhgwvr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtkndipibj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tanke756.top/gtnkcosxjy.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gthojtkjaq.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtmcybecja.html

PHP:  public string $name = "x";
来源：http://hz.sysykeji.top/gtiocppgwy.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtbxgijehc.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gtjhhckdqv.html

Java: private String name;
来源：http://hz.mhx1999.top/gtirjchatx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gterpzhyvm.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtppewajtu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.havefunace.top/gtbzaobylm.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtzxttxtdz.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtojzvthjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gteyiyqcfm.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gtsbljuwpb.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gthewnzent.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gteeylpjew.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtbbvzgxpk.html

Ruby: def greet; @name; end
来源：http://hz.9152youxi.cn/gtmxqeskmz.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtyqgvfzpy.html

[G05] 继承
来源：http://hz.smart0.xyz/gtquyoopqh.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtimsdxnel.html

PHP:  class Admin extends User {}
来源：http://hz.daxiang520.top/gtddcfjkgn.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtaiejatve.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gthkeatfgk.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gttkkwhcop.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtkawcixxa.html

Ruby: class Admin < User; end
来源：http://hz.ivvv.top/gtinufepen.html

C#:   class Admin : User {}
来源：http://hz.hammf.cn/gtdmdkwdlq.html

[G06] 重写方法
来源：http://hz.xinyue.icu/gtzcpwsern.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtbvtzkvmd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtvaywesam.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtlciqlbvh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtbuowcvab.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gtdgmdjnlu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtgkddizff.html

Ruby: def greet; "admin"; end
来源：http://hz.zhiwuduotai.top/gtxtkmfoop.html


<!-- 参考信息 -->