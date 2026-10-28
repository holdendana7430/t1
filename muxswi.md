代发 wailian999

[T49] Perl：函数
来源：http://hz.sysykeji.top/gtshcpdxwj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gtixcwgnvx.html

[T50] Perl：逐行读文件
来源：http://hz.zdqjudy.top/gtxhadmzoj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtnobhbkxf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jlsjyb.cn/gtswpqaaep.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtedmxfzhe.html

println("Hello")
来源：http://hz.zhixingplan.top/gttampduhc.html

[T52] Scala：变量
来源：http://hz.ywan-chungtsiang.top/gtfvtxgozq.html

val a = 1;  var b = 2
来源：http://hz.andypj.xyz/gtwkxnoprx.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtajylznkg.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtcotnmrdb.html

[T54] Scala：集合映射
来源：http://hz.ywan-chungtsiang.top/gtfsausoob.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fengsongda.top/gtzpkdhhbr.html

[T55] Scala：集合过滤
来源：http://hz.shangyingyoupin.top/gtkmasutgj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yanxiufei.cn/gtjwasphff.html

[T56] Scala：样例类
来源：http://hz.jianghu66.top/gtvutagjiy.html

case class User(name: String, age: Int)
来源：http://hz.xziqi.cn/gtflwmyhuk.html

[T57] Scala：模式匹配
来源：http://hz.zhijiandao.cn/gtoscjplzc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj20258.top/gtfdtneiaf.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gtfnxwsopf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.dianchejie.cn/gtetmuojty.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtrdvndnqs.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangshuangyany.cn/gtvurpoweu.html

[T60] Scala：折叠
来源：http://hz.pengpengdd.cyou/gtpveazahy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtndrtbbho.html

================================================================================
来源：http://hz.guannengcc.top/gtqokyhylm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gzhubu.top/gtmptiiyel.html

================================================================================
来源：http://hz.andypj.xyz/gthmxsgznq.html

[U01] Py：创建虚拟环境
来源：http://hz.jiagoushi.top/gtkdnrkgmc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aibaodan.cn/gtyialzsfc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jiagoushi.top/gtwyqcgjuq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.andypj.xyz/gthbdcklly.html

[U03] Py：加载 .env 配置
来源：http://hz.hnqzz.top/gtkqrwysoe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangkeji.top/gtlnniqmgt.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gtcjqrcapl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtwahnaesr.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigfzy.top/gtlpmkjnwm.html

list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtlkubtgdl.html

[U06] Py：合并两个字典
来源：http://hz.cashguo.top/gtbumefnre.html

{**a, **b}
来源：http://hz.hnxiangtu.top/gtwxvcucjx.html

[U07] Py：反转字典键值
来源：http://hz.ywan-chungtsiang.top/gtbgjvasxr.html

{v: k for k, v in d.items()}
来源：http://hz.jlsjyb.cn/gtixdukymx.html

[U08] Py：展平二维列表
来源：http://hz.gaohongyu789.top/gtamdocucz.html

[y for x in nested for y in x]
来源：http://hz.chenzaomai.com/gtpnwmlzhe.html

[U09] Py：字典取最大值的键
来源：http://hz.52xcode.cn/gtlpizoilj.html

max(d, key=d.get)
来源：http://hz.zycfv.cn/gtzwtczpjc.html

[U10] Py：按值排序字典
来源：http://hz.aibaodan.cn/gtlgkwdepz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.iojbl.cn/gtmoverweg.html

[U11] Py：生成器表达式
来源：http://hz.andypj.xyz/gttgiiagra.html

(x * 2 for x in arr)
来源：http://hz.jinqigfzy.top/gtagrjqodu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ehwqpu.com/gthmqmpvsl.html

Counter(arr).most_common(3)
来源：http://hz.shzxlz.cn/gtpuskeqig.html

[U13] Py：固定长度队列
来源：http://hz.hammf.cn/gtxahfkyof.html

deque(maxlen=10)
来源：http://hz.yangfankeji.com/gtndvqtodi.html

[U14] Py：分组收集到列表
来源：http://hz.zhengqikj.top/gtcbwmtbvc.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtjweeneau.html

[U15] Py：高精度计时
来源：http://hz.svipenyu.cn/gtfonnvhut.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtdptohxet.html

[U16] Py：命令行参数解析
来源：http://hz.bjfxy.top/gtfypqnxmp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtsamphizw.html

[U17] Py：初始化日志
来源：http://hz.cashguo.top/gtdtrirjkl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.pengpengdd.cyou/gtmeohwonp.html

[U18] Py：预编译正则
来源：http://hz.yuxming.cn/gtfxdnhspy.html

pat = re.compile(r"\d+")
来源：http://hz.kuanghao11.cn/gtuohfahxn.html

[U19] Py：正则替换带回调
来源：http://hz.nanxuanxn.top/gtkrwqtdas.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj202588.top/gthwqvjngl.html

[U20] Py：缓存函数结果
来源：http://hz.c1oappe.top/gtjagghggr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtncoxrjjo.html

[U21] Py：自定义上下文管理器
来源：http://hz.jiagoushi.top/gtltyowxtk.html

@contextlib.contextmanager
来源：http://hz.xingfuxueyuan.xyz/gtzjagkgjw.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gtjwwtkxos.html

list(zip(*m))
来源：http://hz.gaohongyu789.top/gtgdjeplga.html

[U23] Py：分块读取大文件
来源：http://hz.aizwys.cn/gtbvawfxnx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guannengcc.top/gtxyjdjmjv.html

[U24] Py：路径操作
来源：http://hz.haohaochexian.top/gttqyspcpu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenlongwang.top/gtpdibnmes.html

[U25] Py：CSV 按字典读
来源：http://hz.sufxvd.cn/gtmpestrle.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtlduspedc.html

[U26] Py：并发下载
来源：http://hz.xingfuxueyuan.xyz/gtxqzktudy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtofznzgna.html

[U27] Py：异步 HTTP
来源：http://hz.havefunace.top/gtryuigxhc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gotoacloud.top/gtglamcfwv.html

[U28] Py：类型别名
来源：http://hz.svipenyu.cn/gtjzwysmec.html

UserId = int
来源：http://hz.redwolf501.top/gtrbfdstqe.html

[U29] Py：属性校验
来源：http://hz.pycfn.com/gtlixgzhed.html

@property 与 @x.setter 配合
来源：http://hz.shzxlz.cn/gtssjrkzpo.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtwspihoar.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtkxpgtoan.html

[U31] Py：单测
来源：http://hz.xylfe.cn/gtlaqdlweu.html

python -m pytest -q
来源：http://hz.jqgfzy.top/gtnthlgycz.html

[U32] Py：代码格式化
来源：http://hz.dianchejie.cn/gtreerouon.html

ruff format . && ruff check --fix .
来源：http://hz.yongpay.top/gtdbbaputf.html

[U33] Py：打包发布
来源：http://hz.xuanzx.com/gtmrqffbon.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cdnleiting.top/gtkkqdpfeb.html

[U34] Py：判断编码
来源：http://hz.yangfankeji.com/gtmxboeoqu.html

chardet.detect(raw)
来源：http://hz.aizwys.cn/gtqvnzpsfp.html

[U35] Py：发送邮件
来源：http://hz.jlsjyb.cn/gtbnvmenop.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.svipenyu.cn/gtvhrwzfeo.html

[U36] Py：定时任务
来源：http://hz.fzhhl.top/gtozgmbgnp.html

schedule.every(10).minutes.do(job)
来源：http://hz.gzhubu.top/gtvxodmecp.html

[U37] Py：读写 Excel
来源：http://hz.nanxuanxn.top/gtqppyefeq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sweek.top/gtvbpfbnxl.html

[U38] Py：获取脚本所在目录
来源：http://hz.cucudq.cn/gtpthcgpqb.html

Path(__file__).resolve().parent
来源：http://hz.jyoumei.cn/gtvltjjvpk.html

[U39] Py：判断是否在交互环境
来源：http://hz.ywan-chungtsiang.top/gtiohkoaur.html

sys.stdout.isatty()
来源：http://hz.guannengcc.top/gtqqzncgis.html

[U40] Py：打印到标准错误
来源：http://hz.jinyuanbaomall.cn/gtywmvrnrk.html

print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtahozontv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hywenlv.cn/gtwaqliqnr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.52xcode.cn/gtnztjdgrx.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jyoumei.cn/gtlrtuvowq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenlongwang.top/gtuvqkwvng.html

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtufrnezuo.html

namespace App\Http;
来源：http://hz.shangyingyoupin.top/gtmyimzvyv.html

[U44] PHP：开启严格类型
来源：http://hz.xylfe.cn/gtjkbkcclg.html

declare(strict_types=1);
来源：http://hz.shanyushiyangtech.top/gtjtuwttez.html

[U45] PHP：类型声明与返回类型
来源：http://hz.c1oappe.top/gtvjufzodi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtgoniqnlb.html

[U46] PHP：可空类型
来源：http://hz.zdqjudy.top/gtmbebkcxx.html

?string $name = null
来源：http://hz.jinqigfzy.top/gtklekjibb.html

[U47] PHP：联合类型
来源：http://hz.aizwys.cn/gtdgurzrka.html

int|string $id
来源：http://hz.yanxiufei.cn/gtkasixgia.html

[U48] PHP：纯枚举
来源：http://hz.0kj1m.cn/gtbhhrbmxf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gtssejrmie.html

[U49] PHP：只读属性
来源：http://hz.kuanghao11.cn/gtgjqabame.html

public readonly string $name
来源：http://hz.nanxinkj.top/gtquyvzzns.html

[U50] PHP：构造器属性提升
来源：http://hz.xuetiantiany.cn/gtdskutrrp.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtkxhgpgum.html

[U51] PHP：数组解构
来源：http://hz.wangdashe.top/gtmdeacouo.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtfjfmxxux.html

[U52] PHP：箭头函数
来源：http://hz.redwolf501.top/gtohufuuem.html

$double = fn($x) => $x * 2;
来源：http://hz.dashuyun.cn/gthfyjusil.html

[U53] PHP：空合并运算符
来源：http://hz.yj202588.top/gtzyqceyhw.html

$v = $a ?? $b ?? "default";
来源：http://hz.fzhhl.top/gtfpzaxvps.html

[U54] PHP：空安全调用
来源：http://hz.havefunace.top/gtbfrnrwtt.html

$obj?->method()
来源：http://hz.ivvv.top/gtiguprplk.html

[U55] PHP：match 表达式
来源：http://hz.haohaochexian.top/gtblstkydc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cqqwz.cn/gtjqktblfi.html

[U56] PHP：命名参数
来源：http://hz.kuanghao11.cn/gtkiqjiwhn.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtsvtqlcta.html

[U57] PHP：字符串插值
来源：http://hz.jianghu66.top/gtwtlwjvpu.html

"值: {$a}"
来源：http://hz.iojbl.cn/gtovibqupl.html

[U58] PHP：数组三件套
来源：http://hz.hywenlv.cn/gtgbsjcggl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shzxlz.cn/gtqrcrukpj.html

[U59] PHP：自定义排序
来源：http://hz.sufxvd.cn/gtinmsthmt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtayngrgnx.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtvggmtjzm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.iojbl.cn/gtfknikxwb.html

[U61] PHP：正则
来源：http://hz.jianghu66.top/gtlcrmvnmq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtmngsdlzu.html

[U62] PHP：日期对象
来源：http://hz.shanyushiyangtech.top/gtmtikibnf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhijiandao.cn/gtmieipegq.html

[U63] PHP：文件读写
来源：http://hz.yj202588.top/gtaigwvaqq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dashuyun.cn/gtxkznvzru.html

[U64] PHP：目录遍历
来源：http://hz.zhijiandao.cn/gtdlzlslxy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.c1oappe.top/gtijoyblrh.html

[U65] PHP：会话
来源：http://hz.zhixingplan.top/gtxbrmuoum.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.smart0.xyz/gtdpfpuumw.html

[U66] PHP：设置 Cookie
来源：http://hz.jlsjyb.cn/gtpaejixog.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jiagoushi.top/gtychlvhry.html

[U67] PHP：处理文件上传
来源：http://hz.shuidangran.top/gtbutqpcou.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ybcxt.top/gtxqxahpvf.html

[U68] PHP：PDO 连接
来源：http://hz.birdmap.top/gtxotdhhps.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258.top/gtmxmavyvd.html

[U69] PHP：PDO 预处理
来源：http://hz.jianghu66.top/gtczhmllpp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hysaishi.cn/gtzynhdwfj.html

[U70] PHP：PDO 事务
来源：http://hz.jinghuilouyu.cn/gtkmucnmyb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.snrcjt.cn/gtqxagwxrc.html

[U71] PHP：抛出异常
来源：http://hz.svipenyu.cn/gtjosquzis.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhijiandao.cn/gtwamsyxqn.html

[U72] PHP：写错误日志
来源：http://hz.cqqwz.cn/gthbjjxcwu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.birdmap.top/gtaqpxnlzg.html

[U73] PHP：读取 ini 配置
来源：http://hz.sufxvd.cn/gtpqbklnmg.html

parse_ini_file("config.ini", true)
来源：http://hz.yongpay.top/gtsrnvcgjl.html

[U74] PHP：读取环境变量
来源：http://hz.shuidangran.top/gtofaznclj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ydjk.org.cn/gtstocpxqk.html

[U75] PHP：依赖注入
来源：http://hz.chenzaomai.com/gtirnxpwcg.html

composer require psr/container
来源：http://hz.gotoacloud.top/gtsfvoftce.html

[U76] PHP：简单路由
来源：http://hz.jyoumei.cn/gtpljibqac.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yuxming.cn/gtrhqakrca.html

[U77] PHP：模板渲染
来源：http://hz.hfpthk.cn/gtlzzmjzhj.html

composer require twig/twig
来源：http://hz.ydjk.org.cn/gthjasqoif.html

[U78] PHP：单元测试
来源：http://hz.cdnleiting.top/gtmpxjgfeh.html

composer require --dev phpunit/phpunit
来源：http://hz.kuanghao11.cn/gthbpieauh.html

[U79] PHP：静态分析
来源：http://hz.c1oappe.top/gtlzchhzar.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxinkj.top/gtrktzwren.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtsasulfsp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenlongwang.top/gtbmhcfnzk.html

[U81] JS：初始化项目
来源：http://hz.0kj1m.cn/gtcbiobwna.html

npm init -y;  npm i express
来源：http://hz.tianlin.xyz/gtbdzytddk.html

[U82] JS：package.json 脚本
来源：http://hz.hongshengwenyu.top/gttissgmsn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtkqbjonfr.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydjk.org.cn/gtonwiodcr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenjidiqi.icu/gtbvtuoyyg.html

[U84] JS：CommonJS 写法
来源：http://hz.nanxinkj.top/gtvvcydfux.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ppjwa.cn/gtwhxnhnnu.html

[U85] JS：可选链
来源：http://hz.zycfv.cn/gtdqcqynlp.html

a?.b?.c
来源：http://hz.ydzc1.top/gtcbimnnng.html

[U86] JS：空值合并
来源：http://hz.hfpthk.cn/gtvhahiysr.html

a ?? b
来源：http://hz.shuidangran.top/gtdxprnjox.html

[U87] JS：解构默认值
来源：http://hz.chenjidiqi.icu/gtwqvkjkhh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.wangshuangyany.cn/gtxtzeecdi.html

[U88] JS：对象展开合并
来源：http://hz.daria6918.cn/gtschelxoq.html

{ ...a, ...b }
来源：http://hz.guannengcc.top/gtbugbckhi.html

[U89] JS：数组去重
来源：http://hz.0kj1m.cn/gtbwbpkapa.html

[...new Set(arr)]
来源：http://hz.yongpay.top/gtbwcbrrxu.html

[U90] JS：数字数组排序
来源：http://hz.fzhhl.top/gtfqzsfhgu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gttzwzofxt.html

[U91] JS：对象键值遍历
来源：http://hz.havefunace.top/gtbjdxoigi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yangfankeji.com/gtmneofxhm.html

[U92] JS：深拷贝
来源：http://hz.jinyuanbaomall.cn/gtelxbhyyy.html

structuredClone(obj)
来源：http://hz.xziqi.cn/gtgtpohrpn.html

[U93] JS：模板字符串
来源：http://hz.shuidangran.top/gtbkdztfsi.html

`共 ${n} 条`
来源：http://hz.jinyuanbaomall.cn/gtmutntihu.html

[U94] JS：箭头函数
来源：http://hz.fengsongda.top/gthzheykse.html

const double = x => x * 2;
来源：http://hz.yanxiufei.cn/gtohtzwqpz.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gtdsdtmwsd.html

new Promise((resolve, reject) => {})
来源：http://hz.meibo888.top/gtmwrukghg.html

[U96] JS：async/await 与异常
来源：http://hz.wangdashe.top/gtqowmipja.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtjtvrgxbd.html

[U97] JS：并发请求
来源：http://hz.xziqi.cn/gtsuwpqbnk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gthvkxggky.html

[U98] JS：fetch 带 JSON
来源：http://hz.daxiang520.top/gtcfrrxisx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.dashuyun.cn/gtinjjuyrx.html

[U99] JS：事件监听
来源：http://hz.yj202588.top/gtbzfvinkd.html

el.addEventListener("click", e => {})
来源：http://hz.nwbrower.top/gtsnytujmh.html

[U100] JS：DOM 查询
来源：http://hz.zycfv.cn/gtsxyajsof.html

document.querySelector(".item")
来源：http://hz.jqgufenzy.top/gtpkmlkkgf.html

[U101] JS：classList 操作
来源：http://hz.zhijiandao.cn/gtmjcoonnb.html

el.classList.toggle("active")
来源：http://hz.ybcxt.top/gtlfetkapt.html

[U102] JS：本地存储
来源：http://hz.aibaodan.cn/gtpacyicjw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xylfe.cn/gtnxgyqmin.html

[U103] JS：定时器
来源：http://hz.daria6918.cn/gtwjgllgdl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.haohaochexian.top/gtyndoupud.html

[U104] JS：防抖
来源：http://hz.zhoulong.xyz/gtfpfthpsm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtxsneljey.html

[U105] JS：节流
来源：http://hz.guowangkeji.top/gttewbfsrk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cucudq.cn/gtcnprfslj.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gttwvbvium.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yongpay.top/gtirzahjhs.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtdxsaoufr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhoulong.xyz/gtiirzlxgz.html

[U108] JS：随机整数
来源：http://hz.guowangkeji.top/gtvaqpdjrf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zycfv.cn/gtektyykar.html

[U109] JS：数组分组
来源：http://hz.sxryk.cn/gtgfhzrvam.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gthpeuugit.html

[U110] JS：数组分块
来源：http://hz.zhaomingkeji.xyz/gtivqoohyr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.iojbl.cn/gtwqijkxhu.html

[U111] JS：对象转 Map
来源：http://hz.cdnleiting.top/gtgamvxqbt.html

new Map(Object.entries(obj))
来源：http://hz.yangfankeji.com/gtxwowxywg.html

[U112] JS：字符串补位
来源：http://hz.fzhhl.top/gtlmaibodp.html

"7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtsgguxctj.html

[U113] JS：正则替换全部
来源：http://hz.fzhhl.top/gtbtipzpux.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtoekkdyya.html

[U114] JS：JSON 深比较
来源：http://hz.jqgfzy.top/gtwreqgjqg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtcekidsjx.html

[U115] JS：生成 UUID
来源：http://hz.chenlongwang.top/gttvvbgjnx.html

crypto.randomUUID()
来源：http://hz.hammf.cn/gtsoxabkdw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.mhx1999.top/gtgfesuqje.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtnyaafztf.html

[U117] JS：单元测试
来源：http://hz.yj20258888.top/gtkpnxknoc.html

npm i -D vitest;  npx vitest
来源：http://hz.nwbrower.top/gtmtnranzn.html

[U118] JS：开发服务器
来源：http://hz.yuxming.cn/gtmygzengt.html

npm i -D vite;  npx vite
来源：http://hz.svipenyu.cn/gtftxzqgve.html

[U119] JS：生产构建
来源：http://hz.jinqigufen.top/gtqxqmrymj.html

npx vite build
来源：http://hz.aibaodan.cn/gtitwrqcbx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cucudq.cn/gtifzjazkf.html

import.meta.env.VITE_API_URL
来源：http://hz.xuanzx.com/gthviupnqn.html

================================================================================
来源：http://hz.mhx1999.top/gtnlhqoqms.html

统计汇总
来源：http://hz.zhongyouzk.top/gtdnfxwhai.html

================================================================================
来源：http://hz.redwolf501.top/gtorrjjugf.html

按语言统计（条）：
来源：http://hz.ydjk.org.cn/gtskxlyrpv.html

Python ......... 252
来源：http://hz.nanxinkj.top/gtjxktyosj.html

PHP ............ 252
来源：http://hz.yonumen.top/gtvbztvgxr.html

JavaScript ..... 252
来源：http://hz.shzxlz.cn/gtgrdvndeg.html

TypeScript ..... 212
来源：http://hz.jinqigfzy.top/gtqwxrfqiy.html

Java ........... 212
来源：http://hz.gaohongyu789.top/gtlgzusjmq.html

Go ............. 212
来源：http://hz.guowangkeji.top/gtvluekquu.html

Ruby ........... 212
来源：http://hz.feifeiyinyue.top/gtensjyexy.html

C# ............. 212
来源：http://hz.yuanzhike.top/gtreygyxku.html

C .............. 30
来源：http://hz.0kj1m.cn/gtfnriywnl.html

C++ ............ 30
来源：http://hz.52xcode.cn/gtiwvaxhvn.html

SQL ............ 90
来源：http://hz.yuanzhike.top/gtrcrfrrlw.html

Bash ........... 80
来源：http://hz.feifeiyinyue.top/gtplubybiv.html

Kotlin ......... 15
来源：http://hz.yongpay.top/gtsiliiyny.html

Swift .......... 15
来源：http://hz.fengsongda.top/gthssskfbj.html

Lua ............ 10
来源：http://hz.jiagoushi.top/gtadttmtam.html

Perl ........... 10
来源：http://hz.redwolf501.top/gtpabernyr.html

Scala .......... 10
来源：http://hz.hnqzz.top/gtacdbgoua.html

------------------------------------
来源：http://hz.yj20258888.top/gtcomjrxep.html

合计 ........... 2106 条
来源：http://hz.xylfe.cn/gtvyygsscq.html

按章节统计：
来源：http://hz.jyoumei.cn/gtufrswveo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ivvv.top/gtagaiiolz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtyjtxtcke.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtqoysyhwm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hfpthk.cn/gtmsdtqpca.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yvedp.cn/gthzmnuhzf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gttiisfvvv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtfrrskhyv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guannengcc.top/gthsbbhkdw.html


<!-- 参考信息 -->