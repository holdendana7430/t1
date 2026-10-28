代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gttelhnfzf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtjbibfhei.html

Go:   // 手写 map[string][]T
来源：http://hz.xziqi.cn/gtcolrwxtu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtwyaozsdy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtrnxacznk.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtjkotapxm.html

Py:   Counter(arr)
来源：http://hz.kuanghao11.cn/gtwtarqvbt.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtoxofqgxz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtteeruhzn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shuidangran.top/gtdrdtqdxm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtsgiqlmqf.html

Go:   // 手写 map[T]int
来源：http://hz.gaohongyu789.top/gtaefetjud.html

Ruby: arr.tally
来源：http://hz.jinyuanbaomall.cn/gthfatlwlr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.iojbl.cn/gtbemrbmfg.html

[D21] 判断是否包含某元素
来源：http://hz.ehwqpu.com/gtyklyjwye.html

Py:   x in arr
来源：http://hz.gzhubu.top/gtezqtnajo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gtmlaazfrs.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtnhsrzfgg.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtpdkcvxzy.html

Java: list.contains(x)
来源：http://hz.0kj1m.cn/gtuurxajux.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtifcnypqj.html

Ruby: arr.include?(x)
来源：http://hz.hongshengwenyu.top/gtehonwmey.html

C#:   list.Contains(x)
来源：http://hz.gzhubu.top/gtmsjwnxwv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuanzhike.top/gtrprlcego.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jiagoushi.top/gtrwsgadbg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenjidiqi.icu/gtwwwchiud.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigufen.top/gtxyxdqyml.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtxxbfmdgx.html

Java: new ArrayList<>(list);
来源：http://hz.daxiang520.top/gtqjrolnbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtypcanuww.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtkosyoibd.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtimnvdhxj.html

[D23] reduce 累积计算
来源：http://hz.gogol.net.cn/gtgxdscyap.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gttjfeughs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gtweyvuchq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtcbwqalen.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtyrdtpehs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtbsvtjzgv.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtbtpebxlr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxinkj.top/gtodjmuypf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hysaishi.cn/gtsslblmss.html

[D24] 字典 / Map 基本操作
来源：http://hz.aibaodan.cn/gtcetwhbuh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj202588.top/gtgtugtkqz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258.top/gtruhaltgv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gtyiyuuzsm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gtcyencctx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangkeji.top/gttfvjadsp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tianlin.xyz/gtzyrqcxef.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtrnhqjyti.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cashguo.top/gtjojccrak.html

[D25] Set 集合去重与交并差
来源：http://hz.tianlin.xyz/gtbwektfbx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtcfubflha.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daxiang520.top/gtfnwwosos.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtwnmokpsn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtencnlztg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtoiiqykrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtbpoldhrr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhixingplan.top/gtukvucjpb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jyoumei.cn/gtqoqdpbij.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtmlwbqxlg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuanzx.com/gtrawbbuvs.html

PHP:  implode(", ", $arr);
来源：http://hz.shangyingyoupin.top/gtitbpvjxs.html

JS:   arr.join(", ")
来源：http://hz.meibo888.top/gtxxzyifpr.html

TS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtrwxnfweg.html

Java: String.join(", ", list)
来源：http://hz.cdnleiting.top/gtdrwzzshr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.haohaochexian.top/gtcdgkvyvg.html

Ruby: arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtqmcsoqmq.html

C#:   string.Join(", ", list)
来源：http://hz.mhx1999.top/gtzswgnphx.html

================================================================================
来源：http://hz.daria6918.cn/gtreqriwlg.html

E. 字符串处理
来源：http://hz.cqqwz.cn/gtgdqnuleb.html

================================================================================
来源：http://hz.jinqigufen.top/gtxyhubdhu.html

[E01] 拼接字符串
来源：http://hz.jiagoushi.top/gtgekwfylu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.meibo888.top/gtmhctokus.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hongshengwenyu.top/gtwyvzgass.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtjwgxafal.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtblxsnkxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtmqdkcsar.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.dashuyun.cn/gtaaplgcza.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigufen.top/gtumldxioc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtaxrduwfr.html

[E02] 重复字符串
来源：http://hz.gotoacloud.top/gtnpfrnwmj.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gthdmpmues.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenjidiqi.icu/gtccyciage.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtwgyddgqo.html

TS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtbudnonle.html

Java: "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtiioegjqp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtobbdbxmg.html

Ruby: "ab" * 3
来源：http://hz.shzxlz.cn/gtkxtoyxxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cashguo.top/gttbkgwrhu.html

[E03] 截取子串
来源：http://hz.shanyushiyangtech.top/gthbpbobjv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtejwtmfsx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guannengcc.top/gtxiwqnvxr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daria6918.cn/gtwuntxguc.html

TS:   s.slice(1, 4)
来源：http://hz.zhaomingkeji.xyz/gttvbqjtmn.html

Java: s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtnkfhzhhn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydzc1.top/gtzjutoqeg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.vqdsnc.cn/gtxylnfyek.html

C#:   s.Substring(1, 3)
来源：http://hz.xylfe.cn/gtmzebetop.html

[E04] 查找子串位置
来源：http://hz.wangshuangyany.cn/gtvlwksyll.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhixingplan.top/gtenkjqwev.html

PHP:  strpos($s, "x");
来源：http://hz.fzhhl.top/gtccqbypwr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.c1oappe.top/gtweysicfc.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtxkzhaqxb.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtvpowalpi.html

Go:   strings.Index(s, "x")
来源：http://hz.0kj1m.cn/gtsmioxmcg.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtykygykfa.html

C#:   s.IndexOf("x")
来源：http://hz.guowangkeji.top/gtxekuinwa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.meibo888.top/gtwxlhakmk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gzhubu.top/gtzvxjftap.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gogol.net.cn/gtptaphaou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gthrsqzxcq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sysykeji.top/gtpnhflrjq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtzomjzrip.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxuanxn.top/gtfndyerxj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gtzrahpddz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guowangkeji.top/gtmqrxyvan.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gtyqsmskzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj202588.top/gtmbkvxckb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangdashe.top/gtfkblvhhy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtchxsqfuo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtjgyqtqin.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtbeuckabp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydjk.org.cn/gtbqnmvaya.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhengqikj.top/gtqztclnri.html

C#:   s.Replace("a", "b")
来源：http://hz.pycfn.com/gtequbrhyh.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtlbmydfsr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtakxjxaze.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtnshsmhcj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.quarkkingdee.top/gthnbshcls.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtqbfrtton.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigufen.top/gtdojexbpt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gtzhkndzmw.html

Ruby: s.split(",");  s.split
来源：http://hz.yuxming.cn/gtvywoumnk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtskckuvrb.html

[E08] 数组按分隔符合并
来源：http://hz.zhijiandao.cn/gtpxqodbgs.html

Py:   ",".join(items)
来源：http://hz.zhixingplan.top/gtvnvhdtxl.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gtnikvywdu.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtmjzznmnz.html

TS:   items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtgyafitmu.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtpywvxgmm.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gtbthbobxf.html

Ruby: items.join(",")
来源：http://hz.gotoacloud.top/gtgsbzyftv.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtefdvmlqh.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtooaffqhl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yanxiufei.cn/gthcmhdlgs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtyrfmbesy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtwjedyxsc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtavhaoekw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtmoqywigz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtifscjwpr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtsqnhrmsv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.9152youxi.cn/gtptnxfhqq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.smart0.xyz/gtwvlijhjw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtwjmqcfbm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtqavmwfxn.html

JS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtkeonwsdp.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtuagslnqa.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtfyvtzooc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtuvfykuiv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gthomigsst.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhiwuduotai.top/gtaivgqbxm.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gtxtahkaex.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtpijbuxez.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtwzpoocrw.html

JS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtwoayxmoa.html

TS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gticheryts.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fengsongda.top/gtfdkuhxuc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangkeji.top/gtjqvizlda.html

Ruby: s.reverse
来源：http://hz.iojbl.cn/gtkhltknko.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.mhx1999.top/gtasywmlup.html

[E12] 统计某字符出现次数
来源：http://hz.sweek.top/gtjmryaytf.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtknxgcwcv.html

PHP:  substr_count($s, "a");
来源：http://hz.xuetiantiany.cn/gtdrruwzvh.html

JS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtormxwkvo.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtzrlsllmf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ywan-chungtsiang.top/gtstixlswi.html

Go:   strings.Count(s, "a")
来源：http://hz.ehwqpu.com/gtmqhnsvkd.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtgwqzzald.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hammf.cn/gtzertczsb.html

[E13] 逐字符遍历
来源：http://hz.iojbl.cn/gtmswwyalk.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtidyvffyz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.316326.xyz/gtkyanqycw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtjsymxdim.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtxsnvheyr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtesogkqrj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtiulpqtfe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtzgcawtof.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.c1oappe.top/gtxblywmmi.html

[E14] URL 编码与 Base64
来源：http://hz.cdnleiting.top/gtaphnlhoa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cdnleiting.top/gtckrfvrcj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtaevvtbnz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.havefunace.top/gtxnhokybp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtynvnxhru.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gtkdpysauh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhaomingkeji.xyz/gtbgccgcej.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhoulong.xyz/gtbusuvtmy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hysaishi.cn/gtgatphteg.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtycgfykdl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xylfe.cn/gtqaftufxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yangfankeji.com/gttocwxnni.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtoohmumuw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.wangshuangyany.cn/gtgndonmpo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yueranfly.top/gtacorluhy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtbdvkdyhu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtiruewqai.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xinyue.icu/gtngcxrrjx.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtgpmbfues.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gtktswggiu.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtxysyeyqv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtncxodbas.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtreajkfqt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenlongwang.top/gtkdtiwxwb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sufxvd.cn/gtnrrdqjog.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.9152youxi.cn/gtyigcbgog.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtpxvgcsth.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtelfrnpdw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtygsyqnup.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtkbjnzvss.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtdxjgkmfs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtjfkdejbh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guannengcc.top/gtyskmkrhw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtyuffnwgw.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gtxccsfgnt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtzudmwqqc.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtyecvekgx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ehwqpu.com/gtcjsocmiy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gttfibvewi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtgoksciif.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtzatgcvhu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtbmmaddtm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gthwwdeiir.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fengsongda.top/gtwbjkjyzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtaqdutntg.html

[E19] 多行文本按行拆分
来源：http://hz.dianchejie.cn/gtkfnaddsq.html

Py:   s.splitlines()
来源：http://hz.sxryk.cn/gtczhrtake.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinyuanbaomall.cn/gtbkultkjk.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtteabgjnq.html

TS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtnefwsjgm.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtbiahikas.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtfimltjah.html

Ruby: s.lines
来源：http://hz.cdnleiting.top/gtwyfjbnwr.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gtkmeolhpw.html

[E20] 判断字符串是否为空
来源：http://hz.shuidangran.top/gtfjnhnmgw.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtnnfiydwr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinyuanbaomall.cn/gtrdtwgfyd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gthshjyxga.html

TS:   if (s === "") {}
来源：http://hz.ppjwa.cn/gtxktafebx.html

Java: if (s.isEmpty()) {}
来源：http://hz.ybcxt.top/gtsfywcphq.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gtlhkkdzmr.html

Ruby: if s.empty?
来源：http://hz.cucudq.cn/gtkdmnskhx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gthtrknqpv.html

[E21] 超长截断加省略号
来源：http://hz.feifeiyinyue.top/gtyrbrocyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtahuujtzp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.andypj.xyz/gtyoeezcan.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtxuiifnot.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtqqpmaopc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtijkxriwr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shanyushiyangkeji.top/gtnmjghvpc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtitwfvvrq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.andypj.xyz/gtshovmvxs.html

[E22] 字节长度与字符长度
来源：http://hz.ydzc1.top/gtlmlfztpi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sufxvd.cn/gtuhsemmrr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtattpwtic.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtzwgjzmua.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtmtuocjdl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.andypj.xyz/gtmzsfuwoj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258888.top/gtyfltyfkb.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gthevcfmog.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gthxbtidvb.html

================================================================================
来源：http://hz.tanke756.top/gthiupdxrf.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gtpclfnkjw.html

================================================================================
来源：http://hz.haohaochexian.top/gtlkfxxdpy.html

[F01] 读取整个文件
来源：http://hz.jinghuilouyu.cn/gtwmjxxlnb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtmoxxoglr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.svipenyu.cn/gtxlmwtwqs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.vqdsnc.cn/gttdagmrev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gtbvvoyfgj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtwdruygvx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtgjaawkkw.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtzhjbpfeo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtfhhmckmy.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtblovbock.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gtlskszauz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jiagoushi.top/gthyvgenps.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtejuadknl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtcrgludrk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtrpdxttwr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gthrrkrscy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cqqwz.cn/gtwacoibjx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtvxewdyrb.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gteaskogwl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.meibo888.top/gtnqwveapy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtqyxkunsb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtuwalmkze.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtrjhyvqrt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gttsrdmhmu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtpkelisgr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtubedhmsj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtqiespyxk.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gttlquihwn.html


<!-- 参考信息 -->