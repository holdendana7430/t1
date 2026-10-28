代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtbsojqdqj.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtukcdzpxo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zdqjudy.top/gtsvrtrena.html

[R37] 把输出赋给变量
来源：http://hz.ywan-chungtsiang.top/gtqusymwpj.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtqzjppeye.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtrhpdrjan.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtpnhucdiu.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gttwffehng.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtdhmpubwa.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtahgmwyrv.html

echo "log" >> out.log
来源：http://hz.316326.xyz/gtonpfdels.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtsbupgbhc.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gtzmalgozx.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gtbhwiuywu.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtbndovmdb.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtulmlgdpn.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtmncfqqkh.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtntjvicnb.html

find . -mtime -7 -type f
来源：http://hz.jlsjyb.cn/gtycmcjlvu.html

[R45] 批量删除
来源：http://hz.dianchejie.cn/gtdesikvlk.html

find . -name "*.tmp" -delete
来源：http://hz.shzxlz.cn/gtkldervaw.html

[R46] 递归替换文件内容
来源：http://hz.zhaomingkeji.xyz/gtxfbxikwg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gtsbznbczu.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtemywxfrm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gttqylacgg.html

[R48] awk 取指定列
来源：http://hz.yuxming.cn/gtvlzvoizd.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinyuanbaomall.cn/gtktybogaa.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtveqbveoy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtallnwxxf.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gtnzgarayu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtqxpyhlmq.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gtawthgcjg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hywenlv.cn/gtqhjgkwrv.html

[R52] 统计行数
来源：http://hz.hysaishi.cn/gtgjadchej.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gtbjmtyheh.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtbliqsvds.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.iojbl.cn/gtbvdklcao.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtcylzrxpf.html

diff a.txt b.txt
来源：http://hz.yj20258.top/gtedlybiab.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtnrcxwlpu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtgbyptohv.html

[R56] 远程拷贝
来源：http://hz.kuanghao11.cn/gtfsommwad.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gtoryuiulu.html

[R57] 远程执行命令
来源：http://hz.quarkkingdee.top/gtuxvsavoy.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gtzlplzdec.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gttgqbepjp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gtbqlsbldq.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtxkeraqlt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ehwqpu.com/gtqlamoiom.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtpghdbrqe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtgjnymhtw.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtrqdskucl.html

df -h;  du -sh *
来源：http://hz.ivvv.top/gtztodgqah.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtxfzsrzzw.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtlckyzmin.html

[R63] 内存与进程
来源：http://hz.xuetiantiany.cn/gtgmwfjvum.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtcbzrkxhw.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtugrlirqt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gtglgpwrtv.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gtmkmiwavt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtxeqtwzzh.html

[R66] 定时任务
来源：http://hz.nwbrower.top/gtfgtttcty.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gttfigsvxp.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gtfswiapnt.html

openssl rand -hex 16
来源：http://hz.jlsjyb.cn/gtfqihmuzw.html

[R68] 计算文件校验值
来源：http://hz.hfpthk.cn/gtygysbkrv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtrgchuvwc.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtodrqhmpb.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gtrnupzbqh.html

[R70] 时间戳与互转
来源：http://hz.gotoacloud.top/gtuvctbmdf.html

date +%s;  date -d @1700000000
来源：http://hz.xinyue.icu/gtlzrhlnro.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtritgpvbm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gtmyfqrdrv.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gthqnxrrhl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.redwolf501.top/gtseohzhjg.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtjnnfupnc.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtypiozcin.html

[R74] 批量重命名
来源：http://hz.vqdsnc.cn/gtuogyfoov.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxinkj.top/gtpfmwarel.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtrtooffal.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sweek.top/gtrocxrkni.html

[R76] 使用临时文件
来源：http://hz.yongpay.top/gtyjdquliy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtfownskwq.html

[R77] 读取用户输入
来源：http://hz.jinghuilouyu.cn/gtpnpjrfbo.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtwibacxgf.html

[R78] 交互式菜单
来源：http://hz.aizwys.cn/gtfxaxsdgq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtkvvsroed.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtrshdfmlm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnxiangtu.top/gthlocwyah.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtdotdwhyk.html

time ./run.sh
来源：http://hz.zycfv.cn/gttyrxbkkk.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttorttnaz.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtmrxxlirp.html

================================================================================
来源：http://hz.cucudq.cn/gtfwzowefp.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtqzjuwbdn.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtvilnyuti.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtrwhrlwmw.html

[S02] C：变量与格式化输出
来源：http://hz.yvedp.cn/gtbqtijyzm.html

int a = 10; printf("%d\n", a);
来源：http://hz.gzhubu.top/gtqdefhkrl.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gtedlaqydm.html

int x; scanf("%d", &x);
来源：http://hz.ywan-chungtsiang.top/gtmtnjcvnp.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gthbnkstfb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtisfhazod.html

[S05] C：字符串长度
来源：http://hz.gzhubu.top/gtfhndjfsg.html

strlen(s)
来源：http://hz.sufxvd.cn/gtysqpcein.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtbjfzwzfp.html

strcmp(a, b) == 0
来源：http://hz.shzxlz.cn/gtoscdcwfn.html

[S07] C：数组遍历求和
来源：http://hz.gzhubu.top/gtizfaofgf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yueranfly.top/gtqwcstqkl.html

[S08] C：动态内存分配与释放
来源：http://hz.xziqi.cn/gtdyfanyjf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtepuxjwot.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtgntcloij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hongshengwenyu.top/gtzhyjwkiy.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gtquuiwavg.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gtuttqerxf.html

[S11] C：逐行读文件
来源：http://hz.yj202588.top/gtdvnnxmrv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ywan-chungtsiang.top/gtanabtrfd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gtqsqejluj.html

fclose(f);
来源：http://hz.gzhubu.top/gtzabxlnzv.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gtnqmgvfzj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hfpthk.cn/gtsnwbzvdn.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtdlxmbqwl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtttizmchh.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtpkelmvab.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinghuilouyu.cn/gtyrgvumqp.html

[S15] C：类型转换
来源：http://hz.snrcjt.cn/gtvymfrwye.html

(double) a / b
来源：http://hz.shanyushiyangtech.top/gtcrucdrme.html

[S16] C：位操作置位
来源：http://hz.gotoacloud.top/gtvoaeymtn.html

x |= (1 << 3);
来源：http://hz.jinqigufen.top/gtluvbawim.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtfgzwguee.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.iojbl.cn/gtxjrjsavi.html

[S18] C：命令行参数
来源：http://hz.sufxvd.cn/gtkwvabjrh.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtmjzrkeld.html

[S19] C：快速排序
来源：http://hz.shanyushiyangtech.top/gtnfdxnrja.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtidgofeux.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtojyjntdb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtqdxzoypx.html

[S21] C：字符类别判断
来源：http://hz.bjfxy.top/gtfwpiogyl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtombjdczg.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtmzzirynk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinghuilouyu.cn/gtkfcqyseb.html

[S23] C：随机数
来源：http://hz.yonumen.top/gtyedazrvw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtwthtyumn.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gtjqupwqdp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhijiandao.cn/gtprgjobqs.html

[S25] C：内存拷贝
来源：http://hz.yj20258.top/gtkbxdeskl.html

memcpy(dst, src, n);
来源：http://hz.tianlin.xyz/gtyulzxmnn.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtoievrfdh.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtwrpdyfpc.html

[S27] C：定义常量
来源：http://hz.ehwqpu.com/gtlretijja.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtghmkjrpt.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gtqbceiebp.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtdavfgzgh.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gtvlqtqfia.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuxming.cn/gtfdlvphhm.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gttybboitl.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtzyuzqdqa.html

#define X_H
来源：http://hz.gogol.net.cn/gtcszptmci.html

#endif
来源：http://hz.yonumen.top/gtweveapch.html

[S31] C++：Hello World
来源：http://hz.bjfxy.top/gtkcvirwku.html

#include <iostream>
来源：http://hz.yuxming.cn/gtxvxkacff.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtfnuoaxdx.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gtcpfalzin.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtjkwksihx.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtdtihkerv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtqzafopqi.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtofuyqfic.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yvedp.cn/gtlxlunvco.html

[S35] C++：map
来源：http://hz.gaohongyu789.top/gtoszhezli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtvhapihkc.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtweqakukv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtzeyjydxk.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtqqxmdqzt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtbrxddwbu.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtwaczbumf.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtuvfujuau.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtjhumazvd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtgvkpeaka.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtldfxhynl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhengqikj.top/gthtxecopu.html

[S41] C++：类与构造函数
来源：http://hz.0kj1m.cn/gtldtxtfrk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtyyamfxmq.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtnhittqjy.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtmbpkxnvj.html

[S43] C++：智能指针
来源：http://hz.yuanzhike.top/gtpkpqptkz.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gttyfeyqgk.html

[S44] C++：引用传参
来源：http://hz.pycfn.com/gtpeilptuq.html

void inc(int &x) { ++x; }
来源：http://hz.shangyingyoupin.top/gtlujozqax.html

[S45] C++：lambda
来源：http://hz.havefunace.top/gtushncdco.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gtfirxtrcb.html

[S46] C++：函数模板
来源：http://hz.zhoulong.xyz/gtcjrukezv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtzsipwtkj.html

[S47] C++：结构化绑定遍历
来源：http://hz.cdnleiting.top/gtmerfvigd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258.top/gtwcndhdzn.html

[S48] C++：逐行读文件
来源：http://hz.shuidangran.top/gtucibvepv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.svipenyu.cn/gtheflojcv.html

while (std::getline(in, line)) { }
来源：http://hz.yanxiufei.cn/gtifejrdah.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtpkeypftk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangkeji.top/gtnnirylmt.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gthuvwvjib.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zdqjudy.top/gtjqjdazdv.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtjlzfafgc.html

static_cast<double>(a) / b
来源：http://hz.316326.xyz/gtkcbkcian.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtsewxmezl.html

int size() const noexcept { return n_; }
来源：http://hz.yj202588.top/gtztineihv.html

[S53] C++：移动语义
来源：http://hz.0kj1m.cn/gtveoloaim.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtptqolxrn.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gtonklevaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtenvtrgwz.html

[S55] C++：结构化绑定
来源：http://hz.tianlin.xyz/gtfmhipeze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hfpthk.cn/gttfrkmewa.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gtvlbsmctj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.andypj.xyz/gtpsgweimm.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtbnweeico.html

constexpr int N = 10;
来源：http://hz.dashuyun.cn/gtrwozqrtg.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtitdnmwmf.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtsvvvrryq.html

[S59] C++：静态断言
来源：http://hz.chenzaomai.com/gtlzjnfjml.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtwwilpczu.html

[S60] C++：遍历并删除元素
来源：http://hz.chenjidiqi.icu/gtbaklxacj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtuxprveqb.html

================================================================================
来源：http://hz.zhengqikj.top/gtaicrueeu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtftrdiedq.html

================================================================================
来源：http://hz.yuxming.cn/gtgguiflqr.html

[T01] Kotlin：Hello World
来源：http://hz.zhaomingkeji.xyz/gtjbekxqys.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtbqkeiriz.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtxnfbwrgu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtobtgtnlc.html

[T03] Kotlin：字符串模板
来源：http://hz.haohaochexian.top/gtbodqiaoi.html

"值: $b"
来源：http://hz.dashuyun.cn/gtqkppfzxl.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gtcodcfzdp.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtprbpcote.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtnzimblby.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cheryme.top/gtbavcmlcw.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gtcxzdmqft.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtvdsiyjbr.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtnrekmpoz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtmatqjebp.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gttmmqbyfe.html

data class User(val name: String, val age: Int)
来源：http://hz.pycfn.com/gtkpetsnpl.html

[T09] Kotlin：扩展函数
来源：http://hz.chenjidiqi.icu/gtaetimjnq.html

fun String.exclaim() = this + "!"
来源：http://hz.chenjidiqi.icu/gtppoaysqn.html

[T10] Kotlin：默认参数
来源：http://hz.tian-w.cn/gtbmvwxisx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guowangkeji.top/gtkutrdhht.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtwdklggef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtsxgwqfsb.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtwfxknphu.html

val (a, b) = Pair(1, 2)
来源：http://hz.gotoacloud.top/gtlaocjdow.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtahykeoyi.html

val m = mapOf("a" to 1)
来源：http://hz.sysykeji.top/gtoeozdelp.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtrmfnbdmv.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtsvxnptti.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtmlhqfswc.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gtfhecslqw.html

[T16] Swift：Hello World
来源：http://hz.zhoulong.xyz/gtskhpudeq.html

print("Hello")
来源：http://hz.hywenlv.cn/gtjclrrojy.html

[T17] Swift：变量与常量
来源：http://hz.meibo888.top/gtdsxkhyjj.html

var a = 1;  let b = 2
来源：http://hz.haohaochexian.top/gtxvxqpzwt.html

[T18] Swift：字符串插值
来源：http://hz.nanxuanxn.top/gttvtmazuh.html

"值: \(b)"
来源：http://hz.xziqi.cn/gtdmshxzjt.html

[T19] Swift：可选绑定
来源：http://hz.sufxvd.cn/gtsydxewvc.html

if let n = opt { print(n) }
来源：http://hz.birdmap.top/gtfwsnwjbe.html

[T20] Swift：数组操作
来源：http://hz.fengsongda.top/gteumvegfr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtjfnyoxib.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gtapmbeokx.html

for x in a { print(x) }
来源：http://hz.yvedp.cn/gtzostokrd.html

[T22] Swift：字典
来源：http://hz.316326.xyz/gtgtmzwjzp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shangyingyoupin.top/gtdbpcqlnu.html

[T23] Swift：函数
来源：http://hz.yueranfly.top/gtlpqwjark.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cdnleiting.top/gtxouyhklh.html

[T24] Swift：闭包
来源：http://hz.52xcode.cn/gtkahdkbxp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shuidangran.top/gtvxlamhub.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtabhvmvtt.html

struct P { var x: Int }
来源：http://hz.sweek.top/gttfypwfcn.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtdtpkmtln.html

class A: Base { override func f() {} }
来源：http://hz.sweek.top/gtogxmejxf.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtkoptsggz.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gtoizfjvaj.html

[T28] Swift：枚举
来源：http://hz.jinqigufen.top/gtdometjnq.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtfavxeozk.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gttbyllrxn.html

guard let x = opt else { return }
来源：http://hz.daxiang520.top/gtjfvgisvt.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtaosbrtnu.html

protocol Shape { func area() -> Double }
来源：http://hz.chenlongwang.top/gtuajkzute.html

[T31] Lua：Hello World
来源：http://hz.aibaodan.cn/gtwrcrmtky.html

print("Hello")
来源：http://hz.smart0.xyz/gttsumjwsv.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtlcdmrkyo.html

local a = 1
来源：http://hz.daxiang520.top/gtzwhophrw.html

[T33] Lua：表（数组）
来源：http://hz.gotoacloud.top/gtrihwtmoq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.quarkkingdee.top/gtulajkrxk.html

[T34] Lua：遍历表
来源：http://hz.pengpengdd.cyou/gtsfcqxocu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinghuilouyu.cn/gtihanrmpf.html

[T35] Lua：字典表
来源：http://hz.ivvv.top/gtorzyhwcd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtgyexrwjl.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtgallnekt.html

function add(a, b) return a + b end
来源：http://hz.havefunace.top/gtirqptjdy.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtkvrtggmp.html

"a" .. "b"
来源：http://hz.iojbl.cn/gtqudbcapr.html

[T38] Lua：条件
来源：http://hz.c1oappe.top/gtqfzcgvmb.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtzimcdlad.html


<!-- 参考信息 -->