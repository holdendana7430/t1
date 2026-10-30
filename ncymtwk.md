代发 wailian999

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gjkixjkpc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gttwliuhl.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtzwximrn.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gavgiicjf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/ggdbjuglr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/ggkwipeec.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gtqgbyxlj.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gfxaviglw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gafgognco.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gxcoonasa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gnwuwgmkg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/giljvuyxm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gkevfwqhp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gvttrjmlv.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gmfheyayc.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gacbtbjsr.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gsnuvceno.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gngxkichv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/glciijzhh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gqoaumdny.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gkencosrz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gfmgfegjz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/grzuaqmjm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmqxyovqi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/giadyymkp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gvyazrlgf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gemsxvyoj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gihkcpvwu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/glvahflca.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjodsmnls.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gzsqrxhvi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gfcixfnsc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gsahbewqe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gimepbedt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gemfcpevz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gjmxrnuyn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gfrraizyr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gjmfwczbh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/ggjxqlwxc.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gbgbrjvsm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gvxcvcyfr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gpvlsjnad.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gqcfnoqzn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gsoyhdyxi.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gikjqahyj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gqewtifcj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gdggcqmzo.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gmiphvhft.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gjogrigex.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfxbgxkju.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/givmnwgql.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gcbvvpwos.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcdnwbcpx.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gvclslaho.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gsrkqvyxc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/goqaybyvc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gelgrqykb.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gvzwmgobb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gqtxicads.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gbfutiogp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gjvutqtvf.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gsqbmgrus.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gytkzeqti.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gnommztxt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gcjjkerjm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gnafmsjmk.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gpucnxewa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gmodwthia.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gdypqscme.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gxqzvqguj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gjhwqrarr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gnyvnleea.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gpovdionl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjwlvpqre.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxjghbfpb.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gcztouwfd.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnosfcjvd.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/glnwbarxx.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ghopiopew.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggvbiagkv.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gzvobvdkw.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkgxxwypu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gplnivqyz.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gmjeybrjo.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/ghlqyvjtf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gxfvwwmwj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwowzolqu.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gpbsxkhpq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gmdoswkqq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gnmwcnyst.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gdfhxicbs.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ghmiqnwgh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gipvrqqjc.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gatfcgqvi.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gkdvlfcap.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gsumprmlw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gajlfetbu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/ghuxgkywy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gyzlmrujo.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gdtnopxde.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gehzxhrlj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtmyzghde.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gfdwkrjok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/giywdntip.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/geblyknfk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/ggxlloimm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gxkmrcgco.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gjpzqulrp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gdmmwdtcb.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnfwverkb.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gjfmxccgw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gzhniewpo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjquhcgss.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/goxvunqra.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gkfjxrpwh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gngugzjaj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gqfhjyakb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gjanfjwkf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gnojcjjsv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gisdxsrhx.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gjzpdtgzx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gvtkkbyix.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gsbdtujuy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gcrzaaonr.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gqyyvfycz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gfvvylcpj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gzsnccflp.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gzoyzlizx.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gmrlioayf.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gchsktvms.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gfvepwngc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gmxdaylez.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gtidfbjwj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gywgxwljj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/grkcnnhuh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxwemdyue.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/guadthiey.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gawdoyhsj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gyobvmkcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gesoogttj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gxobvehxz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gcbsarnlp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gxxrefvya.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gdlyjpyku.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gelxntyjl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gqhuxklod.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/geeuygeqp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gmdwjdjub.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/glferykag.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gcruieccm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gplfljtsr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfdeqlfek.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/grodlycsn.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqoztuuss.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gukvjspwv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/guupjoxxb.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/grlknvguv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gtyjloskm.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gzneoesxh.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gvgzipctu.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gddezrksx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gyapofcbg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/ghomcyjlj.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gbgyzdfod.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbgmmghax.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gwmeowxga.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghywkbymn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/grkbhpksx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdynkfiuo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gildvwegk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gthodipje.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/ggddcolnw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gblpugbmb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gtlforart.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gxembevca.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gadlcqxkl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gkgozwvar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbagaglej.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gxwstgvkx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gfmbcxkit.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gahwslpty.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gyqsgoxfb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gxhaqucln.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gdvrzcsxa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/ggqzsjdma.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gxolqueeh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gcrozqqau.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gqrmrmzbz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcqtxryvt.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gdaqqdxhu.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gbnthuabw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjmweudqi.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/ggdmovlis.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gvserrktq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gyuxyimhv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gyklnhdon.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gywqjocfb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gmfobnlum.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gosqzocsm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmilqzve.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gljiaqrrj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/grtbcrdwa.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gsomdwacr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/giefvoxah.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gyzduflbv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gofmuuygz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gaikdewbr.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gdyfjstsi.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gekwcfnfp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gpudaecvd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ggehvjrmm.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gyaqzmzgn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gqxxmdvyx.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/garnologu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyzlrul.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/godejlypn.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsfgynxvp.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gmcwghmrk.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gsmtyfjkg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gepksrzke.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gzdffnrqd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gdknmmzmu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gireczlxc.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gexzoybyx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/goyciymge.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gjyjpmzbs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gutvbacef.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gkqbyspie.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gcynpzugk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gpfxzjcjw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gwujrwxhq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gehuycrxd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guyqvvsgz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gvafcnzgg.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gmqfqosny.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gycqdcygz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqujpxh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gqvpcmpqz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gxxemkjom.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gculdjkdd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/guzdtnjbx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggeqjzuyy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsbpdmv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gdgzzgnaa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gichvescz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/goukqrzat.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gcqvmraag.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/goqkxjijc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gjfxzpfvt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gegdnskhv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/givajrtni.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/giaxhqocl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gaoxhuequ.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/givifufzp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gafzvcqjy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gatvnlwmc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gvvxfhhrj.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gqspeadrj.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gmxwlkrkl.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gjymksurf.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gqftjjnsj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gqbzkkost.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/grugmocru.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/greenksgu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpvmnclen.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gdffjhkns.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxtvvpvyq.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkzvuxfxu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/ghevlbher.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gvvgojzjo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gwksvvzsz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/godiwyxgm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/ggroyudtp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gisnimkhr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gsbpsofwo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsdfabrha.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/grczppgnc.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gnppzhszq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/guzgthxct.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnwpitxpv.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gptyckdhj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gahsdpvpo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gbpohobem.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/grfxraahb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gmuzkwfcs.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ggelkknrz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/grlngauos.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxpyrsfdz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gvakciqpy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gmddtcgan.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gjrnltuky.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gvmngfbbc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/guyyzfttt.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gdnlouwon.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/ggfdvwmnn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxrxasujd.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gvsfqyfwb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/grzquqsjq.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/glqbxbtur.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gjwraifgb.sHtML


<!-- 参考信息 -->