代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmfvvxd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tesbkrhi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cglxpbud.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2twkqucla.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2oaaryfsm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ipggxeme.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tbedfphx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eeldtgxe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wmchdqqr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pkkpmvez.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ycrlbfkc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wbwuucgd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dywaxymo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvjlgomh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hntmjyux.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jehugkwv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zicmuqog.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2afmlbrxo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qmvrsvag.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qmxkpzmw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mcdoxmbc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cljwqpbo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pjpjjlss.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ckbaigom.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nbtwwmlq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2omdvifbr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lojiachh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfukhvbw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ocphpecg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lwssuggb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mydercoa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rbqgvxxk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gpjddcav.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dpomsjts.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wllphgxj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qanubdxc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bouustcy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2sxesrdis.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jdtdlysg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fykfebbu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bgudyxqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiltaldl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cijgstej.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfxvvvbu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gyjsccmk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2skyjhjvq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rodwtvma.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rppcefjh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bijcciue.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hxhdfmpg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ebrivxxh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wrkyrlnk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ecvvtaxy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hblpvpcu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bujecwwi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmmucxkx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yakasvwb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2whehpwdm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tixkjwyg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dwjvatij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fywiofzb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xxghmakf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tnjvdfdg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lcmmfmam.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cvzaaixf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enbnmnfd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qzpdeuap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oseuwiey.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yeboacpn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rhfdlkmw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uszwtetm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mcnefsdp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vigyuecq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxjttmlj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ybqqiujh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqmiznny.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igzznrvb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvmkidwb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yvyrhjrc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nadwbtge.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iaouylkp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ockiwbqb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2swpqcrpx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtjwkxwx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zuhdulrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qwcyqxdm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mjdeefzx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pkvljjoy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tarqdkji.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nozjyfig.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qdfqfjim.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kfuzxddq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ucdhslso.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jevmvfvc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vnnfhfgl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sobjglsm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xaehvzwj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hkscxojt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hsmossdo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2imamqcda.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tkaawwju.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ettgdoor.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fywypubj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mtzjieav.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dkoxnnma.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nmcmvxst.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfopcxlq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhwlznzo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkeqvwhw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uvzoterm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ulenqbai.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nirlbfak.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccwcujym.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2axivvjew.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krzzetaa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xcdfbdrl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2viuyjfch.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxchsrzw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2edfbhson.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otezkuej.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvbahvem.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkozdaxw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wcvojgks.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfkclqz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bakvktkl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cyxlclvo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wygupiac.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfsggrah.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cepsdbkp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vzupoltf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xqgwdcmd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tdyybjgo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ublrwlti.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkaoqeud.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nrhtrrhw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2omphoyil.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lbsqffha.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ktcyfasi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zlmpaxmj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hsvftixj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tdplykvk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlgtlhil.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uiblwajt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vwkombrc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ckwtvubd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqglgbgj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cfpwypor.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtjkemlf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wufrqvhy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hcpxzwlv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtqvvude.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qhvxfeiv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwahhhms.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyvhqwej.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2axbdnrxm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmtpxmkh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olbdfoow.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iyuhmryi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibrwerxt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yirafxol.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kitoygbw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yawpafws.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqjpepdf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2samwxxoq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mljlrbyo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gofdsbip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2drgrycyc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vesgrtnh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwmhxsi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lumpfpai.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2njhmjasa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sbyvazqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hbxeqieu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nblxdhae.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ydkhvpvm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mphmleod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbpkstku.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lssudpgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsfhuhlq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hysjicsb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zdtckxej.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nwrdgrpz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eldltlkh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2alxqhijr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwxyguyu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qrlrthvh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbvslowb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnivvpfr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2awwqrtdw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ocyzlpqt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rstxndpi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kowemvmb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iujdpbzw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fxnsioqs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yiikemdm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zvojocxv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yrdabvtk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nzoeukqc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xjwvlsrw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qnvdzxnb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2stpbzmox.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kmirouub.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wfnojqad.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lisuurkp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ydkedcol.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kkcfujmt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ijphqqgw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vhwvzqjt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuyuhgmn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cjwopmoh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hrkbxxyh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ldgclria.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kmfhcubu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2epqfbiec.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2duxkhawk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2esziwnim.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2biuddczc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2obcimhmc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vbleplyw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mdhvsxju.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ulbzophk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fzrnsxle.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jipolbxu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wsdoiixa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ksieumae.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qkhirips.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pmwvwmkr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vrdtjpfa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjdhfwso.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xazxiavr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zvqjtcnp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nqixglsr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vbfifqpm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dzditkji.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eietxfwl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kcahmlud.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivczdqiq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uozqteju.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tjjjavkm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kgrlpipl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mxgztljz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nihssptw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eqbtdhup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2sjmltbhk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2elgdmgae.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bkfymfvz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cvklwtbd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mxtmytvo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zepbqpye.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hkoutkhj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qinmujyx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sxqjtfnc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jbylztsu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hjtakfau.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2memcgfcm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jmchcwqy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdeakwad.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nasmnvxm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mqtgdsaq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qgpdizgt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zeunplxe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tpgjencb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gemnjvza.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2geyeqzyf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zodohpru.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fbkwhvgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kkfknuie.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gqstywbt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fipskfsw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tiacykqc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lalzvflv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zrzmkkvx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cnkkyrjk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsqlkbe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xwgltsgk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2obnxuisq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mqhqxezu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2saqxtsel.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icedldul.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aeislnvb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifcheeai.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odxudxbl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egajvwkr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnysvfil.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iqoqnutl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qddegwtp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qkgscxsl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ffohrdgu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2knaylrai.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iimisuuf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wjimqbim.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zplwxbvf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nrfqdrpq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgdpnp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fkcpzwqh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qcbiggjt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xjrxvdkc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gvumrcgm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2adjaxgfn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nywqmudm.html


<!-- 参考信息 -->