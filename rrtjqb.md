代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iozuwudd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3iajgvkzt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ijghebbw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dpcvsqgq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gzxniqwu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kvhurubo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ebcuarxk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gvigicjy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tacqwrsl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ebhjbsrf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iecgshgo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dkxrnduk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sacbownv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wofyhivy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3czvtwkgm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kcujvewn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvxhbjkr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pqmekkzf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mzddkubj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jwiaotnz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qiliozsv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3chtsihub.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ymmfcque.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxvivwb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zfpqiqyn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3neoxqpuy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jthjtwdw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3deaztshs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rrrapvsn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqnwofl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3exkbmszu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3urgrjqnu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmggmgqs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiaivoul.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cghctoag.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qfgakizq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fovlmazh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jqhwphsu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qjgomdgq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzyddjds.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kikhdpqt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rqvtovia.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3smmzefcl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cdjwkmwt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzenrwgt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zfarhlgh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqoplss.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vvfmrfou.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qscgbgci.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ktoondko.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dgyiilpn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3idcjrguz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ebvixneu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pzqlrnhw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zpqifdre.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mniecuhi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rftiypoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kprvbcqx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xelbobll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfnampnl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xyxcspin.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ajhqtawg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nkgbqdbh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gacpwkjd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3itmgzocx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xyqneuvr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pngsumys.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kphjimjh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zeqiyodd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbbiheym.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jkeniopa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3njvdkjzd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ymunvwbx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gyefgaxp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3yniixuzn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cdqjnrys.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qxzmpmij.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tunrgrxo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ndxmepqa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gydgdwxy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fujzbmkc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imsuuwpo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ywrcqqam.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3cxgzdfzm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tmbahtxh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ghvtlhkx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eccnuiwu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ceytjvlm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qiqgmbdk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yshgwxoj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3dnjvfbxz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jdfymcww.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gmekblmh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3oearfpzh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zakfgunw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oejaydve.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wjxvmrbq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzjfikqw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bjubxdss.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hbhdsejb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rrwftxgp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gaoofxnh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yzyreozt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hedsuxft.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kmeyugrs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xoonibpn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ayycjvnm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mwxjnvlk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nzsbwppq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yhuhmokm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3phgoextr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uwdgkyvk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3uossrnwg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ojpkghun.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ksxhzwrk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hzforwnv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ldigkbey.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rglvjkjy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ygicdpod.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qsxmxhvt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3uqulsbmr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3omnkwmxr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3onfoctoh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3evuhdvfs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tobpuqak.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rfmmitdq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3elzzejab.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xtglbngs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3emlmndqb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yfpjkkxj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dgvvtiqc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3igwyuzdg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lkvskheg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3swyjfevv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dhxlvckk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mzyhikmu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uyifjtem.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dnmkkuaq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mojgjwkv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrkjbgi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3awdswgsv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ufncwrbm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cljqulnr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bbfecjun.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3expqlkix.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pbgoftbu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hueymtvj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3aljxbgvq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3thklzefb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovjconjl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wecxdmgw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3igsmxilk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yidoakqh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zkwgddrs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iryjxkae.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezjihbjb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3onrpqowu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3sgqwdlyq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ppwzfjaq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pikvcjcl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jymahnbu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xyegajut.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nrsouaro.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fjxjmexq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rbomhlom.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3joejeyov.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3cdaswhow.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gqiyiyyp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rwdjpesu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3giixgagw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kwxgersm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehtbtbty.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qhnnyawn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3iwhnojum.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3oyvkbtqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3baxsmakz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3csgmjuvk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qyvjfavg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qjzdvrpz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ugjkgevj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ccdbgnmj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3epgkyhhz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3etqombgc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3snksdrli.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3huabrmnx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qdevfjnu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fadnskhj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3uwxgzcqn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xbopcbco.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qjzbwwee.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pyjceonw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xrjoksqn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tiavklpm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gehmnbhz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ujcjaloy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vnbibohf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fimdjqbq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3agtumavh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eboarbju.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lbtpjpip.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ndzyzlqu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrttkwv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vumendrl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ulmdgjmz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ooykrcai.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yoqmyhoa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijtghxmm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kpckbaga.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kxuqdzln.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zbhmneev.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ahknvdnx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ehadmhom.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ylpoqvom.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dadxcsof.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xypfmaqb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3eppdbacl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bhshlprx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3udvelwwg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xencwiyk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jnjysqdm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ohbdpilb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3yakhulvp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3nqsiajtz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mqgbqjzj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cdsfukrr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3whymymhd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sshjvwzr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zgdhnazo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3twrihfvl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ptfjmldd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mjkancvt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bwlcgcih.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hapfoxym.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vxlupbbr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dinzrvgx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xcakbuxa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ryfcsvto.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gdugouye.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xcrtpyfq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3udiaobeg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gciukvhy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ynlyxkxj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zuzljpuf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zosgbjdr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bpbjxssa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mruaefnj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pxsrbdfi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mieysqvv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3solqpdpk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tpliidbg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pcqcuutz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gapizpjj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rdgqdrvz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wtsajwys.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oftkbtwv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vuytpjrq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3opxkrmdh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rryfzpqy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3sxoxlfkz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gsboavqb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xgrzqoau.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ofgietsx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3spxojlcv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3imfwybmo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3eyydkdkq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wcdwcjrq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3nxlyjsxu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xwqmokgl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3afhbtspw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ltcqgkbh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hrwctemg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3uyaqyvit.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3akplqhdn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3teqnptva.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yqqtgkux.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ojjtyeib.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zlqazhkn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yvaginfw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ermyffdg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ugvkurvf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gkywvycj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3boenvsrb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mhrtjeuc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3orxylpmw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wxwxeajt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lmrnchgd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rkwizjza.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wewhwfzt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bnmhfhqt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jjsatvdn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gytytece.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3telhncva.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zdixfsey.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3khkpbjnb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qjpvpyyx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cchmlsrd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ujaambum.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lvfhyrin.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jjyiihcu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3aopluzfe.html


<!-- 参考信息 -->