代发 wailian999

Ruby: arr.tally
来源：http://hz.guannengcc.top/gthqiwuxil.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtbzrveyan.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gthdilojeb.html

Py:   x in arr
来源：http://hz.meibo888.top/gteawifgwv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinghuilouyu.cn/gtvqqzkjjx.html

JS:   arr.includes(x)
来源：http://hz.yj20258.top/gtbhyxfnhd.html

TS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtnvngnsqn.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtvstpzcxv.html

Go:   slices.Contains(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtichtgzoi.html

Ruby: arr.include?(x)
来源：http://hz.ybcxt.top/gtumbaaehf.html

C#:   list.Contains(x)
来源：http://hz.sweek.top/gtcacsfgpf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yueranfly.top/gtambekcaq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtpaygjfha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtzrrkhiiv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtpfxthjyt.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtiukadmde.html

Java: new ArrayList<>(list);
来源：http://hz.nanxinkj.top/gtuqqipkcb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gtlurutaes.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yueranfly.top/gtjlkwtemb.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtsngsarby.html

[D23] reduce 累积计算
来源：http://hz.shzxlz.cn/gtueqkppsu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pengpengdd.cyou/gtzjuizthy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.9152youxi.cn/gtqiuihvds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtdqshfbzc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtbgsgsons.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cheryme.top/gttcqaunbc.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtzpdldxsh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtbonnpvrw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtloluankb.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gthzjdknzr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.smart0.xyz/gtlgnxuhdr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxinkj.top/gtwexmyack.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgfzy.top/gtsawvdnvw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtbwvwogab.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtftiqqwne.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtczidbyga.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtckvzkzaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtwatrhsgh.html

[D25] Set 集合去重与交并差
来源：http://hz.guannengcc.top/gtahckwutw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tianlin.xyz/gtrzgpqtcr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhaomingkeji.xyz/gtttpemlpt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gaohongyu789.top/gtjyvuolyk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gtkyubdlra.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuanzx.com/gtwoniawob.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shangyingyoupin.top/gtmznjufmn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ivvv.top/gtyxfjwxza.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yanxiufei.cn/gtuydowhbj.html

[D26] 数组转字符串
来源：http://hz.wangdashe.top/gtemicgvhb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gttjpqegau.html

PHP:  implode(", ", $arr);
来源：http://hz.daxiang520.top/gtqaxhxshg.html

JS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtpdqmjlgm.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtgbkuyval.html

Java: String.join(", ", list)
来源：http://hz.haohaochexian.top/gtfcsvwlmi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xziqi.cn/gtdqaggrrl.html

Ruby: arr.join(", ")
来源：http://hz.gaohongyu789.top/gttntvjavp.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtkupydirv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtlletykdu.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtsvvnftur.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjodfsnkh.html

[E01] 拼接字符串
来源：http://hz.yonumen.top/gtrydaceqv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj202588.top/gtxwvybquo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtnibukrbj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtltlypoww.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtnhskwpxe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.316326.xyz/gtdqfhkfft.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtyuymrtkn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtradgghfk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtiktnvjge.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtmdsgaldr.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtbewrvfao.html

PHP:  str_repeat("ab", 3);
来源：http://hz.quarkkingdee.top/gtfisspnwg.html

JS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtyvvkmkif.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtaxqhsiqa.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtplmbqpoy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtnqyilgeq.html

Ruby: "ab" * 3
来源：http://hz.xziqi.cn/gtxifunziw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zdqjudy.top/gtjetgnhwj.html

[E03] 截取子串
来源：http://hz.meibo888.top/gtesyaflrn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtcxotzddy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gtqnkenvnt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtdcnqpfff.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtswvttbfb.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtalobiknt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.andypj.xyz/gtqnkvgdtu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtiqrskoil.html

C#:   s.Substring(1, 3)
来源：http://hz.cashguo.top/gtlgxwkdja.html

[E04] 查找子串位置
来源：http://hz.shangyingyoupin.top/gttdqdthoe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtcarhjssn.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtpffyfjhm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ppjwa.cn/gtrojgyojy.html

TS:   s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtvpkqxiyo.html

Java: s.indexOf("x")
来源：http://hz.havefunace.top/gtxhixhpid.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtyxwbsghh.html

Ruby: s.index("x")
来源：http://hz.snrcjt.cn/gtjhgkmqtp.html

C#:   s.IndexOf("x")
来源：http://hz.xziqi.cn/gtdqchunyz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gtzjpgmxne.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenlongwang.top/gtgnfjhbsm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daxiang520.top/gtpxrntpix.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtmlwvbxrz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jyoumei.cn/gtdrlrpech.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gthqopzjff.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jiagoushi.top/gtejmmrdjo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtrarsqqeh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnxiangtu.top/gthwemlkfk.html

[E06] 替换子串
来源：http://hz.zhijiandao.cn/gtdumfbowg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuanzx.com/gtltjzpfmz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258888.top/gtxbnwgcbb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtrqgcfbsv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtantufvfs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gttysdlwux.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gzhubu.top/gtmnfmpesp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhijiandao.cn/gtibtnrfpy.html

C#:   s.Replace("a", "b")
来源：http://hz.havefunace.top/gtugiliohd.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtlzxzkxnm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuxming.cn/gtfplpxbrk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangtech.top/gtwrpbocpz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhaomingkeji.xyz/gtrhjwxyvv.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtwopogatc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtbknruukk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gthqphuefz.html

Ruby: s.split(",");  s.split
来源：http://hz.guowangkeji.top/gthgwfeiaf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.quarkkingdee.top/gtuurnyuth.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtkswmhdjx.html

Py:   ",".join(items)
来源：http://hz.daxiang520.top/gtafnfmbdb.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtjtanpnrw.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtmhdswybf.html

TS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtitkrqqba.html

Java: String.join(",", items)
来源：http://hz.zhengqikj.top/gttrjkymba.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gttoklyqig.html

Ruby: items.join(",")
来源：http://hz.pengpengdd.cyou/gtjnptamnq.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtoapqkcds.html

[E09] 去除所有空白字符
来源：http://hz.aizwys.cn/gtqfwpnezy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gtfbeysuex.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gtoeowpvap.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtadbdouvw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtcahhkogb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sysykeji.top/gtokrkudrw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhixingplan.top/gtwedisrlg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gtddazxgsj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhongyouzk.top/gttdbaqnrl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtpmsriwen.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zycfv.cn/gtfdtnjfpe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtuonblzjc.html

JS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtzxnaledg.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtwfczzqnl.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtgiezvzpn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtlbmgihep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pycfn.com/gtegwbvvgv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cheryme.top/gtxyijdmzx.html

[E11] 反转字符串
来源：http://hz.zhongyouzk.top/gtpouqhroy.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtbiagqpyu.html

PHP:  strrev($s);
来源：http://hz.zhengqikj.top/gtdchsnviz.html

JS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtasliwuif.html

TS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtqwsvacur.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuanzx.com/gtsvyieszf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinqigfzy.top/gtvzjzqqgq.html

Ruby: s.reverse
来源：http://hz.jianghu66.top/gtwtkyhbjp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtebodqzui.html

[E12] 统计某字符出现次数
来源：http://hz.pengpengdd.cyou/gtqagejovl.html

Py:   s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtzhmtskza.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtbylgires.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtvenxjrkc.html

TS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtvrwfllkt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pycfn.com/gtmiokgarg.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtuznuvfki.html

Ruby: s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtmwjsvurf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daria6918.cn/gtuiynthuu.html

[E13] 逐字符遍历
来源：http://hz.xuanzx.com/gtomtaohdd.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtjqjjchfa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gtfpcoojoi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtyqihazdd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtmrxgzwer.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.c1oappe.top/gtxclcjwsj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtyxwptvqw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gtwmbrpkjj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtazfajydl.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtzzhvxobi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhixingplan.top/gtxebaxgqz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuetiantiany.cn/gtrxogqluv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhixingplan.top/gtjzhokxzc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yanxiufei.cn/gtdaomnxaq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtdyxhcpan.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtcuvddetl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gtavdhsich.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtmebbreoi.html

[E15] HTML 转义 / 反转义
来源：http://hz.yonumen.top/gtxigztluo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gtbukxauqm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtnkynactq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxuanxn.top/gtkuedsfvo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtisadggsw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtvxjifhez.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtnhlqcskw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xziqi.cn/gtqebefyre.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gaohongyu789.top/gtiotviikf.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtihvygluq.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtdoxpxplu.html

PHP:  number_format(1234567);
来源：http://hz.hnqzz.top/gtpcfvfpje.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtsdfatjzu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtyactpehm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnqzz.top/gtcepvfnmy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtdqreljhu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cucudq.cn/gtlfwxuxws.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtexpveppc.html

[E17] 首字母大写
来源：http://hz.ppjwa.cn/gtnzokslgt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtsfvvqqrz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtfayffpns.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtmztkhirk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtzycjytox.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxinkj.top/gtwuznfhkk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtyxumjkab.html

Ruby: s.capitalize
来源：http://hz.yuxming.cn/gtlwavwyja.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtqhgosljt.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtsfkwdbbk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtgqqkpaif.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxuanxn.top/gtazsezxif.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtuctvpbxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtpwadjyew.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tianlin.xyz/gtngkjltix.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtszvgzszy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtzcidwyzz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gaohongyu789.top/gtbcyzblmv.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtjzzndktr.html

Py:   s.splitlines()
来源：http://hz.daria6918.cn/gtynattkzz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangkeji.top/gtpzrxjrbx.html

JS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtynrbzimj.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtradcfcjl.html

Java: s.lines().toList()
来源：http://hz.zhongyouzk.top/gtfgnebhwe.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenjidiqi.icu/gtyxbyyyfr.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtkumskpma.html

C#:   s.Split('\n')
来源：http://hz.xuanzx.com/gtamyaepek.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtictiixsf.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtdiofceac.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hfpthk.cn/gtbomppegf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jiagoushi.top/gtriqkysmj.html

TS:   if (s === "") {}
来源：http://hz.yonumen.top/gthhjtlyfn.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtzatnvqde.html

Go:   if s == "" {}
来源：http://hz.jianghu66.top/gtcpwzfwnw.html

Ruby: if s.empty?
来源：http://hz.smart0.xyz/gtyykrbmjm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtqmhcczpu.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtcmqqizkr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtgnnyoyrk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtirolfquf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtdmpmwgyw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtqbzbgcxf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtybvlzqgp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.quarkkingdee.top/gtsrueramn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtgtejhlnm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtgczalkyj.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtlegbkauy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.bjfxy.top/gtsdekqtcw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtssnmdnjg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtvviojymy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtxcxdegdo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtwtjynyss.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tianlin.xyz/gtrzrcgoch.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtirqqkmpe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ehwqpu.com/gtatwfhvrp.html

================================================================================
来源：http://hz.jianghu66.top/gtgpcmcjxu.html

F. 文件与目录
来源：http://hz.yj202588.top/gtmfolhxmm.html

================================================================================
来源：http://hz.cucudq.cn/gtqrjyvzlc.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtmqkxnfpb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtupawlckh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yvedp.cn/gtdwaolsgt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinghuilouyu.cn/gtlhlofyca.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtzzrxxfru.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtoyxusqyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yvedp.cn/gtaakyjntx.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtdttyoprt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.meibo888.top/gtujqsgrbl.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtwkcfiihe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtydpsuqny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yongpay.top/gtovpvffol.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtbfwmvpaa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtaymetfoy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtecrrxqej.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinghuilouyu.cn/gttpuzvkyq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gtusvzdlgo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.c1oappe.top/gtcwywgqik.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtbginjxzn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhengqikj.top/gtnrnkqage.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yvedp.cn/gtmdksgiua.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtinlffcya.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtoophyctw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtbrgilkua.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.316326.xyz/gtnrzctjzc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cucudq.cn/gttusyouvf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtfmumrbnj.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtrdpkbjja.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.iojbl.cn/gtookywuun.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtuyfpmzfa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtqmpyabfo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtubtvjzjc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aibaodan.cn/gthlllwjgy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtwapgtdcf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtmvjkaich.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gthyokhagi.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtdwhaxgny.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtfwzafwaq.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258.top/gtyesnavgj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtyjaeypuz.html


<!-- 参考信息 -->