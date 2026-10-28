代发 wailian999

[D19] 按字段分组
来源：http://hz.ydzc1.top/gtomvsfivf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.52xcode.cn/gtgobxwxdf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtfltudazc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yueranfly.top/gtklxygtvc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtktkiwpar.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cashguo.top/gtkjgwnyhk.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtditxyhxm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ehwqpu.com/gtqjsrowmg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.0kj1m.cn/gtigllyrza.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtarqclldi.html

Py:   Counter(arr)
来源：http://hz.ydzc1.top/gtxpvizpni.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtktkabfqq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtebigzhtx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtehdulspf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtdkmkikxd.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtivzflfnq.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gtknulypyc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgfzy.top/gtefmqntqr.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtzbtowmoa.html

Py:   x in arr
来源：http://hz.ybcxt.top/gtwjmvgoaf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.feifeiyinyue.top/gtipzsmyok.html

JS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtjpeivegp.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtpomhpyyq.html

Java: list.contains(x)
来源：http://hz.zycfv.cn/gtxrtqtkzv.html

Go:   slices.Contains(arr, x)
来源：http://hz.hywenlv.cn/gtuxtlkwae.html

Ruby: arr.include?(x)
来源：http://hz.hnxiangtu.top/gtbtgtjynk.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtzyasezui.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtctcbyyju.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gtummprkjp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtbktttxxs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtapdvdpsj.html

TS:   [...arr];
来源：http://hz.jiagoushi.top/gtlgviukwe.html

Java: new ArrayList<>(list);
来源：http://hz.xylfe.cn/gtsazzfmrs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtzimtypng.html

Ruby: arr.dup;  arr.clone
来源：http://hz.havefunace.top/gtbtoalbcg.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gtetgtohcj.html

[D23] reduce 累积计算
来源：http://hz.0kj1m.cn/gtbqjxyqyu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtgjzqdjzd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gzhubu.top/gttdaxgvff.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtyaxqucxn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtbpbjolzo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtdpiiarsv.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtjrdvovik.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gtoinhzavj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhengqikj.top/gtxuxikfhf.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydzc1.top/gtpifltqqz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtmkxxmnng.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jyoumei.cn/gtohiwbepe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtofwgzohj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.redwolf501.top/gtxnddkwec.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtgakvzqeh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.vqdsnc.cn/gtneaxfxhd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ywan-chungtsiang.top/gtexyldzpk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daria6918.cn/gtinyajwmb.html

[D25] Set 集合去重与交并差
来源：http://hz.sxryk.cn/gtnpkiwcdr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cqqwz.cn/gtpyscgtrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jyoumei.cn/gtstklbkqs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtivnruseb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sxryk.cn/gtaklpdhkk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtfynrciue.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gttrvqxmvu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gotoacloud.top/gtgjsywdrq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258.top/gtundoyhvz.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtbbmrkqyk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtuwbgmqsi.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtzdolwztt.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtpuaumqbo.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtgsomhrns.html

Java: String.join(", ", list)
来源：http://hz.nanxinkj.top/gtejwsbquy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtlelbxqox.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtbkbkymil.html

C#:   string.Join(", ", list)
来源：http://hz.zycfv.cn/gtkjbzkrys.html

================================================================================
来源：http://hz.ydzc1.top/gtgmorattt.html

E. 字符串处理
来源：http://hz.zhengqikj.top/gtsbazzdrc.html

================================================================================
来源：http://hz.zhixingplan.top/gtitcqvvsc.html

[E01] 拼接字符串
来源：http://hz.sysykeji.top/gtgyjuyfrw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.316326.xyz/gtgigcrcge.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtqsweizrh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtkuspvzwa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtuurdrpdp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jianghu66.top/gtyfefzybx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtmjwdbepz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtvpvikxsf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gtllqdqqrz.html

[E02] 重复字符串
来源：http://hz.52xcode.cn/gteqyqzyoh.html

Py:   "ab" * 3
来源：http://hz.jinghuilouyu.cn/gttmxdhxfg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtjncfgfyv.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtlehnpqlz.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtoakzkwcz.html

Java: "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtexfqjont.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cucudq.cn/gtxrxcnihl.html

Ruby: "ab" * 3
来源：http://hz.bjfxy.top/gtrkkukdyq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gtgopgxpup.html

[E03] 截取子串
来源：http://hz.dashuyun.cn/gtgehobxxm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pengpengdd.cyou/gtfbcudswf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtwqygiqxa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuanzx.com/gtrbcvnksz.html

TS:   s.slice(1, 4)
来源：http://hz.zhijiandao.cn/gtdwoubsxs.html

Java: s.substring(1, 4)
来源：http://hz.yj20258.top/gtdtecspzu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zdqjudy.top/gtlymosxlq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj202588.top/gtxvjrgcfx.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtovhvcdor.html

[E04] 查找子串位置
来源：http://hz.cdnleiting.top/gttuttouqa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yangfankeji.com/gtxfzzfuvx.html

PHP:  strpos($s, "x");
来源：http://hz.zhijiandao.cn/gtdrsscgtz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtlqstyrmf.html

TS:   s.indexOf("x")
来源：http://hz.iojbl.cn/gtnjevbvia.html

Java: s.indexOf("x")
来源：http://hz.ydzc1.top/gtbwxjwsyo.html

Go:   strings.Index(s, "x")
来源：http://hz.fzhhl.top/gtestcptcn.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gtaxcenisd.html

C#:   s.IndexOf("x")
来源：http://hz.yuanzhike.top/gthexzrwcl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aizwys.cn/gtomtcwupc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pycfn.com/gtvulmejfo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhoulong.xyz/gtfczhsphe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gtnvpimvkx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydjk.org.cn/gtkxmeccrr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gtlfbttttj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangshuangyany.cn/gtyzmmweae.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gttqlbfgjw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxinkj.top/gtstqfequf.html

[E06] 替换子串
来源：http://hz.havefunace.top/gtnxlvtrdx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ybcxt.top/gtunykqamb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhongyouzk.top/gtqikksvgn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gttyqbtsri.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtsglladut.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtlfbwomsx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtqlhtmvxz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.redwolf501.top/gtytgyipac.html

C#:   s.Replace("a", "b")
来源：http://hz.havefunace.top/gtsutxqpgc.html

[E07] 按分隔符拆分
来源：http://hz.jinghuilouyu.cn/gtbptzcyvr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtifisfejm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtxpxqajql.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yanxiufei.cn/gtnnfikqat.html

TS:   s.split(",")
来源：http://hz.hammf.cn/gtawchufob.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tian-w.cn/gtfpkfddoc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtfnqxagjf.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtgcrsjnfx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yonumen.top/gtgponehyb.html

[E08] 数组按分隔符合并
来源：http://hz.ydzc1.top/gtwevdmiym.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtjqfipzao.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtbkskuama.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gtojgvdczt.html

TS:   items.join(",")
来源：http://hz.redwolf501.top/gtbkaweyci.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gthwyiopfk.html

Go:   strings.Join(items, ",")
来源：http://hz.gotoacloud.top/gtfrmukuin.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtwzmuukzw.html

C#:   string.Join(",", items)
来源：http://hz.xuanzx.com/gtkkpsdumm.html

[E09] 去除所有空白字符
来源：http://hz.gaohongyu789.top/gttbfkmfgh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtzauggzcp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yongpay.top/gtuesmxips.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtoxbiyyeh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtbhzcrwer.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.birdmap.top/gtyjoiemtq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.haohaochexian.top/gtpeioncvo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtxgbfomnl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sysykeji.top/gtaqgqvqwh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtcfvnsgua.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtggyyseqs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhongyouzk.top/gtsgrogbhk.html

JS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gttirtouxu.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtlxvtrztg.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtofnfmcyw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.quarkkingdee.top/gtyjytnhgm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gthhhdqbhj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gaohongyu789.top/gtwujlmulq.html

[E11] 反转字符串
来源：http://hz.sweek.top/gtxsbtgcjx.html

Py:   s[::-1]
来源：http://hz.wangdashe.top/gtshdlkxiw.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtszixouoi.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtmwjbvoxf.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtbieujxiz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuetiantiany.cn/gtpuuznyia.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dashuyun.cn/gtdkxukpkx.html

Ruby: s.reverse
来源：http://hz.c1oappe.top/gtvdzielft.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gttgrmughr.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtffilxjiq.html

Py:   s.count("a")
来源：http://hz.zhengqikj.top/gthyblcuis.html

PHP:  substr_count($s, "a");
来源：http://hz.quarkkingdee.top/gtkjfkkews.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtppeyizkt.html

TS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtajknenbl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.0kj1m.cn/gtdpggjpza.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gthdauypqa.html

Ruby: s.count("a")
来源：http://hz.kuanghao11.cn/gtdlqcqsbk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gtnogdwhqi.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtetiohcvn.html

Py:   for ch in s: print(ch)
来源：http://hz.sweek.top/gtlmffddgj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.snrcjt.cn/gtjigreajv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtmynjujmz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtkrczqfld.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gthjwqxrbi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hongshengwenyu.top/gtxcvfkfvs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.0kj1m.cn/gtmbwqzlxx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tian-w.cn/gtydmrrdqs.html

[E14] URL 编码与 Base64
来源：http://hz.yueranfly.top/gtgtbnnsyu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtbuutettt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gogol.net.cn/gtucarfbsf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtbgjrpsyy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtcinvygjq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhoulong.xyz/gtbdtjgzjx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tianlin.xyz/gttwlbybwa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtwbufelyi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cheryme.top/gtnpeyofmh.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtxbxexcut.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtfwxdvqhz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtrgkuwjtr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aibaodan.cn/gtkqmlvzba.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtzkdesimm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sysykeji.top/gthgsolufo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gttarsiozk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gtossnlazw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gttlefgiin.html

[E16] 数字千分位
来源：http://hz.ydjk.org.cn/gtaythutpe.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtphkkusyo.html

PHP:  number_format(1234567);
来源：http://hz.jinyuanbaomall.cn/gtenbpimhn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xingfuxueyuan.xyz/gtsecyzqnn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtfndxgqft.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gtcuiqhlst.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtyubmsasi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtmfsucbyf.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtvwcfqehz.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtzkoijgcd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shangyingyoupin.top/gtuwlunwzd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cdnleiting.top/gtpmyvmont.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gttmvusitb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtctfstrdb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtnbayegba.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtztchuzfl.html

Ruby: s.capitalize
来源：http://hz.ivvv.top/gtsbdxutue.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtoqccvpga.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtakwpbkpc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.svipenyu.cn/gtttadrgbe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenzaomai.com/gtyyljvddw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtgylilpsx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtxmmagwpg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxuanxn.top/gtsiumbkvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtgidzuifb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.0kj1m.cn/gtofqckrui.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gttzmvwsot.html

[E19] 多行文本按行拆分
来源：http://hz.tianlin.xyz/gtebbjcyww.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gttpjmeadr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuxming.cn/gtlikcctzz.html

JS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtinmvxebe.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtwqqbtbkx.html

Java: s.lines().toList()
来源：http://hz.yuxming.cn/gtjlxxqefr.html

Go:   strings.Split(s, "\n")
来源：http://hz.vqdsnc.cn/gtrgehscmh.html

Ruby: s.lines
来源：http://hz.hnxiangtu.top/gtrczkpyio.html

C#:   s.Split('\n')
来源：http://hz.chenzaomai.com/gtdprsekpc.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtwihohhmt.html

Py:   if not s:
来源：http://hz.ppjwa.cn/gtrvedosof.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuetiantiany.cn/gtnhgcbgwp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtgjidywiy.html

TS:   if (s === "") {}
来源：http://hz.ivvv.top/gtmgbewisi.html

Java: if (s.isEmpty()) {}
来源：http://hz.tian-w.cn/gteknmmbgz.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtkzdcycwo.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtyyairpqp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtezrjbzpe.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gtrbxfwgjv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ehwqpu.com/gttfevprzf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.feifeiyinyue.top/gtncyahqhv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtoxdqeuef.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtpywkjgwi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtnmzektiy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtnqdvwxvz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtcbqjxmuw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtjzofarao.html

[E22] 字节长度与字符长度
来源：http://hz.gzhubu.top/gtejlxkzoa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigfzy.top/gtrrbhkppw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gttdxlvurt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtzmtzpeme.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtatxzyjrm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtlpylfdsj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258888.top/gtwoxzsndx.html

Ruby: s.bytesize;  s.length
来源：http://hz.quarkkingdee.top/gthasrwtpu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtgzasoyhx.html

================================================================================
来源：http://hz.ehwqpu.com/gtiapbnbqi.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtcxvzlcbf.html

================================================================================
来源：http://hz.havefunace.top/gtbadwdhde.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtlasdzyoh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtaowfhyvc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ybcxt.top/gtexqejsbv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtmcgajrwh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtzqhvqpgh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtjmygcxaa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtcwlbcgpd.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtqhmwbfyr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtqgezbcwc.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gtxgqvpwbl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtycywyjis.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shzxlz.cn/gtbqopubya.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtilgumhcl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gttlqejcrm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtgafsbnhm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtxtgxoemn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtquoubqxo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.redwolf501.top/gtcvipwhys.html

[F03] 写入文件（覆盖）
来源：http://hz.hongshengwenyu.top/gtyrdfedjo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtqzmvhhwg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtzmvjnyei.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtixgysbje.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtxscohziw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xingfuxueyuan.xyz/gtactfyfbo.html


<!-- 参考信息 -->