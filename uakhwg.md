代发 wailian999

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtqeiygpkk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtqgsndrtd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuanzhike.top/gtnftfkxvy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtnplxnnty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gtxcmasznk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtxkyoecou.html

Go:   // 手写 map[string][]T
来源：http://hz.mhx1999.top/gthccbwdjh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtlczxabsa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtfdhylgtr.html

[D20] 统计每个元素出现次数
来源：http://hz.ydzc1.top/gtrcubprth.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtghlgsvji.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtmcucmtkx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtppayipvb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtbludggcu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtiotdiior.html

Go:   // 手写 map[T]int
来源：http://hz.andypj.xyz/gtoblrqtyo.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtmlrkstqh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gttzsbaqul.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtkvxwipwz.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtajgyrriw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jianghu66.top/gtpoadsoue.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtjkwqtxzg.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gthrfoghfq.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtzmebwmlu.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenzaomai.com/gtrnijzttx.html

Ruby: arr.include?(x)
来源：http://hz.jqgfzy.top/gtegnladiv.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtizqvmgjj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtydhdwxrl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtreigckqd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtexvhsmhc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tanke756.top/gtfujrnwzz.html

TS:   [...arr];
来源：http://hz.yueranfly.top/gtikyswwwa.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gtqmixpdqg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.9152youxi.cn/gtulcfaogr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zdqjudy.top/gtuwawhnxc.html

C#:   new List<int>(list);
来源：http://hz.316326.xyz/gtxfpumioy.html

[D23] reduce 累积计算
来源：http://hz.chenzaomai.com/gtwrnyacrm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtgbskxrmb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtzgmbxsih.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtuouonwwf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtinbruyky.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtxiwdpzxi.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtlkgsvuvm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shuidangran.top/gtcpondcid.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtcvnilxao.html

[D24] 字典 / Map 基本操作
来源：http://hz.sysykeji.top/gtestxtich.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gtgqfdecuh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gttseoooej.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtvxlnnsmk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhongyouzk.top/gtzparpfnk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtcwgcbfsp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtcmtgcmgo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtaetfjbxd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cdnleiting.top/gtjylnoxkg.html

[D25] Set 集合去重与交并差
来源：http://hz.daria6918.cn/gthhloopuw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.svipenyu.cn/gtuiubuskw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.pycfn.com/gtttbtuiuz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtidzwdcty.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuanzhike.top/gthrewpjff.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gttfjsyccu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigufen.top/gtvsyzziop.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtaepzqvkl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuanzx.com/gtqdbinpni.html

[D26] 数组转字符串
来源：http://hz.nanxuanxn.top/gtqoqlvewa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhoulong.xyz/gtlxbiqdri.html

PHP:  implode(", ", $arr);
来源：http://hz.fzhhl.top/gtepjxdnun.html

JS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtddpqdipw.html

TS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtqadcaynk.html

Java: String.join(", ", list)
来源：http://hz.quarkkingdee.top/gtbjejyfjp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ppjwa.cn/gtkdfrqpyz.html

Ruby: arr.join(", ")
来源：http://hz.mhx1999.top/gtyvaeqfmb.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gtnnfnihnk.html

================================================================================
来源：http://hz.xuanzx.com/gtsizktavh.html

E. 字符串处理
来源：http://hz.dashuyun.cn/gtbdrfhaau.html

================================================================================
来源：http://hz.ivvv.top/gtizpjfvwu.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtlxtwgevb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtiivffssg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.316326.xyz/gtyqcowhch.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtxdhmxwyi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gttkzoauke.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuxming.cn/gtirarvalp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtvjuoocgd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.snrcjt.cn/gtesumqssy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gthfimmijm.html

[E02] 重复字符串
来源：http://hz.ydzc1.top/gtrsdltjlc.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gtsipvmsfr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dianchejie.cn/gttlqsyvcy.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtfijipngu.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtafnokbdg.html

Java: "ab".repeat(3)
来源：http://hz.yuanzhike.top/gttiynxjfh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gtzshvmlmf.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtcmrcyezw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sysykeji.top/gtaocxnxcn.html

[E03] 截取子串
来源：http://hz.pengpengdd.cyou/gtpxhcgtub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cqqwz.cn/gtnhagnijg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtcynborew.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtcgygcauh.html

TS:   s.slice(1, 4)
来源：http://hz.vqdsnc.cn/gtswrfvtpg.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtxshouudw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuanzx.com/gtuqvlepgj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sxryk.cn/gtfcdfnwys.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtzoxlpuln.html

[E04] 查找子串位置
来源：http://hz.zdqjudy.top/gtpzkihvgo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtyokzedau.html

PHP:  strpos($s, "x");
来源：http://hz.hfpthk.cn/gtquuojkru.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtwoziqogt.html

TS:   s.indexOf("x")
来源：http://hz.nanxuanxn.top/gtvwjtsnsx.html

Java: s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtdqtqgjsf.html

Go:   strings.Index(s, "x")
来源：http://hz.sufxvd.cn/gtkuxqakrc.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtwkxbwtsn.html

C#:   s.IndexOf("x")
来源：http://hz.xylfe.cn/gtkgdmtvzb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtmxnbolih.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shangyingyoupin.top/gtgpmhqjzh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhoulong.xyz/gtdkyqdhou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtnodrrcxc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydzc1.top/gtuvlskkzg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtuxotlqzz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtqfemqfsh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gthgovtojs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtuojtphfy.html

[E06] 替换子串
来源：http://hz.yangfankeji.com/gtolkxxmae.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtuwgtariw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtxbwzxmzu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtiewyzbfk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtzwwilupk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtxgkjvbeo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgufenzy.top/gtheoqdlze.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtubtluqrd.html

C#:   s.Replace("a", "b")
来源：http://hz.haohaochexian.top/gtyhsamcne.html

[E07] 按分隔符拆分
来源：http://hz.yj202588.top/gtvxqufufx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnqzz.top/gtxyzakqud.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtdrxuuxlk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtvovuxuny.html

TS:   s.split(",")
来源：http://hz.pycfn.com/gtcmecexce.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtdnjatkhq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtimbogouc.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtxtfuizts.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pengpengdd.cyou/gteduxydpl.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtqqjbtsst.html

Py:   ",".join(items)
来源：http://hz.hysaishi.cn/gtyjzsqtbo.html

PHP:  implode(",", $items);
来源：http://hz.cucudq.cn/gtjhhzyncg.html

JS:   items.join(",")
来源：http://hz.xylfe.cn/gtbxxzihda.html

TS:   items.join(",")
来源：http://hz.aibaodan.cn/gtwzsvezzz.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gthufgcvvs.html

Go:   strings.Join(items, ",")
来源：http://hz.hfpthk.cn/gthnudgdmy.html

Ruby: items.join(",")
来源：http://hz.tian-w.cn/gtxqbosxhw.html

C#:   string.Join(",", items)
来源：http://hz.sysykeji.top/gtytvgxcdh.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtvxyvgtdq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtosrjjjmn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtoazynapp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtfsxzvbvg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtdcvazxng.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.c1oappe.top/gtesibzqaf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenzaomai.com/gttltnuwrl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gteoyidlzo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xylfe.cn/gtpirdzpoq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.smart0.xyz/gtseulhlih.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gttwnjdefv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtgqxbvcjr.html

JS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtyefshjew.html

TS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtwgechnbs.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtabhoaipn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtpgaodfph.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtezcmjtib.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtylgqkrjt.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtbjjvcfgs.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtkeqngfzj.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtwprtyfts.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtdwexzikh.html

TS:   [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtcmzmcacb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtbbzlisoz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj202588.top/gtstvbyvuj.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtdafbduxv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtoilnsbgf.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtularuzrs.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtndiuoard.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gtjdnnornk.html

JS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtznmaplvk.html

TS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtadmwuaha.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtnqvuujrm.html

Go:   strings.Count(s, "a")
来源：http://hz.andypj.xyz/gtfrpvbaez.html

Ruby: s.count("a")
来源：http://hz.nwbrower.top/gtquwyxgox.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtgcrgqvpi.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtfakttvhf.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtjpnsowpv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258.top/gtpzrcqlkj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtdywcetgn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtbanslmmz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jqgufenzy.top/gtdwojksmc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pengpengdd.cyou/gtbbdxmpdy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhixingplan.top/gtcroyaepv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtogynudda.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtpwycajcv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.daxiang520.top/gtyqlbtpkb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtifjagbax.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gtlatsjnvb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtqnfohatl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtbiirxytu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.c1oappe.top/gtfdevzpfn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daria6918.cn/gtlktwtddw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pycfn.com/gtuwdprsbg.html

[E15] HTML 转义 / 反转义
来源：http://hz.cheryme.top/gtjubfqors.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtvihymfmv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtkwsmtheb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtdiyghgdt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dianchejie.cn/gtmzavuckb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gtolqcvqyx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gtxdnbmoua.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhiwuduotai.top/gtlglntxmw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hammf.cn/gtjvuofoge.html

[E16] 数字千分位
来源：http://hz.gaohongyu789.top/gtannvryss.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtninmodbw.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtvmrivijt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtsrihbkkp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtwhjvjbjy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gtydrdxqnb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.birdmap.top/gtprcjtmxr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtonzmrvwx.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258888.top/gtyihrorpw.html

[E17] 首字母大写
来源：http://hz.gzhubu.top/gtzfpptyfw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.daria6918.cn/gtqcwqmhyj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj202588.top/gtjvinitjw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtqswyhpim.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtxnboityj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtriedvglb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ybcxt.top/gtfwjedmfu.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtlzdrugfi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtpoyvreqr.html

[E18] 模板占位符替换
来源：http://hz.yuanzhike.top/gtrkrxtzvc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.9152youxi.cn/gthxeejmde.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtomqmjsdy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtzkpotraz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtnvhfpjrd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtjvpqnukl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj202588.top/gtujcvuwag.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.9152youxi.cn/gtznrhftqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtvlvzbouw.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtxbmzeqag.html

Py:   s.splitlines()
来源：http://hz.316326.xyz/gtzulonnxl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daria6918.cn/gtvjdnrxhn.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtozchnune.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtpktqpikj.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtvnyywmec.html

Go:   strings.Split(s, "\n")
来源：http://hz.gotoacloud.top/gtdiawkqhp.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtoswcgfqs.html

C#:   s.Split('\n')
来源：http://hz.hongshengwenyu.top/gtacxptafr.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtdbojvnqi.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtzujxefwl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtpcezleab.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hywenlv.cn/gtkkkvkjug.html

TS:   if (s === "") {}
来源：http://hz.nanxuanxn.top/gtgzhigmej.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtwqekpqir.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtjwntbqjf.html

Ruby: if s.empty?
来源：http://hz.tianlin.xyz/gthckqvlec.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhaomingkeji.xyz/gtfalhegsh.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtrjpxtsuq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hywenlv.cn/gtuxsiivol.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtyhemrbwk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtothqtoeq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtyqlcoirh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtumtfwofc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtuzfmnyez.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtiwhtcrqz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtnnfkcjry.html

[E22] 字节长度与字符长度
来源：http://hz.gaohongyu789.top/gtwhvhpogl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuxming.cn/gtwzwrvxdz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtkbxssick.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtdvcgatex.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtanosbzkk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.birdmap.top/gtygvhostq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gttkiqroah.html

Ruby: s.bytesize;  s.length
来源：http://hz.jiagoushi.top/gtrkslaawh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtkyxedpjh.html

================================================================================
来源：http://hz.hnxiangtu.top/gtimmdcalw.html

F. 文件与目录
来源：http://hz.sxryk.cn/gtrmsqffsx.html

================================================================================
来源：http://hz.0kj1m.cn/gtblbjcfww.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtfunajbbu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tanke756.top/gteccvlxsv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nwbrower.top/gtgswltwzp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigfzy.top/gtuvqicncw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ivvv.top/gtapnygsje.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtognqcjix.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gttwnmcfxz.html

Ruby: File.read("a.txt")
来源：http://hz.yanxiufei.cn/gtuzbxejsz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gtcfzsytge.html

[F02] 逐行读取文件
来源：http://hz.9152youxi.cn/gtqozjsmhs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtbdhqshsg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gttitdoqhc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtfpdluujb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtxobvnduj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtljkzqwkp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtazhpjxok.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jyoumei.cn/gtnlgzvtxz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenlongwang.top/gthiuurbwc.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gteugxfdoe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtdviksdjn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtrtijucva.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtcshblgiz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtoknaxvrc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnqzz.top/gtxortdncx.html


<!-- 参考信息 -->