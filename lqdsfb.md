代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtqujjxpbt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yanxiufei.cn/gthbuccrvn.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtatatarcm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtcvutkfvf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtewgphavi.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtprndofab.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtgsxmkvhu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydzc1.top/gtnsdwhgjz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gtjosdtlir.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.haohaochexian.top/gtbvporhem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhijiandao.cn/gtdnupwopr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gthczihfur.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangkeji.top/gtcwqbejmf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtmvjmrtan.html

[D25] Set 集合去重与交并差
来源：http://hz.havefunace.top/gttlxrulqt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtuomlcndq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.52xcode.cn/gtardopdig.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.mhx1999.top/gtqkcoovhu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtpgmbgodo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nwbrower.top/gtlaciuzya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgfzy.top/gtrbbggvks.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenzaomai.com/gtajuwfppi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cashguo.top/gtckqbwbin.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gtgxpljpps.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtmiipbnug.html

PHP:  implode(", ", $arr);
来源：http://hz.pengpengdd.cyou/gtcmjgcees.html

JS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtarxsjxjp.html

TS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtqwtduayc.html

Java: String.join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtkmfqirbc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.dashuyun.cn/gthhqdskno.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtqitkrppa.html

C#:   string.Join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtjynnkvsd.html

================================================================================
来源：http://hz.yueranfly.top/gtdxflojsg.html

E. 字符串处理
来源：http://hz.ehwqpu.com/gtrwptcwnn.html

================================================================================
来源：http://hz.yonumen.top/gtpyxgcvhp.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtqawfwgju.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gtbsaimrnu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jlsjyb.cn/gtogywbnnu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gttafgtvbg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtadxvwowb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pycfn.com/gtyejcdukk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuetiantiany.cn/gtlizrxhtg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daria6918.cn/gttizuseao.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangtech.top/gtqbdflyjb.html

[E02] 重复字符串
来源：http://hz.bjfxy.top/gtioywpzaf.html

Py:   "ab" * 3
来源：http://hz.sysykeji.top/gtdoapanjj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtahlfknlu.html

JS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtssxxcbqk.html

TS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gteicndbvt.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtmorxyjrm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gthbnvrjhc.html

Ruby: "ab" * 3
来源：http://hz.cheryme.top/gtqoqxxcuq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtscrsvsti.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gttqtfkzvz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtkfrmyxoo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gtrquycvap.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtqsbkfmdh.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtzpstauuy.html

Java: s.substring(1, 4)
来源：http://hz.zycfv.cn/gtsfdjagbc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.meibo888.top/gteyyjdflh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fengsongda.top/gtsitgxcva.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gtnthbklie.html

[E04] 查找子串位置
来源：http://hz.gotoacloud.top/gtnmajiecu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtqmaytefu.html

PHP:  strpos($s, "x");
来源：http://hz.quarkkingdee.top/gthjwnrqmo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tanke756.top/gthcjjvypa.html

TS:   s.indexOf("x")
来源：http://hz.hywenlv.cn/gtshsocwko.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtyiawinjg.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gteoaduusu.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gtpozfqhec.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtohbhfiqf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnqzz.top/gtafmtlkfh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aizwys.cn/gtrphddbae.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tian-w.cn/gthkobfwdk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtcnsrsewx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtguvuubzf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtyvjyjonr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhongyouzk.top/gtjjkobdha.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangtech.top/gtkdkumabg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cqqwz.cn/gtkiqbbhgc.html

[E06] 替换子串
来源：http://hz.guannengcc.top/gtpsjcdqto.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtheyfhhgl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tianlin.xyz/gttdfnlzqy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtytzopqan.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gttdifsaif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtspnryrtd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tanke756.top/gtenkfwgpo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtllcxbsuk.html

C#:   s.Replace("a", "b")
来源：http://hz.316326.xyz/gtuajejuyj.html

[E07] 按分隔符拆分
来源：http://hz.andypj.xyz/gtyfeswxqf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhengqikj.top/gtheyfmnwd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenlongwang.top/gtzbvdrhrs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.guannengcc.top/gtjmtmrpor.html

TS:   s.split(",")
来源：http://hz.guannengcc.top/gtlvfvolxp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258.top/gtqnaajeeb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtolgzkuir.html

Ruby: s.split(",");  s.split
来源：http://hz.yanxiufei.cn/gtmnlxpaba.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.havefunace.top/gtewmmlpua.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gttdxpomrl.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtenwhmdxo.html

PHP:  implode(",", $items);
来源：http://hz.hywenlv.cn/gtcdncwbyk.html

JS:   items.join(",")
来源：http://hz.chenzaomai.com/gtrvohldmg.html

TS:   items.join(",")
来源：http://hz.birdmap.top/gtpygpmaoy.html

Java: String.join(",", items)
来源：http://hz.tanke756.top/gtyspcddhs.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtdhqwcusk.html

Ruby: items.join(",")
来源：http://hz.xziqi.cn/gtpieuuyyq.html

C#:   string.Join(",", items)
来源：http://hz.sweek.top/gtlzvphrbf.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gtilcxdklj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gtvnmzpnlr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtjmvzovqg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtdhoqhcsm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtlllevcvg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cashguo.top/gtcmvgdzyn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinyuanbaomall.cn/gtrqpzcaew.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtlqygiajd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cashguo.top/gtyitcjmvp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtfrjgdlsm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhongyouzk.top/gtdkigrndr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtlwyelbjd.html

JS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gteqmqabtb.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtmlolhqgx.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtybicfion.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.daxiang520.top/gtajhyadko.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtzcjxyiyw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtezbmuzay.html

[E11] 反转字符串
来源：http://hz.jinghuilouyu.cn/gtqrrazkin.html

Py:   s[::-1]
来源：http://hz.wangdashe.top/gtzrzkhqhn.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gttfzbymcs.html

JS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtegansdmz.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtzsdhvwdk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.mhx1999.top/gtuhzjueqh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gtyynapqey.html

Ruby: s.reverse
来源：http://hz.xuanzx.com/gtkxntaypy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtmsrfndbi.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gtpkcdexmb.html

Py:   s.count("a")
来源：http://hz.nwbrower.top/gtuvfovzdk.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gtbvxypdza.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtbrztnxid.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtnqvvibsu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtwnkekhxo.html

Go:   strings.Count(s, "a")
来源：http://hz.cheryme.top/gtthkpxlqy.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtlyhwnycw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guannengcc.top/gtwzyjteuo.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtbcbdiwcb.html

Py:   for ch in s: print(ch)
来源：http://hz.haohaochexian.top/gtarryjwzz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtrnhmxktp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtcjgssrjh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtyetcckop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tianlin.xyz/gtnvjgsghz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.mhx1999.top/gtanhrpdkl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yvedp.cn/gtdtujzicr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtymngivzi.html

[E14] URL 编码与 Base64
来源：http://hz.zhoulong.xyz/gtfkonhxdp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gteyrswjqe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtcfzfucvw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.meibo888.top/gtiqukqdbv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xinyue.icu/gtojhczkmi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gogol.net.cn/gteelunifd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cucudq.cn/gtbecnahkn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtkcbalttm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtlthejylu.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtaezgauaa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yangfankeji.com/gtndisankc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtodisrfqs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.haohaochexian.top/gtxbmpjmwe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yanxiufei.cn/gtxaojikco.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtnylibzuw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sysykeji.top/gtamdcztbh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ppjwa.cn/gtrtzvquzr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.haohaochexian.top/gtpshxpose.html

[E16] 数字千分位
来源：http://hz.yongpay.top/gtgavrlypi.html

Py:   f"{1234567:,}"
来源：http://hz.hnxiangtu.top/gtuqxnlikq.html

PHP:  number_format(1234567);
来源：http://hz.chenzaomai.com/gtblrpyixa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtlfmfjeny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtazzzkiqm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtnzwaqabp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtkgxnxcio.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.9152youxi.cn/gthyurhtaa.html

C#:   1234567.ToString("N0")
来源：http://hz.yangfankeji.com/gtbbehzitw.html

[E17] 首字母大写
来源：http://hz.chenjidiqi.icu/gtnpnijczi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtxkhapael.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydjk.org.cn/gtqhfyqanw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtpwlhjcjd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtjlahsuuq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtubyuxchz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtqkdvcwov.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtbcgscobb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigufen.top/gtpntnhgnn.html

[E18] 模板占位符替换
来源：http://hz.cqqwz.cn/gtnfbekeog.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gteatiqzsb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daxiang520.top/gtoykymwbq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtwhlthpcp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtewdmfcyw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtnktvbqfp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daxiang520.top/gtflvsmukc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtpndvfjea.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gtpubwilib.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtiwktcoqi.html

Py:   s.splitlines()
来源：http://hz.birdmap.top/gtnzhqqwag.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.316326.xyz/gtlmhjqexq.html

JS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtaavvsvbx.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtbpitrunb.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtxwjgcsvh.html

Go:   strings.Split(s, "\n")
来源：http://hz.yueranfly.top/gtqktlesjx.html

Ruby: s.lines
来源：http://hz.havefunace.top/gtlaynwddn.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtesgetkao.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtzonjbgng.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtsgftilyd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtggjckqkf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gzhubu.top/gtxouqyuzi.html

TS:   if (s === "") {}
来源：http://hz.jinyuanbaomall.cn/gtjqucoewo.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtgvjivbkj.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtdwhbjkkd.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtbojvzywq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtdjdxcqta.html

[E21] 超长截断加省略号
来源：http://hz.yj202588.top/gtmkwxhsgl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sufxvd.cn/gtnghenoqp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtubcpxgwj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtbdmfptku.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtlrsyoltk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtubpciipt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gtjmbxfxmf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.meibo888.top/gtnhhozkek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtnriozlmo.html

[E22] 字节长度与字符长度
来源：http://hz.vqdsnc.cn/gtbunntvtv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gtrxlfnsov.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtppthvmlh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtrsvmftex.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tian-w.cn/gthnrvhhhu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yvedp.cn/gtjstqtyjv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtjgzpmhfn.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhoulong.xyz/gtzbfpecpk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtfzsilqva.html

================================================================================
来源：http://hz.cucudq.cn/gtnnozatwq.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtycdyzbvi.html

================================================================================
来源：http://hz.birdmap.top/gtzpdwrbcr.html

[F01] 读取整个文件
来源：http://hz.yj202588.top/gtebfklhyc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gthzczbuat.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtwcetvlwf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guowangkeji.top/gtuzierdbk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cdnleiting.top/gtkmrfpwlk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtmwdlavxj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtkssoajym.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gticncjisp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtlztmvnkh.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtwscvdvhk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtxfrysrju.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gtmfkuafop.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gthjaigrdf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtxpuewusd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtfjtuoerv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hongshengwenyu.top/gtsdlrnrmq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.kuanghao11.cn/gttqapcpsu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtyxfpppad.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gtxgupnihh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.bjfxy.top/gtmgxsikbw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtqypervxz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtrxyhmcnj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtcmtzbeic.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.mhx1999.top/gtoalzwtpa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.havefunace.top/gtcqrrmwst.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.andypj.xyz/gtonhpzqca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zdqjudy.top/gtzlcfuynn.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gthwoitdxh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gtfofloqoy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtvetjhoqp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtjqsjyocb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtnkfyujdm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ehwqpu.com/gtzedarjcw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gtdttvwbem.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtgjgfwlti.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigfzy.top/gtvmhjzpbc.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtikxbzcrh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtlkbdfild.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtydmpqbpb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtzrjjahmu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gthwarjqxg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtiklsqqyg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtjernvikz.html

Ruby: File.exist?("a.txt")
来源：http://hz.meibo888.top/gtuiwoicwd.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtqbsngsik.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtcwatcade.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtyhgandai.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtaodwfmtr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gthrovrnlc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtdflvfvin.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtsbzxmibu.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtgqrcdroh.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gtqpfzlvgt.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtrjivbckw.html

[F07] 创建目录（含多级）
来源：http://hz.yj202588.top/gtdggmjcmx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtavyqgamq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.52xcode.cn/gtopecnlvn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtfargyxxk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtsyrauepq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtinxuyrhx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gthouahoyu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.316326.xyz/gtrewhhlmt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yangfankeji.com/gtbkzgxbpa.html

[F08] 遍历目录
来源：http://hz.jinghuilouyu.cn/gtwylsgxye.html


<!-- 参考信息 -->