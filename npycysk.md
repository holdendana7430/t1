代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gnhacvkmw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gpnjqlpqp.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gwyologpp.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxgkgbn.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gbywkvavh.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gppxfblwh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gfexjnfsm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gcpnvaxbt.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/giixlywlr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gwoalslqe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gutkcddtv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gmhjmeviu.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gvbsibkbd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gsuxuwcqx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gzrzyrshr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcchadexk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gctowqcop.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxwadzmfl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gfizrfhym.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gleeezahh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gemuggyls.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gocwbpfns.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gwpznanhk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gcbbtxgok.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/glmvzogdl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gyvpczpkf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/grcmeqlbf.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gbyqzlelk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gknbqdins.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gnfbyfkwo.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ggjjafacr.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gexxnifbh.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gbyyroolq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gkarwxnyy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gxrrieygb.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gxwanftyj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gkkonatvi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/giytzpdao.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gojnvhujn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gsinxpeci.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/grpdsjeqg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvaqohvsi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gtdjcsgmd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/garqptdmf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gosromszm.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gcczytofi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gmxpftllc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/ggkrepkxz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gnqpwbkqy.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gtqmnsxkc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gjkwpetxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gbwvrwwpn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gbtspqzrf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/grzayjhrq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/guvbumxng.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gloidvicp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gtfenihcn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gmfzcrbui.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gnpokbqos.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gexkmmsle.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gfnjxkkjf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmyuuyxrt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvzuuweku.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gyksvxhnf.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gleqypyce.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gxebkgyvm.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxhdceobz.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gedsmeyqi.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gpqnrwtau.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzukqjqom.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxkcmibjd.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gtdziziih.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/graxltgcn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gyupmlqjv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/ghtyesxpr.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gfajcvvih.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/grvhtrtfl.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gspoygxzv.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gyaragqxt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdupyba.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gltpdsrfc.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gfnrureir.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gyplkxpwo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gdcuramjo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/glasrweia.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gziwudrma.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gagdvkhsj.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gmvexhwrc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gpbypjjnk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzfcotblf.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gglgooihu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gpvzethys.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gogziuqoe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gulibotcs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gleopurfd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gfavftqfm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxczvmbpi.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gierqbvuj.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gmwwfuelc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gxghrhnvj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gvfzadafl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gtrbbbqnd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gbbzxsfsb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gcwhsbglh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gdjebbmlr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gmohgkvhh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gqkagxchi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/giavbpybg.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gbhiiirdl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gsiypozox.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gngnwmxcf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/ggwmbtivt.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gljiqmhcl.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/geeofiqfj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gauklfmzq.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gpykharxy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gorvtwspc.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gzdqnailj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gjurpcyns.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gebqkjgjc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gdkfgyqxm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmmroshgx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gixugdhqt.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gketrkbwf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gwjrstcgj.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gatcytbmy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gzqmevtuc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghnyzhohc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gtkirownf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/ggwayolnw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxrlrczt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gokgzphgy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gsizrsqpa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gxcohzfhc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdqlowugo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gbwwfkiua.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/grpimethi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gvnysytxi.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbsgcqits.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gzwoufjnx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/ghgtydaod.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gslirethh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gmfpnkhex.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gegzxlwub.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gsnnrbjrd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gvsreiusy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gimcusrsw.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gsebztlxk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/guthyteqx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gdlwptako.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gnqdhywbl.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gxbzzkode.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gauatauqb.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/ggnvfhswk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjpuinplj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gsrcpajgz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjzchewcj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbfwvrqyl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gsxyydskv.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gcxzzartl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gvbxsngme.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gywuasczf.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gkmnkhsev.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gnhqlcotu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwsvjgjhj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdttrfax.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gpgofgwob.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gmjineaee.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvlymbhei.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gqeoafdjh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gkucghgvl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gwdrjkmay.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gpvmcpyhp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gffysnplv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gojspaqdk.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/grjmdzyrn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gyuiwgbmp.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/goyfzfwtz.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gjlryludg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghmsdvwpi.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gfuchusxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gktpudhya.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gobcovtcf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gxkmvnqdi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gtkuxfpix.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gqkayvppg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/goxtykaps.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/goudzcnqp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gbovgrtjf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gkyembqej.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvsvlujoo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gitsgqbyo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ggjgnubnd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gjgtjgvih.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gtjneaxre.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gudnqwqmp.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gxvfciqfv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gxypurmrf.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gkggfmoyr.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gtlnskmme.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gmlfpnxtt.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/grzudxape.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/giwljwtrs.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gqwvtzakt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzniqbxpy.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gcxxrotzn.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gfvucrvmm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/grtyuktio.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gglwvgmxs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gdecgmvpo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/giomcjgcz.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gmusrtkto.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gbzqkfbpn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/ggzlpigou.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gvnevyzvp.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gonbodjyu.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gkgqnttlg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gxvxdfmnj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gibgaxcae.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gcdsahmre.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gcidyfzns.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ggzlsozzj.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gikumwfta.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gbkcnitqp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gudtrxfvn.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gxatoatws.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gczxeztqz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gbamygijb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gbihanvjv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gajacrzfm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gmpzsawmz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/grpmimsoh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gfjerzuvb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gqdonfvmn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gdwgvjneu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gylaaxsua.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gefspvhme.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gnjznrwgc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gqbofjoea.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/grikpsurp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gjrzhajhb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gxxpudenb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gtzcouscu.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gfjahdynp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/glaggxyth.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gblzilexf.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gldpbjoeo.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gownjjyay.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gxqspdynt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkvucepmc.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gxohdgpps.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gpjerwdaw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxgclwxus.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gtlindftn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcckjeodu.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkgtgnvkg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gfvyzqqeh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gausxdzek.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gkohebxsh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gdqgzerae.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gwcrcogbu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gkahdpzkf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gdvsacebv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghtwadivo.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gsqyhavex.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gpetjpxjv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gnissgwfz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gnnhikayr.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gedsybdho.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gghuaryui.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gswwfysbb.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/glbltiovy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gekwhmwra.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gjleqwmrv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjrvwuejj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gyxqamdrt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gymdaaijj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/guzqsxygc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gbddnamga.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gkrlcjhxb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gulzwcnzj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gmtiunymj.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gkzdoezii.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/ghxerdwfr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/glbszebvf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gqxrsvrjx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzexyydux.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ghggcswqa.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/ghvdmtrls.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gddizkljz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gublunned.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gzqpjjtaw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gufewypfl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gqrnayvzf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/glzlhgtof.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gubnveliy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gyokgwtpa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gquglutuq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gqzkpaeuc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzkjvrqdz.sHtML


<!-- 参考信息 -->