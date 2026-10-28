代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtwqjvvhyq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtzuatxhzx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtsilnhhnd.html

Go:   // 手写 map[T]int
来源：http://hz.yangfankeji.com/gtdjesktdp.html

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gtagmceqqc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigfzy.top/gtfzmsqyvs.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtclerieee.html

Py:   x in arr
来源：http://hz.andypj.xyz/gtwkuuliqe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.52xcode.cn/gtcteddsiq.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtunkvwhly.html

TS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtpjwqyijc.html

Java: list.contains(x)
来源：http://hz.c1oappe.top/gtyuhrqbii.html

Go:   slices.Contains(arr, x)
来源：http://hz.jlsjyb.cn/gtnmotxafe.html

Ruby: arr.include?(x)
来源：http://hz.sufxvd.cn/gtvwpsdtip.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtbsqkgrvc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangdashe.top/gtmdiwqiig.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gttuyluucq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cucudq.cn/gtfzksnmdc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hammf.cn/gtubyzrpqb.html

TS:   [...arr];
来源：http://hz.xylfe.cn/gtspsyxyrt.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gtkjtukhbf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.bjfxy.top/gtnoymekid.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhiwuduotai.top/gtozbeuatx.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtgnnotovr.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtgypjjiws.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yongpay.top/gtkptlhlyg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnxiangtu.top/gtipvxaort.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtkwobzuuo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtinxfyhcf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtdkhegadz.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtlsisknqs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yongpay.top/gtxtgsodjy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guowangkeji.top/gthdkntqaj.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtjtxwfeqv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtlosmjlub.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxinkj.top/gtfrigpjfi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtfcncmfpd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtatggzqpw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.0kj1m.cn/gtcfuewqbg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shangyingyoupin.top/gtiuzvptrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sufxvd.cn/gtsezzuoha.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xinyue.icu/gtzqodxzzp.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtsjdufqcj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtqoahjykz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gzhubu.top/gtpdaemndj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtdknyohqq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtbgdphltk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gttamagjvm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gthxgbhmhv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtgpkbxell.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.52xcode.cn/gtnszlxxix.html

[D26] 数组转字符串
来源：http://hz.zhixingplan.top/gtlioppbwn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cheryme.top/gtsvoghvcx.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangkeji.top/gttxumzpnu.html

JS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtanyyipvn.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtohfdbnzc.html

Java: String.join(", ", list)
来源：http://hz.jqgufenzy.top/gtoltseaeu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuanzhike.top/gttgrbuwbi.html

Ruby: arr.join(", ")
来源：http://hz.quarkkingdee.top/gtmejwflvp.html

C#:   string.Join(", ", list)
来源：http://hz.zhiwuduotai.top/gtpvoknjmc.html

================================================================================
来源：http://hz.zhiwuduotai.top/gttchccrgi.html

E. 字符串处理
来源：http://hz.zhiwuduotai.top/gtwaetnxtg.html

================================================================================
来源：http://hz.tian-w.cn/gtvgkbupvq.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gthdxqzthm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yangfankeji.com/gtnzqqoxqw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtumkufmzs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtgvaekwoy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtnxrcbttk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtekmsmgui.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cqqwz.cn/gtpoibdihx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtrlicdqjo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtxpyuaowy.html

[E02] 重复字符串
来源：http://hz.daria6918.cn/gtbugmywxk.html

Py:   "ab" * 3
来源：http://hz.yanxiufei.cn/gtuuimzjjs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tian-w.cn/gtnotejfoo.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtgrctrgrh.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtfvhxarri.html

Java: "ab".repeat(3)
来源：http://hz.zycfv.cn/gtzpjypvga.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtrgbluswj.html

Ruby: "ab" * 3
来源：http://hz.sxryk.cn/gthlzacqjw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtmmeqmioi.html

[E03] 截取子串
来源：http://hz.jiagoushi.top/gtydbiirsl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtpawvansf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.c1oappe.top/gtgpofeaec.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yvedp.cn/gtvytgqels.html

TS:   s.slice(1, 4)
来源：http://hz.cashguo.top/gtnfjgjopl.html

Java: s.substring(1, 4)
来源：http://hz.pycfn.com/gttzdhvvem.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gtzecxkvrq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtpgkgnhqd.html

C#:   s.Substring(1, 3)
来源：http://hz.dashuyun.cn/gtongkdyvz.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtiugqbrcd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fengsongda.top/gthuheinfh.html

PHP:  strpos($s, "x");
来源：http://hz.dianchejie.cn/gtoymlayat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.vqdsnc.cn/gtjrtgxmrv.html

TS:   s.indexOf("x")
来源：http://hz.mhx1999.top/gtekimxdbj.html

Java: s.indexOf("x")
来源：http://hz.haohaochexian.top/gtocuzcmzx.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtaiqhhhqj.html

Ruby: s.index("x")
来源：http://hz.yj20258888.top/gtmfjqpbui.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtdiktoqvn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gttbgspjsk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.52xcode.cn/gtgzmekubg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtdtoblbma.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtkacrllds.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shangyingyoupin.top/gtfrfyhano.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtkzvmaura.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtwsziqsds.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.bjfxy.top/gtnhrlifjk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.c1oappe.top/gtsfnhpwfb.html

[E06] 替换子串
来源：http://hz.xingfuxueyuan.xyz/gtebixvrrn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtqpqjwgrn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.9152youxi.cn/gtrcghktkr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtitttpkxy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtacshxpsv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtxrdqbskn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhixingplan.top/gtdbghxyuj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gtisjxnxzz.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtdaovvwvw.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtxhzqcxll.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtyicawzvt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gtvuuquzih.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cashguo.top/gtgynmdqyd.html

TS:   s.split(",")
来源：http://hz.9152youxi.cn/gtdqexxwln.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtynxirkmj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ivvv.top/gtkffydnai.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtrjkskddd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jlsjyb.cn/gtwtgggkrb.html

[E08] 数组按分隔符合并
来源：http://hz.haohaochexian.top/gtlkqzazwg.html

Py:   ",".join(items)
来源：http://hz.daxiang520.top/gtlbeqgejx.html

PHP:  implode(",", $items);
来源：http://hz.jiagoushi.top/gtevygfmga.html

JS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtievfijro.html

TS:   items.join(",")
来源：http://hz.chenzaomai.com/gttqdvivbo.html

Java: String.join(",", items)
来源：http://hz.ivvv.top/gtyirnatib.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtosgeklhv.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gttdomqpux.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtkuzpxiyy.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtfzojhqwh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtoiehocmc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xziqi.cn/gtbyvmwtkf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gttteswmbt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtuovdgrei.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gtcjxwxtut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gthinnqkdd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.svipenyu.cn/gtanbbefha.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hfpthk.cn/gtjkmtkcca.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtdhqtdxob.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gtfgzcnytq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinyuanbaomall.cn/gtpbtemtnj.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtocwskfku.html

TS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtdzncfcse.html

Java: String.format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtynjcpdsu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gtmwtfipok.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gtejqvqzsv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtyuxsjwjq.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtmsrahjtx.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtllnyyhrs.html

PHP:  strrev($s);
来源：http://hz.yuxming.cn/gtdgvpkpbm.html

JS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtyprtnpve.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtefpryfmh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gturijgxho.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtcfriignr.html

Ruby: s.reverse
来源：http://hz.jinyuanbaomall.cn/gtpxtcavwx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtwvlsfora.html

[E12] 统计某字符出现次数
来源：http://hz.bjfxy.top/gtsgsaefkj.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtynsghiqi.html

PHP:  substr_count($s, "a");
来源：http://hz.yj202588.top/gtphejhgjc.html

JS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtwmegjqut.html

TS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gttlrfitaw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhengqikj.top/gttyyitysf.html

Go:   strings.Count(s, "a")
来源：http://hz.jinyuanbaomall.cn/gtgvgyoqao.html

Ruby: s.count("a")
来源：http://hz.sysykeji.top/gtqsmpepfh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tanke756.top/gtxrzrxysi.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gtlvbmrngw.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxinkj.top/gtajhzvavs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangtech.top/gtuardsebp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gttxbrzdlm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtyiiyvhxo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ppjwa.cn/gtchfgaruc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jiagoushi.top/gttgtwaijj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258888.top/gttqawxmfc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtlfwvvose.html

[E14] URL 编码与 Base64
来源：http://hz.daria6918.cn/gtoovwyhsc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtgrajgopw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jianghu66.top/gtbccfbhil.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gtdhescetd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gotoacloud.top/gtfzmcygux.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sweek.top/gtoimawufe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtesgdjaam.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtpdfbmsrd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.9152youxi.cn/gthenyxlsa.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydzc1.top/gtjlxcoiel.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtkoovccqk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtyilagswv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtvxwzikoc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtgakmtxau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtjyrpttzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtnmwstgcu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtzyuuupzp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtcbrdmgfg.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtizcqsbbp.html

Py:   f"{1234567:,}"
来源：http://hz.shuidangran.top/gtpvanlpst.html

PHP:  number_format(1234567);
来源：http://hz.ybcxt.top/gtrajfblcc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtdgqfqiam.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtmgxkisxq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hfpthk.cn/gtdqxstwni.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tian-w.cn/gtekmyepbq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hywenlv.cn/gtkokqtonn.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gtfhghmtgr.html

[E17] 首字母大写
来源：http://hz.tianlin.xyz/gtaplznzwp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtifvynllv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtbrckhrvq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtqaeuyvtr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtxwksoets.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xingfuxueyuan.xyz/gtyahvhptx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtbyygwbbi.html

Ruby: s.capitalize
来源：http://hz.yvedp.cn/gtlsnnqyqv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtkhsqncch.html

[E18] 模板占位符替换
来源：http://hz.yuanzhike.top/gtseyunnvl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj202588.top/gtszhxoist.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.feifeiyinyue.top/gtamqxgrlm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gterbgfnul.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtuctbwrum.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhongyouzk.top/gtjjmhmdzk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtivdegrrl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtgnkvmjlr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gtwwldenzp.html

[E19] 多行文本按行拆分
来源：http://hz.fengsongda.top/gtcrhtibib.html

Py:   s.splitlines()
来源：http://hz.dianchejie.cn/gtrvpeukka.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtiurdsfcx.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gttnoabcbb.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtiqgrovmo.html

Java: s.lines().toList()
来源：http://hz.sxryk.cn/gtxfhzrrvq.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtxgvuijmj.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtosiwxhcu.html

C#:   s.Split('\n')
来源：http://hz.yangfankeji.com/gtezlljfjh.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gthwoyycaa.html

Py:   if not s:
来源：http://hz.jiagoushi.top/gtoymlswao.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtbtffpgdv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daxiang520.top/gtzvkgvrpk.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtejmajufj.html

Java: if (s.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtmoqhglpw.html

Go:   if s == "" {}
来源：http://hz.0kj1m.cn/gtpiqobqge.html

Ruby: if s.empty?
来源：http://hz.sufxvd.cn/gtvpbosjbr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yueranfly.top/gtxrfddrbx.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gtxdqsrgqw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinghuilouyu.cn/gtesefqyyg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtfmllplfd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtgczacfpk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtxvnzwhwm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gthqiuypiq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnxiangtu.top/gtaadslyvl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gttnqryklc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtiarhjzih.html

[E22] 字节长度与字符长度
来源：http://hz.cdnleiting.top/gtozuaulpi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.quarkkingdee.top/gtrciiiusf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtokskuvob.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtypyiwyft.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtugquiocs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.52xcode.cn/gtyvlpnban.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhengqikj.top/gtdlyblprb.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gtecprpndv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtckmbbost.html

================================================================================
来源：http://hz.fzhhl.top/gtwsdxpnij.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtqwsdqeef.html

================================================================================
来源：http://hz.smart0.xyz/gtwkavymzb.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtnxfmnbsn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtgdgpklhf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gtcwgpmuzg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenzaomai.com/gtqcisghmg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtpaegrpis.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gthhfotkdm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jlsjyb.cn/gtrgfdwblr.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtxismkxql.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xylfe.cn/gtdkgqwefl.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtqncrifoc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtthzccvsp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nwbrower.top/gtpkihdysu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtdaotdbvp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gthzlrplcp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtcpxgivkr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gtlyllafoi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shangyingyoupin.top/gtxiralogj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtrlzmtzmi.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258888.top/gtwvuostye.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gtdvzvbhbe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yongpay.top/gtntvjihhj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aizwys.cn/gtdieesoed.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtsdprcbrh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtuypocqar.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aibaodan.cn/gtqpoeknbp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sysykeji.top/gtkxcepgjj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gttuylahxs.html

[F04] 追加写入文件
来源：http://hz.wangdashe.top/gtffxcaajp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtlzvxorex.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shzxlz.cn/gtjpylgdaz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtavdrjwiv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtwfwlaqby.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ppjwa.cn/gtncbiaawj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hammf.cn/gtfqwzcllj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtxugxvjpm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtvzxinjti.html


<!-- 参考信息 -->