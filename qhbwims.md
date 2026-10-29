代发 wailian999

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gnqdxreka.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/giqaziude.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gepsjvmpw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gsadehisc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/giyueujnz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gxbdzskue.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gfukgxyva.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gfvhpqmar.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gtpdnyzuy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gtutljsij.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghqzhdbwi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/grzffhwte.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/glxmsmdaf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gglliqlml.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghijscjsa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ggvjdjibw.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gqvwrpvph.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gcssafglk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gngcpiqjw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gapdqggdo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gpoeeivmm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghaqwbqik.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzofxayob.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gnvqtnpty.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gpefndcwf.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gvwcelbfz.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gfsgewvke.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gczlqhwfd.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gzeghkqru.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gbczscwaw.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gwxmtzevj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/glzkcjxwo.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/glnhvqtjd.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gbtrghyul.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/girwbpnkg.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/grnwklpgk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gncnyoqxe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gwpxcxusz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gvxgxykof.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gaciioimr.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gaxgxqyau.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gpwyveyrh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gslblmxpy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gcgonsmwg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gibsfwjpa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/guurkcnrq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gnjipjflm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gkgpxebda.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gohorrihz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gbvpzrrrz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gitqjgozb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbxadymhd.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gyutzrkyu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gobbmjjfc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkptudowz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmqurvtoi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gmrncoham.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gwaebuhyh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gikktscao.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gefxkwsif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gxhkaaere.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giqrjkgst.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gmbxjaezd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsyxlyiku.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gfqddrkca.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gezkhhbux.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gevrqsbxc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gblxagbhy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gagxpuhyx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdgbtjqxd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/glwsanwdd.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gystehqdy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzdafpnvs.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gjcnacbdz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gademxvbw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghepnfucm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/grtrladpt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxbpdnqoa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvyrkdsn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gkbxgemej.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gyiupfvtf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gqdxrwzgl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gpdoylodn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ggebbfxxt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gapxkilym.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grpmqaqvz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gnbwshwit.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gjzsinowl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gvrkijfea.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gcucnujtt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gnndoldgi.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gddfcrumw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/geedulifr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gcoxkdtli.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gnfexvdze.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gekdifyle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gpxjryrps.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gcnwynnaf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gelogonsu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/glepcpgnd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/ghyfsecgk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/ghrtyfjhz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/guiikbijr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvhtmdn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grmybmkkf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggwaaslrb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gpbuphpmi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdcnfauzg.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxxoognyg.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gznqjekpg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gconqzsss.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmsduchel.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gunzrtcxe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gneuxicdj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxkgyzajk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gefkuoery.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxqbvndge.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsssfwbkg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/guskusehh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gciposdwh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gfbsdtzpx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gkdmmyplr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gjnbutrgi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gggvbydwc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gzkjgieuu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/geumyaapf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gykhygjfw.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gmvhlkgxv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gzenfovln.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/guslrxtcn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjskeglne.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gpofmwrqw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gmeiycjcs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gbzoxmwld.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gefirdzgh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gkwfssbwc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gosuyegmy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdomjuqas.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/giqxpczur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ghlpuhbsd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gvpjidylv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gssfqrgoi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ggoabhzzw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdyfokvwp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gpasnoqfl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gsghxwwvk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxojwhxvj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gwamdnrqb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glhpsmryy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzybqyakw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gtziajwfd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gneurimel.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjnbaxrji.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxghrrhzy.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gejxygtfh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gnamadwtc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gklmelnay.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqqwekzjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxzjiqaev.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gvhbwwqaa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gkywfuqxk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjvzcwrml.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gmmnecqsf.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/grgtybvqj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gaejtopmq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gcofmfpoo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gmbgaizug.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gjzmxkejt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gggpmvcte.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gymlbltuw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gmlyaeoaq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gihpiupeb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geusqboyu.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gyuvjeqoc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gytdyzvya.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gtcaayvba.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gbxthqsjn.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gujsyqfoz.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gzwmkashg.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gwrwfxqqp.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghbzjkedr.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gcwutypib.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gjhkakdtc.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggiisynvg.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gjzkihbfa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/getuikmnd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/goflqigcu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gqfmlspng.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gsnagyunb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gpjdurvdf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gdfkywjtx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwavnybic.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gjyhasnji.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gncwmujmf.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gzuvuvfsx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gtanztlvt.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gjdqyctsh.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/giunojjkw.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gklhyrjiz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gqzibmswy.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/ggqnjrbom.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gosunwapy.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gkoezatuw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gnepytsho.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gcusfouon.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grqaoykqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggqwtutcs.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqsxqaxfy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gszxwvjbs.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gjbnizztz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gmxffsprs.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/grlyuyipv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gfifnzxjb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gniqtogjg.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gluepukaz.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/geigzpfxc.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpmxhjkbf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/guythjzvo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gibdxlqwn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpdbfmijp.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/grjkhchat.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gvbvdtjqq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxtazfmno.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gewxkgsgd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnprphzaz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gzfaeoxoz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gaxbfneha.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gvlofvsht.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/givlybils.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gjdgtpmex.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gtkbmbdnx.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gvrynhdnl.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gucyegonk.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grmtrboic.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gptgvrptr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gzggaptyy.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gdybheznf.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyhrkwqzc.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gosmbzein.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gdwxwdebc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbhozlrfx.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gkdqzafus.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gdtwocban.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/guzrbouod.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gdqbrgwee.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gxcsdwtmg.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gfzjkkbhl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gocjdlrhi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gzuvredjz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/glclzyvsj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gsqjxydlr.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gvmifwhud.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gpxqeygdf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gyllngscq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gtkefqnjy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghrcvoccu.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gutcrcpym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gykfelnsp.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxrliozhz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/goosliilm.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gntjfvchb.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gxqaduepc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gcymyuxoa.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gyklfpfcs.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gybnonrnp.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gdliainau.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gjuwazmta.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gprxsrkys.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gchjvvjjy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gvwitbacm.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/goaofgadv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gzffelxjj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gzskvlzsj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gcqfucufj.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gyfrzdlax.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gnfretaqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gukyzwxjj.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjhqpombg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqpnwvbup.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghrwwwxqc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbuijxvnf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gntuprsff.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/geiexsioc.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ghimhjpti.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gfeooahzt.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqhzumzav.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gsltmansl.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/giayvkegn.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gazvfyakw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/guqnbyith.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gapxuhaye.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gbslswdku.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gbipumlrp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/glcomfikh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gsakbmdzu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gvpnhdvll.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gihhejdgg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/giiymmtwk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gasyzlfuv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gswioyigv.sHtML


<!-- 参考信息 -->