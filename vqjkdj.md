代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgufenzy.top/gtjcyesokm.html

================================================================================
来源：http://hz.gotoacloud.top/gtigeerdws.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtuziuiknx.html

================================================================================
来源：http://hz.zhengqikj.top/gtrgrhwmxy.html

[U01] Py：创建虚拟环境
来源：http://hz.zhongyouzk.top/gtodmulyin.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.kuanghao11.cn/gtdkobpgrh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dianchejie.cn/gtwgflstwd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tanke756.top/gthioozsbe.html

[U03] Py：加载 .env 配置
来源：http://hz.sweek.top/gtdmfjgdut.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cashguo.top/gtymeljxrw.html

[U04] Py：变量调试打印
来源：http://hz.jqgfzy.top/gtgwrubknu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sxryk.cn/gtugkobcgz.html

[U05] Py：列表去重且保序
来源：http://hz.aizwys.cn/gtrvquadre.html

list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtthkxxtbp.html

[U06] Py：合并两个字典
来源：http://hz.zhixingplan.top/gtqqmwipdb.html

{**a, **b}
来源：http://hz.ybcxt.top/gtndnwptsu.html

[U07] Py：反转字典键值
来源：http://hz.sweek.top/gtsejeubug.html

{v: k for k, v in d.items()}
来源：http://hz.pycfn.com/gtaemyykvx.html

[U08] Py：展平二维列表
来源：http://hz.wangshuangyany.cn/gtnlzqwplo.html

[y for x in nested for y in x]
来源：http://hz.nanxinkj.top/gtpmblivyf.html

[U09] Py：字典取最大值的键
来源：http://hz.chenjidiqi.icu/gtautniabb.html

max(d, key=d.get)
来源：http://hz.fengsongda.top/gtetjokwca.html

[U10] Py：按值排序字典
来源：http://hz.chenzaomai.com/gtfrsjgxqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nwbrower.top/gtayajwaog.html

[U11] Py：生成器表达式
来源：http://hz.svipenyu.cn/gtuszowpms.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtxqpkbquj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.haohaochexian.top/gtghkembgc.html

Counter(arr).most_common(3)
来源：http://hz.smart0.xyz/gtlyatdpiu.html

[U13] Py：固定长度队列
来源：http://hz.jianghu66.top/gtsjbpxaub.html

deque(maxlen=10)
来源：http://hz.ywan-chungtsiang.top/gtvlaqmjwt.html

[U14] Py：分组收集到列表
来源：http://hz.quarkkingdee.top/gtalqpwlaa.html

defaultdict(list)
来源：http://hz.9152youxi.cn/gtgvjeqkrk.html

[U15] Py：高精度计时
来源：http://hz.smart0.xyz/gtfmhhhymh.html

t = time.perf_counter()
来源：http://hz.aizwys.cn/gtjegzjuyf.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigfzy.top/gtradovysx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tian-w.cn/gtxlstjaxi.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtktotpzaf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ywan-chungtsiang.top/gtkhbeywcc.html

[U18] Py：预编译正则
来源：http://hz.xylfe.cn/gtjfpocowb.html

pat = re.compile(r"\d+")
来源：http://hz.hywenlv.cn/gtncfevrgh.html

[U19] Py：正则替换带回调
来源：http://hz.sysykeji.top/gtrkloskrc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.redwolf501.top/gtyswqbmat.html

[U20] Py：缓存函数结果
来源：http://hz.yangfankeji.com/gtriagtpdi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hammf.cn/gtmockxadk.html

[U21] Py：自定义上下文管理器
来源：http://hz.xinyue.icu/gtfacqaobe.html

@contextlib.contextmanager
来源：http://hz.hongshengwenyu.top/gtuluujscp.html

[U22] Py：矩阵转置
来源：http://hz.hammf.cn/gtxrpofjsm.html

list(zip(*m))
来源：http://hz.mhx1999.top/gtpifjeuxf.html

[U23] Py：分块读取大文件
来源：http://hz.kuanghao11.cn/gtaregnejf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hammf.cn/gtuzajoovf.html

[U24] Py：路径操作
来源：http://hz.cashguo.top/gtciwflldd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.smart0.xyz/gthgejufuj.html

[U25] Py：CSV 按字典读
来源：http://hz.mhx1999.top/gtfbfrwmmp.html

csv.DictReader(f)
来源：http://hz.ehwqpu.com/gtljvpbomf.html

[U26] Py：并发下载
来源：http://hz.zhixingplan.top/gthwcgxedh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xuetiantiany.cn/gtnpodpgya.html

[U27] Py：异步 HTTP
来源：http://hz.yvedp.cn/gtwjuxhuvb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yuanzhike.top/gtcktcibgo.html

[U28] Py：类型别名
来源：http://hz.guannengcc.top/gtofectxud.html

UserId = int
来源：http://hz.sysykeji.top/gtxarrhiur.html

[U29] Py：属性校验
来源：http://hz.shangyingyoupin.top/gtxqljapxf.html

@property 与 @x.setter 配合
来源：http://hz.ehwqpu.com/gtjahnadcg.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtcnlhgizt.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtigylkqdp.html

[U31] Py：单测
来源：http://hz.hysaishi.cn/gtiqmmgbzn.html

python -m pytest -q
来源：http://hz.daxiang520.top/gtiykavgms.html

[U32] Py：代码格式化
来源：http://hz.fzhhl.top/gtvllrqiqj.html

ruff format . && ruff check --fix .
来源：http://hz.cqqwz.cn/gtyqqdsoxy.html

[U33] Py：打包发布
来源：http://hz.yonumen.top/gtbqjzfatm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtznelmruj.html

[U34] Py：判断编码
来源：http://hz.sufxvd.cn/gttjtezcpa.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtnoovfpcx.html

[U35] Py：发送邮件
来源：http://hz.zdqjudy.top/gtkqffvkcl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pycfn.com/gtwaqscvap.html

[U36] Py：定时任务
来源：http://hz.jiagoushi.top/gtgoictpki.html

schedule.every(10).minutes.do(job)
来源：http://hz.cqqwz.cn/gtbcwkapnb.html

[U37] Py：读写 Excel
来源：http://hz.jinqigfzy.top/gtjozipzmv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtofklmuvf.html

[U38] Py：获取脚本所在目录
来源：http://hz.pycfn.com/gtblycwagf.html

Path(__file__).resolve().parent
来源：http://hz.aibaodan.cn/gthgqyiivt.html

[U39] Py：判断是否在交互环境
来源：http://hz.aizwys.cn/gthqobtejb.html

sys.stdout.isatty()
来源：http://hz.aibaodan.cn/gtarwjqjyk.html

[U40] Py：打印到标准错误
来源：http://hz.zhijiandao.cn/gtzpkopsuv.html

print("err", file=sys.stderr)
来源：http://hz.jlsjyb.cn/gtjbjujhnb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.redwolf501.top/gtsekaddvv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cheryme.top/gtqbxwiazw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jlsjyb.cn/gtbblbzzlk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hysaishi.cn/gtcdgqenvz.html

[U43] PHP：声明命名空间
来源：http://hz.quarkkingdee.top/gtflxfrohv.html

namespace App\Http;
来源：http://hz.iojbl.cn/gtxtyazyqu.html

[U44] PHP：开启严格类型
来源：http://hz.sufxvd.cn/gtsujuzvlg.html

declare(strict_types=1);
来源：http://hz.hnxiangtu.top/gtdmdxdhbp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xinyue.icu/gtwkmdyglb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnqzz.top/gttogytbmu.html

[U46] PHP：可空类型
来源：http://hz.ywan-chungtsiang.top/gtznuthztk.html

?string $name = null
来源：http://hz.sxryk.cn/gtdzzbxdxs.html

[U47] PHP：联合类型
来源：http://hz.yanxiufei.cn/gtaiitnsae.html

int|string $id
来源：http://hz.gzhubu.top/gtrsaaqzbw.html

[U48] PHP：纯枚举
来源：http://hz.jinqigfzy.top/gtyymzwbhs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tanke756.top/gtofnyawlo.html

[U49] PHP：只读属性
来源：http://hz.yj202588.top/gtnofdpwgm.html

public readonly string $name
来源：http://hz.wangdashe.top/gtgjpquexx.html

[U50] PHP：构造器属性提升
来源：http://hz.ehwqpu.com/gthseqzmur.html

public function __construct(private int $id) {}
来源：http://hz.nwbrower.top/gtaeckblie.html

[U51] PHP：数组解构
来源：http://hz.hysaishi.cn/gtsanezxag.html

[$a, $b] = $arr;
来源：http://hz.hnxiangtu.top/gtfiajctnr.html

[U52] PHP：箭头函数
来源：http://hz.zhongyouzk.top/gtcojstgax.html

$double = fn($x) => $x * 2;
来源：http://hz.jlsjyb.cn/gtmibnnryl.html

[U53] PHP：空合并运算符
来源：http://hz.hywenlv.cn/gtowrvksxc.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuanzhike.top/gtqlpktzve.html

[U54] PHP：空安全调用
来源：http://hz.redwolf501.top/gtofcnvvke.html

$obj?->method()
来源：http://hz.daria6918.cn/gtizefgrno.html

[U55] PHP：match 表达式
来源：http://hz.ehwqpu.com/gtqziagyas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj202588.top/gtelsyfcvb.html

[U56] PHP：命名参数
来源：http://hz.kuanghao11.cn/gtmuzimzap.html

f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtodvvxujr.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gtphmbotpi.html

"值: {$a}"
来源：http://hz.dashuyun.cn/gtyyzvgkdm.html

[U58] PHP：数组三件套
来源：http://hz.hnqzz.top/gtlttbrqgl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xingfuxueyuan.xyz/gtwkvltaus.html

[U59] PHP：自定义排序
来源：http://hz.chenlongwang.top/gttdoawnlq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtkvlopeyg.html

[U60] PHP：JSON 编解码
来源：http://hz.yonumen.top/gtbwxifnqt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhaomingkeji.xyz/gtlmhngfli.html

[U61] PHP：正则
来源：http://hz.svipenyu.cn/gtnunmjsad.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtowijwtqu.html

[U62] PHP：日期对象
来源：http://hz.jinqigufen.top/gtahrlzvhd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhoulong.xyz/gtrutsytbv.html

[U63] PHP：文件读写
来源：http://hz.ydzc1.top/gtxqbyxjye.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cqqwz.cn/gtznjwxluu.html

[U64] PHP：目录遍历
来源：http://hz.zdqjudy.top/gthumxghek.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj202588.top/gtoqraknfl.html

[U65] PHP：会话
来源：http://hz.cheryme.top/gtjvvtcmdd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.nanxinkj.top/gtcpkshmdg.html

[U66] PHP：设置 Cookie
来源：http://hz.zycfv.cn/gtgeufrlrz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtkzaqizho.html

[U67] PHP：处理文件上传
来源：http://hz.pycfn.com/gtbzgepbjp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ydzc1.top/gtzwbtopzz.html

[U68] PHP：PDO 连接
来源：http://hz.nwbrower.top/gteydzclmr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtbfohqxwq.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxuanxn.top/gtsljxwfyf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinqigfzy.top/gtjftnadgw.html

[U70] PHP：PDO 事务
来源：http://hz.jyoumei.cn/gtdnjzsuad.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xziqi.cn/gtxxzwfgcb.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtechnqvip.html

throw new RuntimeException("失败", 500);
来源：http://hz.fengsongda.top/gtbilfapke.html

[U72] PHP：写错误日志
来源：http://hz.jiagoushi.top/gtumnjcsrg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hysaishi.cn/gtbczxwyfq.html

[U73] PHP：读取 ini 配置
来源：http://hz.yvedp.cn/gtfykrjgkk.html

parse_ini_file("config.ini", true)
来源：http://hz.zhiwuduotai.top/gttnhplnco.html

[U74] PHP：读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtontrjrdx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xylfe.cn/gtfxihnbxb.html

[U75] PHP：依赖注入
来源：http://hz.haohaochexian.top/gtlnrdtwte.html

composer require psr/container
来源：http://hz.shanyushiyangkeji.top/gtmxahjnjp.html

[U76] PHP：简单路由
来源：http://hz.jinyuanbaomall.cn/gtzpehqzhb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.feifeiyinyue.top/gtsichsktd.html

[U77] PHP：模板渲染
来源：http://hz.gzhubu.top/gtrjryjvkh.html

composer require twig/twig
来源：http://hz.feifeiyinyue.top/gtfgdxekqq.html

[U78] PHP：单元测试
来源：http://hz.tian-w.cn/gtmoqgydxj.html

composer require --dev phpunit/phpunit
来源：http://hz.hnxiangtu.top/gtkhesdskf.html

[U79] PHP：静态分析
来源：http://hz.jlsjyb.cn/gtvfvqlnmx.html

composer require --dev phpstan/phpstan
来源：http://hz.xylfe.cn/gtclbzvmvl.html

[U80] PHP：代码规范修复
来源：http://hz.cucudq.cn/gtsueurowk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhongyouzk.top/gteuqzbhhi.html

[U81] JS：初始化项目
来源：http://hz.ivvv.top/gtenyzfdzn.html

npm init -y;  npm i express
来源：http://hz.sufxvd.cn/gtvquikijj.html

[U82] JS：package.json 脚本
来源：http://hz.birdmap.top/gtiooiscyt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fengsongda.top/gtgvbxqbia.html

[U83] JS：ES Module 导入导出
来源：http://hz.yj20258888.top/gtavisvznq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.vqdsnc.cn/gtykovhmon.html

[U84] JS：CommonJS 写法
来源：http://hz.xingfuxueyuan.xyz/gtgdvvgvpu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ppjwa.cn/gturooyggy.html

[U85] JS：可选链
来源：http://hz.xylfe.cn/gtzwnkmsgc.html

a?.b?.c
来源：http://hz.yueranfly.top/gtqracakes.html

[U86] JS：空值合并
来源：http://hz.snrcjt.cn/gtniawoqwr.html

a ?? b
来源：http://hz.nwbrower.top/gtxxaizjou.html

[U87] JS：解构默认值
来源：http://hz.hnxiangtu.top/gtcrirqfjn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.andypj.xyz/gtbupacrcc.html

[U88] JS：对象展开合并
来源：http://hz.316326.xyz/gtgqpykosg.html

{ ...a, ...b }
来源：http://hz.gogol.net.cn/gttiqmgepo.html

[U89] JS：数组去重
来源：http://hz.xinyue.icu/gtmxbfnzkw.html

[...new Set(arr)]
来源：http://hz.zhengqikj.top/gtaajuzexe.html

[U90] JS：数字数组排序
来源：http://hz.jinghuilouyu.cn/gthrwukvnp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtilkijhni.html

[U91] JS：对象键值遍历
来源：http://hz.cdnleiting.top/gtoakastph.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.vqdsnc.cn/gtlglcxrfm.html

[U92] JS：深拷贝
来源：http://hz.aizwys.cn/gtgugjjmrr.html

structuredClone(obj)
来源：http://hz.daria6918.cn/gtxabyfziu.html

[U93] JS：模板字符串
来源：http://hz.cheryme.top/gtoavcmyey.html

`共 ${n} 条`
来源：http://hz.bjfxy.top/gtruvlwwwg.html

[U94] JS：箭头函数
来源：http://hz.yueranfly.top/gtaqytnfpb.html

const double = x => x * 2;
来源：http://hz.hywenlv.cn/gtoqsbwdur.html

[U95] JS：Promise 包装
来源：http://hz.smart0.xyz/gtidbyhnor.html

new Promise((resolve, reject) => {})
来源：http://hz.smart0.xyz/gtvdpltivk.html

[U96] JS：async/await 与异常
来源：http://hz.jiagoushi.top/gtpnktfric.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtoksphpua.html

[U97] JS：并发请求
来源：http://hz.guannengcc.top/gtgoxtkfdh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtglohnqfz.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhoulong.xyz/gteeaowxej.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yangfankeji.com/gtbuzgkmwe.html

[U99] JS：事件监听
来源：http://hz.xuetiantiany.cn/gtlsqpzuxu.html

el.addEventListener("click", e => {})
来源：http://hz.nanxinkj.top/gtcdroosmc.html

[U100] JS：DOM 查询
来源：http://hz.zhongyouzk.top/gtpiyqzuwz.html

document.querySelector(".item")
来源：http://hz.yanxiufei.cn/gtxxohijwq.html

[U101] JS：classList 操作
来源：http://hz.ppjwa.cn/gtymaldneh.html

el.classList.toggle("active")
来源：http://hz.hammf.cn/gttalxzzcq.html

[U102] JS：本地存储
来源：http://hz.sufxvd.cn/gtcrvwpvtp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnqzz.top/gttomboava.html

[U103] JS：定时器
来源：http://hz.jinqigfzy.top/gthwlcwpkw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuanzhike.top/gtxljxtgkx.html

[U104] JS：防抖
来源：http://hz.zycfv.cn/gtisvyzxqg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtvvbodpuk.html

[U105] JS：节流
来源：http://hz.ydjk.org.cn/gtdwyxlzsx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.aibaodan.cn/gtnofrtkvw.html

[U106] JS：日期格式化
来源：http://hz.yvedp.cn/gtbhwabxsf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gttcihgmsc.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gtrndmobju.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuanzhike.top/gtzrjzcwgy.html

[U108] JS：随机整数
来源：http://hz.yj20258888.top/gtocejyvjs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtfptaamny.html

[U109] JS：数组分组
来源：http://hz.cqqwz.cn/gtwxpvkhzn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtpalfnpko.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtfpvanpoz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.chenlongwang.top/gtduolqnyq.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gthydajqsw.html

new Map(Object.entries(obj))
来源：http://hz.c1oappe.top/gtaleyhief.html

[U112] JS：字符串补位
来源：http://hz.hnxiangtu.top/gtouqnmwkj.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtuokfgxhs.html

[U113] JS：正则替换全部
来源：http://hz.hammf.cn/gtnzpovoin.html

s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtpkwwrnhe.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtrbhyeggh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aizwys.cn/gteqwlpiup.html

[U115] JS：生成 UUID
来源：http://hz.guowangkeji.top/gtqlsywrmw.html

crypto.randomUUID()
来源：http://hz.fengsongda.top/gtfmhftszg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hongshengwenyu.top/gtfkqgefqn.html

/** @param {string} name */ function f(name) {}
来源：http://hz.c1oappe.top/gthvgpvaca.html

[U117] JS：单元测试
来源：http://hz.zhongyouzk.top/gtrxymkhpx.html

npm i -D vitest;  npx vitest
来源：http://hz.hongshengwenyu.top/gthjswsmlk.html

[U118] JS：开发服务器
来源：http://hz.tianlin.xyz/gtiybbukxj.html

npm i -D vite;  npx vite
来源：http://hz.vqdsnc.cn/gtptlbsnvq.html

[U119] JS：生产构建
来源：http://hz.havefunace.top/gtwetvptpk.html

npx vite build
来源：http://hz.gzhubu.top/gtcqnlrtfs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xylfe.cn/gtoqspokcg.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtsvppxvgl.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuijaehdk.html

统计汇总
来源：http://hz.sufxvd.cn/gtxbezvpam.html

================================================================================
来源：http://hz.iojbl.cn/gtelxzjxdb.html

按语言统计（条）：
来源：http://hz.zhoulong.xyz/gtzzbmlrks.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtjrrdmszj.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtyhrxtohb.html

JavaScript ..... 252
来源：http://hz.tianlin.xyz/gtjsmfxujk.html

TypeScript ..... 212
来源：http://hz.zhaomingkeji.xyz/gtcrrcoddx.html

Java ........... 212
来源：http://hz.dianchejie.cn/gtfryitknm.html

Go ............. 212
来源：http://hz.xinyue.icu/gtsyeuwlqa.html

Ruby ........... 212
来源：http://hz.guannengcc.top/gtlhwnjagx.html

C# ............. 212
来源：http://hz.sufxvd.cn/gtculvjqze.html

C .............. 30
来源：http://hz.c1oappe.top/gtpeyxiuob.html

C++ ............ 30
来源：http://hz.nwbrower.top/gtkakkcxfb.html

SQL ............ 90
来源：http://hz.ppjwa.cn/gtcemzzkxr.html

Bash ........... 80
来源：http://hz.wangdashe.top/gtyaqoxcup.html

Kotlin ......... 15
来源：http://hz.jqgufenzy.top/gtuhlptwmq.html

Swift .......... 15
来源：http://hz.sxryk.cn/gtxcegkwkg.html

Lua ............ 10
来源：http://hz.bjfxy.top/gtrupclmrb.html

Perl ........... 10
来源：http://hz.xinyue.icu/gtaqewyavy.html

Scala .......... 10
来源：http://hz.daria6918.cn/gtjnixsjfx.html

------------------------------------
来源：http://hz.mhx1999.top/gtiqbmryco.html

合计 ........... 2106 条
来源：http://hz.0kj1m.cn/gtqkyqibxt.html

按章节统计：
来源：http://hz.xuanzx.com/gtuzmvdjfi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.meibo888.top/gtmwcsdfrs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtzfeomwnn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtpmbrizab.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gtrociuksx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gtmbfqgxub.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtanbncuqj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gteedqvzte.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtjlvzdmni.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtwfyhnvzu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yanxiufei.cn/gtksmdjsbc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtxihzkcgf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtdjdidaab.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtrptkaoaq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhoulong.xyz/gtojavaakb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhongyouzk.top/gtxdkzbpoh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtvwaavadh.html

Q SQL 专题                              90
来源：http://hz.yongpay.top/gtiwsozfry.html

R Bash 专题                             80
来源：http://hz.sufxvd.cn/gtkugjunyj.html

S C / C++ 专题                          60
来源：http://hz.feifeiyinyue.top/gtjlkdfpai.html

T 其他语言补充                          60
来源：http://hz.shanyushiyangtech.top/gtseijsiba.html

U 高频实用片段                         120
来源：http://hz.xziqi.cn/gtrleiboxt.html

------------------------------------
来源：http://hz.guowangkeji.top/gtrudmmuvf.html

合计                                  2106 条
来源：http://hz.fzhhl.top/gtefubuucn.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gthkrxucdc.html

使用提醒
来源：http://hz.fzhhl.top/gtizxjtzfr.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtzxcfhmar.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtcvclzpqe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xziqi.cn/gtddalozac.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnqzz.top/gtvfsowsto.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xingfuxueyuan.xyz/gtvwzgsvwz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhongyouzk.top/gtgndrqozy.html

—— 文件结束 ——
来源：http://hz.bjfxy.top/gtyqbgpttn.html


<!-- 参考信息 -->