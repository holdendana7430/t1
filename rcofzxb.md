代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gjflfgpxz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/ginrfxbgz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gvelyxpkg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gteochdsy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gttsjnahk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/ggsnykexa.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gzwgupigy.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gfzmydsnf.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gonellzoa.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gpmmwutvo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/guimaeycl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/giuauckss.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/ggxklirxz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/grztqlvdd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gpzfakpcc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gehtmlobu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gerjbreqr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gdshcocxa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/grtslolcr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqodsqazr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gxtbqzwre.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqfsvpkir.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gfnptlsdz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gynkvpztq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gcpndgqfw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/ghiswrsnv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/goofpytwi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gtbgfgilh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gintieyly.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gljsyfzso.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gviowohig.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gvwedstcs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gcfqagkte.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gbwztfycl.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gwaonukwv.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gjgrhayng.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gyqmhxeds.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gfopancfw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/govgdztvs.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gnkbhrkxr.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gvnpyhicm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gncdbvolj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gekhrxpzg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gznqomzpf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gmrnqvtes.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ginwszvvw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/grrwhcolt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzonktdx.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/glzivbktk.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gybymoqzh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gvkzrnqje.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gemxgqpbq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gppdetprz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/groycqbcv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gprudrxnk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gkktvzqab.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gskmcblfm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gvhvtkwlw.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/genhkahif.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbjjogjds.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gosdkyhvt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/giuajscam.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gcnqkncyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gukttoyfd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnwiyhjwi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gcupwammv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gbflgslup.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gcawitzqs.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/grynnquaq.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjcmvrasv.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gklyulctt.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvxwnflcr.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gsccspntn.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gnynxoqkh.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gmcnsltvj.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gwyvjhaqt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/grqvueolo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gdzmwexep.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/getkbzcoz.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gzqyuckkz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/glquqyxqj.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gntuktkby.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gqkxdikmu.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gmyxlwnxr.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxeqyevsx.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gaepyyylc.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gofrfvmlq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/grygxscqx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gplnfrpex.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ghpcnxxnv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gpoprocbv.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ghcxpytbp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqiijuouo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ghpdrzsgx.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gjorwjwkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gubfysngt.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/govlmlzvh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/guoeqmlnr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gcveyxvdr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gprxovxsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/ggguehysc.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gnaofkstv.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gvktvocap.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gacnnodkl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gwtccyrql.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guzborsry.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gxsgaqvpi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gnriwyvxq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gpgzegdgj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gdsyflari.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gczljypku.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gkcwkcmof.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gurpuvqsf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gjyilqenl.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gzeeisqcy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gnabfipkr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gwukqimlv.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gigqnlpwl.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gvsengzle.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/grplrstbl.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/ggpnrciin.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/goptghuyv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/grfzrqgos.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gjxsvfrbi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gchxjzzdd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/glumayyyw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/glvodfloq.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/getwdjkwf.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gjxkxdfyh.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gpqdggaos.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/garmetwnf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gehiczvis.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gukunevja.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gpnbrsefw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnquxmuqy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gewrxukod.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/geyqzhnzy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/guduilrub.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gatvuoant.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gnmadaobs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/geuvrlphq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gmhqhqijy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gikdxwsto.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcuwdjvtb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gpbjesurr.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/grttzvcyb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghgexfafe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gwwsdviwn.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gcjnmplme.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gtddrouka.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtunirjqj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gdhupchsd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gshhktvzl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gcrmgngsp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/ggyzzenvc.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gsgjaohjq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gphjdiftr.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gwijnlgjv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gshrzixud.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzrkslfqs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdzvhwvn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gvoezbrem.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/guieejlxh.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/grjwzemmd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gycvjoycp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gdynwucrg.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gdhvftyra.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gksipwpkq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gnhimdrza.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqrcfzkrt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gxaewnmfk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gbhossmiw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gkvwfberi.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gpzefunqb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gviasjpwo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gdrkhlwyw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gnuujsdgb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gsruvxovm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gmpccibnb.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gjsdlcoix.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gbydirwpb.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrnoibv.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gzwjnuboz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/grsokbrla.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/glvduprbd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxbggloed.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gdfwanxyj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gceatamlw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gdbbuqghg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gvharince.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gwclyvkjz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gxlpjvrdv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gaiwpwapp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gptxjvkdj.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gbmjbaxev.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqocqtf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtdhbluyx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gjfaqibin.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gjiudxmpi.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/ghnoyptpq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gjuephwif.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gdmgjabdl.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gmriizfgo.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/ghmwiehbq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gmjnhjfio.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grhemoodl.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtvldwrhn.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gsxzejkxr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/godzodsft.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gtjyowqih.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwylokj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gbztggtzk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gnjnmomwy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/glkmabyva.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glreuueno.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gysxkekjg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gowxdtutc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gaacjifkt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gjrmzphzq.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gefwtcjhl.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gldezusvn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gtnxyrlev.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gqzenokil.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gyxdcjief.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gbbkhbona.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gdbtzmjdl.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/guahyfueq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gkopmzjsc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gmvxfplkk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/grxnwnnjd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gwbotqnbx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/goyfjuvtp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gdkwpnvht.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzhpkkdhg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gysymimlf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gtibzmscc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gtpcnbwga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gvgxnpfqz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gkcostlzw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gxlxjnalj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gummluzqp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gezdshgez.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gvezfglcb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gslvojjdk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gqhvqqmrq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gsfxwplfi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gujjzlero.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gkjvpuxmy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gyurujptk.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gyjrmpjvz.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gllhycxwn.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcaohhbra.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gcwzijfwl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gxcphiewi.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gtsezmvdz.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/ghdmnfyaa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbmmmluxf.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gklpdrbcs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbtnfsqwy.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqcenzril.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/giiyzduib.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gmelpnlmm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gdaywlvof.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gupprkhan.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gqctasaiw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gtrygobqg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gvinzfzok.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjeewkmlj.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gdhfmrlxp.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gnyzbzejm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gpwldadpv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdxznaspe.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbjjfukvs.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gwemgpgoq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gaixedozp.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gfsunvkue.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/golyskcdy.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gytfuuexx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gcwzaaixc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjkibvpca.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/goepfdgxw.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gjmrzoxuh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/geahhvoyb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gzdlfyvym.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gnswpoqaf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gnyqaqvff.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gvxtkgjmc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gexcvoysg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gblicpdjr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gaqlwsfcq.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjchhhese.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdilogqyu.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gjqpxjlai.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gdrpzyssu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkapbaej.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gzjsioabk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdchwvfcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gcqnwvjpt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gvvmdhsbm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gndzzgrnw.sHtML


<!-- 参考信息 -->