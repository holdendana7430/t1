代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3msfgeebe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3feajfkyg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dkyylmmo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnqvtddz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3lubzxdhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wpixpblq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sxbnuaex.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jbxefclv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kdnhhrim.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yayeqdxa.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kxggdebq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nfdahgul.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sszphcgh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvutgybt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szjhiqsf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3enoeaxrj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eltleyti.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kbjagrbr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bgrerqas.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cylslhba.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nobvegtn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lvjquwtk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3thwntcud.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3czqbwbik.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qprfzbbk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xderivea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fcyytmim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wmqpzevr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxqrxrpq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oqlzobre.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wysjeups.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3icgpanlp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rihihuwx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3plksdaau.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tdyhdfik.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3spufobbh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3irelkdxo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cyoivcfd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ncocrtpg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ndrxwaze.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rvrnqvvm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqrrfbjf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbugtrnq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwfpnvds.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jycstaob.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cryqrjoj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuojplwp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3aabjblan.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3psmjrzew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mgovxrvt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jzevyvff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kqdciibg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dmqwcglu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3yfkflzbl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pmsoknvk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rvcnxtla.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ikmxhifi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsrfhlr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pzoawriz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pofnfxxe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jrbnigub.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ctgwkeho.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xabncmap.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yjoeclsg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rjnaleoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkshkanj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nmovttae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tiskmftj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwrgzpjb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ajohoyum.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwuwekqi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xjxludwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xsddnrth.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ueurcqiu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vioztsqs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eivcxooh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vlijhkui.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3meymptup.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3znzaiauh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfxrmbv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbzhbleb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uzihobvv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3faxlwjgk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3eowlmyaq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lornjijs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tqzqccno.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ivpctegp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bmtovsom.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dqzzgxtj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zmxirevz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3slscsuzl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ffzimhrp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tupohxpa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cuhfwndt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cyzacibu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nmzebjcs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ofslwpom.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bjrgbrdp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3brdjotrh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nfcddwnn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dqbrrvth.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ylbntatc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyzuqoz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ckwtrmof.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yghrqrnw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ynieojuz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ebvxbvxn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqotfjyf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htbjvpnt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eqlypiyj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qtimpnpq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdoavyt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsickevc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3oruxkcxo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfaoxcre.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hjsjxkbp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfbairfa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmerjkrd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fugsnkiz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvevngzv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsdgnvfh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3goaqapip.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rgsujvgc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wpdjdoiw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pmegjwub.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fcuvxssn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ruclupyq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bkukbbms.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mnezomim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hhhygkhh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3aoqyzdgr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3knytdnuq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qotxdpwk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qcposwqm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sylliuur.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wxwwmgtt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hcmoweag.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dwzufiqr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3khbgmibk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ybkvcxgx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xxyqdlta.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yritxyjb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3waingkzf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tzvjsvol.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cxxrhuna.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbvieeun.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kznflkyk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixlemxog.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ooyppkjk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iipjlzpt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oawziprt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tuatwcxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtfxsuyu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwvgwlqb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lguwwuvs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmkrlkmm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxwkcbhb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wusadswa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3oyooevaf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bokppydi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzhggokb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsiphxrv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lptcbsjw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3djqemntk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qhrwlubv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tosoilps.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3agscmmqb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3usehjbum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pkslilxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3miksrjsg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3agirwzhz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3eqsjucwe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pvysbrjp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zqthlojk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gcoagmqg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qbwfnroy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qanpkmdt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wfpzmdwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqjmkkso.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kojumndn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ewogqhpg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ogvhqikx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcgnkzev.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3nvwxiatk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3veemfzzf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fsojwcbx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpjrpnwd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyjbxnhs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gzsaqwmw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xrfjcwnw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3npbcwnls.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tkcyvihf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyzzbksd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nqxmrcok.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3omygzzod.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yvgrebpg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrwgideq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jniodgcl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dcplpzbm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tchvdqjk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3llyahwju.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3oobxgrhb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nlovpdks.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ehuyabxk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xvytjbyb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3skljoqni.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nxghumzc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yalxoszs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nupmhojo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qavuttzp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tymqquss.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lappixks.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rvglytlk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwuxskae.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dzagnpnk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ngdeskns.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zsvjfcwr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfrmfwun.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzxbypea.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgylxkkv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifqwcpix.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dbrbaezp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrjqbolv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdkonmes.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3iegkukaq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nibozlar.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cdsqrqwg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oatypqnz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lcaavjmi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aespeqiu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ympompbx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3spvvssbc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3eytuyjty.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ackdohks.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rdvacild.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mizwgfky.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eanwxzus.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uxljacli.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yiherrpf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gifqbcjv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fbmcbabn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dibfbcbx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wnmwuflg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wqtraqke.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlqlrdka.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uugyrpwu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmgkpmym.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vchdwroo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zhgacgee.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxcokeaz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgktctrs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yqmtzpla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vbksggbr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3frchsxya.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kmttcjhw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhjjjcgl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ghnypyuu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ndulwndj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sjvowkqh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vpgcukpv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uziwmcvg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ddcjxyyp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gvinxnmz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ppnqanwc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3javzbalx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qtcielos.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ketgpbmh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cziyifkr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rqahtlww.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aiylnnke.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rgduaexn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyborutr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iqmuwibl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hiyhphby.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbnxbeah.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ngwlktqu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jwnuaoie.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aoysslpq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ssczybqb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uphxigcy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guvucsrc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vglovalv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulgngebu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qvlzvkzh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qzcdvbhr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ruxrkjan.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bofwjizn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ahoeanxu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ngqnlnfc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3smjossrl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eztjztyx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3niiyqgeq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cfdouric.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3whazpvhv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vyqrawem.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3sagcwzlq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eydjxkes.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cbvhlnyf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sjzvjbad.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tzazpfku.html


<!-- 参考信息 -->