代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkhiyeidh.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gnhttcoga.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gzwogcatb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gyrfxlgxx.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gxjojosuz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gptcvioer.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gbgygoyij.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gryaqdkyl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gighrmgsh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gxbhovgvg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/glqjfkzun.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gosdxxeaq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gekrpvjwi.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gusdgmkpb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gsjrwahim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gnjiqaqas.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gegnktztl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gbnoobghx.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwsumrgrr.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/givayrjps.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gjjaflxfr.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gifjnwsuv.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/givigltnr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gvibnkcdj.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gdlkhtcrs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gcvesrxlu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gukebrswt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnuqjeakg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gnqavyzuj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/ghobroewu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gtxnktzew.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfewibcyd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gficiepym.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gidkggjzc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/glcpbwlay.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gmzpdovsd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gkmdpnxvb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gwbbjgfcp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gxbcapbjd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gpfqgfzkt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/ghkxrqynv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/ghycvkfzj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gupscoonn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gjsdojajs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gmsepzyyf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gtoydhkif.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ggcoezbkk.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gegtovucg.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gjrwrhmdk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gokwczvva.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/glrcgduxk.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gvufvqdzz.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gtlomqrpx.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gcnomzilf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gzysgsqgh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gyvclkctw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxaclnllq.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gxqdscksj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gqdrsnmdw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/ghplhezra.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ggcdrhyyp.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gmttvkpzh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gkwpwjmwa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guogiqzrv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gioxgnhrl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gilzffdzm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gqiygchdq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gvgmluwfh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gjfrmhqhf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gqvpubpju.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gmstozkmo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ganyvawiw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gswzcbdal.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gshaqisju.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gvanssmzb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gbrwcrhxe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/grofflekn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/galjtquww.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdvzecosv.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqlyytvwn.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfjgwrcbh.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gtqizzbdx.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/giowdyevu.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gaysqkqkb.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gwfkexcyn.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/glmhvxdje.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gtdbfzcom.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/giuhzaxwd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsivamy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gkomazkgn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtwenkwiw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gddiichkf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/glqtdvqxj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gsavsavhg.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gxsiyhfkf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gqkmtegve.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gefvypfqs.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gqgaofcpo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghrtfeksa.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gpzalgpob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gxcoltvcv.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gvywxtqqe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gqepxtrfk.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gntctvaup.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gaoykxyhv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gdstszhod.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gcjfebdol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gtxkbmahi.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gntwgrdom.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gkazolxwv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gnvsirjhy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gybmmsxtp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gsrliohoc.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gdfbsrigy.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gfxvdkmsv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gruheflhy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxjnjmtiz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gknnhtooj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtinovuto.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gkixhmjko.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gctqttpqc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gipjekhxm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gadlrsvui.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gpwdonjqc.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gadysvzlk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gfdklefae.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtvxbrfrf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/govguihyd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gpofdhsol.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gxlhcwgxd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/goffmwddi.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqkjbarws.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/geqlvrqff.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gqgotvimd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/ghtmzsvze.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gxxbgiypa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gybdymofm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gkgnhdjbh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gmhvcnlfh.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gprhfrfww.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gapkzvwhd.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gkdbxxftc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/ggebmarvm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gtwuzetkb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/goihuzsdg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gdprlczoo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gyblltpun.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghhcssnoq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/goiojzerl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gyqlbgvsx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/ggizczmjt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gsjfptico.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gnsgbsghm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghenrzter.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gddzsxvzk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkscozhyt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/glsphvilg.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/giqlcevkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gkcrymjbr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gcjjgmnoi.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gzzwldokl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gazbbenoi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/grwiegwaq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gqltcuazn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gyazecpth.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gmsfeuyku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gdudpnazq.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/ghrcyivhf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnnfqhxvl.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/geajlmqcy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gbbfxhyjc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjgedmuxq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gdtokumao.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/ghpruihch.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gqldvkejh.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/glfweobne.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gmligtkau.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gjtmikdfq.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gmhozfllk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gwquymrbx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdfpfigto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gtfktlkzt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gjhlwjvmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gnyrpduoo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gzzadckkn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/grdjxzmnz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gngycyhst.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gjwnxeuvy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gtohjwqab.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gugjasheo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gtoytqtcg.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gvmcprqzk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gtxbmhroc.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gasthywqa.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gunwiufji.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gveenzeao.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gczwsrzlj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gvujqmxko.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gfiqbilhu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gudyydcqa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/geytxpfwf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gisdfhimm.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/glpbiwvjg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gzuyksbrx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gqkkadcgd.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gagfouutl.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gmabwfqlw.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/ggvriewsr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gdmkzxfhf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/geqnnjjax.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gyvzgulht.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gdurfjncz.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gwywhlobm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gyiqjsaic.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/glztyhocq.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gvcvwpqhg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gfbnwrpwm.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gouqfgqhw.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gaxkyzigk.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gkklbwqvd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtvexvylx.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gubvkqhwi.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gduhunwaj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gwrztndcf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gzngvcdvc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gbfnibabu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/grpknxjrm.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/grceexxei.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gsyuozdqk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gfgpcljfw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gxjogbbnd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/griswhlbc.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/giznprson.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnttvydeb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gkomwhmyi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/glsxpeirt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gyzoltxxg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/goatoitjn.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/geqqpacqb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gmfoblekq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gxsvwxowj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/guthtrudl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gktlreesv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpqxzpkdj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gcigrpmrh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gfxjjxpma.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gyhllzzmj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gddtjdals.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gtdwntoub.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gygxfbibr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gvofiqdkq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gfymvnhdf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gnadwtlfl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gnuzopxuh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/grplmdlou.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gltuickkf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/giijabvac.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gqtpjdlob.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gefoxcobh.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gtdnmakvw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gzpdbrlgt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdjkqhrnv.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfuccgbbe.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gdoszdoyn.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ghdzyqblc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gayicoxxc.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gfkhwusdb.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ghmqqhbot.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzdvgcina.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gqbdxtsrf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvxuvpzxl.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gndfscmmk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/geowncfuq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gfkhivhyy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gcwkdhrti.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gfxvwebog.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjxscwj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gafhlfutq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gspdeajsu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvvosfqvi.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/grzkubuot.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gdoiadauo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gswotbxwh.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gkuikddcw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghikjnfbn.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gaksdirbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gvmfknokp.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/giyttrjcc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gkdqikehf.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gwclwsjpv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gdefvsdsu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbvcdsdjw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gsohxgtmu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gnctwnhkl.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gounprncz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gmdzkpgul.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/ggcwhheqo.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gjhzeoqec.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gvgdeblfs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gwgrvlybn.sHtML


<!-- 参考信息 -->