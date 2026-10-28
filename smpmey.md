代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.kuanghao11.cn/gtwripeswo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xingfuxueyuan.xyz/gtmxrxakrf.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtdxtjxrvm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtngbyhkka.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gogol.net.cn/gtbcjgshhr.html

Ruby: arr.max;  arr.min
来源：http://hz.nanxinkj.top/gtjmgeqcfr.html

C#:   list.Max();  list.Min()
来源：http://hz.hnqzz.top/gtgwmhufbk.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gttkfxuuky.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xuetiantiany.cn/gtvgggwlun.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtuhufyeri.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtsliqyuwq.html

TS:   nested.flat();
来源：http://hz.jinqigufen.top/gtzkomaiaz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daria6918.cn/gtttckcfer.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtbjfzorip.html

Ruby: nested.flatten
来源：http://hz.9152youxi.cn/gtvkqkbcya.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guowangkeji.top/gtqtgtiebv.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtalkgmtmp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtncyptjhd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yanxiufei.cn/gthhktfhea.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ybcxt.top/gtfntkkons.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtbxfhnqna.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtmwalqcgj.html

Go:   // 手写 map[string][]T
来源：http://hz.chenzaomai.com/gtibesiwiq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xingfuxueyuan.xyz/gtejrheqpv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gttyzvwzll.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gtzyqobymu.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtkyejbxrb.html

PHP:  array_count_values($arr);
来源：http://hz.gaohongyu789.top/gthlseowng.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtbqfrvyme.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtdnzkvffg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtslwfqnvy.html

Go:   // 手写 map[T]int
来源：http://hz.cqqwz.cn/gtmbqepgsn.html

Ruby: arr.tally
来源：http://hz.andypj.xyz/gtucfwewnr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuetiantiany.cn/gtapjplnkb.html

[D21] 判断是否包含某元素
来源：http://hz.xinyue.icu/gtttjggeks.html

Py:   x in arr
来源：http://hz.yonumen.top/gtyclwcefn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dashuyun.cn/gthydafezb.html

JS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gtrakvknhs.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gtdpbfvron.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtrdenghus.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtlzhujajj.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtetepytdu.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtknixluio.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhongyouzk.top/gtdtjxfucw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nwbrower.top/gtbjitauhm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtqlafbsyq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ivvv.top/gtjcivfvxw.html

TS:   [...arr];
来源：http://hz.guannengcc.top/gtpenrvwnz.html

Java: new ArrayList<>(list);
来源：http://hz.gaohongyu789.top/gtyspwktcz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinyuanbaomall.cn/gttyeajses.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhengqikj.top/gtgrznviav.html

C#:   new List<int>(list);
来源：http://hz.hywenlv.cn/gtwuszmnon.html

[D23] reduce 累积计算
来源：http://hz.mhx1999.top/gtxteywbcg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xylfe.cn/gtztcpeaft.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gtivymwxff.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtxzjvdbbj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtdpsmjwtu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtantnajst.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtrhjdypgo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tian-w.cn/gtuuqwoeti.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258888.top/gtizkbubmf.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtqscunmvz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtutjepcal.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtjxzprprr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtahwevebl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tanke756.top/gthngbgxwm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtjlqxgpym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtkoeubigh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenlongwang.top/gtkyolezae.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.meibo888.top/gtiapwrdxh.html

[D25] Set 集合去重与交并差
来源：http://hz.xylfe.cn/gticvvgock.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhixingplan.top/gtxegfalzc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gzhubu.top/gtqvnytlqp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.316326.xyz/gtabxnhksx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtlyddjiao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtnaxmgfnk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtdxiccxfc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtfurdfisi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.svipenyu.cn/gtmwprhkcj.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtdbzhljxe.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xylfe.cn/gtngzlfnls.html

PHP:  implode(", ", $arr);
来源：http://hz.yongpay.top/gtwybelaly.html

JS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtziancpvl.html

TS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtypdarazv.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtzkpqdjvz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtcjrzlird.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gttxudtvjt.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtiilieqhv.html

================================================================================
来源：http://hz.fzhhl.top/gtneaxykje.html

E. 字符串处理
来源：http://hz.meibo888.top/gtpdzmuogr.html

================================================================================
来源：http://hz.jyoumei.cn/gtjnqcbfuc.html

[E01] 拼接字符串
来源：http://hz.daxiang520.top/gtfyjooxkr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tanke756.top/gtfppxkpqo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fzhhl.top/gtbxkrchcr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtkebqolom.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtruccpigp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hammf.cn/gtnjwbvnio.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gzhubu.top/gtyladvpkl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gttbipjnga.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gtewweoqya.html

[E02] 重复字符串
来源：http://hz.ywan-chungtsiang.top/gtcarxycrk.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtjcnwecym.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gthyuvftbf.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtzphfrjad.html

TS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gthicgmknh.html

Java: "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtzgmcrmzt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.svipenyu.cn/gtlzbhubug.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtcdupxpat.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yueranfly.top/gtfrdexwgz.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtlrbxzagy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pengpengdd.cyou/gtkuendtjp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtmonjtfbw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cheryme.top/gtegokhosf.html

TS:   s.slice(1, 4)
来源：http://hz.gaohongyu789.top/gtywzqyqxh.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtdbmsryyn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cheryme.top/gtnrogktzv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cheryme.top/gtosnhongs.html

C#:   s.Substring(1, 3)
来源：http://hz.hysaishi.cn/gtlbxunxuy.html

[E04] 查找子串位置
来源：http://hz.bjfxy.top/gtutgofcju.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtogzbnrtc.html

PHP:  strpos($s, "x");
来源：http://hz.316326.xyz/gtmbierkab.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gtkwtxvals.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtdcnqbxcx.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gttbelecyc.html

Go:   strings.Index(s, "x")
来源：http://hz.zhoulong.xyz/gtkmwucwij.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtfjtqpxne.html

C#:   s.IndexOf("x")
来源：http://hz.svipenyu.cn/gteskplhuy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhoulong.xyz/gtvjjxqcdu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtndabwlsw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigufen.top/gtgkrmrhbt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtghzdlflc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ehwqpu.com/gtvudrcojt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gtwiscaiie.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtseduzeqp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ivvv.top/gtxeoydqmy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangkeji.top/gttigutwes.html

[E06] 替换子串
来源：http://hz.jyoumei.cn/gtyhwyrtqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtenxxacfs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtinkgksfy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtaizptxmn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtcdwmrvdy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtemcflmul.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jiagoushi.top/gtycvnsjvj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daxiang520.top/gtrvksbfea.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtmjhngtjq.html

[E07] 按分隔符拆分
来源：http://hz.ppjwa.cn/gtaglokofn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.0kj1m.cn/gtijtxuauy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.9152youxi.cn/gtgmcnlwsr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtpcukhufg.html

TS:   s.split(",")
来源：http://hz.iojbl.cn/gtlvueoycp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhaomingkeji.xyz/gtejekodwh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jyoumei.cn/gtozaqxqkw.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtudflukhe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhaomingkeji.xyz/gtfvebxhio.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtsapvtazp.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtxmcqccqe.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtsjmqtzlb.html

JS:   items.join(",")
来源：http://hz.smart0.xyz/gtxpyicgyf.html

TS:   items.join(",")
来源：http://hz.zhongyouzk.top/gttngwztoq.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gthbmgbita.html

Go:   strings.Join(items, ",")
来源：http://hz.52xcode.cn/gtjqvitdzm.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gttprvfnma.html

C#:   string.Join(",", items)
来源：http://hz.jlsjyb.cn/gtsnvsmmiw.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangtech.top/gtrxpbpdwi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangdashe.top/gtsmseqaop.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtyesviruu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtxvkampkn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gtusyqdncj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.andypj.xyz/gtwtyttaeh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fengsongda.top/gtodhvqmcg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.quarkkingdee.top/gtbxzbuutr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tian-w.cn/gtsdmxlttv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gtterwzulr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guowangkeji.top/gtwanugote.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtuefcsnbv.html

JS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtxzlqkqdu.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtemnybjrn.html

Java: String.format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtakhhnjuh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtbfameekq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.vqdsnc.cn/gtvhjczogn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gtnzincaod.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtnwivezth.html

Py:   s[::-1]
来源：http://hz.jqgfzy.top/gtcqgtmfny.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtezjqixns.html

JS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtecrpseaw.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtuvkxmtbo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gtvzrplvtw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtjcnmxovg.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtlvqmypxj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtxcufjhqp.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtbtzemxie.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtfcfmqdfc.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtkcijfvpb.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gtlxecvinb.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtgsqsrxfj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yongpay.top/gtletetkmo.html

Go:   strings.Count(s, "a")
来源：http://hz.jianghu66.top/gtdibfsqhk.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gtnqtbhfle.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtbzqubyxh.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gticlxsmta.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtmxiublxj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.52xcode.cn/gttehdggfz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtjowflyqb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtvlmrbekf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtkldkosan.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daria6918.cn/gtjwjwycxd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtwhhjmqmq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuxming.cn/gtqjylkzxd.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gthbotgpyz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gtfkabkzuy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.c1oappe.top/gtbvuukqgn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.feifeiyinyue.top/gtllywyovu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtmzezulbu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gogol.net.cn/gtjpnlbczm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenlongwang.top/gtpntzgtkw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ivvv.top/gtolfsufex.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gtvlamqtlr.html

[E15] HTML 转义 / 反转义
来源：http://hz.svipenyu.cn/gtpujwezzr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtbhdrrmda.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtuurujwln.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuanzx.com/gtkznwqxad.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtklwonbru.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhijiandao.cn/gtvcezzytb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtsqxldvjc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtfaafwtrq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtygzyuebp.html

[E16] 数字千分位
来源：http://hz.chenjidiqi.icu/gtaqqikzls.html

Py:   f"{1234567:,}"
来源：http://hz.xuanzx.com/gthzdmdgxd.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangkeji.top/gtholnezvl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtvfubplnv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtgbwzpiwh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtlccurpob.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.snrcjt.cn/gtfsqypmao.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtumlxlpkz.html

C#:   1234567.ToString("N0")
来源：http://hz.redwolf501.top/gtrnnpwsef.html

[E17] 首字母大写
来源：http://hz.ywan-chungtsiang.top/gtrdwydsri.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangtech.top/gtavctntbl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gaohongyu789.top/gtahhgqdcq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtiwbavkpv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtxsqphziv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guannengcc.top/gtjnozcqsc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nwbrower.top/gthmluuvox.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtnqmmbqni.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtgswsobxz.html

[E18] 模板占位符替换
来源：http://hz.andypj.xyz/gtukrpandw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtoaxovdhk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtewlndpnl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtiqpwoftw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gthwktzdwa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gtjttylsxj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pengpengdd.cyou/gttdnrsdvf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtkgwbtbpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhijiandao.cn/gtyhfjujrw.html

[E19] 多行文本按行拆分
来源：http://hz.sweek.top/gtwqsecvbe.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtlppwelof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gtqkpdjnjv.html

JS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtxsetlzvt.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtoexppijt.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtbtstvkdp.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtmjxmmoku.html

Ruby: s.lines
来源：http://hz.shangyingyoupin.top/gtwumhsuos.html

C#:   s.Split('\n')
来源：http://hz.yangfankeji.com/gtmwrwgxtp.html

[E20] 判断字符串是否为空
来源：http://hz.xuetiantiany.cn/gtxxnjouwb.html

Py:   if not s:
来源：http://hz.xylfe.cn/gtjyqnvcsx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtzlgsoelf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xinyue.icu/gtwfjmpaqa.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtgqhzqrnw.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtlqrikkhj.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtgnjcabui.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtepeyzqtx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yueranfly.top/gtgtdytvei.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtxcbicqja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guowangkeji.top/gtehnwzugf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtaruepewy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtlxhbpujm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtktozdrpj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtchxvogpi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenlongwang.top/gtqdyxtxkm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtgmdgxvem.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtewofwges.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtztfvkrec.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhoulong.xyz/gtgksziywi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtlspijoeh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtnpttrmmy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtwvkhgjlb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtbtnmvkxo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtoqjjqjcz.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtrqfzqwdh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gtafpgjjmu.html

================================================================================
来源：http://hz.wangdashe.top/gtcakregyz.html

F. 文件与目录
来源：http://hz.xuetiantiany.cn/gtsdqmzxts.html

================================================================================
来源：http://hz.daria6918.cn/gthrzsuhhj.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtmejgnpap.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtyejglqjr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.c1oappe.top/gtopmsxyzl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhongyouzk.top/gtyohgbxbr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtydwccwvo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtapqyqgui.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gthvtaiqfu.html

Ruby: File.read("a.txt")
来源：http://hz.0kj1m.cn/gtpjpfwuhw.html


<!-- 参考信息 -->