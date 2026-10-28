代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.yueranfly.top/gtnnywagfm.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtjtzrqwwq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.pengpengdd.cyou/gtptbzkqsd.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtbjbmrdmx.html

case class User(name: String, age: Int)
来源：http://hz.yj20258888.top/gtdgfwsexq.html

[T57] Scala：模式匹配
来源：http://hz.shzxlz.cn/gtrojmcebp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxinkj.top/gtibahyzbq.html

[T58] Scala：函数定义
来源：http://hz.daxiang520.top/gtdalieowz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xuetiantiany.cn/gtznmfmqld.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtmqkaluxi.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtatnajiau.html

[T60] Scala：折叠
来源：http://hz.jqgfzy.top/gtdfkrfcld.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtndmhylwh.html

================================================================================
来源：http://hz.cashguo.top/gtaldhuxxz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gtmndavvpt.html

================================================================================
来源：http://hz.gaohongyu789.top/gtzcgarcps.html

[U01] Py：创建虚拟环境
来源：http://hz.hfpthk.cn/gtfbrhpvav.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gtrnoexlkm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shangyingyoupin.top/gtqhdmzevq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnqzz.top/gtlineroxe.html

[U03] Py：加载 .env 配置
来源：http://hz.jinyuanbaomall.cn/gtdngoonva.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhoulong.xyz/gtrilhoxuu.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gtinejnrzm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtairpzstc.html

[U05] Py：列表去重且保序
来源：http://hz.tian-w.cn/gtcdxigqaf.html

list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtphnrrvni.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gtjuppmfgd.html

{**a, **b}
来源：http://hz.zhongyouzk.top/gttmnafmqk.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtxduxpwdp.html

{v: k for k, v in d.items()}
来源：http://hz.fzhhl.top/gttyvtdvrf.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtxvzjfagp.html

[y for x in nested for y in x]
来源：http://hz.nanxuanxn.top/gtuwvtqxfq.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gtligoeqrl.html

max(d, key=d.get)
来源：http://hz.yueranfly.top/gtfwoxyjbp.html

[U10] Py：按值排序字典
来源：http://hz.yangfankeji.com/gtbwfrwiwu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.aibaodan.cn/gtcyaclzui.html

[U11] Py：生成器表达式
来源：http://hz.cqqwz.cn/gtcovnshri.html

(x * 2 for x in arr)
来源：http://hz.yonumen.top/gtqerjhfpi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.snrcjt.cn/gtuecfwovd.html

Counter(arr).most_common(3)
来源：http://hz.pycfn.com/gtzlhnrusq.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gtqinnsmmh.html

deque(maxlen=10)
来源：http://hz.chenzaomai.com/gtkivetmix.html

[U14] Py：分组收集到列表
来源：http://hz.cdnleiting.top/gtqfjhkdjh.html

defaultdict(list)
来源：http://hz.yj202588.top/gtcbpaomjg.html

[U15] Py：高精度计时
来源：http://hz.c1oappe.top/gtktqgnzim.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtdledvrzu.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gttcgbjbsc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sweek.top/gtjklnjefx.html

[U17] Py：初始化日志
来源：http://hz.jqgfzy.top/gtchvrtlby.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xziqi.cn/gtscvwumkk.html

[U18] Py：预编译正则
来源：http://hz.hammf.cn/gtkkqhvkaw.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigfzy.top/gtzqugmqkd.html

[U19] Py：正则替换带回调
来源：http://hz.fengsongda.top/gtnxkhmtju.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hfpthk.cn/gtiokaqvzi.html

[U20] Py：缓存函数结果
来源：http://hz.hysaishi.cn/gtexxqufra.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtasnzybtq.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuanzx.com/gtxmrdvmcc.html

@contextlib.contextmanager
来源：http://hz.yueranfly.top/gtlbbscwdm.html

[U22] Py：矩阵转置
来源：http://hz.jianghu66.top/gtqfgfyqij.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtevncjfme.html

[U23] Py：分块读取大文件
来源：http://hz.tanke756.top/gtzfcymkch.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ivvv.top/gthlchhxqd.html

[U24] Py：路径操作
来源：http://hz.yangfankeji.com/gtdpviurjn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnxiangtu.top/gtqydqexfy.html

[U25] Py：CSV 按字典读
来源：http://hz.sufxvd.cn/gtquipjwrs.html

csv.DictReader(f)
来源：http://hz.jiagoushi.top/gtdcojkcar.html

[U26] Py：并发下载
来源：http://hz.wangshuangyany.cn/gtaejoemqg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.iojbl.cn/gtmyeevtnq.html

[U27] Py：异步 HTTP
来源：http://hz.zycfv.cn/gtqrhvkrat.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.birdmap.top/gttzglztpt.html

[U28] Py：类型别名
来源：http://hz.yonumen.top/gtpykmfykb.html

UserId = int
来源：http://hz.yueranfly.top/gtvttqimny.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gtkncqcndw.html

@property 与 @x.setter 配合
来源：http://hz.0kj1m.cn/gtbkinnnxy.html

[U30] Py：数据类
来源：http://hz.redwolf501.top/gtbbjepfaa.html

@dataclass(slots=True)
来源：http://hz.sysykeji.top/gtoytcxqfa.html

[U31] Py：单测
来源：http://hz.ivvv.top/gtgzvenzwa.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtdcingxgl.html

[U32] Py：代码格式化
来源：http://hz.jqgfzy.top/gtfcwpwfsp.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtqehevocz.html

[U33] Py：打包发布
来源：http://hz.hnxiangtu.top/gtrneslcqj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tanke756.top/gtmqfpfezp.html

[U34] Py：判断编码
来源：http://hz.xuetiantiany.cn/gtorhabisu.html

chardet.detect(raw)
来源：http://hz.shzxlz.cn/gtqnvrrvpw.html

[U35] Py：发送邮件
来源：http://hz.guannengcc.top/gtjvgeptoi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.birdmap.top/gtopixltjc.html

[U36] Py：定时任务
来源：http://hz.yuanzhike.top/gtexwpnauy.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydzc1.top/gtqqzdnuwa.html

[U37] Py：读写 Excel
来源：http://hz.chenjidiqi.icu/gtwpugrolv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtdfzpsaaq.html

[U38] Py：获取脚本所在目录
来源：http://hz.hongshengwenyu.top/gttzcybuvn.html

Path(__file__).resolve().parent
来源：http://hz.ppjwa.cn/gtjkxxlkij.html

[U39] Py：判断是否在交互环境
来源：http://hz.yj202588.top/gtvuflxfdv.html

sys.stdout.isatty()
来源：http://hz.jyoumei.cn/gtrkupqent.html

[U40] Py：打印到标准错误
来源：http://hz.tanke756.top/gtcxjmyzem.html

print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtzqsgzbos.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ywan-chungtsiang.top/gtrfkkbrlw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jianghu66.top/gtxomdotyr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnxiangtu.top/gtuzdqopyr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zycfv.cn/gtjmvecpht.html

[U43] PHP：声明命名空间
来源：http://hz.xingfuxueyuan.xyz/gtvjmtroec.html

namespace App\Http;
来源：http://hz.zhijiandao.cn/gtewziwugm.html

[U44] PHP：开启严格类型
来源：http://hz.yvedp.cn/gtshevqwsq.html

declare(strict_types=1);
来源：http://hz.yj202588.top/gtusoowabi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yongpay.top/gtrpmwkrtf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtjwscednp.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtyfiuycvv.html

?string $name = null
来源：http://hz.gogol.net.cn/gtxsabtutz.html

[U47] PHP：联合类型
来源：http://hz.0kj1m.cn/gthfatftwk.html

int|string $id
来源：http://hz.ydjk.org.cn/gttbgrzddy.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gttutrqplp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenzaomai.com/gtoptroeut.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtyvbzbpnx.html

public readonly string $name
来源：http://hz.hysaishi.cn/gtxlmsfpup.html

[U50] PHP：构造器属性提升
来源：http://hz.zhixingplan.top/gtjjsrdbvy.html

public function __construct(private int $id) {}
来源：http://hz.xingfuxueyuan.xyz/gtflqlghnm.html

[U51] PHP：数组解构
来源：http://hz.iojbl.cn/gtluzfkssu.html

[$a, $b] = $arr;
来源：http://hz.mhx1999.top/gtlfllacti.html

[U52] PHP：箭头函数
来源：http://hz.gzhubu.top/gtftspeucj.html

$double = fn($x) => $x * 2;
来源：http://hz.gotoacloud.top/gtrajepacb.html

[U53] PHP：空合并运算符
来源：http://hz.pycfn.com/gtshfhohzv.html

$v = $a ?? $b ?? "default";
来源：http://hz.cqqwz.cn/gtwgozjzix.html

[U54] PHP：空安全调用
来源：http://hz.yuxming.cn/gtipbwbllp.html

$obj?->method()
来源：http://hz.9152youxi.cn/gtunzidzyp.html

[U55] PHP：match 表达式
来源：http://hz.zdqjudy.top/gtwoeletrb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xinyue.icu/gtzdmtuiyd.html

[U56] PHP：命名参数
来源：http://hz.zhixingplan.top/gtiekadpso.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtaedbwiji.html

[U57] PHP：字符串插值
来源：http://hz.ehwqpu.com/gtcnseyjne.html

"值: {$a}"
来源：http://hz.shanyushiyangkeji.top/gtumvfjuyc.html

[U58] PHP：数组三件套
来源：http://hz.zhijiandao.cn/gtqjkrsmsh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.meibo888.top/gtuzjwwsst.html

[U59] PHP：自定义排序
来源：http://hz.nanxinkj.top/gtafqeahuv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtbjodsfec.html

[U60] PHP：JSON 编解码
来源：http://hz.andypj.xyz/gtsakjlbqc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gtltggtnht.html

[U61] PHP：正则
来源：http://hz.zhiwuduotai.top/gtcdgclpip.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtgymclgpi.html

[U62] PHP：日期对象
来源：http://hz.daxiang520.top/gtrkoeyqqr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aizwys.cn/gthisukxqo.html

[U63] PHP：文件读写
来源：http://hz.yj202588.top/gtufkpvfiz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hysaishi.cn/gtsqjrzhbg.html

[U64] PHP：目录遍历
来源：http://hz.yangfankeji.com/gtrxiyqzed.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yueranfly.top/gtqarngmxj.html

[U65] PHP：会话
来源：http://hz.andypj.xyz/gtpepkwpjz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.mhx1999.top/gtwaiijfuh.html

[U66] PHP：设置 Cookie
来源：http://hz.quarkkingdee.top/gtebpnhhjv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gtwnmuxtkp.html

[U67] PHP：处理文件上传
来源：http://hz.quarkkingdee.top/gtotollkss.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.havefunace.top/gtswijdbnc.html

[U68] PHP：PDO 连接
来源：http://hz.zhongyouzk.top/gtdnxtouyf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtidvrntpi.html

[U69] PHP：PDO 预处理
来源：http://hz.zhijiandao.cn/gtzrowgexi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtyehpykuh.html

[U70] PHP：PDO 事务
来源：http://hz.tanke756.top/gtjbvmtdkj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtzkwftnse.html

[U71] PHP：抛出异常
来源：http://hz.guannengcc.top/gtqrkvugyw.html

throw new RuntimeException("失败", 500);
来源：http://hz.feifeiyinyue.top/gtposiqejr.html

[U72] PHP：写错误日志
来源：http://hz.xingfuxueyuan.xyz/gtoeywwezl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yuxming.cn/gtyuhduwim.html

[U73] PHP：读取 ini 配置
来源：http://hz.jianghu66.top/gtfuziumiu.html

parse_ini_file("config.ini", true)
来源：http://hz.xuanzx.com/gtebkqnmyt.html

[U74] PHP：读取环境变量
来源：http://hz.xuanzx.com/gtypvcflry.html

getenv("APP_ENV") ?: "production"
来源：http://hz.fengsongda.top/gtyfycstku.html

[U75] PHP：依赖注入
来源：http://hz.fengsongda.top/gtwawvhzfb.html

composer require psr/container
来源：http://hz.ybcxt.top/gtrrbfbgij.html

[U76] PHP：简单路由
来源：http://hz.9152youxi.cn/gtiirshzgy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxuanxn.top/gtfcifeiwx.html

[U77] PHP：模板渲染
来源：http://hz.wangdashe.top/gteaqcxyvk.html

composer require twig/twig
来源：http://hz.hnqzz.top/gtrkddglmq.html

[U78] PHP：单元测试
来源：http://hz.sxryk.cn/gtmvhkxgpl.html

composer require --dev phpunit/phpunit
来源：http://hz.redwolf501.top/gtejedgqrx.html

[U79] PHP：静态分析
来源：http://hz.yj20258.top/gtapjimczw.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxuanxn.top/gtkxqylhac.html

[U80] PHP：代码规范修复
来源：http://hz.yj20258.top/gtryeckqtz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aibaodan.cn/gtyhbbmrak.html

[U81] JS：初始化项目
来源：http://hz.hongshengwenyu.top/gtzaecoden.html

npm init -y;  npm i express
来源：http://hz.yj20258.top/gtetumhjmi.html

[U82] JS：package.json 脚本
来源：http://hz.yvedp.cn/gtjpzhobaw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jqgufenzy.top/gtfxpybidz.html

[U83] JS：ES Module 导入导出
来源：http://hz.kuanghao11.cn/gtxevmwors.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ivvv.top/gtepovswlm.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangkeji.top/gtafthwakr.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtnjuippmw.html

[U85] JS：可选链
来源：http://hz.yanxiufei.cn/gthxfxedif.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtcadrycrq.html

[U86] JS：空值合并
来源：http://hz.zhiwuduotai.top/gtnqaeojin.html

a ?? b
来源：http://hz.xinyue.icu/gtnrcarmpr.html

[U87] JS：解构默认值
来源：http://hz.hongshengwenyu.top/gtuwxbkhod.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ywan-chungtsiang.top/gtphreslcs.html

[U88] JS：对象展开合并
来源：http://hz.yj20258.top/gtxhtviwjb.html

{ ...a, ...b }
来源：http://hz.yj20258888.top/gtswwwgtrm.html

[U89] JS：数组去重
来源：http://hz.yuxming.cn/gtryuhkelt.html

[...new Set(arr)]
来源：http://hz.snrcjt.cn/gthvxgjhvx.html

[U90] JS：数字数组排序
来源：http://hz.ywan-chungtsiang.top/gtjbbsnipf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtxsptolgw.html

[U91] JS：对象键值遍历
来源：http://hz.ydzc1.top/gtndxpveuy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.dianchejie.cn/gtxjfqvqxt.html

[U92] JS：深拷贝
来源：http://hz.chenzaomai.com/gtpyfhizap.html

structuredClone(obj)
来源：http://hz.quarkkingdee.top/gthghmiglz.html

[U93] JS：模板字符串
来源：http://hz.yonumen.top/gtmazllnmm.html

`共 ${n} 条`
来源：http://hz.52xcode.cn/gtpptkgsxf.html

[U94] JS：箭头函数
来源：http://hz.cucudq.cn/gtcqxqrcwo.html

const double = x => x * 2;
来源：http://hz.gotoacloud.top/gtlahupuwv.html

[U95] JS：Promise 包装
来源：http://hz.shanyushiyangtech.top/gtbvgwowle.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtinatjfxk.html

[U96] JS：async/await 与异常
来源：http://hz.tianlin.xyz/gtimohergc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtabgvuwjy.html

[U97] JS：并发请求
来源：http://hz.iojbl.cn/gtyxaqfegp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtjrqcgzvx.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinqigfzy.top/gtqsyqfrap.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuanzhike.top/gttjzzhvym.html

[U99] JS：事件监听
来源：http://hz.ydzc1.top/gtuwimimeg.html

el.addEventListener("click", e => {})
来源：http://hz.yj202588.top/gtskoysnxh.html

[U100] JS：DOM 查询
来源：http://hz.haohaochexian.top/gtmgdqnuao.html

document.querySelector(".item")
来源：http://hz.guowangkeji.top/gtiftdjqiv.html

[U101] JS：classList 操作
来源：http://hz.jinyuanbaomall.cn/gtdnwflodc.html

el.classList.toggle("active")
来源：http://hz.jinghuilouyu.cn/gtsyosakra.html

[U102] JS：本地存储
来源：http://hz.sysykeji.top/gtvouxqdqt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dianchejie.cn/gtidoqhxeq.html

[U103] JS：定时器
来源：http://hz.ivvv.top/gtajysigpl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jiagoushi.top/gtaselhqza.html

[U104] JS：防抖
来源：http://hz.quarkkingdee.top/gtcstircyl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtpissqedf.html

[U105] JS：节流
来源：http://hz.chenzaomai.com/gtvfonakok.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinyuanbaomall.cn/gtttumudfd.html

[U106] JS：日期格式化
来源：http://hz.jiagoushi.top/gtddkuevqs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zdqjudy.top/gthfmjqmai.html

[U107] JS：数字千分位
来源：http://hz.jqgufenzy.top/gtfaluswid.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtiklbnqdj.html

[U108] JS：随机整数
来源：http://hz.tian-w.cn/gtzinyzofi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yvedp.cn/gtkqmscskt.html

[U109] JS：数组分组
来源：http://hz.yongpay.top/gtancixhca.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtpnemzhkv.html

[U110] JS：数组分块
来源：http://hz.yonumen.top/gtnntktiyg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhengqikj.top/gticdutgsw.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtqjatszep.html

new Map(Object.entries(obj))
来源：http://hz.shanyushiyangtech.top/gtvunflssa.html

[U112] JS：字符串补位
来源：http://hz.yangfankeji.com/gtsqmqbfjv.html

"7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtmakteicn.html

[U113] JS：正则替换全部
来源：http://hz.hnqzz.top/gtukwdlxwy.html

s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtyvouhybp.html

[U114] JS：JSON 深比较
来源：http://hz.yuanzhike.top/gtdvgvwdhv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtiqajnntx.html

[U115] JS：生成 UUID
来源：http://hz.cucudq.cn/gteetpplli.html

crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gttvrbiton.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xingfuxueyuan.xyz/gteultdaio.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jlsjyb.cn/gtpwedbjbg.html

[U117] JS：单元测试
来源：http://hz.gzhubu.top/gtsklmuxcc.html

npm i -D vitest;  npx vitest
来源：http://hz.yueranfly.top/gtosndmdma.html

[U118] JS：开发服务器
来源：http://hz.yueranfly.top/gttdjavbxx.html

npm i -D vite;  npx vite
来源：http://hz.cheryme.top/gtplrjwdpa.html

[U119] JS：生产构建
来源：http://hz.yj20258.top/gtiljtetlw.html

npx vite build
来源：http://hz.zhengqikj.top/gtujdlwryv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhaomingkeji.xyz/gtqridhrxl.html

import.meta.env.VITE_API_URL
来源：http://hz.hammf.cn/gtjrarkssr.html

================================================================================
来源：http://hz.cucudq.cn/gtrnlipfhn.html

统计汇总
来源：http://hz.gaohongyu789.top/gtxvimenhj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyssmngmx.html

按语言统计（条）：
来源：http://hz.birdmap.top/gtbrsarpfc.html

Python ......... 252
来源：http://hz.jyoumei.cn/gtxrsuyzla.html

PHP ............ 252
来源：http://hz.pengpengdd.cyou/gtuzwflsee.html

JavaScript ..... 252
来源：http://hz.gotoacloud.top/gtgbisgvoz.html

TypeScript ..... 212
来源：http://hz.cucudq.cn/gtjyqsjspx.html

Java ........... 212
来源：http://hz.aizwys.cn/gtwwvafdjl.html

Go ............. 212
来源：http://hz.xylfe.cn/gtgpxlrmmd.html

Ruby ........... 212
来源：http://hz.aibaodan.cn/gtmvyiophv.html

C# ............. 212
来源：http://hz.andypj.xyz/gthfrmikzv.html

C .............. 30
来源：http://hz.wangshuangyany.cn/gtkttycdig.html

C++ ............ 30
来源：http://hz.hfpthk.cn/gtlkqeetrj.html

SQL ............ 90
来源：http://hz.guannengcc.top/gtdnlwpfir.html

Bash ........... 80
来源：http://hz.smart0.xyz/gtlfwnzion.html

Kotlin ......... 15
来源：http://hz.zycfv.cn/gtgqrianzc.html

Swift .......... 15
来源：http://hz.haohaochexian.top/gthozdaoxe.html

Lua ............ 10
来源：http://hz.xylfe.cn/gtnsusotpd.html

Perl ........... 10
来源：http://hz.shuidangran.top/gtrcjcjurl.html

Scala .......... 10
来源：http://hz.jyoumei.cn/gtvrbxcqne.html

------------------------------------
来源：http://hz.yangfankeji.com/gtromkablq.html

合计 ........... 2106 条
来源：http://hz.chenjidiqi.icu/gtszxcjgdm.html

按章节统计：
来源：http://hz.yj20258.top/gtrtvhaffx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtnwpvcevj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.316326.xyz/gtcpwoedmw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtkwjvwuig.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shanyushiyangkeji.top/gtvwauczkx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.pengpengdd.cyou/gthlrzblla.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtphilqpoh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtrcwrkgfp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtkqfxuchr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtysldljbp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gterageqbi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtbrhjffzx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gttyruqgxw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtvetcvwua.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xziqi.cn/gtiydxuhif.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yvedp.cn/gtxhbpadcy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtfloeesnx.html

Q SQL 专题                              90
来源：http://hz.yvedp.cn/gtgjueippy.html

R Bash 专题                             80
来源：http://hz.daxiang520.top/gtjpjvbbbs.html

S C / C++ 专题                          60
来源：http://hz.ivvv.top/gthkoqtuix.html

T 其他语言补充                          60
来源：http://hz.shuidangran.top/gtbgorudpo.html


<!-- 参考信息 -->