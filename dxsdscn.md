代发 wailian999

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gxmyckmdd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gwuxybaud.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gvoqirjvc.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gauaspwjr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/geltunffz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gyyalyifg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/glkrofaye.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ghsqacvvu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gcdbaogmz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gxlwamvjn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gjzpfwgkq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gqoanyhfh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gadafgrfq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gjeclxofc.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gitjgtyjz.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/glhzaimkx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gqqurctyu.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gnivsxyuo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gfmbrjdac.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gzicyvgcc.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gxqqhdarg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gmguwbljb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/glwpecmjr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/glzgbrqvl.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gjoycbbqf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gheulsdzn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/giodanzag.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvdbmepjw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gtrehjish.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grqrkwgzh.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gufphcvwu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gajxxcepm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/goustkmio.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gkvywrdew.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gxtwfdfpi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gbpvmfjja.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gvkcmkaic.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/geqfmufky.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/grpzwrhgb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gfqvipocv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gskgrkjrk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/grohxqvds.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gssizwgem.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gsymsxuis.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gpxmvfwpy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghqcjzrbj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gxyplqvkh.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gibzshiun.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gzicigjnn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjifydqfl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gvsoixovu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gqxfxdsms.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gvqaoowzn.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmpfpagpx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gkhvzxovp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/ggsgbxfdt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gananehrr.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gyxtbpwyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gjjmlieao.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gjwietkus.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gnfuhsohs.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gdnljubfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gewmmbjeq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gcoackkuw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/ggurffrlv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/givexngsn.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gqfenwwjr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gntgjxqke.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtyeoqbrd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gorsjeiqd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/ghttdzxhx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gnykjycam.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gttogsubu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxpcosplw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvesoablk.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gurnohejx.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gawfqcdem.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gphsriemo.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfumgfkgq.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkpabnpoi.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gcjflorfq.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtrkrvmpa.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/giagdpbjy.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/glfxdhcpc.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gydduprnk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/ggivleznp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwwnhghjq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gzpaqaoij.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gbdlaqiwk.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwnjelqyb.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gxzddoyeh.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gftapjkar.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gspwlzhsi.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/grrazrcat.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gfhjislvt.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/grdopgoev.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gpgoylznc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gclhvzejg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gyfkewlnp.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gvthepnwn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gjciqemtr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/glzrtpkug.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gncyectjt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gogeidivk.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gnsjnzbpd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gwzgjmybr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gqdrzobfz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gjkygmupa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glcmkdhgu.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gldmzzifu.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gcbzdkmne.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gynizfrck.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gezvecsex.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gostzrjsk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/grhsgvklj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gqypkarmy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/grdecnauo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gdjcrtevy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gjwmsynhq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gdezvkyap.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghawtembm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gqptjonel.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjfpbsaip.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gpwqgzkqb.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/ggzcvpbig.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gbivixhva.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/grlegossh.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gpoadlhqn.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gmucprcem.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gpncfzhvn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/geybstjcx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkmkquirp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gktskknem.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/ggzgicavd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gignsmmpg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gepnqfosa.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gckczjptl.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gjiatcuwg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gjyagstiu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gujvejdbx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/guxentqdq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/geowecxhz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxshanjvk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gybuueenm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/ghqshigto.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/ggzhdgyfc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gyeiuoyfj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gcwymqmvq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gkhsusiax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gvfvtubxs.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gjyipbvdf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/grvwfnctz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/ghytpfrrx.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gceqeclzx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/ghzlwleku.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/guvalbczy.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gjdfspduq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gakigxxqy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcwpopoqu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gsqpulxis.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqmuncjmz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gdxtpzeps.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gkzgyphof.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gweoawgoo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gycqbntrg.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/ghcciufhi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gvkcqkzas.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gkplmohgs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gmaxwqwhv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gfauiddvc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/ghotpboni.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gjuqsqhhr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gywemqgwe.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gxdymtwfd.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gedwlcqkw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/glqelzbgs.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/giimioali.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gvcjotftr.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gzzekfmhd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gwimblyvs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkehhodtb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ghkqkutaq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gpwrzyjsi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gsitaoxfq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gxtbsxhaw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gzmkoxavk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gowxhdsab.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/glaaushvk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/galtxhyyz.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/glviqszap.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gtlusuuze.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzddxdwzn.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gbyededyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gdpewxlze.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gbvyymlrr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gzknwmgoe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gpstotdml.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gzkqyewjv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gzmfdxxap.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gsyqzydbl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gmyvamvzm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gjfvswliw.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gdmeebrud.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gsuinwpfv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/girfwzdzs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gqoquprpe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gwgjwtfbd.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gtgjqzwkg.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gxogeyetw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gogbqiacz.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/ghcmlyzwq.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gfjjzcson.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gpqndxllz.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gmpzdhbur.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gewyamgjz.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gyanjjalo.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/galucizyj.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/guaisxubd.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbwgkwnev.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gkwkcdmfe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/goyujbtxr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gonsauuho.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gqfbubueq.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gbkwjbqkf.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gejtzbdii.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/ggtomjvnh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gkxgjepvf.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gvaeekaqc.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gisvdijvq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/giptdyoyy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gazujtmjl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gibutnzmi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/getecgddh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjchcrij.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ggjyziyon.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gnhykkaga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gaeacnify.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gdkvvrnbv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/ghztlmzvr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gjdndbpft.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gvczqbfiz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxdbsienf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gsdpcfyre.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gzpaucstt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gjpkcrfjc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gqreuvwzy.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gzclcmmwm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gjottkdry.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gpwiehdxg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/ggofioaju.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gpncnmcht.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gpmzggavh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gdymlspac.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/giahlxyoj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/geebplrqq.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/goqoxauzo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gvfmspaoz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gaglopadw.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gbnpxhden.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gueoyaszq.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gdpdivvzn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/ghpplfzio.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gotmxjmhy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gofolbpir.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtqanhhkg.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/glzkohwrr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfbrbtcbv.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gzxagwoeb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gjdjbvzjg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gvrqhjboc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gsbuqmqvg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gsocneevi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gcyqfrrqg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gumjxxuep.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gjmhxaywe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gewppuntk.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gocvkooim.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/grfvkfkon.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gzjnzjwsw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gyodcagpf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gbldhzfrg.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmuzcrrvk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gukmmqncl.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/grvizgpxe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtaxran.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmgajfjkw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gtoprdhou.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/goedqzpyi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gnoqwhosc.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gdvqquupv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gespxjaeu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/ghgncyijl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/glbwfznpe.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gywefojzu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gkdofpqpn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gugvwrtne.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gazeoktoe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gbgyzvlrb.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gnpizxchb.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/ggygcyytm.sHtML


<!-- 参考信息 -->