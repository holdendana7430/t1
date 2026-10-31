代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ja.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://pn.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://ul.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gz.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qm.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://cd.hahajie.cn

[E04] 查找子串位置
来源：http://fl.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://ab.colortex.cn

PHP:  strpos($s, "x");
来源：http://dw.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gt.szxytkj.cn

TS:   s.indexOf("x")
来源：http://ql.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ef.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://tc.panjiajie.cn

Ruby: s.index("x")
来源：http://id.colortex.cn

C#:   s.IndexOf("x")
来源：http://bl.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wu.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://in.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jy.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rq.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gu.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vi.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://et.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ax.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yz.huixiangedu.cn

[E06] 替换子串
来源：http://sp.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://et.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ds.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iq.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://ik.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lp.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lv.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mf.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://uc.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://dz.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ym.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dh.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gu.nszjky.cn

TS:   s.split(",")
来源：http://sx.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fm.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ah.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://zj.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zf.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://zx.nicolike.cn

Py:   ",".join(items)
来源：http://dk.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://ti.szsharing.cn

JS:   items.join(",")
来源：http://eo.colortex.cn

TS:   items.join(",")
来源：http://ku.panjiajie.cn

Java: String.join(",", items)
来源：http://pk.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://dc.521024.cn

Ruby: items.join(",")
来源：http://iv.9csxet.cn

C#:   string.Join(",", items)
来源：http://ro.newstarts.cn

[E09] 去除所有空白字符
来源：http://rk.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pj.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uk.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://kd.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://iq.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://gc.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tl.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kl.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ur.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://eu.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fp.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://me.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://sc.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://zu.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://ue.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://li.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xh.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uo.haigaiapp.cn

[E11] 反转字符串
来源：http://dm.hahajie.cn

Py:   s[::-1]
来源：http://rk.nicolike.cn

PHP:  strrev($s);
来源：http://qf.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://yn.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://eh.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ik.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mu.huanxung.cn

Ruby: s.reverse
来源：http://vi.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tk.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://nl.huanxung.cn

Py:   s.count("a")
来源：http://wo.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://wl.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://bl.nszjky.cn

TS:   s.split("a").length - 1
来源：http://xw.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yr.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://cq.hnjuh.cn

Ruby: s.count("a")
来源：http://fd.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://rk.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://lq.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://rm.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jf.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://je.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uf.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ap.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rn.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://my.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jf.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://wr.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oz.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qx.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://io.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vj.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zv.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bo.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cc.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://og.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://pd.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://of.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oc.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xr.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eq.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ak.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xe.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tq.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zs.lnxyls.cn

[E16] 数字千分位
来源：http://gx.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://co.asd995.cn

PHP:  number_format(1234567);
来源：http://mk.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yz.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ly.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ks.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jr.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rm.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://wq.huanxung.cn

[E17] 首字母大写
来源：http://db.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vi.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xh.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bx.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qq.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fm.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jg.jctech888.com.cn

Ruby: s.capitalize
来源：http://fl.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ph.nszjky.cn

[E18] 模板占位符替换
来源：http://op.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hn.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ti.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ue.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ce.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jp.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://id.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pd.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://an.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://af.wgjwhj.cn

Py:   s.splitlines()
来源：http://mj.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tu.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://rn.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ie.521024.cn

Java: s.lines().toList()
来源：http://nr.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://rj.newstarts.cn

Ruby: s.lines
来源：http://yt.szxytkj.cn

C#:   s.Split('\n')
来源：http://ba.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://vc.bjjhwx.cn

Py:   if not s:
来源：http://fr.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rr.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ba.nicolike.cn

TS:   if (s === "") {}
来源：http://aq.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://nz.wgjwhj.cn

Go:   if s == "" {}
来源：http://dz.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://uj.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gj.gzmigu.cn

[E21] 超长截断加省略号
来源：http://mp.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ap.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fa.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qv.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uj.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://db.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://fm.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rk.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pl.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://fo.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rq.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zd.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vi.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cu.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vo.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yl.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://wz.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ss.haigaiapp.cn

================================================================================
来源：http://nj.yuexingan06.cn

F. 文件与目录
来源：http://mc.shtwfgs.cn

================================================================================
来源：http://tu.521024.cn

[F01] 读取整个文件
来源：http://jf.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cb.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://au.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://is.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cx.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yp.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sq.colortex.cn

Ruby: File.read("a.txt")
来源：http://en.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://tl.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://nv.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://md.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xo.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tb.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zb.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uo.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yu.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rh.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fg.colortex.cn

[F03] 写入文件（覆盖）
来源：http://zx.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gw.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qs.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hf.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://df.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zq.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wh.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://bu.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wb.huanxung.cn

[F04] 追加写入文件
来源：http://sd.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ev.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wn.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lp.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xv.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sh.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wa.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xf.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rz.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://rf.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vw.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ww.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://as.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://vm.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wk.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jr.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://zk.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://ob.yuexingan06.cn

[F06] 删除文件
来源：http://sa.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://ao.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://id.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gw.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bg.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qj.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://vc.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://ai.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://mh.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://rn.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://el.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://th.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xl.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sw.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nb.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xe.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://og.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dw.huanxung.cn

[F08] 遍历目录
来源：http://rv.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://np.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://df.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://ig.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://it.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zh.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fz.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://bf.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://fv.huanxung.cn

[F09] 获取文件大小
来源：http://vs.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://qe.newstarts.cn

PHP:  filesize("a.txt");
来源：http://dg.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://qy.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://hc.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hw.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mo.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://ir.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://md.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://lu.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ar.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jv.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jq.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://fg.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hh.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aa.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ty.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://dl.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vi.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://od.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fy.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xb.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nq.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://op.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ep.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vp.newstarts.cn

[F12] CSV 读写
来源：http://lo.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vi.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ny.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qc.lnxyls.cn

TS:   // 同上
来源：http://yx.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mn.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fw.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jj.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xm.521024.cn

================================================================================
来源：http://bq.9csxet.cn

G. 面向对象
来源：http://sn.jctech888.com.cn

================================================================================
来源：http://fs.jianghongdianzi.cn

[G01] 定义类
来源：http://lc.yuntaijiaju.cn

Py:   class User: pass
来源：http://xa.gzmigu.cn

PHP:  class User {}
来源：http://vh.huixinmuqiang.cn

JS:   class User {}
来源：http://hl.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://cd.szsharing.cn

Java: class User {}
来源：http://da.nicolike.cn

Go:   type User struct { Name string }
来源：http://zc.hahajie.cn

Ruby: class User; end
来源：http://fi.yuntaijiaju.cn

C#:   class User {}
来源：http://pt.jctech888.com.cn


<!-- 参考信息 -->