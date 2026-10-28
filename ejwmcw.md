代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtqifyqbzh.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gtbgkpkqus.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtyefjbdea.html

[R43] 按名字查找文件
来源：http://hz.c1oappe.top/gtkbhidsqz.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gtuspvfukw.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtdwmlpjzu.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtlejlsagl.html

[R45] 批量删除
来源：http://hz.haohaochexian.top/gtigcpezwv.html

find . -name "*.tmp" -delete
来源：http://hz.hnxiangtu.top/gtuvvsjpsq.html

[R46] 递归替换文件内容
来源：http://hz.fengsongda.top/gtdtlkwzfx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtvfgycskb.html

[R47] sed 单行替换
来源：http://hz.xuanzx.com/gtvcoijtib.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gthrsvmcfb.html

[R48] awk 取指定列
来源：http://hz.316326.xyz/gtmldltzud.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuxming.cn/gtdqbaadmg.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtjxlflzpu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuanzhike.top/gthysrcrng.html

[R50] awk 求和
来源：http://hz.cqqwz.cn/gtaxarehmf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtnzcttmjq.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtlrmjwpge.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinyuanbaomall.cn/gtnsoxszlp.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gtpktjjyxx.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtbkrjqbjn.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtinxscjau.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gttjedpkzi.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtevjvawbl.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtruzwlhzc.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtctltliae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtomsmwxis.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtjxjqpwdn.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gtdszkymda.html

[R57] 远程执行命令
来源：http://hz.aizwys.cn/gtjuhtxffx.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gtolzeyjbf.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gttbiuxesz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guannengcc.top/gtwjgkzffv.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtrddzubyt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtgumoqfdz.html

[R60] 只看 HTTP 状态码
来源：http://hz.c1oappe.top/gtqswoddua.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtwgawofqz.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtonvjvhoo.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtwsrlhzwj.html

[R62] 找最占空间的文件
来源：http://hz.sweek.top/gtrapntcmi.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtxlmjjumr.html

[R63] 内存与进程
来源：http://hz.9152youxi.cn/gtxycjyayk.html

free -h;  ps aux | grep nginx
来源：http://hz.redwolf501.top/gtmcuxefrp.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtdqsnoiew.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtghvsxudi.html

[R65] 查看端口占用
来源：http://hz.jiagoushi.top/gtiafkfafv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtbsbpvtlx.html

[R66] 定时任务
来源：http://hz.xylfe.cn/gtluhbuvlk.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtyuddlowb.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtndrtpqyi.html

openssl rand -hex 16
来源：http://hz.9152youxi.cn/gtypajeshu.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtgpigewfd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fengsongda.top/gtugnloxrq.html

[R69] 生成随机密码
来源：http://hz.sufxvd.cn/gteqmwfllt.html

head -c 16 /dev/urandom | base64
来源：http://hz.52xcode.cn/gtnmpmdmji.html

[R70] 时间戳与互转
来源：http://hz.feifeiyinyue.top/gtcmyevuev.html

date +%s;  date -d @1700000000
来源：http://hz.52xcode.cn/gtwzztkvrt.html

[R71] 日期格式化
来源：http://hz.ydjk.org.cn/gtbtzxxfgh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtwanriqzi.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gtqmhlcbut.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.smart0.xyz/gtseszbrmp.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtnucgvixd.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gtrwzpynxj.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gtoajkttwd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gttcxkvrxj.html

[R75] 导出环境变量
来源：http://hz.dianchejie.cn/gtzgzmlzzf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gttcknwcsd.html

[R76] 使用临时文件
来源：http://hz.zhijiandao.cn/gtbiuyqpwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gthortyvcr.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gtmipecyyt.html

read -rp "请输入: " ans
来源：http://hz.yongpay.top/gthwzzkakf.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtenkjuvzw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtgdmgsuit.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtvyjmyakd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtfkrdpfop.html

[R80] 查看脚本执行耗时
来源：http://hz.yanxiufei.cn/gtqocspmgb.html

time ./run.sh
来源：http://hz.havefunace.top/gtouaodmys.html

================================================================================
来源：http://hz.tianlin.xyz/gtcrebhdne.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtbcyraulk.html

================================================================================
来源：http://hz.daxiang520.top/gtuxrzypws.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtzuzhcmfv.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gtszrniqnh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yanxiufei.cn/gtizcjahhj.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtjldjoewd.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtnneuanle.html

[S03] C：读入整数
来源：http://hz.iojbl.cn/gterrklxmi.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtkyzujsbl.html

[S04] C：字符串复制
来源：http://hz.dashuyun.cn/gthrlfghlz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtmffswfit.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtsfkklwsh.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtjopixkof.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtvrqtbfzd.html

strcmp(a, b) == 0
来源：http://hz.andypj.xyz/gtetbzlekz.html

[S07] C：数组遍历求和
来源：http://hz.tian-w.cn/gtfzqycjhc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtezwlrpom.html

[S08] C：动态内存分配与释放
来源：http://hz.xylfe.cn/gtcazrdtge.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtntktnpch.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gttcqbntyk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tian-w.cn/gtfzirxmwb.html

[S10] C：指针与解引用
来源：http://hz.zhoulong.xyz/gtcpostlel.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtbkepmpid.html

[S11] C：逐行读文件
来源：http://hz.shzxlz.cn/gtfodarngl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtfppcavif.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zdqjudy.top/gtdqvxylqj.html

fclose(f);
来源：http://hz.tanke756.top/gtdnfkikri.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtefgsipap.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zycfv.cn/gtpzkjfdwt.html

[S13] C：宏定义
来源：http://hz.jinyuanbaomall.cn/gtwisemfyj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtpodnunzs.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtrlyhsgqr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gteivrzhhw.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtcccydfyv.html

(double) a / b
来源：http://hz.meibo888.top/gtzplxowzb.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtglgfzirm.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtdayliwbd.html

[S17] C：安全拼接字符串
来源：http://hz.9152youxi.cn/gtsspcblld.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigufen.top/gturwchfad.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gtabmazkah.html

int main(int argc, char **argv)
来源：http://hz.hongshengwenyu.top/gtjznaeofg.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtalqzkivs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtjwzxpgvb.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtyijbkuqx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtjosoqrjk.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtilivinzj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtnatpihxt.html

[S22] C：字符串转数字
来源：http://hz.chenzaomai.com/gtolzoiues.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gtiopnvdwe.html

[S23] C：随机数
来源：http://hz.hnqzz.top/gtbgnxnqxs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydzc1.top/gtljxenchz.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtunslbecf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtnkkouutm.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gtrhknycaq.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtajipoygj.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtpynfmphf.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gtevlpsamq.html

[S27] C：定义常量
来源：http://hz.gogol.net.cn/gtjxycdmxg.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtdkkenyir.html

[S28] C：静态变量
来源：http://hz.sxryk.cn/gtguieuvpv.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtrkzslrai.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtelshxkcp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gttfrrgaqc.html

[S30] C：头文件保护
来源：http://hz.hysaishi.cn/gtjvbqsrun.html

#ifndef X_H
来源：http://hz.nanxinkj.top/gtigmjbaor.html

#define X_H
来源：http://hz.cashguo.top/gtjikyudur.html

#endif
来源：http://hz.gaohongyu789.top/gtuodvlmqx.html

[S31] C++：Hello World
来源：http://hz.zhaomingkeji.xyz/gtjsggqqud.html

#include <iostream>
来源：http://hz.hfpthk.cn/gtbpqdimit.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhaomingkeji.xyz/gtytvxxrfq.html

[S32] C++：字符串
来源：http://hz.jinqigfzy.top/gtxzmqxjrn.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtyizbjzni.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtaxyddisl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenzaomai.com/gtufxitpvt.html

[S34] C++：遍历 vector
来源：http://hz.cashguo.top/gttxxbnyoe.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtlhjlyiiy.html

[S35] C++：map
来源：http://hz.zhiwuduotai.top/gtwdtmzqgp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtbcxytedw.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtpaydnmhu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtfqjzvrng.html

[S37] C++：set
来源：http://hz.jinqigfzy.top/gtfhefebia.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xinyue.icu/gtjzrzgwed.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtisltnyuh.html

std::sort(v.begin(), v.end());
来源：http://hz.cdnleiting.top/gtiazeoroa.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtqfixmgrz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gtwcozxqsw.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtxdqairwj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gtnbqagaqd.html

[S41] C++：类与构造函数
来源：http://hz.zhijiandao.cn/gtfauccjls.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtsplclsgj.html

[S42] C++：继承与虚函数
来源：http://hz.gotoacloud.top/gtxkixccyp.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gttwfsklaj.html

[S43] C++：智能指针
来源：http://hz.yvedp.cn/gtnbbdfrjx.html

auto p = std::make_unique<int>(5);
来源：http://hz.tanke756.top/gtjfwjcaqz.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gtlizwhypx.html

void inc(int &x) { ++x; }
来源：http://hz.tian-w.cn/gtnwsbjjhu.html

[S45] C++：lambda
来源：http://hz.nwbrower.top/gtqynmojiu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtexlfveus.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gttwbfwqfo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gthejbahnf.html

[S47] C++：结构化绑定遍历
来源：http://hz.nwbrower.top/gtoujpfycr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.birdmap.top/gtflfuinki.html

[S48] C++：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtcpcguuxs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtsspopryo.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gthkuxltuq.html

[S49] C++：写文件
来源：http://hz.feifeiyinyue.top/gtkfuvahla.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtarsahxqz.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtjxgavwjn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhiwuduotai.top/gtrieegnvg.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtxooelbfd.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtplmlpjxb.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gtbmscmogt.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtplzidwaj.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtrqogmxqr.html

std::vector<int> w = std::move(v);
来源：http://hz.pycfn.com/gtwqcndogw.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtzjjhovox.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangtech.top/gtpjymltww.html

[S55] C++：结构化绑定
来源：http://hz.0kj1m.cn/gtmbiuwxiu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxuanxn.top/gtulcfoier.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtbozxnxkb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhengqikj.top/gtliqjeedo.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtiwpwuzwx.html

constexpr int N = 10;
来源：http://hz.shangyingyoupin.top/gtddklxvrl.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gtquhpaysu.html

namespace ns { int f() { return 1; } }
来源：http://hz.hywenlv.cn/gtmjzsmbzc.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtwrjajitq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtyykudgiu.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gtmdrdxlwo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtrspldztz.html

================================================================================
来源：http://hz.snrcjt.cn/gtascjypmp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtbfwdcrln.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuehrjzum.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtlpbiwibk.html

println("Hello")
来源：http://hz.meibo888.top/gtnuusihou.html

[T02] Kotlin：变量
来源：http://hz.cdnleiting.top/gtnvjdivpf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtaeykcpag.html

[T03] Kotlin：字符串模板
来源：http://hz.guannengcc.top/gtdpynvinc.html

"值: $b"
来源：http://hz.jianghu66.top/gtuofffdjo.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gtmjpropbe.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtfzsjlinb.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxuanxn.top/gtmdjuaceu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shuidangran.top/gtztenuutd.html

[T06] Kotlin：集合映射
来源：http://hz.hammf.cn/gtwbftiptu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gtfoweaidb.html

[T07] Kotlin：集合过滤
来源：http://hz.xylfe.cn/gthoqmikhh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtksblhfpm.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtyarjeuvv.html

data class User(val name: String, val age: Int)
来源：http://hz.kuanghao11.cn/gtpxcwvhps.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgfzy.top/gtnsuicmnh.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtgqavlngj.html

[T10] Kotlin：默认参数
来源：http://hz.xinyue.icu/gtjaevkfag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shuidangran.top/gthpuwohkv.html

[T11] Kotlin：协程
来源：http://hz.vqdsnc.cn/gtxqonovdq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aizwys.cn/gtjopqsfwr.html

[T12] Kotlin：解构声明
来源：http://hz.jiagoushi.top/gteptzejkt.html

val (a, b) = Pair(1, 2)
来源：http://hz.hywenlv.cn/gtjisdtust.html

[T13] Kotlin：只读 Map
来源：http://hz.yueranfly.top/gtvjnzzlnd.html

val m = mapOf("a" to 1)
来源：http://hz.zhaomingkeji.xyz/gtogjwrwom.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtnvpyfqxm.html

for (i in 1..10) println(i)
来源：http://hz.yanxiufei.cn/gtjwejhxqo.html

[T15] Kotlin：接口
来源：http://hz.jinyuanbaomall.cn/gtnmtvhrbm.html

interface Shape { fun area(): Double }
来源：http://hz.quarkkingdee.top/gtnqyvcmbm.html

[T16] Swift：Hello World
来源：http://hz.hnqzz.top/gtzortqcpo.html

print("Hello")
来源：http://hz.jianghu66.top/gtfrzdlzpu.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtrivdzxjp.html

var a = 1;  let b = 2
来源：http://hz.yonumen.top/gtqinkjwyp.html

[T18] Swift：字符串插值
来源：http://hz.jiagoushi.top/gtczqjufvk.html

"值: \(b)"
来源：http://hz.shangyingyoupin.top/gtukblgrmu.html

[T19] Swift：可选绑定
来源：http://hz.dashuyun.cn/gtqwsztala.html

if let n = opt { print(n) }
来源：http://hz.cashguo.top/gttgauflgo.html

[T20] Swift：数组操作
来源：http://hz.pengpengdd.cyou/gttzmkvgsa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xinyue.icu/gtajoizyeu.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtsvxxurxu.html

for x in a { print(x) }
来源：http://hz.fzhhl.top/gtczdfzawq.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtblbzoijj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cqqwz.cn/gtfereydfv.html

[T23] Swift：函数
来源：http://hz.hnxiangtu.top/gtfmgmldrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sufxvd.cn/gtccwixiuv.html

[T24] Swift：闭包
来源：http://hz.chenjidiqi.icu/gtbfhlihtg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.52xcode.cn/gtwtonoali.html

[T25] Swift：结构体
来源：http://hz.gogol.net.cn/gtepblmjtw.html

struct P { var x: Int }
来源：http://hz.zhixingplan.top/gtqhqyidga.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtgzwndefk.html

class A: Base { override func f() {} }
来源：http://hz.jyoumei.cn/gtqpafwsbf.html

[T27] Swift：错误处理
来源：http://hz.andypj.xyz/gtwdvhjltn.html

do { try f() } catch { print(error) }
来源：http://hz.smart0.xyz/gtjmistifk.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gtmlgydxfz.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtzeofsryi.html

[T29] Swift：guard 提前返回
来源：http://hz.tanke756.top/gtwpzybmqc.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtfrfeyyka.html

[T30] Swift：协议
来源：http://hz.yangfankeji.com/gtgrgvlunn.html

protocol Shape { func area() -> Double }
来源：http://hz.ybcxt.top/gtsqnehvea.html

[T31] Lua：Hello World
来源：http://hz.shuidangran.top/gtzhpqazdb.html

print("Hello")
来源：http://hz.ydzc1.top/gtymgjrlup.html

[T32] Lua：局部变量
来源：http://hz.yuxming.cn/gthxwsqigp.html

local a = 1
来源：http://hz.snrcjt.cn/gtxgofsath.html

[T33] Lua：表（数组）
来源：http://hz.jqgfzy.top/gtpuqubwjb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtyaaablss.html

[T34] Lua：遍历表
来源：http://hz.chenlongwang.top/gtywazxdcj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhixingplan.top/gtegkrjhjr.html

[T35] Lua：字典表
来源：http://hz.jinqigufen.top/gtgnzvkaed.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtczhcstgv.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtnzfwmkpc.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtqxjdjlxd.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtakxbymio.html

"a" .. "b"
来源：http://hz.kuanghao11.cn/gtqpugoicl.html

[T38] Lua：条件
来源：http://hz.yueranfly.top/gtvpbyfkgz.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtycqcdzzd.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtgachkovp.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangtech.top/gtqdizujfk.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtzdidiwyq.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtnksrflwq.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtsfsjkhat.html

print "Hello\n";
来源：http://hz.c1oappe.top/gttghkzlhu.html

[T42] Perl：变量类型
来源：http://hz.kuanghao11.cn/gtsasczniu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yvedp.cn/gtfsggvydf.html

[T43] Perl：字符串插值
来源：http://hz.cheryme.top/gttgrbnfqm.html

"值: $a"
来源：http://hz.zycfv.cn/gtjstumawq.html

[T44] Perl：条件
来源：http://hz.ivvv.top/gttnjolfii.html

if ($a > 0) { print "正"; }
来源：http://hz.shuidangran.top/gtzpxqysln.html


<!-- 参考信息 -->