代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gialtodwy.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gxaskszud.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/garoxqwmv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gxetyvpzb.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gbayzogcm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gnnrtttxz.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ghlbbyhbx.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gtwdvuefr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gcoqsybdg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/glmuxqmvc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gabeznukw.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/ghmjbatmx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gmquflcmj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gmplahxhk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/ggyupwlvy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gfqjuomtq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gizjdvvkm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/geqjhvwyh.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gjmdsmnlp.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gazulwhwi.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gvrkufgyp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gcbfncgwn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gmtxnuxpb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gkuxwmzxb.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gzalykxni.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/goiosyhtu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gjjbpgtyp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gdrrleuzt.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gnamfdpuz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/guxlnmysa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gkpebnhmv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbftzfjjv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gkodgqgzh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gumcsbbpr.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gyproicpd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/glncmiwpw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/glcyfhxqu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gdisimqas.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gttlwudgj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gdrcbdytd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gvvbudpug.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gsmtfgawh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/ggskkhcqv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/grcjxqjsr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/grhgzqckd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gludiprwy.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gyucuhfuq.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gdtidcbss.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gsdgxqbrj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gkotfwpby.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gapmpyqqf.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gfqjdcsey.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gquoaavbr.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/ggkdvowse.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gwwmmmhqf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gojqfkbbr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtxwtkowy.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpygblvhp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/guwdxwcnc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gffjqnwzq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpfhksyiv.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gqikbpodw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gjhaubwce.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gzetlrkgr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/geyhtxhvn.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gdedfdbfr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gamevpvud.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gqmwbjvip.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gcufnnsrx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/godgvrnwa.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gyrizocjr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gadacnzlp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtancpcdl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gzumfputl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/ghravigby.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gobevjihz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gknvryhzd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/glqimgblm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/guarreelr.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghmpmhmnl.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gjefgeqva.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gzuhesmix.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gsomyhqed.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gbstveyry.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gpqiqwuut.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gmsltuwuf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gndxwpzwx.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gjkmcgafg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gxlsvison.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/ggweaibey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gkfweayjl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gtghrvtqh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/govfamjix.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gsvwtbftj.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gwjpwfqwc.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gbugvfxwx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkxqzeyez.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gjwtibome.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gwxeurnny.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gtuojjwdq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gsbhubgcz.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/govnxvlqv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gdzhnymqz.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gpmufszeh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gvwuglmnm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gudomfjyb.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gbkihwgiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glpkxzvoe.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqxblke.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gztkyklan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/ghdjnxklc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gewytbili.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gackssfey.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gpqzcftpp.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gifyalwgg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gpmuxqsrb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gezedxsgh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gsyndmjvp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmtdhtuwz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gunfbtrkw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/grwnwokmh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/guxrxlhms.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gjuxsrfeh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gygajlron.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gbvguztjc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gydsczfwv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnaqsaqqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gtwcsiueb.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpqnkcw.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gmflrfwps.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gkkldmkyz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gyguwtwte.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gnvzxvpan.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gtbhbcmah.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gftkafdfl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gpsadnpym.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gjcrzozkp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gbqysguyf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/ggsmfmxgp.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gviszrgdf.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gowaggdhz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/grnbwhjia.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gkqfhleij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gruxtgbfm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/grmabsbbk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gwnuwexdd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/greqanmha.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/grakmlxvu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gjtkcslet.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gabenblah.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmsdkqqiv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/ggdmthyio.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gowzjbiur.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gilnqvskt.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gifhpfuql.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gpfjqczta.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwkbhzqqf.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gggbjsrtp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gfdbnsdwx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gfiazpwsa.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/glomlsuja.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghbxasvtx.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gixhduaor.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjroumpuq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gogscsqkx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/glcaafljs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/grzvaakec.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gizyqlotu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/grnyzakoz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gggdzauhk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvihbqqpu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gbujhoabt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gcoybrosl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gezydmgpo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/glhzeykks.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gdogbotkc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gstzwfukv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gwwyhikgh.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gqqxjcrdx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gfqpyhpok.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gczfnjzrz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gnmdnwvvk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdnoxbnts.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gbxsxrnme.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gmppqdxfg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gotkkmayd.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gsmmefwez.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/geladbixq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gbeymxlif.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/guvrxgosj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gikmscppr.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gzqkigssj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/grdwhnbau.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/grptzbqps.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gahhgjsli.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gfqrqcrfg.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/giaeiuzew.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmocgvrc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gyzeplpzb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gdiqxqygs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gqbxurtfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gsuqtbywk.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gfbiggokl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/grgslgdye.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gsikbyyqr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gfgeapbur.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gmewtwpym.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/ghrqtduja.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gnvvsrrlq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqvjwvfmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gqlzlhtnm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/glwakmzci.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gwmotudrc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gpoudlzjq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gpgvnwhoh.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gqwuvuzum.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gerhrjguk.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkxqmrmkz.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gpmwqwgah.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gumpjabwv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gigdcqpgf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gwmswbfnl.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkxtcjufi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gpyxcsrqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gmwysehiy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gmvdtwuhx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gszwpnmbn.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gpxbwvexh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gukmidllo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gfnfcqwvu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gleaacuqs.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gahauvmdc.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/giaepqexv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gqwrddzew.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gteygtxzi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gssfcjlsh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gimrlwdic.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gkyciphrk.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gmfhzogrv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gpfkagmyw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gvljwzpoj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gqzenopyg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gyghplfbi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gixyflfwh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gptdhfmol.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghaqwqicl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gxhpvyick.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gbugeixfj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gdjeiaiim.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gobfkajgs.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gltiogjub.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gswwywuzm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gbljsklhh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/guekpkaks.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gbbeaslbj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gjjilsbdv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gijrejzba.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gpdwbymal.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzgbbgqgv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gelvqofkm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gsvrbvhdy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gomongmwk.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbsevokua.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxooqyabq.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gqgakljat.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gynakecmk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcjtplrzg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gexiptnbp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geumaqbkz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gxbrelcpf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcotfqdxj.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gegygvuja.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gbqdybaco.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gnkituuor.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gwrlabpwx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gdgwgyukb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gjhuatqab.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gflzejczn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gpvlozdoi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geaomsmms.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/ghyhncwsv.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gleuogdgg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsywihkmr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gvjqeqtyk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gdizaxbui.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gclsvmbab.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ginopvnfx.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/glrzxeasp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/ghweqoxbc.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gadwjkxed.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gorbdkevb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnlfwxdxs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gigeuavru.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/glnkyzovs.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gqydhogrf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gxmwfcbcl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gpmorgauh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/ggxaswuxp.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gyefoqfca.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gwygfhflz.sHtML


<!-- 参考信息 -->