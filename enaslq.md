代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtnjrxoukl.html

[R30] 函数返回状态码
来源：http://hz.andypj.xyz/gtgqspmhoe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtneuxveoe.html

[R31] 局部变量
来源：http://hz.guannengcc.top/gttmqpwubw.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtdyyqdynd.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtqdvsxcpv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtazocnwwm.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gteqeddoyf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guowangkeji.top/gtwyukhoco.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gthyavaxvg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtamwdjppp.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtukmytesz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.iojbl.cn/gtirvytair.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtnpncbgqy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtvkabopea.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtdluvsfip.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtkounydfg.html

[R38] 管道串联
来源：http://hz.jyoumei.cn/gtjwzwxstc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fengsongda.top/gtgjfnfqng.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtcxyhyjhh.html

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gtnyvpmoqb.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtsskannjp.html

echo "log" >> out.log
来源：http://hz.xuanzx.com/gtsvjfbowr.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtzxjuhxmm.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gthytbprlq.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtknntuamn.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtantluuhq.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtsthufbgd.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtvvlgoudo.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtlwsicxnn.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtkiegbxip.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gtvzpvlymn.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigufen.top/gtcnsiubst.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtzyyeijrr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhijiandao.cn/gtcjvelnms.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtfwblsqsy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shangyingyoupin.top/gtpjoyemgc.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gtddgirmdg.html

awk '{print $1, $3}' a.txt
来源：http://hz.c1oappe.top/gtoyuunsdv.html

[R49] awk 带条件
来源：http://hz.yongpay.top/gtfvgddnab.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtqqfcdelv.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtfgwnsnwf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.mhx1999.top/gtgslgklsu.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtlqpmubbz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gtkkdadmsq.html

[R52] 统计行数
来源：http://hz.guowangkeji.top/gtrahuqwjv.html

wc -l a.txt
来源：http://hz.mhx1999.top/gtkadimrgb.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtyzsdunqt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtgyxopezb.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtolwtcttb.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gtcrfvabve.html

[R55] 压缩与解压
来源：http://hz.snrcjt.cn/gtkjvopuwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fengsongda.top/gtcjggodnm.html

[R56] 远程拷贝
来源：http://hz.hywenlv.cn/gtazetaehd.html

scp file user@host:/path/
来源：http://hz.yonumen.top/gtwdsgkwjd.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtijcunjmv.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtkzfqsshi.html

[R58] 下载文件
来源：http://hz.xingfuxueyuan.xyz/gtnojvxoxd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtdfymitwd.html

[R59] 发 POST JSON
来源：http://hz.cdnleiting.top/gthpdnljbb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gtyxbkpvea.html

[R60] 只看 HTTP 状态码
来源：http://hz.fengsongda.top/gtryedsohw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtawgxbryk.html

[R61] 磁盘占用
来源：http://hz.wangshuangyany.cn/gtwprxefky.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gtscbiyuhq.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gttwmaujgi.html

du -ah . | sort -rh | head -10
来源：http://hz.gogol.net.cn/gtkximnlfm.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gthpnbmeun.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gtslmoqonf.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtpsyxtayo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtyffovnxx.html

[R65] 查看端口占用
来源：http://hz.sxryk.cn/gthutyvbfm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtrjbrzyxr.html

[R66] 定时任务
来源：http://hz.sysykeji.top/gtnomdeyxy.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtestlbfph.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtmecvfrxz.html

openssl rand -hex 16
来源：http://hz.yangfankeji.com/gtbnbfhpue.html

[R68] 计算文件校验值
来源：http://hz.daxiang520.top/gtmlwopejl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gtxerhrklz.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtotztemas.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtwipcmhiu.html

[R70] 时间戳与互转
来源：http://hz.fengsongda.top/gtpujbznwj.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtnxlrwyzq.html

[R71] 日期格式化
来源：http://hz.0kj1m.cn/gtbmtezgyu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gtmviidiej.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtdjgdkmle.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtiwxfjtre.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtsvtjorjn.html

split -l 1000 big.log part_
来源：http://hz.chenlongwang.top/gtajfrrpib.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtudhcavzk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yonumen.top/gtnwflhtoi.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtueojqkwt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtulvncqno.html

[R76] 使用临时文件
来源：http://hz.iojbl.cn/gtykyylyre.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtqhzuvcuj.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtfjlnvsla.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtrvvpnzqv.html

[R78] 交互式菜单
来源：http://hz.shzxlz.cn/gtbbmjeueu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hysaishi.cn/gtrcgmybcl.html

[R79] 解析命令行选项
来源：http://hz.xylfe.cn/gtukbqhjdq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtqzibgexg.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258.top/gtkawccibf.html

time ./run.sh
来源：http://hz.iojbl.cn/gtshgpbxzm.html

================================================================================
来源：http://hz.havefunace.top/gttabwmqds.html

S. C / C++ 专题
来源：http://hz.hongshengwenyu.top/gtvvktiwqc.html

================================================================================
来源：http://hz.gogol.net.cn/gtxjlznzsc.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtnophgemm.html

#include <stdio.h>
来源：http://hz.gogol.net.cn/gtszlwxipe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dianchejie.cn/gtmhpzqwcz.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtxqpoilcq.html

int a = 10; printf("%d\n", a);
来源：http://hz.tianlin.xyz/gtnxthwowe.html

[S03] C：读入整数
来源：http://hz.yonumen.top/gtzoljjugp.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtvzqjcgkn.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gthxjprxle.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtoibvghpq.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtdpauofel.html

strlen(s)
来源：http://hz.tianlin.xyz/gtntjfvblz.html

[S06] C：字符串比较
来源：http://hz.gaohongyu789.top/gtquftfzbe.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtntaiycjw.html

[S07] C：数组遍历求和
来源：http://hz.nanxinkj.top/gtbrahnhih.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtgrrobctk.html

[S08] C：动态内存分配与释放
来源：http://hz.meibo888.top/gtsuqlwdry.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtfhnvcgvl.html

[S09] C：结构体定义与初始化
来源：http://hz.kuanghao11.cn/gtioooiwot.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gotoacloud.top/gtxpqkzkni.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gtjiutorvk.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gttybybopl.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtyjtfkawc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gtlwpassbr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gtfytdkfrm.html

fclose(f);
来源：http://hz.hnqzz.top/gtaqlgxjsk.html

[S12] C：写文件
来源：http://hz.birdmap.top/gtoxkkqnkn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ehwqpu.com/gtygowbisg.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gtzaumckxw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtsywthnza.html

[S14] C：枚举
来源：http://hz.sweek.top/gthomykvce.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtmwsjlvqt.html

[S15] C：类型转换
来源：http://hz.dashuyun.cn/gtrggkvhqm.html

(double) a / b
来源：http://hz.haohaochexian.top/gtbwklhkkv.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtgrgfznqb.html

x |= (1 << 3);
来源：http://hz.pycfn.com/gtgdoqunfg.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtpqvdeoil.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xziqi.cn/gtgoeiknni.html

[S18] C：命令行参数
来源：http://hz.fzhhl.top/gtrjzyacth.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gtkymgurbe.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtjpkdtgxa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtxodvmxsd.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtocxsonww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtgrbnqowl.html

[S21] C：字符类别判断
来源：http://hz.xylfe.cn/gtqignjusf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtsyuwuepk.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtjzozqopq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtunmfewdu.html

[S23] C：随机数
来源：http://hz.iojbl.cn/gtjkyepxeg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtimbctdpd.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtoradbigp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtpmykdbdv.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtfxoikksn.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtqxawzwff.html

[S26] C：内存清零
来源：http://hz.chenlongwang.top/gtelnkyhfg.html

memset(a, 0, sizeof a);
来源：http://hz.aizwys.cn/gtqdosiqbb.html

[S27] C：定义常量
来源：http://hz.andypj.xyz/gtlklxmhlx.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtvietswlj.html

[S28] C：静态变量
来源：http://hz.aizwys.cn/gtahfiofbu.html

static int counter = 0;
来源：http://hz.gotoacloud.top/gtzjhlkyus.html

[S29] C：变参函数
来源：http://hz.xuanzx.com/gtfmfjlgty.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtasmobncg.html

[S30] C：头文件保护
来源：http://hz.gaohongyu789.top/gtugkafnbo.html

#ifndef X_H
来源：http://hz.xuetiantiany.cn/gtwyxhlugp.html

#define X_H
来源：http://hz.nwbrower.top/gtrlonnjjf.html

#endif
来源：http://hz.hnqzz.top/gthcgsbjjj.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtikbjepai.html

#include <iostream>
来源：http://hz.yongpay.top/gtptsgpvmt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gtlphkcpaj.html

[S32] C++：字符串
来源：http://hz.sxryk.cn/gtfnmbvbvk.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtybygkeau.html

[S33] C++：vector 增删
来源：http://hz.redwolf501.top/gtfqhrkkis.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtgfielcgz.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gtepbiahlz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gotoacloud.top/gtrlboztyb.html

[S35] C++：map
来源：http://hz.zycfv.cn/gtcjlgtkwi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtpmvaxiio.html

[S36] C++：unordered_map
来源：http://hz.jianghu66.top/gtitgcngio.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtkgjyopnj.html

[S37] C++：set
来源：http://hz.mhx1999.top/gtktmtxarq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nwbrower.top/gtomcjtmae.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtnkqtbizk.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtefrzlgia.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gtzdbjdtcg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gtmjyvmons.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gtdzqnncdu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtkjxajqbx.html

[S41] C++：类与构造函数
来源：http://hz.jianghu66.top/gtqxexjeqm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gtexgrejdv.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtybhbmhjy.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gtzhkqdwsl.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtcjxgkuss.html

auto p = std::make_unique<int>(5);
来源：http://hz.gogol.net.cn/gtigfvrxwn.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtzrmkdirz.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtaeaayeko.html

[S45] C++：lambda
来源：http://hz.zhaomingkeji.xyz/gtqxmrghyp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtohqmdngs.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtrppqrora.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtaajqcocb.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtgrpthwcs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtfoxzcaoh.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtaipnpmyi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.bjfxy.top/gtymnfalft.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtexrbikmk.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtjdxipcgp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shzxlz.cn/gtnyxejzny.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtknrkpnwc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtqjqjwwrg.html

[S51] C++：显式类型转换
来源：http://hz.yanxiufei.cn/gtrnlzcazb.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtagsdwnso.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gthtvxzyst.html

int size() const noexcept { return n_; }
来源：http://hz.hfpthk.cn/gtdflemkzb.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtrhxeirvu.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtoiiyrkdc.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtqvqqzlze.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtjswhynck.html

[S55] C++：结构化绑定
来源：http://hz.gzhubu.top/gtrxanugqq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtxugoxanm.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gtucmnogby.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.quarkkingdee.top/gtawjauupz.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtnlullene.html

constexpr int N = 10;
来源：http://hz.xinyue.icu/gtqtfpqtqp.html

[S58] C++：命名空间
来源：http://hz.tanke756.top/gtndivacqh.html

namespace ns { int f() { return 1; } }
来源：http://hz.snrcjt.cn/gtzmryqpnw.html

[S59] C++：静态断言
来源：http://hz.svipenyu.cn/gthqybtuij.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtravgqszd.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtvcgxczmp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtnnuhvaat.html

================================================================================
来源：http://hz.tianlin.xyz/gtmysphtcr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtmktzirxt.html

================================================================================
来源：http://hz.tian-w.cn/gtqlcwhvba.html

[T01] Kotlin：Hello World
来源：http://hz.shuidangran.top/gtwukbgfif.html

println("Hello")
来源：http://hz.shzxlz.cn/gtjpqkhdnh.html

[T02] Kotlin：变量
来源：http://hz.hywenlv.cn/gtexwihqjm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.0kj1m.cn/gtlzbzmlkz.html

[T03] Kotlin：字符串模板
来源：http://hz.gzhubu.top/gtbctqdyfs.html

"值: $b"
来源：http://hz.chenlongwang.top/gttjkeqnjf.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gtoeacqygg.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtkkfqikwf.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtnqsmurzb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtvbeegzcm.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gtrhoieqks.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xingfuxueyuan.xyz/gteuallhmk.html

[T07] Kotlin：集合过滤
来源：http://hz.yuxming.cn/gtbyponlqx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtvtqryoqp.html

[T08] Kotlin：数据类
来源：http://hz.nanxinkj.top/gtbaxlntkw.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtpgfzgaxm.html

[T09] Kotlin：扩展函数
来源：http://hz.snrcjt.cn/gtymlwkeho.html

fun String.exclaim() = this + "!"
来源：http://hz.gzhubu.top/gtllszuiju.html

[T10] Kotlin：默认参数
来源：http://hz.shuidangran.top/gtarqfghfk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhaomingkeji.xyz/gtrydbvqeq.html

[T11] Kotlin：协程
来源：http://hz.jinqigfzy.top/gtngpwislk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.vqdsnc.cn/gtwauhfxsk.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtgjjzxwdj.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtovmufont.html

[T13] Kotlin：只读 Map
来源：http://hz.chenjidiqi.icu/gtlndsyawv.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtjeyecoqk.html

[T14] Kotlin：循环
来源：http://hz.316326.xyz/gtecieevew.html

for (i in 1..10) println(i)
来源：http://hz.nanxuanxn.top/gtwlgbtpag.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtpdgfegak.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtzfumtxwk.html

[T16] Swift：Hello World
来源：http://hz.guowangkeji.top/gtelzvhgop.html

print("Hello")
来源：http://hz.ivvv.top/gtrkocmxrc.html

[T17] Swift：变量与常量
来源：http://hz.yanxiufei.cn/gtuntlranf.html

var a = 1;  let b = 2
来源：http://hz.jianghu66.top/gtxpxkpflr.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtmhcbtqre.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtemrbucpi.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtpfgqjzlv.html

if let n = opt { print(n) }
来源：http://hz.yuxming.cn/gtrybkyoxe.html

[T20] Swift：数组操作
来源：http://hz.ybcxt.top/gtqgxuoyyi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhiwuduotai.top/gttmqkwgvd.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtihljonvk.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtriyzvjhd.html

[T22] Swift：字典
来源：http://hz.yj20258888.top/gttluysfgk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnxiangtu.top/gtysnvwbut.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtmbxmqzji.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtbynhmppp.html

[T24] Swift：闭包
来源：http://hz.tianlin.xyz/gtfejrtdtl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.birdmap.top/gtmldglxde.html

[T25] Swift：结构体
来源：http://hz.cucudq.cn/gtinlahzdo.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtkcgmmidk.html

[T26] Swift：类与重写
来源：http://hz.yuxming.cn/gtuqmczpdg.html

class A: Base { override func f() {} }
来源：http://hz.cdnleiting.top/gtftwlynjy.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtclamtfvv.html

do { try f() } catch { print(error) }
来源：http://hz.zhoulong.xyz/gtmfqkpuad.html

[T28] Swift：枚举
来源：http://hz.sysykeji.top/gtyxtxtktz.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtgahqatjh.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gtgdhayimv.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtckjwswox.html

[T30] Swift：协议
来源：http://hz.redwolf501.top/gthohydnxg.html

protocol Shape { func area() -> Double }
来源：http://hz.pengpengdd.cyou/gtjehnzznp.html

[T31] Lua：Hello World
来源：http://hz.shangyingyoupin.top/gtadapsrdr.html

print("Hello")
来源：http://hz.smart0.xyz/gtjxxywsnr.html

[T32] Lua：局部变量
来源：http://hz.0kj1m.cn/gtebyswcov.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gthnjzwgqs.html


<!-- 参考信息 -->