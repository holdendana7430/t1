代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.svipenyu.cn/gtiqendjer.html

[D20] 统计每个元素出现次数
来源：http://hz.ywan-chungtsiang.top/gtiauaerik.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gtjktudrrz.html

PHP:  array_count_values($arr);
来源：http://hz.shzxlz.cn/gtstugwbei.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtpqneufmo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtxdwqoroc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gttindtynq.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigufen.top/gtgdmczwwh.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtwqgmymnw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yongpay.top/gtbouuevbe.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtaijjynxb.html

Py:   x in arr
来源：http://hz.zhaomingkeji.xyz/gtvkiqpuis.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtkyktxodr.html

JS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtjahbcekl.html

TS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtwlbkpzef.html

Java: list.contains(x)
来源：http://hz.jlsjyb.cn/gtbcrzwohf.html

Go:   slices.Contains(arr, x)
来源：http://hz.nwbrower.top/gtqzoniise.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gttwtupsvl.html

C#:   list.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtpbfwlsoo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinghuilouyu.cn/gtnxhdlsdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tanke756.top/gtsvfxtfwg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cdnleiting.top/gtevygyrws.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.c1oappe.top/gtorlnxoyt.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtohuvxhmx.html

Java: new ArrayList<>(list);
来源：http://hz.tanke756.top/gtpiepqnra.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtpectfcro.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yanxiufei.cn/gtmlqgsiic.html

C#:   new List<int>(list);
来源：http://hz.ehwqpu.com/gtkhfonjum.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gthvhipcyy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtmbvryzku.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.kuanghao11.cn/gtpcmnzrjo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtdhbtvhid.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtuhqtgamo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gtkwfvjlpj.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtodajalqf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydjk.org.cn/gtpobwxnrv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtpoisscdd.html

[D24] 字典 / Map 基本操作
来源：http://hz.gzhubu.top/gtnvueaeku.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hysaishi.cn/gtuckypppm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuxming.cn/gticbucwoz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ywan-chungtsiang.top/gtfevkyral.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shangyingyoupin.top/gtgyzollzr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtxvmpxdiw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zdqjudy.top/gtcmckgaxo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yongpay.top/gtwtshywvl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtlfbswysl.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258.top/gtubcswxjc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yvedp.cn/gtegrdbame.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtwyoldyok.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtwsyakhax.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nwbrower.top/gtjyyjbino.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xziqi.cn/gtujzsaurl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtksvdrjqq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtmhvdfexw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gogol.net.cn/gtnmogsirm.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtukmwbtwg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtxcahfmeb.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtgbtodzdh.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtifstvzcn.html

TS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtbxgvrbyt.html

Java: String.join(", ", list)
来源：http://hz.pengpengdd.cyou/gtaaadgrne.html

Go:   strings.Join(strs, ", ")
来源：http://hz.mhx1999.top/gtegowkiic.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gteksensrv.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtedysdfzw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtchhxvdwu.html

E. 字符串处理
来源：http://hz.nwbrower.top/gtngjpmexn.html

================================================================================
来源：http://hz.sysykeji.top/gtkqihhfov.html

[E01] 拼接字符串
来源：http://hz.fzhhl.top/gtnjfdpiso.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtmteccxrb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuxming.cn/gtxofpxmys.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtsalrfyzi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtutrurnsw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtsrrusgmb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zycfv.cn/gthfswqude.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gtfjvxkxua.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ybcxt.top/gtexcdjqkk.html

[E02] 重复字符串
来源：http://hz.yueranfly.top/gtnsbqhhhs.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtpshtzvgf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtgrujbfnl.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtxwnonknp.html

TS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gtqcvtqnvc.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtxtnhagdk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yongpay.top/gtjyberbbz.html

Ruby: "ab" * 3
来源：http://hz.jinghuilouyu.cn/gtoulvrmei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.havefunace.top/gtduwaphtk.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtawkemxnq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtbliwniqp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtuzmyedcb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtggrpobxl.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtrxeobqrq.html

Java: s.substring(1, 4)
来源：http://hz.316326.xyz/gtrrzqthwe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtkcbiatgx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgfzy.top/gtxohplyps.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gtipppznrz.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtwgujqvec.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hysaishi.cn/gtnnvnnnzi.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gttxiecjme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cdnleiting.top/gtywsrndex.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtvbxcnoav.html

Java: s.indexOf("x")
来源：http://hz.cqqwz.cn/gtwdtbokqb.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtckusasxa.html

Ruby: s.index("x")
来源：http://hz.andypj.xyz/gttkuxfwcx.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtveyucqvc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cucudq.cn/gtgplnnsby.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dashuyun.cn/gtgsjviypv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jianghu66.top/gtibvrkjmx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtioopsxpa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zycfv.cn/gtwpzusivk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtakbdgdgn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydjk.org.cn/gttjcjzslt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj202588.top/gtnjfxinhq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gaohongyu789.top/gttnarlfoj.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gtejlyesxx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gtvquhogdl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhengqikj.top/gttmvmzgst.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtzvudlllf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtazpwugzg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtwtsngljg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.andypj.xyz/gtnflrnikd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtfjfzehlt.html

C#:   s.Replace("a", "b")
来源：http://hz.redwolf501.top/gtfivpbglp.html

[E07] 按分隔符拆分
来源：http://hz.chenzaomai.com/gttismjccp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cqqwz.cn/gtcfzkjtap.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtreqktyhz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangtech.top/gtkvermrmk.html

TS:   s.split(",")
来源：http://hz.xylfe.cn/gtzefqkgxg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tianlin.xyz/gtbotqyqpw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtoushqani.html

Ruby: s.split(",");  s.split
来源：http://hz.bjfxy.top/gtqycplkzo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xylfe.cn/gtzpknojwl.html

[E08] 数组按分隔符合并
来源：http://hz.daria6918.cn/gteaowpvrd.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtjskwefqt.html

PHP:  implode(",", $items);
来源：http://hz.jlsjyb.cn/gtaotwwgrf.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtircwxopv.html

TS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtazasqxpk.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtybrdhjbj.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtfxngltji.html

Ruby: items.join(",")
来源：http://hz.iojbl.cn/gtjffchpyy.html

C#:   string.Join(",", items)
来源：http://hz.shuidangran.top/gtyqnluwux.html

[E09] 去除所有空白字符
来源：http://hz.xuanzx.com/gtaryrepid.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangkeji.top/gtcvmwpiqt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.kuanghao11.cn/gtrzpakmqy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtydxgcoov.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtgevpzjnf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jyoumei.cn/gtbvkwmmqq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtfsahfzrv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtpogcpkjp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.iojbl.cn/gtiiexommw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tian-w.cn/gtdwxdhslu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gteajglokj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangdashe.top/gtdajtohfi.html

JS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtrepvcqcw.html

TS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtcclstojf.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtveuuzdyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gtrzmqpbzn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtxebgwndv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhaomingkeji.xyz/gtbspfnmkg.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gtstuwtrjb.html

Py:   s[::-1]
来源：http://hz.yonumen.top/gtmulfigcm.html

PHP:  strrev($s);
来源：http://hz.guowangkeji.top/gtzlegotcp.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtguarxfqi.html

TS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtrzahxxwc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtxnowdtto.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cheryme.top/gtsjsyzqte.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtknqxyrum.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtvkpdlihf.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gtfvifplgx.html

Py:   s.count("a")
来源：http://hz.jianghu66.top/gtmdfqxjmj.html

PHP:  substr_count($s, "a");
来源：http://hz.xingfuxueyuan.xyz/gtiulnbjny.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtpvfivcax.html

TS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtyiatulaa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhengqikj.top/gtvwdxuvew.html

Go:   strings.Count(s, "a")
来源：http://hz.shanyushiyangtech.top/gtharpvqop.html

Ruby: s.count("a")
来源：http://hz.shzxlz.cn/gtudxxpqgg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtzktwwlmm.html

[E13] 逐字符遍历
来源：http://hz.gotoacloud.top/gtdprlcbwx.html

Py:   for ch in s: print(ch)
来源：http://hz.fzhhl.top/gtugvmkonf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ppjwa.cn/gthlihzfzt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtcytqhmrq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtfctljugo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daxiang520.top/gtljvlrplf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtkvlyihzr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gthdygblrq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhixingplan.top/gthbrdllwj.html

[E14] URL 编码与 Base64
来源：http://hz.hfpthk.cn/gtrnnwtlvs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgufenzy.top/gtvmzpujpz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxinkj.top/gtyxxuqxho.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtohtibgya.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtuewkwxnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangshuangyany.cn/gtogxnddmv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuanzhike.top/gtswcbzpeh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtvolkcgen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gaohongyu789.top/gtpkqsupie.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinyuanbaomall.cn/gtnrkfieio.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pycfn.com/gtnrvghypm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtselfdwci.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtlhhxzfpl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.smart0.xyz/gtqhaivdge.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.0kj1m.cn/gtstojiuzi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aizwys.cn/gtfhjveqba.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gtsegtjiuf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gtuyqxsnmr.html

[E16] 数字千分位
来源：http://hz.ybcxt.top/gtkelemnev.html

Py:   f"{1234567:,}"
来源：http://hz.dashuyun.cn/gtjdsflgqr.html

PHP:  number_format(1234567);
来源：http://hz.fengsongda.top/gtdbanacot.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtcmuvwndm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtltpwhqkg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gthizcomwy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtynakgrrj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtggejisdj.html

C#:   1234567.ToString("N0")
来源：http://hz.meibo888.top/gtuakkrfjc.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtjnkqtaaf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtwdrpyxag.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtalugjumq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gtntuadbjg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gteysslqxq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shuidangran.top/gtodobstiz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yvedp.cn/gtiwnpoaax.html

Ruby: s.capitalize
来源：http://hz.jinqigfzy.top/gthlsngedo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtgbzazcoa.html

[E18] 模板占位符替换
来源：http://hz.gotoacloud.top/gtyrftxmkh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jiagoushi.top/gtwkrwyztv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gtwrdjsbun.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtxkunfkfh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtoginzkbu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ybcxt.top/gtzfcoaofl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuanzhike.top/gtgvtpzzpb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtiocikhwl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tanke756.top/gtoskcjdcr.html

[E19] 多行文本按行拆分
来源：http://hz.dianchejie.cn/gtdphykrew.html

Py:   s.splitlines()
来源：http://hz.snrcjt.cn/gtocrcdrdj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhengqikj.top/gtwvxhiirr.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtduqlfizm.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtvupvanke.html

Java: s.lines().toList()
来源：http://hz.52xcode.cn/gtrvyitwgy.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gtfhcisait.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtlxzakqpg.html

C#:   s.Split('\n')
来源：http://hz.daxiang520.top/gtfmciavea.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangtech.top/gtwazccxiy.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gtivpufisd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtcvudqtsl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtfotftdam.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtfaxtaqap.html

Java: if (s.isEmpty()) {}
来源：http://hz.guannengcc.top/gthahdukox.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtyvqgojua.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtrgzlnbcl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtgnxggqwl.html

[E21] 超长截断加省略号
来源：http://hz.zhixingplan.top/gtwykvauxh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj202588.top/gtzdebfgfs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cqqwz.cn/gtjpzwzbsc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtvxrbncqp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtvnzbagxx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtdervyzmd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gtkpbehjof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtywscvdce.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hysaishi.cn/gtsgsbpaat.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gtrjbcdbwr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.9152youxi.cn/gtmtvftrlp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtakzkxmzw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtoseypdba.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtasxzwhvj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gthkfexpeh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtrvfjdcjo.html

Ruby: s.bytesize;  s.length
来源：http://hz.sxryk.cn/gtvvncgexi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtvpzbbvtr.html

================================================================================
来源：http://hz.0kj1m.cn/gtpoqteilm.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtahwphxws.html

================================================================================
来源：http://hz.iojbl.cn/gtyeoicdeq.html

[F01] 读取整个文件
来源：http://hz.316326.xyz/gtfgkwnihn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtjjloedjt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cdnleiting.top/gtdnvkwxco.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtcbmzkbwu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hongshengwenyu.top/gtdxvmntaa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtkqhymzzi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtexlzegmg.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtkynekrxc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtfhmcjmhn.html

[F02] 逐行读取文件
来源：http://hz.xuetiantiany.cn/gtzzyjzkpp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuanzx.com/gtinmfqpqe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuanzhike.top/gtfkwjppvn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtmghxjwuu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtywecogtt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtjvuwrayt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shangyingyoupin.top/gtkbzbdbbw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgufenzy.top/gtduuhdoii.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtvjdilbcb.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtdpmsgvkb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtmmxjejgt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gteyeadltu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtcotojnpe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtbmpigriz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtpsbrrlre.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtkeebafar.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hammf.cn/gtrhmgppmm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtrkrirtlb.html

[F04] 追加写入文件
来源：http://hz.andypj.xyz/gtgnhshxkl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.haohaochexian.top/gtdkccxxgr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuanzhike.top/gtpwommxwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtriprpwch.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtqdpdxbeu.html


<!-- 参考信息 -->