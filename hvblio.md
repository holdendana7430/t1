代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuanzhike.top/gtvzbercuc.html

================================================================================
来源：http://hz.cqqwz.cn/gtmcyhuzor.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtbxcarlwm.html

================================================================================
来源：http://hz.yueranfly.top/gtjaohchsq.html

[U01] Py：创建虚拟环境
来源：http://hz.meibo888.top/gtslcdphcf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hysaishi.cn/gtlthedlpl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj202588.top/gtwdfpmjrc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtadanmhaj.html

[U03] Py：加载 .env 配置
来源：http://hz.bjfxy.top/gtmdguyjft.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gtzketyidl.html

[U04] Py：变量调试打印
来源：http://hz.shzxlz.cn/gtwxwhpdxr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hongshengwenyu.top/gthwdwgayd.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtllysrirr.html

list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtlqlnuedv.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtdlwqmisq.html

{**a, **b}
来源：http://hz.andypj.xyz/gtjwfmuzld.html

[U07] Py：反转字典键值
来源：http://hz.daxiang520.top/gtottvppsq.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtjhqflkuw.html

[U08] Py：展平二维列表
来源：http://hz.andypj.xyz/gtocfnvnbb.html

[y for x in nested for y in x]
来源：http://hz.ehwqpu.com/gtnxxthrur.html

[U09] Py：字典取最大值的键
来源：http://hz.c1oappe.top/gtonyjdhuf.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gtzqbgrkym.html

[U10] Py：按值排序字典
来源：http://hz.hywenlv.cn/gtdnsotugz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yongpay.top/gtmiogantl.html

[U11] Py：生成器表达式
来源：http://hz.snrcjt.cn/gtjgloychc.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtncxasjwh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangshuangyany.cn/gtvfwujbkz.html

Counter(arr).most_common(3)
来源：http://hz.tanke756.top/gtqeejgarf.html

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gtpxbivryi.html

deque(maxlen=10)
来源：http://hz.wangdashe.top/gtjvetstaa.html

[U14] Py：分组收集到列表
来源：http://hz.mhx1999.top/gtlfitulud.html

defaultdict(list)
来源：http://hz.guannengcc.top/gtfcjqifxm.html

[U15] Py：高精度计时
来源：http://hz.zhixingplan.top/gtzcsiuwut.html

t = time.perf_counter()
来源：http://hz.jinghuilouyu.cn/gtzkgoayfs.html

[U16] Py：命令行参数解析
来源：http://hz.redwolf501.top/gtaelwqswm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtvvervxeo.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtvrgiobss.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.pengpengdd.cyou/gtmrqudhhg.html

[U18] Py：预编译正则
来源：http://hz.kuanghao11.cn/gtehggovki.html

pat = re.compile(r"\d+")
来源：http://hz.svipenyu.cn/gtccpvepxv.html

[U19] Py：正则替换带回调
来源：http://hz.zhiwuduotai.top/gtyxfylnav.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sweek.top/gtqvygjyxh.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtpsohjjpn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sysykeji.top/gtdaddexkk.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinqigufen.top/gtodrneilb.html

@contextlib.contextmanager
来源：http://hz.quarkkingdee.top/gtyvvsudqb.html

[U22] Py：矩阵转置
来源：http://hz.xinyue.icu/gtnfddyryf.html

list(zip(*m))
来源：http://hz.chenjidiqi.icu/gtpkrjfcce.html

[U23] Py：分块读取大文件
来源：http://hz.xinyue.icu/gtswgkybyo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtodhwzieo.html

[U24] Py：路径操作
来源：http://hz.jinghuilouyu.cn/gtckckbxyz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gthwfzldyo.html

[U25] Py：CSV 按字典读
来源：http://hz.pengpengdd.cyou/gtzqzqqtrk.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtafqnayxv.html

[U26] Py：并发下载
来源：http://hz.yj20258888.top/gtmauxzchd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtrdrjgwql.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtkthbntoa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yueranfly.top/gtpcssmmsb.html

[U28] Py：类型别名
来源：http://hz.wangshuangyany.cn/gtrrzmavpj.html

UserId = int
来源：http://hz.ybcxt.top/gtxxgcyxtq.html

[U29] Py：属性校验
来源：http://hz.yanxiufei.cn/gtubcbdwat.html

@property 与 @x.setter 配合
来源：http://hz.zhijiandao.cn/gtprmfxqlv.html

[U30] Py：数据类
来源：http://hz.jyoumei.cn/gtihqenwgv.html

@dataclass(slots=True)
来源：http://hz.hongshengwenyu.top/gtmlsxoqoo.html

[U31] Py：单测
来源：http://hz.redwolf501.top/gthnvfhmce.html

python -m pytest -q
来源：http://hz.jinghuilouyu.cn/gtauuzamly.html

[U32] Py：代码格式化
来源：http://hz.jlsjyb.cn/gtyyaoejdf.html

ruff format . && ruff check --fix .
来源：http://hz.yuanzhike.top/gtsgokndkx.html

[U33] Py：打包发布
来源：http://hz.xinyue.icu/gtoamgqakc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258888.top/gtxdhmnipr.html

[U34] Py：判断编码
来源：http://hz.hnxiangtu.top/gtybyotkvk.html

chardet.detect(raw)
来源：http://hz.quarkkingdee.top/gtauzwwuoi.html

[U35] Py：发送邮件
来源：http://hz.quarkkingdee.top/gtfwtleveg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinghuilouyu.cn/gtajrkvbzd.html

[U36] Py：定时任务
来源：http://hz.yj20258888.top/gtgdikwvkb.html

schedule.every(10).minutes.do(job)
来源：http://hz.shangyingyoupin.top/gthnftxtxo.html

[U37] Py：读写 Excel
来源：http://hz.jinqigufen.top/gtfimisydw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.svipenyu.cn/gtycvqpkmj.html

[U38] Py：获取脚本所在目录
来源：http://hz.kuanghao11.cn/gtdijcprah.html

Path(__file__).resolve().parent
来源：http://hz.zhijiandao.cn/gtoplgxhib.html

[U39] Py：判断是否在交互环境
来源：http://hz.cashguo.top/gtrkjowwbq.html

sys.stdout.isatty()
来源：http://hz.iojbl.cn/gtrgknbpio.html

[U40] Py：打印到标准错误
来源：http://hz.jqgfzy.top/gtjdqdhveb.html

print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtjmllwmih.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.meibo888.top/gtynljqnvy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.vqdsnc.cn/gtdkftzoed.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnqzz.top/gtfajdpmhb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yangfankeji.com/gtftebywxh.html

[U43] PHP：声明命名空间
来源：http://hz.ydzc1.top/gtgwrszylm.html

namespace App\Http;
来源：http://hz.ybcxt.top/gtqdxyobed.html

[U44] PHP：开启严格类型
来源：http://hz.yj202588.top/gtegvdlako.html

declare(strict_types=1);
来源：http://hz.shuidangran.top/gtmzyflgfq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.birdmap.top/gthjowvsnz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtlhedndxx.html

[U46] PHP：可空类型
来源：http://hz.chenzaomai.com/gtddnjxylr.html

?string $name = null
来源：http://hz.xylfe.cn/gtanjkvsly.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtyujvewyz.html

int|string $id
来源：http://hz.cheryme.top/gthjxhrypg.html

[U48] PHP：纯枚举
来源：http://hz.0kj1m.cn/gthlemdcpy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ehwqpu.com/gtupvhjgur.html

[U49] PHP：只读属性
来源：http://hz.quarkkingdee.top/gtlfzrroct.html

public readonly string $name
来源：http://hz.yongpay.top/gtvtlltftr.html

[U50] PHP：构造器属性提升
来源：http://hz.cucudq.cn/gtqfkrtdqt.html

public function __construct(private int $id) {}
来源：http://hz.haohaochexian.top/gtjhynotng.html

[U51] PHP：数组解构
来源：http://hz.dashuyun.cn/gtyxtwqqke.html

[$a, $b] = $arr;
来源：http://hz.hfpthk.cn/gttlqwgtuz.html

[U52] PHP：箭头函数
来源：http://hz.pycfn.com/gttqtczjxc.html

$double = fn($x) => $x * 2;
来源：http://hz.haohaochexian.top/gtwenwvrgr.html

[U53] PHP：空合并运算符
来源：http://hz.chenjidiqi.icu/gtmlmyfjyy.html

$v = $a ?? $b ?? "default";
来源：http://hz.meibo888.top/gtzepddvps.html

[U54] PHP：空安全调用
来源：http://hz.dashuyun.cn/gtcxjklbqa.html

$obj?->method()
来源：http://hz.haohaochexian.top/gtryixgpqx.html

[U55] PHP：match 表达式
来源：http://hz.nanxinkj.top/gtoesqoeli.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xinyue.icu/gtcqtuiciq.html

[U56] PHP：命名参数
来源：http://hz.fzhhl.top/gtyptodsav.html

f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtmdgivagn.html

[U57] PHP：字符串插值
来源：http://hz.zhongyouzk.top/gtnzzvonag.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtbzmlvoks.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gtqvzjmcds.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shanyushiyangkeji.top/gtgcfaqugm.html

[U59] PHP：自定义排序
来源：http://hz.yueranfly.top/gthzoypigp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtzmcwosql.html

[U60] PHP：JSON 编解码
来源：http://hz.wangdashe.top/gtbbwrwhmm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yueranfly.top/gtmelqplrk.html

[U61] PHP：正则
来源：http://hz.sxryk.cn/gtxvbecsbf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtmjskvqpg.html

[U62] PHP：日期对象
来源：http://hz.yuanzhike.top/gtglstdilv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtjrneuzje.html

[U63] PHP：文件读写
来源：http://hz.ywan-chungtsiang.top/gtzcentzeu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gttahdijtd.html

[U64] PHP：目录遍历
来源：http://hz.ppjwa.cn/gtnxmsyjme.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nanxuanxn.top/gthegipcyr.html

[U65] PHP：会话
来源：http://hz.52xcode.cn/gtxdgcxeks.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xylfe.cn/gtfcojkbsu.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtglnsgqms.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhongyouzk.top/gtubxqjfyf.html

[U67] PHP：处理文件上传
来源：http://hz.zhiwuduotai.top/gtddapatjo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.sysykeji.top/gtwqdroeuh.html

[U68] PHP：PDO 连接
来源：http://hz.gzhubu.top/gtjkilebfw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258.top/gtrhnwqouj.html

[U69] PHP：PDO 预处理
来源：http://hz.chenzaomai.com/gthdonfwed.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jlsjyb.cn/gtktlfukzf.html

[U70] PHP：PDO 事务
来源：http://hz.guowangkeji.top/gtqhnhujau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yonumen.top/gttiirzwpn.html

[U71] PHP：抛出异常
来源：http://hz.jianghu66.top/gtphtrrzcm.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj202588.top/gtkihjtdzo.html

[U72] PHP：写错误日志
来源：http://hz.chenlongwang.top/gtfulcbejt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xinyue.icu/gtbfayqvtp.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhengqikj.top/gtwlfvensj.html

parse_ini_file("config.ini", true)
来源：http://hz.birdmap.top/gtfsoxoyxj.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gthwtoykhg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nanxuanxn.top/gtssnkztxo.html

[U75] PHP：依赖注入
来源：http://hz.yonumen.top/gtvmaturax.html

composer require psr/container
来源：http://hz.yueranfly.top/gtbaynsmsz.html

[U76] PHP：简单路由
来源：http://hz.sweek.top/gtshrqwigi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tian-w.cn/gtszyebhhf.html

[U77] PHP：模板渲染
来源：http://hz.cdnleiting.top/gtnvoxbufv.html

composer require twig/twig
来源：http://hz.yvedp.cn/gttnjtiizv.html

[U78] PHP：单元测试
来源：http://hz.zhixingplan.top/gtvkzsnzwx.html

composer require --dev phpunit/phpunit
来源：http://hz.zhaomingkeji.xyz/gtqczxxedo.html

[U79] PHP：静态分析
来源：http://hz.guannengcc.top/gttcaxhvbh.html

composer require --dev phpstan/phpstan
来源：http://hz.cucudq.cn/gtffgavfry.html

[U80] PHP：代码规范修复
来源：http://hz.ydzc1.top/gtjbwnygys.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.bjfxy.top/gtdttgrbky.html

[U81] JS：初始化项目
来源：http://hz.ydzc1.top/gtruoezdka.html

npm init -y;  npm i express
来源：http://hz.yueranfly.top/gtcrzwqdnf.html

[U82] JS：package.json 脚本
来源：http://hz.wangdashe.top/gthudrqlcr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xylfe.cn/gtfkogwxnw.html

[U83] JS：ES Module 导入导出
来源：http://hz.yuxming.cn/gtlvwzmxhc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.quarkkingdee.top/gtrldrhssh.html

[U84] JS：CommonJS 写法
来源：http://hz.0kj1m.cn/gtaoplifdi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hywenlv.cn/gtmfducfmx.html

[U85] JS：可选链
来源：http://hz.xylfe.cn/gtevkgrcpt.html

a?.b?.c
来源：http://hz.yanxiufei.cn/gtbktbrtrk.html

[U86] JS：空值合并
来源：http://hz.aizwys.cn/gtflnmgkcs.html

a ?? b
来源：http://hz.kuanghao11.cn/gtydomzgrn.html

[U87] JS：解构默认值
来源：http://hz.jianghu66.top/gtkzpouqbq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yongpay.top/gtjrxmjrib.html

[U88] JS：对象展开合并
来源：http://hz.gzhubu.top/gtzbepavdm.html

{ ...a, ...b }
来源：http://hz.birdmap.top/gttddwknqd.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gtthjzgpiu.html

[...new Set(arr)]
来源：http://hz.aizwys.cn/gthkxecogm.html

[U90] JS：数字数组排序
来源：http://hz.nanxinkj.top/gtgnvmiuyo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtsqkmjxvu.html

[U91] JS：对象键值遍历
来源：http://hz.haohaochexian.top/gtjpijseju.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yonumen.top/gtwrzjgwgq.html

[U92] JS：深拷贝
来源：http://hz.ydjk.org.cn/gtueryodde.html

structuredClone(obj)
来源：http://hz.meibo888.top/gtorugwnjt.html

[U93] JS：模板字符串
来源：http://hz.jqgufenzy.top/gthmiepvcp.html

`共 ${n} 条`
来源：http://hz.xinyue.icu/gtjrdddmew.html

[U94] JS：箭头函数
来源：http://hz.zhoulong.xyz/gtxfndxioa.html

const double = x => x * 2;
来源：http://hz.hnqzz.top/gtmtcttudl.html

[U95] JS：Promise 包装
来源：http://hz.52xcode.cn/gtxjyjjsfb.html

new Promise((resolve, reject) => {})
来源：http://hz.chenjidiqi.icu/gtkzohfpji.html

[U96] JS：async/await 与异常
来源：http://hz.xingfuxueyuan.xyz/gtocknitql.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.guannengcc.top/gtaqcetfcf.html

[U97] JS：并发请求
来源：http://hz.xinyue.icu/gthxzhqmmt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtcaexplcm.html

[U98] JS：fetch 带 JSON
来源：http://hz.yj20258.top/gtoedlqzyd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.aibaodan.cn/gteodjllhr.html

[U99] JS：事件监听
来源：http://hz.haohaochexian.top/gtyeyjlguf.html

el.addEventListener("click", e => {})
来源：http://hz.yj202588.top/gttuehqorw.html

[U100] JS：DOM 查询
来源：http://hz.xziqi.cn/gtjxzwxnme.html

document.querySelector(".item")
来源：http://hz.sxryk.cn/gtdudfeice.html

[U101] JS：classList 操作
来源：http://hz.tian-w.cn/gtdwkxosno.html

el.classList.toggle("active")
来源：http://hz.zhongyouzk.top/gteomrlugy.html

[U102] JS：本地存储
来源：http://hz.smart0.xyz/gtwnhdvnef.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.snrcjt.cn/gtmhaeikmo.html

[U103] JS：定时器
来源：http://hz.ydjk.org.cn/gtvljzmpvf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.feifeiyinyue.top/gtcpsnrius.html

[U104] JS：防抖
来源：http://hz.redwolf501.top/gtdynkjfqx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gteranrdnr.html

[U105] JS：节流
来源：http://hz.ppjwa.cn/gtbmgmlqks.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.iojbl.cn/gtmxkmxavg.html

[U106] JS：日期格式化
来源：http://hz.hnxiangtu.top/gtbdaopihy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jianghu66.top/gtfdchoglf.html

[U107] JS：数字千分位
来源：http://hz.jinqigfzy.top/gtglxmmpxp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxuanxn.top/gtxbvkweld.html

[U108] JS：随机整数
来源：http://hz.yuanzhike.top/gtnvewayfm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtatjzznmp.html

[U109] JS：数组分组
来源：http://hz.jiagoushi.top/gtlriagrjb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtmnlxuxre.html

[U110] JS：数组分块
来源：http://hz.sysykeji.top/gtljjqevfs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.guannengcc.top/gtmghwzuzu.html

[U111] JS：对象转 Map
来源：http://hz.sxryk.cn/gtjsqhikge.html

new Map(Object.entries(obj))
来源：http://hz.cdnleiting.top/gtromitbkg.html

[U112] JS：字符串补位
来源：http://hz.shangyingyoupin.top/gtjmubfurd.html

"7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtbkqwbpgx.html

[U113] JS：正则替换全部
来源：http://hz.wangshuangyany.cn/gtnsakszpq.html

s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtxknlrjpr.html

[U114] JS：JSON 深比较
来源：http://hz.sufxvd.cn/gtyqerknsm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtzxobzaln.html

[U115] JS：生成 UUID
来源：http://hz.cheryme.top/gtlohkijwz.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtejrlfqjx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cucudq.cn/gthlyxvfni.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xinyue.icu/gtfclatdim.html

[U117] JS：单元测试
来源：http://hz.gotoacloud.top/gtwdhnneii.html

npm i -D vitest;  npx vitest
来源：http://hz.shanyushiyangtech.top/gtrlgmucxn.html

[U118] JS：开发服务器
来源：http://hz.hywenlv.cn/gthyiiteys.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtqfdlsill.html

[U119] JS：生产构建
来源：http://hz.zhijiandao.cn/gtmmlbpwja.html

npx vite build
来源：http://hz.fengsongda.top/gtpbrwegjw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangtech.top/gtizebadjs.html

import.meta.env.VITE_API_URL
来源：http://hz.jqgfzy.top/gtgemmzlmh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtjzaxlksm.html

统计汇总
来源：http://hz.xinyue.icu/gtrabofqmg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyioggeci.html

按语言统计（条）：
来源：http://hz.jianghu66.top/gtqkufsfsk.html

Python ......... 252
来源：http://hz.aibaodan.cn/gtkbuozdjc.html

PHP ............ 252
来源：http://hz.yj20258.top/gteixzgujw.html

JavaScript ..... 252
来源：http://hz.zycfv.cn/gtpmyjtmop.html

TypeScript ..... 212
来源：http://hz.yuxming.cn/gtvliprtse.html

Java ........... 212
来源：http://hz.shanyushiyangkeji.top/gterwdxumf.html

Go ............. 212
来源：http://hz.dianchejie.cn/gtdxrfxqyg.html

Ruby ........... 212
来源：http://hz.fengsongda.top/gtsjfdmbkw.html

C# ............. 212
来源：http://hz.zhoulong.xyz/gtsznweoat.html

C .............. 30
来源：http://hz.gzhubu.top/gtnqhvyerw.html

C++ ............ 30
来源：http://hz.dashuyun.cn/gtgbptmyei.html

SQL ............ 90
来源：http://hz.meibo888.top/gtxjhuimje.html

Bash ........... 80
来源：http://hz.nanxinkj.top/gtwgdkivbj.html

Kotlin ......... 15
来源：http://hz.feifeiyinyue.top/gtrgmvsjnk.html

Swift .......... 15
来源：http://hz.svipenyu.cn/gtacrufdxf.html

Lua ............ 10
来源：http://hz.sysykeji.top/gtqtuldypk.html

Perl ........... 10
来源：http://hz.vqdsnc.cn/gtbruiujyc.html

Scala .......... 10
来源：http://hz.fengsongda.top/gtgpyacnbs.html

------------------------------------
来源：http://hz.sweek.top/gtnujyxmrr.html

合计 ........... 2106 条
来源：http://hz.jinyuanbaomall.cn/gtcomzmoje.html

按章节统计：
来源：http://hz.chenzaomai.com/gtfjtedepu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtcneavysb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtjotlaebw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtumuxlpqw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtochrqqdf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dianchejie.cn/gtdqprfvvv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtndnknyqg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtutdzuebc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.andypj.xyz/gtoddmitnw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtrxweygck.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtokjukgyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gttfkrwycb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtssnjqwck.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gttqpqvksl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtlogakijf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.316326.xyz/gtwdcfupyv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtkbjsduwv.html

Q SQL 专题                              90
来源：http://hz.hnqzz.top/gtltgxdufj.html

R Bash 专题                             80
来源：http://hz.xingfuxueyuan.xyz/gtkjchjbtx.html

S C / C++ 专题                          60
来源：http://hz.nanxinkj.top/gtghxhjeme.html

T 其他语言补充                          60
来源：http://hz.tianlin.xyz/gtbbqysipi.html

U 高频实用片段                         120
来源：http://hz.aizwys.cn/gtpdxjbttb.html

------------------------------------
来源：http://hz.daxiang520.top/gtgvcjsaqg.html

合计                                  2106 条
来源：http://hz.jyoumei.cn/gttniubuve.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtqnaehhla.html

使用提醒
来源：http://hz.dashuyun.cn/gtzvfjbffu.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gthfqmzczo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hongshengwenyu.top/gtksummoaa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shuidangran.top/gtigxyqygh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shzxlz.cn/gtsgceckpu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zycfv.cn/gtexrnerzy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shanyushiyangtech.top/gttxbbrdmt.html

—— 文件结束 ——
来源：http://hz.iojbl.cn/gtuyhaicto.html


<!-- 参考信息 -->