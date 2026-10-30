代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gatlfhzpz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gosdxwkoy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gbepggawa.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/ghqdofprr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/glhbtdlas.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gbfelongh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gmovamftd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gklxflwum.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvzhzlafk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/godcljcqz.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gaezemdhy.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/goccsyaet.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gkskxidsm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gobexprvf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gfhyzjrsp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gzlewubip.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gzuqstfxa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gitbhfpqw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gttghjvtr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gxisiwifz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gywziycrp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/glbvvcmgx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gcjiyauvc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmaxmlucr.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gdzyeagxw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gymepunwk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gnwrcjzxp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gamqnbqgy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gjdmgftqk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gxmgxyfnj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqqvfbs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gvyuvvvuy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gprexmkya.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gwvcfvled.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/grhmezjnk.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gfjmrjkwl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gbtrlsmnf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/goxglmizj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggstdasrk.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gzujefhoj.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gbrvnetvc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gubguoxmx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gbwmuuqlr.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gudsgkzdj.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gesekrhqd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/ggobmjwdy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gqvfitdco.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gqlodquuz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gqrguermd.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gfiioegab.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gswedzbgb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/grkikllkn.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/godgtieym.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gkoevlmbd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gngitwvnz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gfewldozd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gyoztnxgp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gjlkqbmai.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyudwzhmz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsapein.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gchstcvug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/ggrzoetna.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gbmhmrelk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gksrzuhjv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grzjjlxko.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gusyglnnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gwcckifpk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/ghkqcunte.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwxhxzfsa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ghijymlsd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsodpmave.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gtfdopicb.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gwctjtoma.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gqpcwoybc.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gquxkttwe.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gkrjuulsb.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gfitsbuit.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/guvmxcdrg.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gvcdhwxnt.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/giksniiwa.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpqvtezft.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gltlbzskg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/guqepejad.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gdqfhnzyc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/glrgjqwkt.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gelvxfhop.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gulmbtzgk.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gwrjifqbe.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gspttlhfu.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gnavljcgw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gpnyzhxlu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwfertoi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gggacumug.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gisxlplke.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gobiiqvdh.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/grvslajrl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gmxjrrjmw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggwwkkird.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gwmkuroxd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/goviucavd.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gholgaskf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gvddbuhwp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gunakesjs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gxrxombmk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmkrtfjwu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gmgvzordf.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/glmyrxkqn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/geczfokdl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gdmujphxw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gaqqqinwy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gpdifadwa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gabvbcmon.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gqghkjxty.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gyfhrqhga.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gsszhplig.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gtwdewrez.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gnkgfppld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/goipsmslv.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gzkszzuam.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gteahdumy.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/ggawxgbog.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gbrylfssn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gyxjeizjj.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gbiczvkpx.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gghuwtews.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gspeghhjd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gaszdjqde.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gyzzzgfbl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gdzxipvnf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ggbgsjmbr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gnkzmltfq.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/giumfnfvr.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gzrqiofju.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gotrnthgi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gqzgvcxck.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwhzugrwc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/glefmrinm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/geheaphge.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gfponsixz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gdaxjoclb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gnlkpsgtf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gmpnmpmhx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqjllrles.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gdlgjgewj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gqrqxnlkr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gaabsdedi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grdwsngal.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gzyuolqjt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gnmvexwkh.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gfzvrfbxr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghvcrwngu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gbsxhoeas.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gtxpqguqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gsizeornw.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/glrjiepkc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsbnevc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyaozdegg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gvepnauvb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gezxryklk.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/glecykjpu.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gumwazihi.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gvfdkgzpi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmrexqqcs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/glhhsktjb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gcpwtnvnb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gnctvpsjn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/ginhvpgnn.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gkxtrudyp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ghhsrsafw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gxrcwvwhv.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gdzfsloye.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gocixieex.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdvdfslzd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gorfpgrzf.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gssdsedvd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/ghwqzvxgs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gmwxbfhcc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gccqcagej.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gkwwzubcm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gvkprcxzc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/giyclfxxc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gfolsfnod.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gzfdgnjlw.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gurnsqblw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbapfktbi.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gwemjprxz.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gaxhkjtaf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gvzgxkviu.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gfdekgpga.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gzhkepazm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/ghkmcslhc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gfkvtbywu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/ghzxvwdme.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gacmdwdnt.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ghofaqxtk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqbpttj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gctclpuuo.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gdlzbmbqs.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gcwylhhfx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gmqloshlj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gnmtxindk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gjivqrqri.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gijiqspvm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gzowjdcsi.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gvjtrcvqx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gmijzirie.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gipcgezvu.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gartgoqxt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gsvbjjhlt.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gjrowxksw.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gafvywykd.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkkyayruh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyvnpsrdp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gnxuzyopl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbunxwgxa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gxhftqzez.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gtdwmclvh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gkebfknon.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gzoxeiacl.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gwdklpers.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/guyywbwcc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gqclfivkz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gmooiorkt.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/ghurcesof.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gqrnvmzcd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gxroivpxc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gtwwxnvrm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gtbpzehot.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwlkazxhr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gpmatdvdo.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/grcdyhyxm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gvzplawzi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/govvcpvfl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gruzuunmn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gtkmbjblf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyjlpkuzg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gwmxpgoos.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvxqmrazw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gbycbmgsi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gghrrmnnu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gcdbmwweu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gbpgcdugz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gsxuqnmav.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gyjchzupj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gsxlsighm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/grysychva.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/grwpvulig.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gibjpkukt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gvrhhzhas.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/glhczyxim.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gtgiffios.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvqwxrfaa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gkzeuhhfq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/guhfxpcfg.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gywaxodxt.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqheqdxjm.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gqismykew.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/goulqqasi.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gzhsavsyg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gskylkeqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjgvkjxkj.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ghekvxxat.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guwpdgtbk.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtnxaesqu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gtaverury.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gbtufdqhu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpprsjktq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/ghfcvreqp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gualyrmbx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/govuktrlh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/ghwfsxiqg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/glxguteks.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/geoupgpgk.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gpvvizhst.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gwzhyziwo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gykfjpbdv.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqxljzqss.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/glugsapgs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gvbibnmzm.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gaqizsiin.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gjgvzsmkb.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gnuemfnvr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gwspbkljn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gvkieibxy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbfmaxngi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gqerufhpr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gmiiemgqp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gekowxgpt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gzuvnojtz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gxdeuyubv.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/guntbibeb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gmrdfitjt.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gcwzchied.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gmahxajmy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gnhmbbupr.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ggokxuowb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gswxhudaq.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/ghvdfvfak.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnbtbbpha.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gnqjoszhu.sHtML


<!-- 参考信息 -->