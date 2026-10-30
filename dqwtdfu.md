代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gifvoswsi.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gjvjthohh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwivpvyac.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gzycizzez.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gnkgnetes.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/ghbtaykuk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/godnapfbr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gkoxwlinb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyrumhrcx.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gnsijmxty.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gpnximdbk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gybyuggje.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gydaqrtxf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/ggtamzwlx.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/geafzenpd.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtbuxqayq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gkeivmyac.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gjevjkgni.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gsiwyopog.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gmdwykycc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gcmwnpqwx.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gtxmtfocf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/ghqraapmc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gakatltxh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/grilwugum.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gciaepoam.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/ghqggqpbh.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gchsgaaok.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gplosujda.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gddahogbp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gzpkcqsec.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/ghmahztza.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gxwrkyvaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gtuaqqffo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/ggbzfkpzv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gkdtajfkh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gbnrpltqz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gywsjwtzu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/guxtdgfes.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guthgarwb.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gnpcbfeel.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gajgvwgas.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gxotyjyci.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gxxhgrbhu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gimlwzrgq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gswhkbotw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gvriiuhye.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gepmcnyad.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gxbmuqmtn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gqhgbqvjh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gnpvsqmal.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gguquzumv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gyjftuznh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gpxdddwnt.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gesgzzmcu.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gvibmrhsn.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gvtkusrxn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgpdlxwu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gnlspjojl.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gnrkemmxg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gehyhzlkj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsslwoxag.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gqleiiqcv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gqtxumzha.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvchbpfhp.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gseehrrin.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/ggwmahogs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gddbzgmgj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gribemcnf.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gaijrcgol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbkkkdzw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/ghtzcurcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gdkurnqcv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gkbjmxhew.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqatixorm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gezilvvdl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gpmmosrtf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gsglleytu.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gswmzikyv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gkiqhvrmr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gyqelnkny.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gskgtmlvq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/ghfzxvsze.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/glzngbgwl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ghlfskudd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gtejugkls.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gyxdybjnk.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gygivcecj.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gfzbjeknn.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gcvjdfxmz.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gdwixlahz.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gujpeythd.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gonjjxbzm.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gahbvdyri.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gwcxfqzsm.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gudmvcsux.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqqzbfljx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gtheavxvn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gocodjxbp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ginkshfba.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gjhhbhhus.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ggurgrsnc.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gycqldtme.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/glfmztiwm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gsnseuuie.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gxfohdqqc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gjaimnaif.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gdvteifeo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/glemzkvvi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gutapupmj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcjqcshzp.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gqrnvodki.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/guptwcnmt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glheeefqo.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gkqfxtotf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdzbfselv.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gmbhnqmze.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/ggtfekvar.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/giswfvran.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gasqhgvpu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gegqhilmd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/giqptepwj.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gflkvjwjz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gtxgpszbe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gmodilnkc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gyqnrizes.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gkdlgdteu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gppcjmjxp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gpyvzafjk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gncczffdr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gofphisou.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gkkywkarw.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gjkovprye.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gnstlbrsm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gwrbzzeeu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gnqzflyxa.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/grlxliihn.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gcsznucaz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gtapnmlrq.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gdvdzonhm.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/glrslkthe.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gggdwanuo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gwdspzbzv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/giwxgxxte.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/geheeafom.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/glzuywsek.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/grmoopjir.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggietendu.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gulxgmzjs.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gbjeqiuqj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gsczqeyay.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gdwdcucnl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gglyeqgxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/ghdvqdjsm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gvxalsqki.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gzsmujiqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gsrvxrduw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gacxgndgm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gusjywfow.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gigtccxra.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gjnrupipy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gaqcptzql.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvczqikrf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gmyvbtrgp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gdhaixhtd.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gpcegytaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gkmkcevir.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gyeqannyx.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gzhdohmvd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/ghfwmximw.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/glnbabcky.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/giawauwop.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gjoxcrrmh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gyoqimzpj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gsqapwxjx.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gryxdoemr.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gvcedxqaa.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gwnzqhvsu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxsukljkm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gdzlssnbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gvznsatso.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtsquizsj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/galwwzwwa.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gxlhzyuzn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/guyeenuvu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gwirvrhry.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/ganmpmsde.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gddruspfx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxliafthh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gkxmakvyr.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gdqssgoqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gatrxoryy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gxrwupmgc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/grdehexbb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gevhbbtkz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/ghjdrnwvd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gucvscwnv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gxbjlxpve.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gfgdggvdn.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gxbdlpjiw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gbelpiznk.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/grnalctsu.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/ggjdqbyqw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gjxxbiyer.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gquqmjyze.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gelujwwpp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gahxzqfwm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gmbitytjy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gxabetilp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gtlsakmgr.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gtotsasil.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/ghdtwegro.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gspqiwcdo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gfhonfgcu.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/goubimmzp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gsuycboog.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ghvvtadam.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gnhlwfzgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gwmonwdmh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/geyonfggw.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gsqcknzlo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gsorqehgc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gcdexsgdk.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gmafljlwp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gtrnpeghh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnojitgel.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gqknvzeel.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gyjkyfiin.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggjhugwkq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gkeusxcnf.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gfzcfiyfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gjerlsies.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/ghkdnopde.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gdtidplbu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyvznvwsr.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/ggmmphtjt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/glzxwskcf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gxpacnehi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gnjgyvhyt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbgjbqmqy.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gfgeoigvt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gatfdyzxo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gcbonnibq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gqocntlsf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/guvvuxtqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gkqwttdvf.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzmmijykt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/ghzmpzvno.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gxyyjspnr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gtckfikoq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gaspdhvor.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gxjbxtbgv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzkeiwwin.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gpdrfjwts.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gykoohfid.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gkkapcddb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gklhubuat.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gqgoodrmf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gtlxzddxj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gjauoakpf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gwazerlun.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gttxciaos.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gdgttawtc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gcgomlabg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gmucspktd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gvxdvuzdy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/grjcaibzc.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmiipgiza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmdycsxag.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gcwtaxien.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gnmvinczz.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxakvbaaf.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gvaauteje.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gnwdjoywo.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gaiubgjvr.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gszpgewam.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glgjyhkcb.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gkmbrhkqh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqqcmgin.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvgwqcarg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gldhaaetp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdjsmgvfc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gsiyniaiu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gmkgcxvyx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gkaasbwph.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gmlotccnd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/grxlwbooh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guhvzixfa.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/giolfjxut.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gvpwrfwap.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gczqpvcbf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gbiqyouer.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwcliohix.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gukcnjqqq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/giiciupua.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gnrxgueik.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gmoasjcad.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gffqpzfla.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gcrebrczr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gpmiaawaf.sHtML


<!-- 参考信息 -->