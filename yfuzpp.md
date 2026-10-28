代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.ybcxt.top/gtihfxzyta.html

JS:   arr.includes(x)
来源：http://hz.zdqjudy.top/gtssqhvoxf.html

TS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtjpiofwif.html

Java: list.contains(x)
来源：http://hz.jlsjyb.cn/gtkxjqaduc.html

Go:   slices.Contains(arr, x)
来源：http://hz.snrcjt.cn/gtjwgugaht.html

Ruby: arr.include?(x)
来源：http://hz.0kj1m.cn/gtaemvlgjt.html

C#:   list.Contains(x)
来源：http://hz.sufxvd.cn/gtssseobbs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tianlin.xyz/gtcybjjiat.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shangyingyoupin.top/gttztgtxms.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.feifeiyinyue.top/gtorxzcatv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuetiantiany.cn/gtkgialsmr.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtqneqrfjm.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtjavusfuv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtqypmnbyj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guowangkeji.top/gtqqrwhugc.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gthpfjwcwj.html

[D23] reduce 累积计算
来源：http://hz.yj20258888.top/gtxyqultgm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtubhajoum.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuanzhike.top/gtfoheorml.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtkpnnoykw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtlevwgfco.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gteyuhfomc.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gthvndfmnx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yongpay.top/gtynuxyzvy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sufxvd.cn/gtygwaejgh.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gtwiwobikp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtuygxnexr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daria6918.cn/gttjharzxi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tanke756.top/gtodsewzwt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtcojgxixk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tian-w.cn/gtgnpbpvot.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtbqfwjozg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yueranfly.top/gtrbdtmzar.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gtwxwsierd.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtvubdeqml.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtgxqmswij.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daxiang520.top/gtauhtxjmq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtwqvmkvbm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ivvv.top/gtcvyhtzqq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gtkidkyhgq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtytlpwjjw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtvqtoagsa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtkblaxxbu.html

[D26] 数组转字符串
来源：http://hz.fzhhl.top/gtxguuukwp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.birdmap.top/gtmmjcplzp.html

PHP:  implode(", ", $arr);
来源：http://hz.feifeiyinyue.top/gtrwvduivn.html

JS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtpfdqkqvf.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtamjzqoak.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtmzbmlwtm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtctsthqfj.html

Ruby: arr.join(", ")
来源：http://hz.316326.xyz/gtdpyaogpk.html

C#:   string.Join(", ", list)
来源：http://hz.gogol.net.cn/gtumfhlvun.html

================================================================================
来源：http://hz.hnqzz.top/gtdhjshnuq.html

E. 字符串处理
来源：http://hz.yonumen.top/gtusooofnx.html

================================================================================
来源：http://hz.aizwys.cn/gtyjawyxbs.html

[E01] 拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtetljyrlw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gtwhrcmgae.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgfzy.top/gtpvjpfvip.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtfuzwmokx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtltbipxwi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hfpthk.cn/gthcnpebyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtdjnjaruv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.svipenyu.cn/gtiqvkavcf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnxiangtu.top/gtkstrufog.html

[E02] 重复字符串
来源：http://hz.xinyue.icu/gtefmaiysn.html

Py:   "ab" * 3
来源：http://hz.andypj.xyz/gtwmgwxeeq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gaohongyu789.top/gttoimgmkx.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtwkmfnnlf.html

TS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtgfzzoczn.html

Java: "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtzkmoayyt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangdashe.top/gtgvardwna.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gtvrjtlsub.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtbgdabkpb.html

[E03] 截取子串
来源：http://hz.tian-w.cn/gtcfrffbjb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gtjgdubsbz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtoeffmket.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nwbrower.top/gtgidxijkw.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtpmulyfuu.html

Java: s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtbgcbengc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydzc1.top/gtctgiipxo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenlongwang.top/gtudpqkyij.html

C#:   s.Substring(1, 3)
来源：http://hz.cucudq.cn/gtpwwfffmz.html

[E04] 查找子串位置
来源：http://hz.dashuyun.cn/gtljzrvylz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtbboofctg.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtimqwxqfp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guannengcc.top/gtdeoxtynj.html

TS:   s.indexOf("x")
来源：http://hz.xziqi.cn/gtsoywdcsp.html

Java: s.indexOf("x")
来源：http://hz.hnqzz.top/gtymerxysm.html

Go:   strings.Index(s, "x")
来源：http://hz.hywenlv.cn/gtbasxstjc.html

Ruby: s.index("x")
来源：http://hz.zhongyouzk.top/gtiduzslds.html

C#:   s.IndexOf("x")
来源：http://hz.zhongyouzk.top/gtejodmzow.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.redwolf501.top/gthlnuhdop.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangtech.top/gtpybwddpy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtfugwrvzu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtyohurrdv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xinyue.icu/gtxsvcastz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.feifeiyinyue.top/gtwdgybcsj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fengsongda.top/gtohwrfltt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.smart0.xyz/gtdpavgymz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xziqi.cn/gttpleqrdo.html

[E06] 替换子串
来源：http://hz.iojbl.cn/gthpnjshzl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gtsexvdzgt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtlhfisdcg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtnfdnhyvy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtkdqyufsd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtehzyptjb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtxwwqwxtr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258.top/gtygkvxaib.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtgjazagng.html

[E07] 按分隔符拆分
来源：http://hz.yongpay.top/gtftkeyjjy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yonumen.top/gtbsfnrynl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtgbflxmyp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sxryk.cn/gtuaolkhdn.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtbsbjgbgc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxinkj.top/gtsmmjwafs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gtjvrmphfs.html

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtuyfcwaji.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnqzz.top/gtxwwgpfnj.html

[E08] 数组按分隔符合并
来源：http://hz.snrcjt.cn/gtfszgyvah.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gthekqudwn.html

PHP:  implode(",", $items);
来源：http://hz.zhixingplan.top/gtsoqnqtze.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtzfeipvkj.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtvbxkscoo.html

Java: String.join(",", items)
来源：http://hz.shangyingyoupin.top/gtwpiakqcq.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtxojtuumv.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtfsndnvji.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gtxevfaxrd.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtcecuvrno.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxinkj.top/gtrinzpalq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jlsjyb.cn/gtbcmwuxoe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gthkleigsg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtkbtlrhks.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtcqxgjqvr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.quarkkingdee.top/gthczurcxk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtixwwniel.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenlongwang.top/gtfjokmryd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tianlin.xyz/gtsbuxtqrj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gteurovzkw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sufxvd.cn/gteebisene.html

JS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtgvybmqay.html

TS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtncydmndg.html

Java: String.format("%03d", 7)
来源：http://hz.xylfe.cn/gttclipjug.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtziwcmmzh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtaagmlrkq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtjpxbkmlo.html

[E11] 反转字符串
来源：http://hz.zhongyouzk.top/gteuisnegd.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtthlvljwy.html

PHP:  strrev($s);
来源：http://hz.xuetiantiany.cn/gtpqnutnzk.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtoxhlxfta.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtncuwfdzn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnqzz.top/gtsvdewugt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtfddjtlbp.html

Ruby: s.reverse
来源：http://hz.feifeiyinyue.top/gtorxewqos.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtspdclxgr.html

[E12] 统计某字符出现次数
来源：http://hz.mhx1999.top/gtufoyojhh.html

Py:   s.count("a")
来源：http://hz.hnqzz.top/gtcacmwhfi.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtzkfybfpk.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtxtnbjlsc.html

TS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtdshasvwa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtovvkfjek.html

Go:   strings.Count(s, "a")
来源：http://hz.shanyushiyangkeji.top/gtoqyeseql.html

Ruby: s.count("a")
来源：http://hz.gogol.net.cn/gtdvmzmbga.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xziqi.cn/gtdnkaokei.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtdlqjwrhi.html

Py:   for ch in s: print(ch)
来源：http://hz.ydjk.org.cn/gtiuagewti.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shzxlz.cn/gtyllycqvq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gtxmfwuyzy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtageyctih.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtuqsgwcmw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtavecbrap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shangyingyoupin.top/gtsdibuthu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yonumen.top/gtuxrdidmq.html

[E14] URL 编码与 Base64
来源：http://hz.zhaomingkeji.xyz/gtoqzjtwhv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gtgqrkombh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtfegetppo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtanpaqtow.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gtxdvgjqdo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenjidiqi.icu/gthchktwet.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.vqdsnc.cn/gtcktjwnxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtdqskwhoe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hfpthk.cn/gtfwyftvcg.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtkbkmboxz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtnzcrupyq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtpikdouhh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.kuanghao11.cn/gtiklfmseo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtvnnjlhgs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtgdaugvns.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtwppgebtw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zdqjudy.top/gtzjgdzlqx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenjidiqi.icu/gtmthyrlaf.html

[E16] 数字千分位
来源：http://hz.gotoacloud.top/gtxqjcurid.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtflniswhg.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtighlfdsd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtwxpiyoey.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtbyioegee.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtmhxtilxk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtrajpavux.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gtuiqezbek.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtxomddhxy.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gtnkpvzgxg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.iojbl.cn/gtgebcgsqb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtbsffkiqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtnxswvuwx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gtzkqhfxun.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgufenzy.top/gtyspknkpv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sysykeji.top/gtshpgqmng.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gtwvjqznzm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shangyingyoupin.top/gtizujnqyj.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtcujfmhxz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtaxfwnnir.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shanyushiyangkeji.top/gtmuxeytjv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtsrazridt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ivvv.top/gtbaewjiai.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtqjgjnldq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.feifeiyinyue.top/gtftpfwviz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhixingplan.top/gtegfmdlbq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xylfe.cn/gtzdwgzton.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtihuqbqrb.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtmxyeolnt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.smart0.xyz/gtqgjchrbg.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtkhmjmqgd.html

TS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtkcdcguie.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtaodtpxvs.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gtcaflgdov.html

Ruby: s.lines
来源：http://hz.ydjk.org.cn/gtsmssflyl.html

C#:   s.Split('\n')
来源：http://hz.feifeiyinyue.top/gtaddcbtgd.html

[E20] 判断字符串是否为空
来源：http://hz.hongshengwenyu.top/gtiangpuzd.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gtacbxbmmg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtjduhlgri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shzxlz.cn/gtegplguph.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtxxyhaeor.html

Java: if (s.isEmpty()) {}
来源：http://hz.ivvv.top/gtgldcikzr.html

Go:   if s == "" {}
来源：http://hz.yuanzhike.top/gtklxhzivx.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gtfzejpfhz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sxryk.cn/gtlorstfjh.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtdqiohwbo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtyuowijvg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gtwbyjajsd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtlgupzgml.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtixtuckuq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtxtjkedat.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtiryzwoca.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtzdvsxqpg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtqmcukddh.html

[E22] 字节长度与字符长度
来源：http://hz.bjfxy.top/gtercvlrta.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hongshengwenyu.top/gtdcgnpukc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtdmrqdrkp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtstvpscjg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtywbtnnrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gthzybuiql.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.9152youxi.cn/gtoggxllra.html

Ruby: s.bytesize;  s.length
来源：http://hz.ivvv.top/gtebgxhixc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sysykeji.top/gtpiemrcpv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtozxdthpn.html

F. 文件与目录
来源：http://hz.svipenyu.cn/gtfujeovok.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtahlvowty.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtgcyxhexc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgfzy.top/gtlaytnaso.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtgqxpfmwa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258.top/gtdypxpjqj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ivvv.top/gtixvcyajt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtjedttuar.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258888.top/gtmscllukm.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtlhrekude.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtgafjcfsz.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtbldsfoet.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtfepwwmeh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gtjqrxfjve.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtcyrtzyav.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtgaajdxtr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtpaouxezw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtljwsozvy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtoegezhis.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tian-w.cn/gtmfjewobg.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtsfpbqhxe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gtsyygvebf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtfeeyxthw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtyzfoolcb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtidbeheiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gtxumrrpup.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gtjxtgsnjm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cqqwz.cn/gtbpxeirkb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtjoqlnkac.html

[F04] 追加写入文件
来源：http://hz.yonumen.top/gtffgtflay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtrkecqooi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenlongwang.top/gtvgxzhgnl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtcxyndnkt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtxnlpvyjv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtwjhyvxso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinghuilouyu.cn/gtoiedhrna.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtimquozjq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gtjuhejvxx.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtyfqqvwdi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtirbpkwih.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtozwtufvo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtfdiywrcy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenlongwang.top/gtakjrphol.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtrkvltqyj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtbtycuhvd.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtstergevm.html


<!-- 参考信息 -->