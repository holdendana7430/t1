代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtnwoyrble.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xinyue.icu/gttwblzgle.html

[T48] Perl：正则替换
来源：http://hz.gogol.net.cn/gtjsceszoh.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtijorreme.html

[T49] Perl：函数
来源：http://hz.yj20258888.top/gtqkavdnxk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtinqfjarb.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtuxdpoqgh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtrmeznwkw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aizwys.cn/gtjodizpmu.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtekmguako.html

println("Hello")
来源：http://hz.guannengcc.top/gtfigsqouw.html

[T52] Scala：变量
来源：http://hz.xylfe.cn/gtudahywle.html

val a = 1;  var b = 2
来源：http://hz.jinqigufen.top/gthsooggdi.html

[T53] Scala：字符串插值
来源：http://hz.jlsjyb.cn/gtjouafudb.html

s"值: $b"
来源：http://hz.jinqigufen.top/gtdzkljjlq.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtdslpytgi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yanxiufei.cn/gtxhlstujh.html

[T55] Scala：集合过滤
来源：http://hz.hammf.cn/gtduqdqdbs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gtnhnvyxkj.html

[T56] Scala：样例类
来源：http://hz.jinyuanbaomall.cn/gtxmlhntgz.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gtlgwnzmpp.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtykrrbcff.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxinkj.top/gtfkxoqdgt.html

[T58] Scala：函数定义
来源：http://hz.9152youxi.cn/gtrzqkrakq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tian-w.cn/gtcatsvugc.html

[T59] Scala：循环
来源：http://hz.jiagoushi.top/gtkyrbdesw.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gtspyzdfty.html

[T60] Scala：折叠
来源：http://hz.guowangkeji.top/gtftdajxdj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhengqikj.top/gtxjezawpi.html

================================================================================
来源：http://hz.aibaodan.cn/gtaglfyjrf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sxryk.cn/gtoavmriqh.html

================================================================================
来源：http://hz.aizwys.cn/gtxtcypvap.html

[U01] Py：创建虚拟环境
来源：http://hz.hammf.cn/gtpfkbjiha.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.316326.xyz/gtoyibwgxr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgufenzy.top/gtmkfagicy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gtkdrkjfxu.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtnhgqgeeu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shangyingyoupin.top/gtonwbckks.html

[U04] Py：变量调试打印
来源：http://hz.52xcode.cn/gtmuepurou.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.kuanghao11.cn/gtqjodcjvb.html

[U05] Py：列表去重且保序
来源：http://hz.pycfn.com/gthjxiesrp.html

list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtyvywbrmy.html

[U06] Py：合并两个字典
来源：http://hz.jinqigufen.top/gttjlgiphd.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtbeezvrbh.html

[U07] Py：反转字典键值
来源：http://hz.redwolf501.top/gtbvodfaih.html

{v: k for k, v in d.items()}
来源：http://hz.tianlin.xyz/gtauecmreh.html

[U08] Py：展平二维列表
来源：http://hz.bjfxy.top/gtroojqtzm.html

[y for x in nested for y in x]
来源：http://hz.smart0.xyz/gtaczvkwum.html

[U09] Py：字典取最大值的键
来源：http://hz.pycfn.com/gtfssashum.html

max(d, key=d.get)
来源：http://hz.xingfuxueyuan.xyz/gtmftkuaoj.html

[U10] Py：按值排序字典
来源：http://hz.andypj.xyz/gtxyptahub.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuanzx.com/gtcgrpamzm.html

[U11] Py：生成器表达式
来源：http://hz.xinyue.icu/gtwvqvwpnd.html

(x * 2 for x in arr)
来源：http://hz.hnxiangtu.top/gtatfpagni.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuxming.cn/gtjhmtflba.html

Counter(arr).most_common(3)
来源：http://hz.ydjk.org.cn/gtqsligpsl.html

[U13] Py：固定长度队列
来源：http://hz.yonumen.top/gtjlrdouvb.html

deque(maxlen=10)
来源：http://hz.kuanghao11.cn/gtnznatjyt.html

[U14] Py：分组收集到列表
来源：http://hz.shzxlz.cn/gtcdcrcclu.html

defaultdict(list)
来源：http://hz.ywan-chungtsiang.top/gtbrtggqvh.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtonapkoxt.html

t = time.perf_counter()
来源：http://hz.jqgufenzy.top/gtgjcjmdgm.html

[U16] Py：命令行参数解析
来源：http://hz.yangfankeji.com/gtklvoelwo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtrcnvzlfe.html

[U17] Py：初始化日志
来源：http://hz.birdmap.top/gthnhwyrgs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guannengcc.top/gtwnsnicak.html

[U18] Py：预编译正则
来源：http://hz.jqgfzy.top/gtjvcbfmsp.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtmqethmxh.html

[U19] Py：正则替换带回调
来源：http://hz.daxiang520.top/gtjybwgrhl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daria6918.cn/gtjqpfyxvu.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtlxtpmkre.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shangyingyoupin.top/gtctstyezz.html

[U21] Py：自定义上下文管理器
来源：http://hz.meibo888.top/gtffvdcjrr.html

@contextlib.contextmanager
来源：http://hz.jinqigufen.top/gtulbbqmbd.html

[U22] Py：矩阵转置
来源：http://hz.ywan-chungtsiang.top/gtgzuyzboi.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtlpvukzyb.html

[U23] Py：分块读取大文件
来源：http://hz.zhiwuduotai.top/gtrkeaxsbk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gotoacloud.top/gtpdohrzma.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtqvwrjpyr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daxiang520.top/gtffxteivu.html

[U25] Py：CSV 按字典读
来源：http://hz.jqgufenzy.top/gtbaezffid.html

csv.DictReader(f)
来源：http://hz.yj20258888.top/gtjtbklumm.html

[U26] Py：并发下载
来源：http://hz.jianghu66.top/gtzhkmvfsw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnqzz.top/gtsshclygi.html

[U27] Py：异步 HTTP
来源：http://hz.yj20258888.top/gtvjgjrfys.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daria6918.cn/gtpawderor.html

[U28] Py：类型别名
来源：http://hz.52xcode.cn/gtmqrdaqvo.html

UserId = int
来源：http://hz.gzhubu.top/gtrhlztwlz.html

[U29] Py：属性校验
来源：http://hz.sufxvd.cn/gtolzzcyor.html

@property 与 @x.setter 配合
来源：http://hz.xylfe.cn/gtylessoph.html

[U30] Py：数据类
来源：http://hz.chenlongwang.top/gtvfyrpdsg.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtbaizyzii.html

[U31] Py：单测
来源：http://hz.shanyushiyangtech.top/gtwvvsfaix.html

python -m pytest -q
来源：http://hz.guannengcc.top/gtoipevweh.html

[U32] Py：代码格式化
来源：http://hz.yvedp.cn/gtyvdwapli.html

ruff format . && ruff check --fix .
来源：http://hz.yongpay.top/gtuuqcgoje.html

[U33] Py：打包发布
来源：http://hz.xylfe.cn/gtiwcdhhfp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuanzx.com/gtfpqarehj.html

[U34] Py：判断编码
来源：http://hz.fzhhl.top/gtmkdexgsw.html

chardet.detect(raw)
来源：http://hz.mhx1999.top/gtfvwmgbxc.html

[U35] Py：发送邮件
来源：http://hz.chenlongwang.top/gtdftuxzrw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xylfe.cn/gtmlmrnjdg.html

[U36] Py：定时任务
来源：http://hz.jinqigfzy.top/gtbqcxzqvn.html

schedule.every(10).minutes.do(job)
来源：http://hz.andypj.xyz/gtstkhnpit.html

[U37] Py：读写 Excel
来源：http://hz.bjfxy.top/gtzbqczplk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jyoumei.cn/gthmvbpcot.html

[U38] Py：获取脚本所在目录
来源：http://hz.yvedp.cn/gtqkvziyfg.html

Path(__file__).resolve().parent
来源：http://hz.zhongyouzk.top/gtplcvwvmx.html

[U39] Py：判断是否在交互环境
来源：http://hz.jqgufenzy.top/gtbpleqvdt.html

sys.stdout.isatty()
来源：http://hz.daria6918.cn/gtnrnztbpy.html

[U40] Py：打印到标准错误
来源：http://hz.haohaochexian.top/gtftxogpxo.html

print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtjruakbwb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sxryk.cn/gteckmfbjd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxuanxn.top/gtfnepxfym.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yuxming.cn/gtftqtugcf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.meibo888.top/gtiqkkcxgt.html

[U43] PHP：声明命名空间
来源：http://hz.smart0.xyz/gtcfhqukgy.html

namespace App\Http;
来源：http://hz.shzxlz.cn/gtkivkekxb.html

[U44] PHP：开启严格类型
来源：http://hz.zhiwuduotai.top/gtnvpysgji.html

declare(strict_types=1);
来源：http://hz.fzhhl.top/gtlkbijvay.html

[U45] PHP：类型声明与返回类型
来源：http://hz.mhx1999.top/gtnvrvhzkf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gteictdvkd.html

[U46] PHP：可空类型
来源：http://hz.tianlin.xyz/gtxrdnqyes.html

?string $name = null
来源：http://hz.zhijiandao.cn/gtswbgtssk.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangkeji.top/gtyyegrtck.html

int|string $id
来源：http://hz.pycfn.com/gtnnbymqhn.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gtdilobtdj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yanxiufei.cn/gtwdpsavnd.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gtcgqksxuo.html

public readonly string $name
来源：http://hz.yangfankeji.com/gtxcuwrznp.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtjyffmupp.html

public function __construct(private int $id) {}
来源：http://hz.daxiang520.top/gtpcjdidwz.html

[U51] PHP：数组解构
来源：http://hz.pycfn.com/gtvodsbxka.html

[$a, $b] = $arr;
来源：http://hz.yj20258.top/gtgcnlnjqa.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtmesveusu.html

$double = fn($x) => $x * 2;
来源：http://hz.ywan-chungtsiang.top/gtfvzudnmf.html

[U53] PHP：空合并运算符
来源：http://hz.daria6918.cn/gtkzxwpzqd.html

$v = $a ?? $b ?? "default";
来源：http://hz.cucudq.cn/gtryrbdfsh.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtwhxffpss.html

$obj?->method()
来源：http://hz.9152youxi.cn/gtljonwbup.html

[U55] PHP：match 表达式
来源：http://hz.daxiang520.top/gtumnevsro.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tianlin.xyz/gtnqagjdco.html

[U56] PHP：命名参数
来源：http://hz.zycfv.cn/gtndxkdpmp.html

f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtylmrtbyh.html

[U57] PHP：字符串插值
来源：http://hz.sysykeji.top/gtnptbsobv.html

"值: {$a}"
来源：http://hz.yj202588.top/gtsqtuerds.html

[U58] PHP：数组三件套
来源：http://hz.ywan-chungtsiang.top/gtpugidpgt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.smart0.xyz/gthloskiva.html

[U59] PHP：自定义排序
来源：http://hz.gogol.net.cn/gthawhtxdu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtmnqikdgn.html

[U60] PHP：JSON 编解码
来源：http://hz.sxryk.cn/gtunrjrhvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sufxvd.cn/gtnzclkhla.html

[U61] PHP：正则
来源：http://hz.shanyushiyangkeji.top/gtcofcdrfp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtoljjjldl.html

[U62] PHP：日期对象
来源：http://hz.xinyue.icu/gtjtnarllg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shuidangran.top/gtyfgvbuyx.html

[U63] PHP：文件读写
来源：http://hz.tianlin.xyz/gtqhqwjixh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.pengpengdd.cyou/gtmkstkbzd.html

[U64] PHP：目录遍历
来源：http://hz.ydzc1.top/gtljfgojgv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhaomingkeji.xyz/gtxotkreqy.html

[U65] PHP：会话
来源：http://hz.cheryme.top/gteznceenx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cashguo.top/gtvgueigsh.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtvhasytof.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.mhx1999.top/gtlefvtdwb.html

[U67] PHP：处理文件上传
来源：http://hz.havefunace.top/gttaykghmd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.andypj.xyz/gtepvsgcgf.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gtjivwpfwc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ybcxt.top/gtyvjgdwac.html

[U69] PHP：PDO 预处理
来源：http://hz.sysykeji.top/gtsxkvglcp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shanyushiyangkeji.top/gtkjpkzisy.html

[U70] PHP：PDO 事务
来源：http://hz.ydzc1.top/gttjasujot.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zycfv.cn/gttspupirm.html

[U71] PHP：抛出异常
来源：http://hz.hfpthk.cn/gteluummuj.html

throw new RuntimeException("失败", 500);
来源：http://hz.sufxvd.cn/gtaflzmaqw.html

[U72] PHP：写错误日志
来源：http://hz.sweek.top/gtekugztme.html

error_log("失败: " . $e->getMessage());
来源：http://hz.feifeiyinyue.top/gtvbiiynxk.html

[U73] PHP：读取 ini 配置
来源：http://hz.jqgufenzy.top/gtxwsbbbtm.html

parse_ini_file("config.ini", true)
来源：http://hz.dashuyun.cn/gtcqynhskt.html

[U74] PHP：读取环境变量
来源：http://hz.xziqi.cn/gtusfwwpqm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jyoumei.cn/gtpukyofas.html

[U75] PHP：依赖注入
来源：http://hz.haohaochexian.top/gtdcboaylk.html

composer require psr/container
来源：http://hz.jinghuilouyu.cn/gtcriwucuy.html

[U76] PHP：简单路由
来源：http://hz.yangfankeji.com/gtdjlekrrc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gaohongyu789.top/gtrchewcak.html

[U77] PHP：模板渲染
来源：http://hz.hysaishi.cn/gttmdfucug.html

composer require twig/twig
来源：http://hz.yanxiufei.cn/gtkkxvwooe.html

[U78] PHP：单元测试
来源：http://hz.smart0.xyz/gtqyisxutp.html

composer require --dev phpunit/phpunit
来源：http://hz.snrcjt.cn/gthohvrqen.html

[U79] PHP：静态分析
来源：http://hz.daxiang520.top/gtqyqjdxgu.html

composer require --dev phpstan/phpstan
来源：http://hz.havefunace.top/gttdnzsmfj.html

[U80] PHP：代码规范修复
来源：http://hz.yj20258.top/gtyivpiecu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daxiang520.top/gtvllvemcg.html

[U81] JS：初始化项目
来源：http://hz.316326.xyz/gtkpkieonf.html

npm init -y;  npm i express
来源：http://hz.tian-w.cn/gtxkivghfo.html

[U82] JS：package.json 脚本
来源：http://hz.yanxiufei.cn/gtnkwbtjjb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gzhubu.top/gtbvrwpzjq.html

[U83] JS：ES Module 导入导出
来源：http://hz.yanxiufei.cn/gtvlokjfhq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.guannengcc.top/gtpwzolxpx.html

[U84] JS：CommonJS 写法
来源：http://hz.sufxvd.cn/gtctktkdsi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuxming.cn/gtzpddrjkr.html

[U85] JS：可选链
来源：http://hz.ppjwa.cn/gtgdqtgiwx.html

a?.b?.c
来源：http://hz.hnqzz.top/gtywzyuibt.html

[U86] JS：空值合并
来源：http://hz.andypj.xyz/gtgoijqgbi.html

a ?? b
来源：http://hz.hnqzz.top/gtnfusqigc.html

[U87] JS：解构默认值
来源：http://hz.yvedp.cn/gtxuiepxhq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhiwuduotai.top/gttbedmbnl.html

[U88] JS：对象展开合并
来源：http://hz.sxryk.cn/gttslzltad.html

{ ...a, ...b }
来源：http://hz.xingfuxueyuan.xyz/gtsxaelyqg.html

[U89] JS：数组去重
来源：http://hz.andypj.xyz/gtpvhyakwj.html

[...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtofadnokh.html

[U90] JS：数字数组排序
来源：http://hz.sysykeji.top/gttkekyjsi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtiqczegle.html

[U91] JS：对象键值遍历
来源：http://hz.zhiwuduotai.top/gtxqxyaysr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cqqwz.cn/gtrtkbfipk.html

[U92] JS：深拷贝
来源：http://hz.vqdsnc.cn/gtfkqjgjpu.html

structuredClone(obj)
来源：http://hz.yuanzhike.top/gtgjuqwayv.html

[U93] JS：模板字符串
来源：http://hz.svipenyu.cn/gtybyasycf.html

`共 ${n} 条`
来源：http://hz.gotoacloud.top/gtylppfbfl.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtgabdgpir.html

const double = x => x * 2;
来源：http://hz.shuidangran.top/gtbiepmmkh.html

[U95] JS：Promise 包装
来源：http://hz.zdqjudy.top/gtmsrwrabz.html

new Promise((resolve, reject) => {})
来源：http://hz.birdmap.top/gtbhqtnlkt.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtadkqlfgz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gthqmvpqkb.html

[U97] JS：并发请求
来源：http://hz.wangdashe.top/gtsvwcicam.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtwfzuchoc.html

[U98] JS：fetch 带 JSON
来源：http://hz.cashguo.top/gtkqbftqzd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj202588.top/gtqnoarqlx.html

[U99] JS：事件监听
来源：http://hz.sweek.top/gtlfrhkhfi.html

el.addEventListener("click", e => {})
来源：http://hz.chenlongwang.top/gtbcqedeyu.html

[U100] JS：DOM 查询
来源：http://hz.yuxming.cn/gtqhttdwmb.html

document.querySelector(".item")
来源：http://hz.andypj.xyz/gtpqidfxjd.html

[U101] JS：classList 操作
来源：http://hz.shangyingyoupin.top/gttoshcryo.html

el.classList.toggle("active")
来源：http://hz.wangdashe.top/gtrpxrtijo.html

[U102] JS：本地存储
来源：http://hz.yvedp.cn/gtwpxzrehm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtfsmtuygl.html

[U103] JS：定时器
来源：http://hz.zhengqikj.top/gtdxfsvdnt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gtkbpiqqda.html

[U104] JS：防抖
来源：http://hz.yj20258888.top/gtyqvnnmpy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtpyijgozo.html

[U105] JS：节流
来源：http://hz.jinyuanbaomall.cn/gtjgqfwymr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dashuyun.cn/gtdyeubeqw.html

[U106] JS：日期格式化
来源：http://hz.pycfn.com/gtatyfdwhh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.snrcjt.cn/gtunuhpxjs.html

[U107] JS：数字千分位
来源：http://hz.redwolf501.top/gtxfeohoyo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pengpengdd.cyou/gtggumpyln.html

[U108] JS：随机整数
来源：http://hz.pycfn.com/gtaqiwozbe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gaohongyu789.top/gtlltlpjvu.html

[U109] JS：数组分组
来源：http://hz.ybcxt.top/gtukkhzbwl.html

Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gtbemsroef.html

[U110] JS：数组分块
来源：http://hz.guannengcc.top/gtmbnkwcod.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258888.top/gtiqghruhd.html

[U111] JS：对象转 Map
来源：http://hz.zhengqikj.top/gtraykocud.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtiouurnbt.html

[U112] JS：字符串补位
来源：http://hz.shuidangran.top/gtryfbdowd.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtgyaxfznx.html

[U113] JS：正则替换全部
来源：http://hz.aibaodan.cn/gtanrmwhkc.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtbhaceaeb.html

[U114] JS：JSON 深比较
来源：http://hz.c1oappe.top/gtxsnahqbh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtlaimagnt.html

[U115] JS：生成 UUID
来源：http://hz.xylfe.cn/gtnznhkviy.html

crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtrwktgmki.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhijiandao.cn/gtfihqecor.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hammf.cn/gtoxsvbdwl.html

[U117] JS：单元测试
来源：http://hz.tanke756.top/gtqwzeieql.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gtsurllziq.html

[U118] JS：开发服务器
来源：http://hz.xinyue.icu/gtlfbswlca.html

npm i -D vite;  npx vite
来源：http://hz.ydzc1.top/gtogndeeqo.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtbyaoqlnr.html

npx vite build
来源：http://hz.0kj1m.cn/gtdrklqebg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ywan-chungtsiang.top/gthcqfibeq.html

import.meta.env.VITE_API_URL
来源：http://hz.mhx1999.top/gtsewfohnu.html

================================================================================
来源：http://hz.birdmap.top/gtjlgewzyw.html

统计汇总
来源：http://hz.tian-w.cn/gthkhaorfy.html

================================================================================
来源：http://hz.fengsongda.top/gtanvgirbz.html

按语言统计（条）：
来源：http://hz.kuanghao11.cn/gtjyhxpyrd.html

Python ......... 252
来源：http://hz.daxiang520.top/gtaulaiidz.html

PHP ............ 252
来源：http://hz.jinyuanbaomall.cn/gtxvykukfm.html

JavaScript ..... 252
来源：http://hz.hongshengwenyu.top/gtoyaavfit.html

TypeScript ..... 212
来源：http://hz.ydjk.org.cn/gtcklshawf.html

Java ........... 212
来源：http://hz.zdqjudy.top/gtpfsbonmz.html

Go ............. 212
来源：http://hz.jianghu66.top/gtzxlokcmf.html

Ruby ........... 212
来源：http://hz.sxryk.cn/gtrlqecbjb.html

C# ............. 212
来源：http://hz.dianchejie.cn/gtifcoufta.html

C .............. 30
来源：http://hz.jinyuanbaomall.cn/gtmmzlsaoe.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtcqafezdn.html

SQL ............ 90
来源：http://hz.cdnleiting.top/gthivqqvgq.html

Bash ........... 80
来源：http://hz.yuxming.cn/gtwbghxigo.html

Kotlin ......... 15
来源：http://hz.daria6918.cn/gteilzpoqe.html

Swift .......... 15
来源：http://hz.gaohongyu789.top/gtxpprhixi.html

Lua ............ 10
来源：http://hz.smart0.xyz/gtaybodwng.html

Perl ........... 10
来源：http://hz.ehwqpu.com/gtngnxnzma.html

Scala .......... 10
来源：http://hz.wangdashe.top/gtscpeyzji.html

------------------------------------
来源：http://hz.daria6918.cn/gtbmakutab.html

合计 ........... 2106 条
来源：http://hz.hysaishi.cn/gttnkrzhnm.html

按章节统计：
来源：http://hz.yanxiufei.cn/gtzeexejwi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.0kj1m.cn/gtdpzprhkl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yongpay.top/gtoeeqphhq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gtqxahuzmj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtxglriuwa.html


<!-- 参考信息 -->