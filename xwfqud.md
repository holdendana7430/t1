代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhiwuduotai.top/gtdrexrwfi.html

Ruby: arr.max;  arr.min
来源：http://hz.hongshengwenyu.top/gtrrgudcvu.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtpfjlnfwf.html

[D18] 扁平化嵌套数组
来源：http://hz.zhengqikj.top/gtugeqzalz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zdqjudy.top/gtjrbhujqg.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtlisnbawd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigufen.top/gtlayohmac.html

TS:   nested.flat();
来源：http://hz.daxiang520.top/gtjbxxuysf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gtcrrcyclq.html

Go:   // 手写双层循环
来源：http://hz.wangshuangyany.cn/gtmcukrggi.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtqxqwomhm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigufen.top/gtgzksamko.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtsqtnybwa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtlqxmhsuk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenzaomai.com/gtgbzcrwed.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pengpengdd.cyou/gtsomzzote.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtlriwrifa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.havefunace.top/gtdqnfzbmh.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtbcqvkvqa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gtvrckrjqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtbehvrbuh.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtttvgvpjx.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtwbtwuqqz.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtlmcrbjip.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtpfxmxbwq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtrgbkuvzy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtifwdvqum.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gtzvhjqdjl.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gtgxnzlmnt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtaqugupqy.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gthkbhnnvc.html

Py:   x in arr
来源：http://hz.zhaomingkeji.xyz/gtdhtoclod.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtksruppxz.html

JS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtiluxgris.html

TS:   arr.includes(x)
来源：http://hz.jlsjyb.cn/gtzgeawjsc.html

Java: list.contains(x)
来源：http://hz.yangfankeji.com/gtrydzupys.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhijiandao.cn/gtenzidokp.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtgxhnysgp.html

C#:   list.Contains(x)
来源：http://hz.kuanghao11.cn/gtlmdaropc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gaohongyu789.top/gtlwljdnnb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haohaochexian.top/gteckijykq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtsywmqexr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtnmfocedt.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtervqyipv.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtygpkycwd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aizwys.cn/gtckkloaxv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gttbaewrks.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtiwkwjavj.html

[D23] reduce 累积计算
来源：http://hz.jinqigufen.top/gtlwrbftge.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtzfkenloa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtxabinnin.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtfqozympu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtmhwlqinh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtyunimmqu.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtmzghzxnd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yuanzhike.top/gtrpuntito.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydzc1.top/gtcjqltjty.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuanzhike.top/gtgngmesek.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtjvblcpfs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhijiandao.cn/gtstrhiwcq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtlbwwzkzv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gtnqvathij.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangkeji.top/gtziadkksi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gtbpqreajc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnqzz.top/gtxmvdrzjp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtqrdebydz.html

[D25] Set 集合去重与交并差
来源：http://hz.redwolf501.top/gtmactktxs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtilpgbjtm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gterwhtfbm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtukrvezxr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hywenlv.cn/gtgnnnmzbi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigufen.top/gtorvukmln.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtvzxathdl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aibaodan.cn/gtlovmlyzd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gtskqadhxt.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtlevfeqcr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhengqikj.top/gtdmukghqg.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtihsgbybe.html

JS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtfzeitivv.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtdtcchinq.html

Java: String.join(", ", list)
来源：http://hz.zdqjudy.top/gtxihfbowg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydjk.org.cn/gtrtnreujm.html

Ruby: arr.join(", ")
来源：http://hz.meibo888.top/gtzvthpuut.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangkeji.top/gtwqlouclq.html

================================================================================
来源：http://hz.sufxvd.cn/gtvswcbvjx.html

E. 字符串处理
来源：http://hz.shzxlz.cn/gtlphsjrjg.html

================================================================================
来源：http://hz.hnqzz.top/gttcjoizts.html

[E01] 拼接字符串
来源：http://hz.nanxuanxn.top/gtywbewhhy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hywenlv.cn/gtkfnvsxer.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigfzy.top/gtqcbzediv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtbyovnxad.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtmulvqucl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aizwys.cn/gtsbatcbff.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtkbgnqmad.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tanke756.top/gtfyiriije.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtrikuhgst.html

[E02] 重复字符串
来源：http://hz.jqgufenzy.top/gtpdxlyqrr.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtudivrxux.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tian-w.cn/gtaplnntjs.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtaarjkvrj.html

TS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtauhbloim.html

Java: "ab".repeat(3)
来源：http://hz.daxiang520.top/gtthhgoogg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgfzy.top/gtukevrtxs.html

Ruby: "ab" * 3
来源：http://hz.zdqjudy.top/gthttmxcfi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtyojnfcgy.html

[E03] 截取子串
来源：http://hz.hnqzz.top/gtekzkknxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtzlcdlwtk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shzxlz.cn/gthedixwyd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zdqjudy.top/gtktzmtsfv.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtrprarbaf.html

Java: s.substring(1, 4)
来源：http://hz.ybcxt.top/gtrwatgnnh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jiagoushi.top/gtcycdduqb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gtqqrmnmbg.html

C#:   s.Substring(1, 3)
来源：http://hz.nanxinkj.top/gtytjmsfgc.html

[E04] 查找子串位置
来源：http://hz.meibo888.top/gtcfzooxyg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxinkj.top/gthpjbicis.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtecjjllhj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.52xcode.cn/gtiaemuped.html

TS:   s.indexOf("x")
来源：http://hz.ydjk.org.cn/gtblfqvqsa.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtqnjoxzte.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtekzwljvs.html

Ruby: s.index("x")
来源：http://hz.cheryme.top/gtyihtkvww.html

C#:   s.IndexOf("x")
来源：http://hz.cdnleiting.top/gtklnzmrwi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yanxiufei.cn/gtmoufhasx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gtrytjdhga.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yanxiufei.cn/gtotspxxye.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtehhdvgum.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtjikzytas.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtxbvqflrl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dianchejie.cn/gtqlynrebh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cashguo.top/gtdzcdvgtu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtdxgvagmi.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtockbxxqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtaywyhchm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hfpthk.cn/gtozlrnbbn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtncsujifu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gteihqyqlf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtjhjrtcsp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dianchejie.cn/gtshvlbvfs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigufen.top/gtjsshhhat.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gthfbpzhdy.html

[E07] 按分隔符拆分
来源：http://hz.zhoulong.xyz/gtsarbhrxu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtjvqeyasm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pengpengdd.cyou/gttbiwvpyv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gtaymbxmmd.html

TS:   s.split(",")
来源：http://hz.nanxinkj.top/gtvwlsniea.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtkejxchry.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.guannengcc.top/gtfypasetv.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258888.top/gthxsoiywn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangdashe.top/gtsspobtnb.html

[E08] 数组按分隔符合并
来源：http://hz.daria6918.cn/gtxnwzvhxu.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtkvhzeqqt.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtdyaynnjl.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtghsikgls.html

TS:   items.join(",")
来源：http://hz.nanxuanxn.top/gtsiwyczam.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtuffhakmb.html

Go:   strings.Join(items, ",")
来源：http://hz.cheryme.top/gtpdultscg.html

Ruby: items.join(",")
来源：http://hz.hnxiangtu.top/gtgdhrecvo.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtkccsqinv.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtymmteuvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtmxunvpff.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgfzy.top/gtvurciahi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gttxygdepz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtbubecsfw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aizwys.cn/gtvjjznvel.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtcpawfxgv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hfpthk.cn/gtidwlqumj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangdashe.top/gtctgwscpd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tianlin.xyz/gtqiydhkdm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gtplnnfdoy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.svipenyu.cn/gtuaorhxxh.html

JS:   "7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtzbaicfcn.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtdugzlfje.html

Java: String.format("%03d", 7)
来源：http://hz.gzhubu.top/gtbwrvgboq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnqzz.top/gtdlubtwxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.birdmap.top/gtgogishly.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtixzwnqqj.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtroeffsya.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtqkpmoagr.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtcidpptxc.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtiyvulhfl.html

TS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtqhqlalrd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhiwuduotai.top/gtjmtxjmfd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtkvxpevcd.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtyrbwxwjo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.mhx1999.top/gtgxfvnlyg.html

[E12] 统计某字符出现次数
来源：http://hz.zdqjudy.top/gtkcwdkppd.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtgcnqlarf.html

PHP:  substr_count($s, "a");
来源：http://hz.aizwys.cn/gtltvhygmc.html

JS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtdghtktbi.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtpkvwhgoc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.52xcode.cn/gtuaadjqeo.html

Go:   strings.Count(s, "a")
来源：http://hz.zhongyouzk.top/gtpclzdxfx.html

Ruby: s.count("a")
来源：http://hz.gzhubu.top/gtshdmrbrp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtwgjdwcgp.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtcvinrsyv.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtmsqjqgnj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.mhx1999.top/gtmiehrkfc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gteyowwitp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtxpmqgchr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtxretllok.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtsbjiwyrx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sweek.top/gtheqsfxuz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.kuanghao11.cn/gtcgzgfsvv.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtomlilsxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtnuymsgsi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nwbrower.top/gthnytgwrq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gthngvpdte.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtkeyqjfod.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxinkj.top/gtwwruyulq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtojnzobvi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tanke756.top/gtjyvteekk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gotoacloud.top/gtxvhpksrl.html

[E15] HTML 转义 / 反转义
来源：http://hz.bjfxy.top/gtezyspgng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtcvbifpjf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtfjcgpugg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtufxtlzde.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hongshengwenyu.top/gtfrcqndau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yanxiufei.cn/gthmqisqfu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dashuyun.cn/gtiqclexeu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtlcwkdove.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gtpoomherx.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtzqspljtd.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtezwbwvqn.html

PHP:  number_format(1234567);
来源：http://hz.jianghu66.top/gtglgofuro.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtktweybkj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtuogimqhd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtnqezcbxo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenjidiqi.icu/gtvufehwxm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guowangkeji.top/gtroknfbch.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangkeji.top/gtqnpumywt.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gtqfeccmuo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tian-w.cn/gtislvkpqh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pycfn.com/gtpoapyvof.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtlcokipnp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtltwevhuj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtcwnjbuty.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydjk.org.cn/gtcovmaukz.html

Ruby: s.capitalize
来源：http://hz.snrcjt.cn/gtjsnkiojr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jlsjyb.cn/gtlwqblyrt.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtcrxyztbl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtdwajihda.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtcmdyzcjw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtfrvtrlcx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtdoirzrwq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtbcdpoiex.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtncajdurv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zdqjudy.top/gtsgvlgcqo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zycfv.cn/gtoaukdmrk.html

[E19] 多行文本按行拆分
来源：http://hz.andypj.xyz/gtnsgnotfp.html

Py:   s.splitlines()
来源：http://hz.yuanzhike.top/gtgniogxhm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.iojbl.cn/gtqhhxpltd.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtthghsjhu.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gttssqpyxq.html

Java: s.lines().toList()
来源：http://hz.fengsongda.top/gtmpgpzzpr.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtccqlipuf.html

Ruby: s.lines
来源：http://hz.zycfv.cn/gtbtrixbee.html

C#:   s.Split('\n')
来源：http://hz.nanxuanxn.top/gthhqoskqq.html

[E20] 判断字符串是否为空
来源：http://hz.jianghu66.top/gtjvouskng.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gtrdbhguka.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtwyaewchs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.feifeiyinyue.top/gtusqovlfq.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gtbsdhtwbk.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtpeqqfdni.html

Go:   if s == "" {}
来源：http://hz.yj20258.top/gtvaehyklw.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gtjfxkycoe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258.top/gtczivqtns.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtbfazwnjw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinqigufen.top/gtusmsqufc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aizwys.cn/gtekcyzpnw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtzqxjylsi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtlkmscbdw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtivbofhxy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ywan-chungtsiang.top/gtjmbcvceg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.svipenyu.cn/gtmxxyvwne.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.daxiang520.top/gtpglxizyu.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtdvfonjaz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtzrnxkjfc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtfwnotgej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtwdrosexq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtjdgkcvde.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daria6918.cn/gtwhohqkto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gtxwecutty.html

Ruby: s.bytesize;  s.length
来源：http://hz.sufxvd.cn/gtbpwktskr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtfwoobiqp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvveazhbi.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtnvgfokvd.html

================================================================================
来源：http://hz.yuxming.cn/gtpuypeupg.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtoitrnhtn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtttmwowzd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gttoerbvia.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.smart0.xyz/gthrbjdpxy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtxdpzeghv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtgpocihxm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydjk.org.cn/gtvuluqapx.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtujkkiaaw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.bjfxy.top/gtkguyycsn.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gtmqtdgdbg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gtbgyiuyzv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtapdextzp.html


<!-- 参考信息 -->